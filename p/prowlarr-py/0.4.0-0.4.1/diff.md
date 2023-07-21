# Comparing `tmp/prowlarr-py-0.4.0.tar.gz` & `tmp/prowlarr-py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prowlarr-py-0.4.0.tar", last modified: Mon May 29 06:41:16 2023, max compression
+gzip compressed data, was "prowlarr-py-0.4.1.tar", last modified: Fri Jul 21 11:35:00 2023, max compression
```

## Comparing `prowlarr-py-0.4.0.tar` & `prowlarr-py-0.4.1.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22160 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.258098 prowlarr-py-0.4.0/prowlarr/
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.262098 prowlarr-py-0.4.0/prowlarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30218 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/app_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53621 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/application_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22492 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30375 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18944 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/development_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54165 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18592 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52868 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_default_categories_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53829 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_proxy_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_stats_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12167 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/indexer_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11837 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42217 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/newznab_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53708 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26683 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26855 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29527 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18422 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/prowlarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/app_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/application_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/application_sync_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/authentication_required_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/book_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/development_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_client_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/host_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_capability_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_privacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_proxy_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_stats_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/indexer_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/localization_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/movie_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/music_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/tv_search_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/models/user_agent_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/prowlarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/prowlarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22640 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 06:41:16.000000 prowlarr-py-0.4.0/prowlarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:41:16.270099 prowlarr-py-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-29 06:41:00.000000 prowlarr-py-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:00.696446 prowlarr-py-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-07-21 11:35:00.696446 prowlarr-py-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22469 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:00.684446 prowlarr-py-0.4.1/prowlarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:00.688446 prowlarr-py-0.4.1/prowlarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30148 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/app_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66319 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/application_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22465 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23365 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30278 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18882 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/development_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67054 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19093 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18476 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65324 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/indexer_default_categories_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54059 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/indexer_proxy_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/indexer_stats_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/indexer_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11493 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42217 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/newznab_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53938 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20883 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21840 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26828 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29349 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18360 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29655 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:00.696446 prowlarr-py-0.4.1/prowlarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/app_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/application_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/application_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/application_sync_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/authentication_required_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/book_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/development_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/download_client_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/host_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_capability_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_proxy_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_stats_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/indexer_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/localization_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/movie_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/music_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/tv_search_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/models/user_agent_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/prowlarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:00.696446 prowlarr-py-0.4.1/prowlarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22949 2023-07-21 11:35:00.000000 prowlarr-py-0.4.1/prowlarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-21 11:35:00.000000 prowlarr-py-0.4.1/prowlarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:35:00.000000 prowlarr-py-0.4.1/prowlarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 11:35:00.000000 prowlarr-py-0.4.1/prowlarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 11:35:00.000000 prowlarr-py-0.4.1/prowlarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:35:00.696446 prowlarr-py-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 11:34:46.000000 prowlarr-py-0.4.1/setup.py
```

### Comparing `prowlarr-py-0.4.0/LICENSE` & `prowlarr-py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/PKG-INFO` & `prowlarr-py-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowlarr-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Prowlarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/prowlarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/prowlarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # prowlarr-py
 Prowlarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.4.0
+- Package version: 0.4.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -118,17 +118,19 @@
 *AppProfileApi* | [**delete_app_profile**](docs/AppProfileApi.md#delete_app_profile) | **DELETE** /api/v1/appprofile/{id} | 
 *AppProfileApi* | [**get_app_profile_by_id**](docs/AppProfileApi.md#get_app_profile_by_id) | **GET** /api/v1/appprofile/{id} | 
 *AppProfileApi* | [**list_app_profile**](docs/AppProfileApi.md#list_app_profile) | **GET** /api/v1/appprofile | 
 *AppProfileApi* | [**update_app_profile**](docs/AppProfileApi.md#update_app_profile) | **PUT** /api/v1/appprofile/{id} | 
 *ApplicationApi* | [**create_applications**](docs/ApplicationApi.md#create_applications) | **POST** /api/v1/applications | 
 *ApplicationApi* | [**create_applications_action_by_name**](docs/ApplicationApi.md#create_applications_action_by_name) | **POST** /api/v1/applications/action/{name} | 
 *ApplicationApi* | [**delete_applications**](docs/ApplicationApi.md#delete_applications) | **DELETE** /api/v1/applications/{id} | 
+*ApplicationApi* | [**delete_applications_bulk**](docs/ApplicationApi.md#delete_applications_bulk) | **DELETE** /api/v1/applications/bulk | 
 *ApplicationApi* | [**get_applications_by_id**](docs/ApplicationApi.md#get_applications_by_id) | **GET** /api/v1/applications/{id} | 
 *ApplicationApi* | [**list_applications**](docs/ApplicationApi.md#list_applications) | **GET** /api/v1/applications | 
 *ApplicationApi* | [**list_applications_schema**](docs/ApplicationApi.md#list_applications_schema) | **GET** /api/v1/applications/schema | 
+*ApplicationApi* | [**put_applications_bulk**](docs/ApplicationApi.md#put_applications_bulk) | **PUT** /api/v1/applications/bulk | 
 *ApplicationApi* | [**test_applications**](docs/ApplicationApi.md#test_applications) | **POST** /api/v1/applications/test | 
 *ApplicationApi* | [**testall_applications**](docs/ApplicationApi.md#testall_applications) | **POST** /api/v1/applications/testall | 
 *ApplicationApi* | [**update_applications**](docs/ApplicationApi.md#update_applications) | **PUT** /api/v1/applications/{id} | 
 *AuthenticationApi* | [**create_login**](docs/AuthenticationApi.md#create_login) | **POST** /login | 
 *AuthenticationApi* | [**get_logout**](docs/AuthenticationApi.md#get_logout) | **GET** /logout | 
 *BackupApi* | [**create_system_backup_restore_by_id**](docs/BackupApi.md#create_system_backup_restore_by_id) | **POST** /api/v1/system/backup/restore/{id} | 
 *BackupApi* | [**create_system_backup_restore_upload**](docs/BackupApi.md#create_system_backup_restore_upload) | **POST** /api/v1/system/backup/restore/upload | 
@@ -145,56 +147,56 @@
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v1/customfilter/{id} | 
 *DevelopmentConfigApi* | [**get_development_config**](docs/DevelopmentConfigApi.md#get_development_config) | **GET** /api/v1/config/development | 
 *DevelopmentConfigApi* | [**get_development_config_by_id**](docs/DevelopmentConfigApi.md#get_development_config_by_id) | **GET** /api/v1/config/development/{id} | 
 *DevelopmentConfigApi* | [**update_development_config**](docs/DevelopmentConfigApi.md#update_development_config) | **PUT** /api/v1/config/development/{id} | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v1/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v1/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v1/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v1/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v1/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_indexer**](docs/HistoryApi.md#list_history_indexer) | **GET** /api/v1/history/indexer | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v1/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v1/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v1/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v1/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v1/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v1/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v1/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v1/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v1/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v1/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v1/indexer/{id} | 
 *IndexerDefaultCategoriesApi* | [**list_indexer_categories**](docs/IndexerDefaultCategoriesApi.md#list_indexer_categories) | **GET** /api/v1/indexer/categories | 
-*IndexerEditorApi* | [**delete_indexer_editor**](docs/IndexerEditorApi.md#delete_indexer_editor) | **DELETE** /api/v1/indexer/editor | 
-*IndexerEditorApi* | [**put_indexer_editor**](docs/IndexerEditorApi.md#put_indexer_editor) | **PUT** /api/v1/indexer/editor | 
 *IndexerProxyApi* | [**create_indexer_proxy**](docs/IndexerProxyApi.md#create_indexer_proxy) | **POST** /api/v1/indexerproxy | 
 *IndexerProxyApi* | [**create_indexer_proxy_action_by_name**](docs/IndexerProxyApi.md#create_indexer_proxy_action_by_name) | **POST** /api/v1/indexerproxy/action/{name} | 
 *IndexerProxyApi* | [**delete_indexer_proxy**](docs/IndexerProxyApi.md#delete_indexer_proxy) | **DELETE** /api/v1/indexerproxy/{id} | 
 *IndexerProxyApi* | [**get_indexer_proxy_by_id**](docs/IndexerProxyApi.md#get_indexer_proxy_by_id) | **GET** /api/v1/indexerproxy/{id} | 
 *IndexerProxyApi* | [**list_indexer_proxy**](docs/IndexerProxyApi.md#list_indexer_proxy) | **GET** /api/v1/indexerproxy | 
 *IndexerProxyApi* | [**list_indexer_proxy_schema**](docs/IndexerProxyApi.md#list_indexer_proxy_schema) | **GET** /api/v1/indexerproxy/schema | 
 *IndexerProxyApi* | [**test_indexer_proxy**](docs/IndexerProxyApi.md#test_indexer_proxy) | **POST** /api/v1/indexerproxy/test | 
 *IndexerProxyApi* | [**testall_indexer_proxy**](docs/IndexerProxyApi.md#testall_indexer_proxy) | **POST** /api/v1/indexerproxy/testall | 
 *IndexerProxyApi* | [**update_indexer_proxy**](docs/IndexerProxyApi.md#update_indexer_proxy) | **PUT** /api/v1/indexerproxy/{id} | 
 *IndexerStatsApi* | [**get_indexer_stats**](docs/IndexerStatsApi.md#get_indexer_stats) | **GET** /api/v1/indexerstats | 
-*IndexerStatusApi* | [**get_indexer_status_by_id**](docs/IndexerStatusApi.md#get_indexer_status_by_id) | **GET** /api/v1/indexerstatus/{id} | 
 *IndexerStatusApi* | [**list_indexer_status**](docs/IndexerStatusApi.md#list_indexer_status) | **GET** /api/v1/indexerstatus | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v1/localization | 
 *LocalizationApi* | [**list_localization_options**](docs/LocalizationApi.md#list_localization_options) | **GET** /api/v1/localization/options | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v1/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v1/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v1/log/file | 
@@ -211,15 +213,14 @@
 *NotificationApi* | [**test_notification**](docs/NotificationApi.md#test_notification) | **POST** /api/v1/notification/test | 
 *NotificationApi* | [**testall_notification**](docs/NotificationApi.md#testall_notification) | **POST** /api/v1/notification/testall | 
 *NotificationApi* | [**update_notification**](docs/NotificationApi.md#update_notification) | **PUT** /api/v1/notification/{id} | 
 *PingApi* | [**get_ping**](docs/PingApi.md#get_ping) | **GET** /ping | 
 *QualityProfileSchemaApi* | [**get_appprofile_schema**](docs/QualityProfileSchemaApi.md#get_appprofile_schema) | **GET** /api/v1/appprofile/schema | 
 *SearchApi* | [**create_search**](docs/SearchApi.md#create_search) | **POST** /api/v1/search | 
 *SearchApi* | [**create_search_bulk**](docs/SearchApi.md#create_search_bulk) | **POST** /api/v1/search/bulk | 
-*SearchApi* | [**get_search_by_id**](docs/SearchApi.md#get_search_by_id) | **GET** /api/v1/search/{id} | 
 *SearchApi* | [**list_search**](docs/SearchApi.md#list_search) | **GET** /api/v1/search | 
 *StaticResourceApi* | [**get**](docs/StaticResourceApi.md#get) | **GET** / | 
 *StaticResourceApi* | [**get_by_path**](docs/StaticResourceApi.md#get_by_path) | **GET** /{path} | 
 *StaticResourceApi* | [**get_content_by_path**](docs/StaticResourceApi.md#get_content_by_path) | **GET** /content/{path} | 
 *StaticResourceApi* | [**get_login**](docs/StaticResourceApi.md#get_login) | **GET** /login | 
 *SystemApi* | [**create_system_restart**](docs/SystemApi.md#create_system_restart) | **POST** /api/v1/system/restart | 
 *SystemApi* | [**create_system_shutdown**](docs/SystemApi.md#create_system_shutdown) | **POST** /api/v1/system/shutdown | 
@@ -243,14 +244,15 @@
 *UpdateLogFileApi* | [**list_log_file_update**](docs/UpdateLogFileApi.md#list_log_file_update) | **GET** /api/v1/log/file/update | 
 
 
 ## Documentation For Models
 
  - [ApiInfoResource](docs/ApiInfoResource.md)
  - [AppProfileResource](docs/AppProfileResource.md)
+ - [ApplicationBulkResource](docs/ApplicationBulkResource.md)
  - [ApplicationResource](docs/ApplicationResource.md)
  - [ApplicationSyncLevel](docs/ApplicationSyncLevel.md)
  - [ApplyTags](docs/ApplyTags.md)
  - [AuthenticationRequiredType](docs/AuthenticationRequiredType.md)
  - [AuthenticationType](docs/AuthenticationType.md)
  - [BackupResource](docs/BackupResource.md)
  - [BackupType](docs/BackupType.md)
@@ -260,29 +262,30 @@
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientCategory](docs/DownloadClientCategory.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Field](docs/Field.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryEventType](docs/HistoryEventType.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [HostStatistics](docs/HostStatistics.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerCapabilityResource](docs/IndexerCapabilityResource.md)
  - [IndexerCategory](docs/IndexerCategory.md)
- - [IndexerEditorResource](docs/IndexerEditorResource.md)
  - [IndexerPrivacy](docs/IndexerPrivacy.md)
  - [IndexerProxyResource](docs/IndexerProxyResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IndexerStatistics](docs/IndexerStatistics.md)
  - [IndexerStatsResource](docs/IndexerStatsResource.md)
  - [IndexerStatusResource](docs/IndexerStatusResource.md)
  - [LocalizationOption](docs/LocalizationOption.md)
```

### Comparing `prowlarr-py-0.4.0/README.md` & `prowlarr-py-0.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # prowlarr-py
 Prowlarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.4.0
+- Package version: 0.4.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -105,17 +105,19 @@
 *AppProfileApi* | [**delete_app_profile**](docs/AppProfileApi.md#delete_app_profile) | **DELETE** /api/v1/appprofile/{id} | 
 *AppProfileApi* | [**get_app_profile_by_id**](docs/AppProfileApi.md#get_app_profile_by_id) | **GET** /api/v1/appprofile/{id} | 
 *AppProfileApi* | [**list_app_profile**](docs/AppProfileApi.md#list_app_profile) | **GET** /api/v1/appprofile | 
 *AppProfileApi* | [**update_app_profile**](docs/AppProfileApi.md#update_app_profile) | **PUT** /api/v1/appprofile/{id} | 
 *ApplicationApi* | [**create_applications**](docs/ApplicationApi.md#create_applications) | **POST** /api/v1/applications | 
 *ApplicationApi* | [**create_applications_action_by_name**](docs/ApplicationApi.md#create_applications_action_by_name) | **POST** /api/v1/applications/action/{name} | 
 *ApplicationApi* | [**delete_applications**](docs/ApplicationApi.md#delete_applications) | **DELETE** /api/v1/applications/{id} | 
+*ApplicationApi* | [**delete_applications_bulk**](docs/ApplicationApi.md#delete_applications_bulk) | **DELETE** /api/v1/applications/bulk | 
 *ApplicationApi* | [**get_applications_by_id**](docs/ApplicationApi.md#get_applications_by_id) | **GET** /api/v1/applications/{id} | 
 *ApplicationApi* | [**list_applications**](docs/ApplicationApi.md#list_applications) | **GET** /api/v1/applications | 
 *ApplicationApi* | [**list_applications_schema**](docs/ApplicationApi.md#list_applications_schema) | **GET** /api/v1/applications/schema | 
+*ApplicationApi* | [**put_applications_bulk**](docs/ApplicationApi.md#put_applications_bulk) | **PUT** /api/v1/applications/bulk | 
 *ApplicationApi* | [**test_applications**](docs/ApplicationApi.md#test_applications) | **POST** /api/v1/applications/test | 
 *ApplicationApi* | [**testall_applications**](docs/ApplicationApi.md#testall_applications) | **POST** /api/v1/applications/testall | 
 *ApplicationApi* | [**update_applications**](docs/ApplicationApi.md#update_applications) | **PUT** /api/v1/applications/{id} | 
 *AuthenticationApi* | [**create_login**](docs/AuthenticationApi.md#create_login) | **POST** /login | 
 *AuthenticationApi* | [**get_logout**](docs/AuthenticationApi.md#get_logout) | **GET** /logout | 
 *BackupApi* | [**create_system_backup_restore_by_id**](docs/BackupApi.md#create_system_backup_restore_by_id) | **POST** /api/v1/system/backup/restore/{id} | 
 *BackupApi* | [**create_system_backup_restore_upload**](docs/BackupApi.md#create_system_backup_restore_upload) | **POST** /api/v1/system/backup/restore/upload | 
@@ -132,56 +134,56 @@
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v1/customfilter/{id} | 
 *DevelopmentConfigApi* | [**get_development_config**](docs/DevelopmentConfigApi.md#get_development_config) | **GET** /api/v1/config/development | 
 *DevelopmentConfigApi* | [**get_development_config_by_id**](docs/DevelopmentConfigApi.md#get_development_config_by_id) | **GET** /api/v1/config/development/{id} | 
 *DevelopmentConfigApi* | [**update_development_config**](docs/DevelopmentConfigApi.md#update_development_config) | **PUT** /api/v1/config/development/{id} | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v1/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v1/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v1/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v1/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v1/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_indexer**](docs/HistoryApi.md#list_history_indexer) | **GET** /api/v1/history/indexer | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v1/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v1/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v1/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v1/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v1/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v1/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v1/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v1/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v1/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v1/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v1/indexer/{id} | 
 *IndexerDefaultCategoriesApi* | [**list_indexer_categories**](docs/IndexerDefaultCategoriesApi.md#list_indexer_categories) | **GET** /api/v1/indexer/categories | 
-*IndexerEditorApi* | [**delete_indexer_editor**](docs/IndexerEditorApi.md#delete_indexer_editor) | **DELETE** /api/v1/indexer/editor | 
-*IndexerEditorApi* | [**put_indexer_editor**](docs/IndexerEditorApi.md#put_indexer_editor) | **PUT** /api/v1/indexer/editor | 
 *IndexerProxyApi* | [**create_indexer_proxy**](docs/IndexerProxyApi.md#create_indexer_proxy) | **POST** /api/v1/indexerproxy | 
 *IndexerProxyApi* | [**create_indexer_proxy_action_by_name**](docs/IndexerProxyApi.md#create_indexer_proxy_action_by_name) | **POST** /api/v1/indexerproxy/action/{name} | 
 *IndexerProxyApi* | [**delete_indexer_proxy**](docs/IndexerProxyApi.md#delete_indexer_proxy) | **DELETE** /api/v1/indexerproxy/{id} | 
 *IndexerProxyApi* | [**get_indexer_proxy_by_id**](docs/IndexerProxyApi.md#get_indexer_proxy_by_id) | **GET** /api/v1/indexerproxy/{id} | 
 *IndexerProxyApi* | [**list_indexer_proxy**](docs/IndexerProxyApi.md#list_indexer_proxy) | **GET** /api/v1/indexerproxy | 
 *IndexerProxyApi* | [**list_indexer_proxy_schema**](docs/IndexerProxyApi.md#list_indexer_proxy_schema) | **GET** /api/v1/indexerproxy/schema | 
 *IndexerProxyApi* | [**test_indexer_proxy**](docs/IndexerProxyApi.md#test_indexer_proxy) | **POST** /api/v1/indexerproxy/test | 
 *IndexerProxyApi* | [**testall_indexer_proxy**](docs/IndexerProxyApi.md#testall_indexer_proxy) | **POST** /api/v1/indexerproxy/testall | 
 *IndexerProxyApi* | [**update_indexer_proxy**](docs/IndexerProxyApi.md#update_indexer_proxy) | **PUT** /api/v1/indexerproxy/{id} | 
 *IndexerStatsApi* | [**get_indexer_stats**](docs/IndexerStatsApi.md#get_indexer_stats) | **GET** /api/v1/indexerstats | 
-*IndexerStatusApi* | [**get_indexer_status_by_id**](docs/IndexerStatusApi.md#get_indexer_status_by_id) | **GET** /api/v1/indexerstatus/{id} | 
 *IndexerStatusApi* | [**list_indexer_status**](docs/IndexerStatusApi.md#list_indexer_status) | **GET** /api/v1/indexerstatus | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v1/localization | 
 *LocalizationApi* | [**list_localization_options**](docs/LocalizationApi.md#list_localization_options) | **GET** /api/v1/localization/options | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v1/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v1/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v1/log/file | 
@@ -198,15 +200,14 @@
 *NotificationApi* | [**test_notification**](docs/NotificationApi.md#test_notification) | **POST** /api/v1/notification/test | 
 *NotificationApi* | [**testall_notification**](docs/NotificationApi.md#testall_notification) | **POST** /api/v1/notification/testall | 
 *NotificationApi* | [**update_notification**](docs/NotificationApi.md#update_notification) | **PUT** /api/v1/notification/{id} | 
 *PingApi* | [**get_ping**](docs/PingApi.md#get_ping) | **GET** /ping | 
 *QualityProfileSchemaApi* | [**get_appprofile_schema**](docs/QualityProfileSchemaApi.md#get_appprofile_schema) | **GET** /api/v1/appprofile/schema | 
 *SearchApi* | [**create_search**](docs/SearchApi.md#create_search) | **POST** /api/v1/search | 
 *SearchApi* | [**create_search_bulk**](docs/SearchApi.md#create_search_bulk) | **POST** /api/v1/search/bulk | 
-*SearchApi* | [**get_search_by_id**](docs/SearchApi.md#get_search_by_id) | **GET** /api/v1/search/{id} | 
 *SearchApi* | [**list_search**](docs/SearchApi.md#list_search) | **GET** /api/v1/search | 
 *StaticResourceApi* | [**get**](docs/StaticResourceApi.md#get) | **GET** / | 
 *StaticResourceApi* | [**get_by_path**](docs/StaticResourceApi.md#get_by_path) | **GET** /{path} | 
 *StaticResourceApi* | [**get_content_by_path**](docs/StaticResourceApi.md#get_content_by_path) | **GET** /content/{path} | 
 *StaticResourceApi* | [**get_login**](docs/StaticResourceApi.md#get_login) | **GET** /login | 
 *SystemApi* | [**create_system_restart**](docs/SystemApi.md#create_system_restart) | **POST** /api/v1/system/restart | 
 *SystemApi* | [**create_system_shutdown**](docs/SystemApi.md#create_system_shutdown) | **POST** /api/v1/system/shutdown | 
@@ -230,14 +231,15 @@
 *UpdateLogFileApi* | [**list_log_file_update**](docs/UpdateLogFileApi.md#list_log_file_update) | **GET** /api/v1/log/file/update | 
 
 
 ## Documentation For Models
 
  - [ApiInfoResource](docs/ApiInfoResource.md)
  - [AppProfileResource](docs/AppProfileResource.md)
+ - [ApplicationBulkResource](docs/ApplicationBulkResource.md)
  - [ApplicationResource](docs/ApplicationResource.md)
  - [ApplicationSyncLevel](docs/ApplicationSyncLevel.md)
  - [ApplyTags](docs/ApplyTags.md)
  - [AuthenticationRequiredType](docs/AuthenticationRequiredType.md)
  - [AuthenticationType](docs/AuthenticationType.md)
  - [BackupResource](docs/BackupResource.md)
  - [BackupType](docs/BackupType.md)
@@ -247,29 +249,30 @@
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientCategory](docs/DownloadClientCategory.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Field](docs/Field.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryEventType](docs/HistoryEventType.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [HostStatistics](docs/HostStatistics.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerCapabilityResource](docs/IndexerCapabilityResource.md)
  - [IndexerCategory](docs/IndexerCategory.md)
- - [IndexerEditorResource](docs/IndexerEditorResource.md)
  - [IndexerPrivacy](docs/IndexerPrivacy.md)
  - [IndexerProxyResource](docs/IndexerProxyResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IndexerStatistics](docs/IndexerStatistics.md)
  - [IndexerStatsResource](docs/IndexerStatsResource.md)
  - [IndexerStatusResource](docs/IndexerStatusResource.md)
  - [LocalizationOption](docs/LocalizationOption.md)
```

### Comparing `prowlarr-py-0.4.0/prowlarr/__init__.py` & `prowlarr-py-0.4.1/prowlarr/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 # x-release-please-end
 
 # import apis into sdk package
 from prowlarr.api.api_info_api import ApiInfoApi
 from prowlarr.api.app_profile_api import AppProfileApi
 from prowlarr.api.application_api import ApplicationApi
 from prowlarr.api.authentication_api import AuthenticationApi
@@ -31,15 +31,14 @@
 from prowlarr.api.download_client_config_api import DownloadClientConfigApi
 from prowlarr.api.file_system_api import FileSystemApi
 from prowlarr.api.health_api import HealthApi
 from prowlarr.api.history_api import HistoryApi
 from prowlarr.api.host_config_api import HostConfigApi
 from prowlarr.api.indexer_api import IndexerApi
 from prowlarr.api.indexer_default_categories_api import IndexerDefaultCategoriesApi
-from prowlarr.api.indexer_editor_api import IndexerEditorApi
 from prowlarr.api.indexer_proxy_api import IndexerProxyApi
 from prowlarr.api.indexer_stats_api import IndexerStatsApi
 from prowlarr.api.indexer_status_api import IndexerStatusApi
 from prowlarr.api.initialize_js_api import InitializeJsApi
 from prowlarr.api.localization_api import LocalizationApi
 from prowlarr.api.log_api import LogApi
 from prowlarr.api.log_file_api import LogFileApi
@@ -65,14 +64,15 @@
 from prowlarr.exceptions import ApiValueError
 from prowlarr.exceptions import ApiKeyError
 from prowlarr.exceptions import ApiAttributeError
 from prowlarr.exceptions import ApiException
 # import models into sdk package
 from prowlarr.models.api_info_resource import ApiInfoResource
 from prowlarr.models.app_profile_resource import AppProfileResource
+from prowlarr.models.application_bulk_resource import ApplicationBulkResource
 from prowlarr.models.application_resource import ApplicationResource
 from prowlarr.models.application_sync_level import ApplicationSyncLevel
 from prowlarr.models.apply_tags import ApplyTags
 from prowlarr.models.authentication_required_type import AuthenticationRequiredType
 from prowlarr.models.authentication_type import AuthenticationType
 from prowlarr.models.backup_resource import BackupResource
 from prowlarr.models.backup_type import BackupType
@@ -82,29 +82,30 @@
 from prowlarr.models.command_priority import CommandPriority
 from prowlarr.models.command_resource import CommandResource
 from prowlarr.models.command_status import CommandStatus
 from prowlarr.models.command_trigger import CommandTrigger
 from prowlarr.models.custom_filter_resource import CustomFilterResource
 from prowlarr.models.database_type import DatabaseType
 from prowlarr.models.development_config_resource import DevelopmentConfigResource
+from prowlarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from prowlarr.models.download_client_category import DownloadClientCategory
 from prowlarr.models.download_client_config_resource import DownloadClientConfigResource
 from prowlarr.models.download_client_resource import DownloadClientResource
 from prowlarr.models.download_protocol import DownloadProtocol
 from prowlarr.models.field import Field
 from prowlarr.models.health_check_result import HealthCheckResult
 from prowlarr.models.health_resource import HealthResource
 from prowlarr.models.history_event_type import HistoryEventType
 from prowlarr.models.history_resource import HistoryResource
 from prowlarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from prowlarr.models.host_config_resource import HostConfigResource
 from prowlarr.models.host_statistics import HostStatistics
+from prowlarr.models.indexer_bulk_resource import IndexerBulkResource
 from prowlarr.models.indexer_capability_resource import IndexerCapabilityResource
 from prowlarr.models.indexer_category import IndexerCategory
-from prowlarr.models.indexer_editor_resource import IndexerEditorResource
 from prowlarr.models.indexer_privacy import IndexerPrivacy
 from prowlarr.models.indexer_proxy_resource import IndexerProxyResource
 from prowlarr.models.indexer_resource import IndexerResource
 from prowlarr.models.indexer_statistics import IndexerStatistics
 from prowlarr.models.indexer_stats_resource import IndexerStatsResource
 from prowlarr.models.indexer_status_resource import IndexerStatusResource
 from prowlarr.models.localization_option import LocalizationOption
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/__init__.py` & `prowlarr-py-0.4.1/prowlarr/api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from prowlarr.api.download_client_config_api import DownloadClientConfigApi
 from prowlarr.api.file_system_api import FileSystemApi
 from prowlarr.api.health_api import HealthApi
 from prowlarr.api.history_api import HistoryApi
 from prowlarr.api.host_config_api import HostConfigApi
 from prowlarr.api.indexer_api import IndexerApi
 from prowlarr.api.indexer_default_categories_api import IndexerDefaultCategoriesApi
-from prowlarr.api.indexer_editor_api import IndexerEditorApi
 from prowlarr.api.indexer_proxy_api import IndexerProxyApi
 from prowlarr.api.indexer_stats_api import IndexerStatsApi
 from prowlarr.api.indexer_status_api import IndexerStatusApi
 from prowlarr.api.initialize_js_api import InitializeJsApi
 from prowlarr.api.localization_api import LocalizationApi
 from prowlarr.api.log_api import LogApi
 from prowlarr.api.log_file_api import LogFileApi
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/api_info_api.py` & `prowlarr-py-0.4.1/prowlarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/app_profile_api.py` & `prowlarr-py-0.4.1/prowlarr/api/app_profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -725,15 +725,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/application_api.py` & `prowlarr-py-0.4.1/prowlarr/api/application_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from prowlarr.models.application_bulk_resource import ApplicationBulkResource
 from prowlarr.models.application_resource import ApplicationResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -39,23 +40,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_applications(self, application_resource : Optional[ApplicationResource] = None, **kwargs) -> ApplicationResource:  # noqa: E501
+    def create_applications(self, force_save : Optional[StrictBool] = None, application_resource : Optional[ApplicationResource] = None, **kwargs) -> ApplicationResource:  # noqa: E501
         """create_applications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_applications(application_resource, async_req=True)
+        >>> thread = api.create_applications(force_save, application_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param application_resource:
         :type application_resource: ApplicationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -66,26 +69,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ApplicationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_applications_with_http_info(application_resource, **kwargs)  # noqa: E501
+        return self.create_applications_with_http_info(force_save, application_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_applications_with_http_info(self, application_resource : Optional[ApplicationResource] = None, **kwargs):  # noqa: E501
+    def create_applications_with_http_info(self, force_save : Optional[StrictBool] = None, application_resource : Optional[ApplicationResource] = None, **kwargs):  # noqa: E501
         """create_applications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_applications_with_http_info(application_resource, async_req=True)
+        >>> thread = api.create_applications_with_http_info(force_save, application_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param application_resource:
         :type application_resource: ApplicationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +112,15 @@
                  returns the request thread.
         :rtype: tuple(ApplicationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'application_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -138,14 +144,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -158,15 +166,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -309,15 +317,15 @@
         _body_params = None
         if _params['application_resource']:
             _body_params = _params['application_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -471,14 +479,156 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def delete_applications_bulk(self, application_bulk_resource : Optional[ApplicationBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_applications_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_applications_bulk(application_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param application_bulk_resource:
+        :type application_bulk_resource: ApplicationBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_applications_bulk_with_http_info(application_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_applications_bulk_with_http_info(self, application_bulk_resource : Optional[ApplicationBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_applications_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_applications_bulk_with_http_info(application_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param application_bulk_resource:
+        :type application_bulk_resource: ApplicationBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'application_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_applications_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['application_bulk_resource']:
+            _body_params = _params['application_bulk_resource']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/v1/applications/bulk', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_applications_by_id(self, id : StrictInt, **kwargs) -> ApplicationResource:  # noqa: E501
         """get_applications_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_applications_by_id(id, async_req=True)
@@ -585,15 +735,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ApplicationResource",
         }
@@ -880,14 +1030,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def put_applications_bulk(self, application_bulk_resource : Optional[ApplicationBulkResource] = None, **kwargs) -> ApplicationResource:  # noqa: E501
+        """put_applications_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_applications_bulk(application_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param application_bulk_resource:
+        :type application_bulk_resource: ApplicationBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ApplicationResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.put_applications_bulk_with_http_info(application_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_applications_bulk_with_http_info(self, application_bulk_resource : Optional[ApplicationBulkResource] = None, **kwargs):  # noqa: E501
+        """put_applications_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_applications_bulk_with_http_info(application_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param application_bulk_resource:
+        :type application_bulk_resource: ApplicationBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(ApplicationResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'application_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method put_applications_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['application_bulk_resource']:
+            _body_params = _params['application_bulk_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "ApplicationResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/applications/bulk', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def test_applications(self, application_resource : Optional[ApplicationResource] = None, **kwargs) -> None:  # noqa: E501
         """test_applications  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.test_applications(application_resource, async_req=True)
@@ -995,15 +1293,15 @@
         _body_params = None
         if _params['application_resource']:
             _body_params = _params['application_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -1283,15 +1581,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/authentication_api.py` & `prowlarr-py-0.4.1/prowlarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/backup_api.py` & `prowlarr-py-0.4.1/prowlarr/api/backup_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -544,15 +544,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[BackupResource]",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/command_api.py` & `prowlarr-py-0.4.1/prowlarr/api/command_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CommandResource",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/custom_filter_api.py` & `prowlarr-py-0.4.1/prowlarr/api/custom_filter_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CustomFilterResource",
         }
@@ -723,15 +723,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/development_config_api.py` & `prowlarr-py-0.4.1/prowlarr/api/development_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DevelopmentConfigResource",
         }
@@ -440,15 +440,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/download_client_api.py` & `prowlarr-py-0.4.1/prowlarr/api/download_client_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from prowlarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from prowlarr.models.download_client_resource import DownloadClientResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -39,23 +40,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_download_client(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
+    def create_download_client(self, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
         """create_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client(download_client_resource, async_req=True)
+        >>> thread = api.create_download_client(force_save, download_client_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param download_client_resource:
         :type download_client_resource: DownloadClientResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -66,26 +69,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DownloadClientResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_download_client_with_http_info(download_client_resource, **kwargs)  # noqa: E501
+        return self.create_download_client_with_http_info(force_save, download_client_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_download_client_with_http_info(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
+    def create_download_client_with_http_info(self, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
         """create_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_with_http_info(download_client_resource, async_req=True)
+        >>> thread = api.create_download_client_with_http_info(force_save, download_client_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param download_client_resource:
         :type download_client_resource: DownloadClientResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +112,15 @@
                  returns the request thread.
         :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'download_client_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -138,14 +144,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -158,15 +166,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -309,15 +317,15 @@
         _body_params = None
         if _params['download_client_resource']:
             _body_params = _params['download_client_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -471,14 +479,156 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def delete_download_client_bulk(self, download_client_bulk_resource : Optional[DownloadClientBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_download_client_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_download_client_bulk(download_client_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param download_client_bulk_resource:
+        :type download_client_bulk_resource: DownloadClientBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_download_client_bulk_with_http_info(download_client_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_download_client_bulk_with_http_info(self, download_client_bulk_resource : Optional[DownloadClientBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_download_client_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_download_client_bulk_with_http_info(download_client_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param download_client_bulk_resource:
+        :type download_client_bulk_resource: DownloadClientBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'download_client_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_download_client_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['download_client_bulk_resource']:
+            _body_params = _params['download_client_bulk_resource']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/v1/downloadclient/bulk', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_download_client_by_id(self, id : StrictInt, **kwargs) -> DownloadClientResource:  # noqa: E501
         """get_download_client_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_download_client_by_id(id, async_req=True)
@@ -585,15 +735,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientResource",
         }
@@ -880,14 +1030,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def put_download_client_bulk(self, download_client_bulk_resource : Optional[DownloadClientBulkResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
+        """put_download_client_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_download_client_bulk(download_client_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param download_client_bulk_resource:
+        :type download_client_bulk_resource: DownloadClientBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: DownloadClientResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.put_download_client_bulk_with_http_info(download_client_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_download_client_bulk_with_http_info(self, download_client_bulk_resource : Optional[DownloadClientBulkResource] = None, **kwargs):  # noqa: E501
+        """put_download_client_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_download_client_bulk_with_http_info(download_client_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param download_client_bulk_resource:
+        :type download_client_bulk_resource: DownloadClientBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'download_client_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method put_download_client_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['download_client_bulk_resource']:
+            _body_params = _params['download_client_bulk_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "DownloadClientResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/downloadclient/bulk', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def test_download_client(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> None:  # noqa: E501
         """test_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.test_download_client(download_client_resource, async_req=True)
@@ -995,15 +1293,15 @@
         _body_params = None
         if _params['download_client_resource']:
             _body_params = _params['download_client_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -1283,15 +1581,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/download_client_config_api.py` & `prowlarr-py-0.4.1/prowlarr/api/download_client_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientConfigResource",
         }
@@ -440,15 +440,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/file_system_api.py` & `prowlarr-py-0.4.1/prowlarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/health_api.py` & `prowlarr-py-0.4.1/prowlarr/api/update_log_file_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,81 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import constr, validator
 
-from typing import List
+from typing import Any, Dict, List
 
-from prowlarr.models.health_resource import HealthResource
+from prowlarr.models.log_file_resource import LogFileResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class HealthApi(object):
+class UpdateLogFileApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_health_by_id(self, id : StrictInt, **kwargs) -> HealthResource:  # noqa: E501
-        """get_health_by_id  # noqa: E501
+    def get_log_file_update_by_filename(self, filename : constr(strict=True), **kwargs) -> object:  # noqa: E501
+        """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id(id, async_req=True)
+        >>> thread = api.get_log_file_update_by_filename(filename, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param filename: (required)
+        :type filename: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: HealthResource
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_health_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_log_file_update_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_health_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_health_by_id  # noqa: E501
+    def get_log_file_update_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
+        """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_log_file_update_by_filename_with_http_info(filename, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param filename: (required)
+        :type filename: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(HealthResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'filename'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,25 +126,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_health_by_id" % _key
+                    " to method get_log_file_update_by_filename" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
+        if _params['filename']:
+            _path_params['filename'] = _params['filename']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -153,25 +153,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['text/plain'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "HealthResource",
+            '200': "object",
         }
 
         return self.api_client.call_api(
-            '/api/v1/health/{id}', 'GET',
+            '/api/v1/log/file/update/{filename}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,21 +180,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_health(self, **kwargs) -> List[HealthResource]:  # noqa: E501
-        """list_health  # noqa: E501
+    def list_log_file_update(self, **kwargs) -> List[LogFileResource]:  # noqa: E501
+        """list_log_file_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health(async_req=True)
+        >>> thread = api.list_log_file_update(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -202,27 +202,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[HealthResource]
+        :rtype: List[LogFileResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_health_with_http_info(**kwargs)  # noqa: E501
+        return self.list_log_file_update_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_health_with_http_info(self, **kwargs):  # noqa: E501
-        """list_health  # noqa: E501
+    def list_log_file_update_with_http_info(self, **kwargs):  # noqa: E501
+        """list_log_file_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health_with_http_info(async_req=True)
+        >>> thread = api.list_log_file_update_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -238,15 +238,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[HealthResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[LogFileResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -262,15 +262,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_health" % _key
+                    " to method list_log_file_update" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -293,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[HealthResource]",
+            '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/health', 'GET',
+            '/api/v1/log/file/update', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/history_api.py` & `prowlarr-py-0.4.1/prowlarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/host_config_api.py` & `prowlarr-py-0.4.1/prowlarr/api/host_config_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HostConfigResource",
         }
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HostConfigResource",
         }
@@ -435,20 +435,20 @@
         # process the body parameter
         _body_params = None
         if _params['host_config_resource']:
             _body_params = _params['host_config_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/indexer_api.py` & `prowlarr-py-0.4.1/prowlarr/api/indexer_proxy_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,77 +17,81 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from prowlarr.models.indexer_resource import IndexerResource
+from prowlarr.models.indexer_proxy_resource import IndexerProxyResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class IndexerApi(object):
+class IndexerProxyApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
-        """create_indexer  # noqa: E501
+    def create_indexer_proxy(self, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> IndexerProxyResource:  # noqa: E501
+        """create_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer(indexer_resource, async_req=True)
+        >>> thread = api.create_indexer_proxy(force_save, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param force_save:
+        :type force_save: bool
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerResource
+        :rtype: IndexerProxyResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_proxy_with_http_info(force_save, indexer_proxy_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """create_indexer  # noqa: E501
+    def create_indexer_proxy_with_http_info(self, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
+        """create_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_with_http_info(indexer_resource, async_req=True)
+        >>> thread = api.create_indexer_proxy_with_http_info(force_save, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param force_save:
+        :type force_save: bool
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +105,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_resource'
+            'force_save',
+            'indexer_proxy_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,59 +131,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_indexer" % _key
+                    " to method create_indexer_proxy" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_resource']:
-            _body_params = _params['indexer_resource']
+        if _params['indexer_proxy_resource']:
+            _body_params = _params['indexer_proxy_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerResource",
+            '200': "IndexerProxyResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexer', 'POST',
+            '/api/v1/indexerproxy', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,27 +194,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_indexer_action_by_name(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_indexer_action_by_name  # noqa: E501
+    def create_indexer_proxy_action_by_name(self, name : StrictStr, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_indexer_proxy_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_action_by_name(name, indexer_resource, async_req=True)
+        >>> thread = api.create_indexer_proxy_action_by_name(name, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -216,30 +223,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_action_by_name_with_http_info(name, indexer_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_proxy_action_by_name_with_http_info(name, indexer_proxy_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_action_by_name_with_http_info(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """create_indexer_action_by_name  # noqa: E501
+    def create_indexer_proxy_action_by_name_with_http_info(self, name : StrictStr, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
+        """create_indexer_proxy_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_action_by_name_with_http_info(name, indexer_resource, async_req=True)
+        >>> thread = api.create_indexer_proxy_action_by_name_with_http_info(name, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -260,15 +267,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'name',
-            'indexer_resource'
+            'indexer_proxy_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -279,15 +286,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_indexer_action_by_name" % _key
+                    " to method create_indexer_proxy_action_by_name" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -303,31 +310,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_resource']:
-            _body_params = _params['indexer_resource']
+        if _params['indexer_proxy_resource']:
+            _body_params = _params['indexer_proxy_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexer/action/{name}', 'POST',
+            '/api/v1/indexerproxy/action/{name}', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -336,21 +343,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_indexer(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_indexer  # noqa: E501
+    def delete_indexer_proxy(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer(id, async_req=True)
+        >>> thread = api.delete_indexer_proxy(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -363,24 +370,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_indexer_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_indexer_proxy_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_indexer_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_indexer  # noqa: E501
+    def delete_indexer_proxy_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer_with_http_info(id, async_req=True)
+        >>> thread = api.delete_indexer_proxy_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -423,15 +430,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_indexer" % _key
+                    " to method delete_indexer_proxy" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -454,15 +461,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexer/{id}', 'DELETE',
+            '/api/v1/indexerproxy/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -471,21 +478,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_indexer_by_id(self, id : StrictInt, **kwargs) -> IndexerResource:  # noqa: E501
-        """get_indexer_by_id  # noqa: E501
+    def get_indexer_proxy_by_id(self, id : StrictInt, **kwargs) -> IndexerProxyResource:  # noqa: E501
+        """get_indexer_proxy_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_by_id(id, async_req=True)
+        >>> thread = api.get_indexer_proxy_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -495,27 +502,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerResource
+        :rtype: IndexerProxyResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_indexer_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_indexer_proxy_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_indexer_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_indexer_by_id  # noqa: E501
+    def get_indexer_proxy_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_indexer_proxy_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_indexer_proxy_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -533,15 +540,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -558,15 +565,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_indexer_by_id" % _key
+                    " to method get_indexer_proxy_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -585,25 +592,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerResource",
+            '200': "IndexerProxyResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexer/{id}', 'GET',
+            '/api/v1/indexerproxy/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -612,21 +619,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_indexer(self, **kwargs) -> List[IndexerResource]:  # noqa: E501
-        """list_indexer  # noqa: E501
+    def list_indexer_proxy(self, **kwargs) -> List[IndexerProxyResource]:  # noqa: E501
+        """list_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer(async_req=True)
+        >>> thread = api.list_indexer_proxy(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -634,27 +641,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[IndexerResource]
+        :rtype: List[IndexerProxyResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_with_http_info(**kwargs)  # noqa: E501
+        return self.list_indexer_proxy_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer  # noqa: E501
+    def list_indexer_proxy_with_http_info(self, **kwargs):  # noqa: E501
+        """list_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_with_http_info(async_req=True)
+        >>> thread = api.list_indexer_proxy_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -670,15 +677,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[IndexerResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[IndexerProxyResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -694,15 +701,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_indexer" % _key
+                    " to method list_indexer_proxy" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -725,19 +732,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[IndexerResource]",
+            '200': "List[IndexerProxyResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexer', 'GET',
+            '/api/v1/indexerproxy', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -746,21 +753,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_indexer_schema(self, **kwargs) -> List[IndexerResource]:  # noqa: E501
-        """list_indexer_schema  # noqa: E501
+    def list_indexer_proxy_schema(self, **kwargs) -> List[IndexerProxyResource]:  # noqa: E501
+        """list_indexer_proxy_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_schema(async_req=True)
+        >>> thread = api.list_indexer_proxy_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -768,27 +775,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[IndexerResource]
+        :rtype: List[IndexerProxyResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_indexer_proxy_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer_schema  # noqa: E501
+    def list_indexer_proxy_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_indexer_proxy_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_schema_with_http_info(async_req=True)
+        >>> thread = api.list_indexer_proxy_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -804,15 +811,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[IndexerResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[IndexerProxyResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -828,15 +835,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_indexer_schema" % _key
+                    " to method list_indexer_proxy_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -859,19 +866,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[IndexerResource]",
+            '200': "List[IndexerProxyResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexer/schema', 'GET',
+            '/api/v1/indexerproxy/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -880,25 +887,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def test_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
-        """test_indexer  # noqa: E501
+    def test_indexer_proxy(self, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> None:  # noqa: E501
+        """test_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_indexer(indexer_resource, async_req=True)
+        >>> thread = api.test_indexer_proxy(indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -907,28 +914,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.test_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
+        return self.test_indexer_proxy_with_http_info(indexer_proxy_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """test_indexer  # noqa: E501
+    def test_indexer_proxy_with_http_info(self, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
+        """test_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_indexer_with_http_info(indexer_resource, async_req=True)
+        >>> thread = api.test_indexer_proxy_with_http_info(indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -948,15 +955,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_resource'
+            'indexer_proxy_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -967,15 +974,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method test_indexer" % _key
+                    " to method test_indexer_proxy" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -989,31 +996,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_resource']:
-            _body_params = _params['indexer_resource']
+        if _params['indexer_proxy_resource']:
+            _body_params = _params['indexer_proxy_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexer/test', 'POST',
+            '/api/v1/indexerproxy/test', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1022,21 +1029,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def testall_indexer(self, **kwargs) -> None:  # noqa: E501
-        """testall_indexer  # noqa: E501
+    def testall_indexer_proxy(self, **kwargs) -> None:  # noqa: E501
+        """testall_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_indexer(async_req=True)
+        >>> thread = api.testall_indexer_proxy(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1047,24 +1054,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.testall_indexer_with_http_info(**kwargs)  # noqa: E501
+        return self.testall_indexer_proxy_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def testall_indexer_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_indexer  # noqa: E501
+    def testall_indexer_proxy_with_http_info(self, **kwargs):  # noqa: E501
+        """testall_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_indexer_with_http_info(async_req=True)
+        >>> thread = api.testall_indexer_proxy_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1104,15 +1111,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method testall_indexer" % _key
+                    " to method testall_indexer_proxy" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1133,15 +1140,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexer/testall', 'POST',
+            '/api/v1/indexerproxy/testall', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1150,63 +1157,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
-        """update_indexer  # noqa: E501
+    def update_indexer_proxy(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> IndexerProxyResource:  # noqa: E501
+        """update_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer(id, force_save, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer_proxy(id, force_save, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
         :param force_save:
         :type force_save: bool
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerResource
+        :rtype: IndexerProxyResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_with_http_info(id, force_save, indexer_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_proxy_with_http_info(id, force_save, indexer_proxy_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """update_indexer  # noqa: E501
+    def update_indexer_proxy_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
+        """update_indexer_proxy  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_with_http_info(id, force_save, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer_proxy_with_http_info(id, force_save, indexer_proxy_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
         :param force_save:
         :type force_save: bool
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param indexer_proxy_resource:
+        :type indexer_proxy_resource: IndexerProxyResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1220,23 +1227,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
             'force_save',
-            'indexer_resource'
+            'indexer_proxy_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1247,15 +1254,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_indexer" % _key
+                    " to method update_indexer_proxy" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1273,37 +1280,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_resource']:
-            _body_params = _params['indexer_resource']
+        if _params['indexer_proxy_resource']:
+            _body_params = _params['indexer_proxy_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerResource",
+            '200': "IndexerProxyResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexer/{id}', 'PUT',
+            '/api/v1/indexerproxy/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/indexer_default_categories_api.py` & `prowlarr-py-0.4.1/prowlarr/api/indexer_default_categories_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[IndexerCategory]",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/indexer_editor_api.py` & `prowlarr-py-0.4.1/prowlarr/api/tag_details_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,79 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from typing import Optional
+from pydantic import StrictInt
 
-from prowlarr.models.indexer_editor_resource import IndexerEditorResource
+from typing import List
+
+from prowlarr.models.tag_details_resource import TagDetailsResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class IndexerEditorApi(object):
+class TagDetailsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def delete_indexer_editor(self, indexer_editor_resource : Optional[IndexerEditorResource] = None, **kwargs) -> None:  # noqa: E501
-        """delete_indexer_editor  # noqa: E501
+    def get_tag_detail_by_id(self, id : StrictInt, **kwargs) -> TagDetailsResource:  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer_editor(indexer_editor_resource, async_req=True)
+        >>> thread = api.get_tag_detail_by_id(id, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_editor_resource:
-        :type indexer_editor_resource: IndexerEditorResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: TagDetailsResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_indexer_editor_with_http_info(indexer_editor_resource, **kwargs)  # noqa: E501
+        return self.get_tag_detail_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_indexer_editor_with_http_info(self, indexer_editor_resource : Optional[IndexerEditorResource] = None, **kwargs):  # noqa: E501
-        """delete_indexer_editor  # noqa: E501
+    def get_tag_detail_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer_editor_with_http_info(indexer_editor_resource, async_req=True)
+        >>> thread = api.get_tag_detail_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_editor_resource:
-        :type indexer_editor_resource: IndexerEditorResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -99,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(TagDetailsResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_editor_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -124,53 +126,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_indexer_editor" % _key
+                    " to method get_tag_detail_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_editor_resource']:
-            _body_params = _params['indexer_editor_resource']
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "TagDetailsResource",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/indexer/editor', 'DELETE',
+            '/api/v1/tag/detail/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -179,55 +180,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def put_indexer_editor(self, indexer_editor_resource : Optional[IndexerEditorResource] = None, **kwargs) -> None:  # noqa: E501
-        """put_indexer_editor  # noqa: E501
+    def list_tag_detail(self, **kwargs) -> List[TagDetailsResource]:  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_indexer_editor(indexer_editor_resource, async_req=True)
+        >>> thread = api.list_tag_detail(async_req=True)
         >>> result = thread.get()
 
-        :param indexer_editor_resource:
-        :type indexer_editor_resource: IndexerEditorResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: List[TagDetailsResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.put_indexer_editor_with_http_info(indexer_editor_resource, **kwargs)  # noqa: E501
+        return self.list_tag_detail_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def put_indexer_editor_with_http_info(self, indexer_editor_resource : Optional[IndexerEditorResource] = None, **kwargs):  # noqa: E501
-        """put_indexer_editor  # noqa: E501
+    def list_tag_detail_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.put_indexer_editor_with_http_info(indexer_editor_resource, async_req=True)
+        >>> thread = api.list_tag_detail_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param indexer_editor_resource:
-        :type indexer_editor_resource: IndexerEditorResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -241,21 +238,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(List[TagDetailsResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_editor_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -266,15 +262,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method put_indexer_editor" % _key
+                    " to method list_tag_detail" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -288,31 +284,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_editor_resource']:
-            _body_params = _params['indexer_editor_resource']
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "List[TagDetailsResource]",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/indexer/editor', 'PUT',
+            '/api/v1/tag/detail', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/indexer_proxy_api.py` & `prowlarr-py-0.4.1/prowlarr/api/indexer_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,77 +17,82 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from prowlarr.models.indexer_proxy_resource import IndexerProxyResource
+from prowlarr.models.indexer_bulk_resource import IndexerBulkResource
+from prowlarr.models.indexer_resource import IndexerResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class IndexerProxyApi(object):
+class IndexerApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_indexer_proxy(self, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> IndexerProxyResource:  # noqa: E501
-        """create_indexer_proxy  # noqa: E501
+    def create_indexer(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_proxy(indexer_proxy_resource, async_req=True)
+        >>> thread = api.create_indexer(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param force_save:
+        :type force_save: bool
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerProxyResource
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_proxy_with_http_info(indexer_proxy_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_with_http_info(force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_proxy_with_http_info(self, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
-        """create_indexer_proxy  # noqa: E501
+    def create_indexer_with_http_info(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_proxy_with_http_info(indexer_proxy_resource, async_req=True)
+        >>> thread = api.create_indexer_with_http_info(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param force_save:
+        :type force_save: bool
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +106,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_proxy_resource'
+            'force_save',
+            'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,59 +132,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_indexer_proxy" % _key
+                    " to method create_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_proxy_resource']:
-            _body_params = _params['indexer_proxy_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerProxyResource",
+            '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy', 'POST',
+            '/api/v1/indexer', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,27 +195,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_indexer_proxy_action_by_name(self, name : StrictStr, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_indexer_proxy_action_by_name  # noqa: E501
+    def create_indexer_action_by_name(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_indexer_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_proxy_action_by_name(name, indexer_proxy_resource, async_req=True)
+        >>> thread = api.create_indexer_action_by_name(name, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -216,30 +224,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_proxy_action_by_name_with_http_info(name, indexer_proxy_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_action_by_name_with_http_info(name, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_proxy_action_by_name_with_http_info(self, name : StrictStr, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
-        """create_indexer_proxy_action_by_name  # noqa: E501
+    def create_indexer_action_by_name_with_http_info(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """create_indexer_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_proxy_action_by_name_with_http_info(name, indexer_proxy_resource, async_req=True)
+        >>> thread = api.create_indexer_action_by_name_with_http_info(name, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -260,15 +268,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'name',
-            'indexer_proxy_resource'
+            'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -279,15 +287,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_indexer_proxy_action_by_name" % _key
+                    " to method create_indexer_action_by_name" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -303,31 +311,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_proxy_resource']:
-            _body_params = _params['indexer_proxy_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/action/{name}', 'POST',
+            '/api/v1/indexer/action/{name}', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -336,21 +344,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_indexer_proxy(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_indexer_proxy  # noqa: E501
+    def delete_indexer(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer_proxy(id, async_req=True)
+        >>> thread = api.delete_indexer(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -363,24 +371,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_indexer_proxy_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_indexer_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_indexer_proxy_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_indexer_proxy  # noqa: E501
+    def delete_indexer_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer_proxy_with_http_info(id, async_req=True)
+        >>> thread = api.delete_indexer_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -423,15 +431,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_indexer_proxy" % _key
+                    " to method delete_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -454,15 +462,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/{id}', 'DELETE',
+            '/api/v1/indexer/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -471,21 +479,163 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_indexer_proxy_by_id(self, id : StrictInt, **kwargs) -> IndexerProxyResource:  # noqa: E501
-        """get_indexer_proxy_by_id  # noqa: E501
+    def delete_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_indexer_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_proxy_by_id(id, async_req=True)
+        >>> thread = api.delete_indexer_bulk(indexer_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_indexer_bulk_with_http_info(indexer_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_indexer_bulk_with_http_info(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_indexer_bulk_with_http_info(indexer_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'indexer_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_indexer_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['indexer_bulk_resource']:
+            _body_params = _params['indexer_bulk_resource']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/v1/indexer/bulk', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def get_indexer_by_id(self, id : StrictInt, **kwargs) -> IndexerResource:  # noqa: E501
+        """get_indexer_by_id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_indexer_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -495,27 +645,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerProxyResource
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_indexer_proxy_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_indexer_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_indexer_proxy_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_indexer_proxy_by_id  # noqa: E501
+    def get_indexer_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_indexer_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_proxy_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_indexer_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -533,15 +683,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -558,15 +708,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_indexer_proxy_by_id" % _key
+                    " to method get_indexer_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -585,25 +735,159 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "IndexerResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/indexer/{id}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def list_indexer(self, **kwargs) -> List[IndexerResource]:  # noqa: E501
+        """list_indexer  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_indexer(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: List[IndexerResource]
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.list_indexer_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def list_indexer_with_http_info(self, **kwargs):  # noqa: E501
+        """list_indexer  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.list_indexer_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(List[IndexerResource], status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method list_indexer" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerProxyResource",
+            '200': "List[IndexerResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/{id}', 'GET',
+            '/api/v1/indexer', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -612,21 +896,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_indexer_proxy(self, **kwargs) -> List[IndexerProxyResource]:  # noqa: E501
-        """list_indexer_proxy  # noqa: E501
+    def list_indexer_schema(self, **kwargs) -> List[IndexerResource]:  # noqa: E501
+        """list_indexer_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_proxy(async_req=True)
+        >>> thread = api.list_indexer_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -634,27 +918,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[IndexerProxyResource]
+        :rtype: List[IndexerResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_proxy_with_http_info(**kwargs)  # noqa: E501
+        return self.list_indexer_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_proxy_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer_proxy  # noqa: E501
+    def list_indexer_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_indexer_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_proxy_with_http_info(async_req=True)
+        >>> thread = api.list_indexer_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -670,15 +954,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[IndexerProxyResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[IndexerResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -694,15 +978,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_indexer_proxy" % _key
+                    " to method list_indexer_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -725,19 +1009,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[IndexerProxyResource]",
+            '200': "List[IndexerResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy', 'GET',
+            '/api/v1/indexer/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -746,51 +1030,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_indexer_proxy_schema(self, **kwargs) -> List[IndexerProxyResource]:  # noqa: E501
-        """list_indexer_proxy_schema  # noqa: E501
+    def put_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_proxy_schema(async_req=True)
+        >>> thread = api.put_indexer_bulk(indexer_bulk_resource, async_req=True)
         >>> result = thread.get()
 
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[IndexerProxyResource]
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_proxy_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.put_indexer_bulk_with_http_info(indexer_bulk_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_proxy_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer_proxy_schema  # noqa: E501
+    def put_indexer_bulk_with_http_info(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs):  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_proxy_schema_with_http_info(async_req=True)
+        >>> thread = api.put_indexer_bulk_with_http_info(indexer_bulk_resource, async_req=True)
         >>> result = thread.get()
 
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -804,20 +1092,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[IndexerProxyResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'indexer_bulk_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -828,15 +1117,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_indexer_proxy_schema" % _key
+                    " to method put_indexer_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -850,28 +1139,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['indexer_bulk_resource']:
+            _body_params = _params['indexer_bulk_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[IndexerProxyResource]",
+            '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/schema', 'GET',
+            '/api/v1/indexer/bulk', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -880,25 +1178,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def test_indexer_proxy(self, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> None:  # noqa: E501
-        """test_indexer_proxy  # noqa: E501
+    def test_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
+        """test_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_indexer_proxy(indexer_proxy_resource, async_req=True)
+        >>> thread = api.test_indexer(indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -907,28 +1205,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.test_indexer_proxy_with_http_info(indexer_proxy_resource, **kwargs)  # noqa: E501
+        return self.test_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_indexer_proxy_with_http_info(self, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
-        """test_indexer_proxy  # noqa: E501
+    def test_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """test_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_indexer_proxy_with_http_info(indexer_proxy_resource, async_req=True)
+        >>> thread = api.test_indexer_with_http_info(indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -948,15 +1246,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_proxy_resource'
+            'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -967,15 +1265,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method test_indexer_proxy" % _key
+                    " to method test_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -989,31 +1287,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_proxy_resource']:
-            _body_params = _params['indexer_proxy_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/test', 'POST',
+            '/api/v1/indexer/test', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1022,21 +1320,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def testall_indexer_proxy(self, **kwargs) -> None:  # noqa: E501
-        """testall_indexer_proxy  # noqa: E501
+    def testall_indexer(self, **kwargs) -> None:  # noqa: E501
+        """testall_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_indexer_proxy(async_req=True)
+        >>> thread = api.testall_indexer(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1047,24 +1345,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.testall_indexer_proxy_with_http_info(**kwargs)  # noqa: E501
+        return self.testall_indexer_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def testall_indexer_proxy_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_indexer_proxy  # noqa: E501
+    def testall_indexer_with_http_info(self, **kwargs):  # noqa: E501
+        """testall_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_indexer_proxy_with_http_info(async_req=True)
+        >>> thread = api.testall_indexer_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1104,15 +1402,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method testall_indexer_proxy" % _key
+                    " to method testall_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1133,15 +1431,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/testall', 'POST',
+            '/api/v1/indexer/testall', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1150,63 +1448,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer_proxy(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs) -> IndexerProxyResource:  # noqa: E501
-        """update_indexer_proxy  # noqa: E501
+    def update_indexer(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_proxy(id, force_save, indexer_proxy_resource, async_req=True)
+        >>> thread = api.update_indexer(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
         :param force_save:
         :type force_save: bool
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerProxyResource
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_proxy_with_http_info(id, force_save, indexer_proxy_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_with_http_info(id, force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_proxy_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_proxy_resource : Optional[IndexerProxyResource] = None, **kwargs):  # noqa: E501
-        """update_indexer_proxy  # noqa: E501
+    def update_indexer_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_proxy_with_http_info(id, force_save, indexer_proxy_resource, async_req=True)
+        >>> thread = api.update_indexer_with_http_info(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
         :param force_save:
         :type force_save: bool
-        :param indexer_proxy_resource:
-        :type indexer_proxy_resource: IndexerProxyResource
+        :param indexer_resource:
+        :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1220,23 +1518,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerProxyResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
             'force_save',
-            'indexer_proxy_resource'
+            'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1247,15 +1545,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_indexer_proxy" % _key
+                    " to method update_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1273,37 +1571,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_proxy_resource']:
-            _body_params = _params['indexer_proxy_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerProxyResource",
+            '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerproxy/{id}', 'PUT',
+            '/api/v1/indexer/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/indexer_stats_api.py` & `prowlarr-py-0.4.1/prowlarr/api/indexer_stats_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerStatsResource",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/indexer_status_api.py` & `prowlarr-py-0.4.1/prowlarr/api/task_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import List
 
-from prowlarr.models.indexer_status_resource import IndexerStatusResource
+from prowlarr.models.task_resource import TaskResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class IndexerStatusApi(object):
+class TaskApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_indexer_status_by_id(self, id : StrictInt, **kwargs) -> IndexerStatusResource:  # noqa: E501
-        """get_indexer_status_by_id  # noqa: E501
+    def get_system_task_by_id(self, id : StrictInt, **kwargs) -> TaskResource:  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_status_by_id(id, async_req=True)
+        >>> thread = api.get_system_task_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -63,27 +63,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IndexerStatusResource
+        :rtype: TaskResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_indexer_status_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_system_task_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_indexer_status_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_indexer_status_by_id  # noqa: E501
+    def get_system_task_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_status_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_system_task_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -101,15 +101,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerStatusResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TaskResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -126,15 +126,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_indexer_status_by_id" % _key
+                    " to method get_system_task_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -153,25 +153,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerStatusResource",
+            '200': "TaskResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerstatus/{id}', 'GET',
+            '/api/v1/system/task/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,21 +180,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_indexer_status(self, **kwargs) -> List[IndexerStatusResource]:  # noqa: E501
-        """list_indexer_status  # noqa: E501
+    def list_system_task(self, **kwargs) -> List[TaskResource]:  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_status(async_req=True)
+        >>> thread = api.list_system_task(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -202,27 +202,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[IndexerStatusResource]
+        :rtype: List[TaskResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_status_with_http_info(**kwargs)  # noqa: E501
+        return self.list_system_task_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_status_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer_status  # noqa: E501
+    def list_system_task_with_http_info(self, **kwargs):  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_status_with_http_info(async_req=True)
+        >>> thread = api.list_system_task_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -238,15 +238,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[IndexerStatusResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TaskResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -262,15 +262,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_indexer_status" % _key
+                    " to method list_system_task" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -287,25 +287,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[IndexerStatusResource]",
+            '200': "List[TaskResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/indexerstatus', 'GET',
+            '/api/v1/system/task', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/initialize_js_api.py` & `prowlarr-py-0.4.1/prowlarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/localization_api.py` & `prowlarr-py-0.4.1/prowlarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/log_api.py` & `prowlarr-py-0.4.1/prowlarr/api/log_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "LogResourcePagingResource",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/log_file_api.py` & `prowlarr-py-0.4.1/prowlarr/api/log_file_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import constr, validator
 
-from typing import List
+from typing import Any, Dict, List
 
 from prowlarr.models.log_file_resource import LogFileResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
@@ -39,15 +39,15 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_log_file_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
+    def get_log_file_by_filename(self, filename : constr(strict=True), **kwargs) -> object:  # noqa: E501
         """get_log_file_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_log_file_by_filename(filename, async_req=True)
         >>> result = thread.get()
@@ -63,15 +63,15 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: object
         """
         kwargs['_return_http_data_only'] = True
         return self.get_log_file_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
     def get_log_file_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
         """get_log_file_by_filename  # noqa: E501
@@ -101,15 +101,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(object, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'filename'
         ]
@@ -151,18 +151,24 @@
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain'])  # noqa: E501
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "object",
+        }
 
         return self.api_client.call_api(
             '/api/v1/log/file/{filename}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
@@ -281,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[LogFileResource]",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/newznab_api.py` & `prowlarr-py-0.4.1/prowlarr/api/newznab_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/notification_api.py` & `prowlarr-py-0.4.1/prowlarr/api/notification_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,23 +39,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+    def create_notification(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
         """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification(notification_resource, async_req=True)
+        >>> thread = api.create_notification(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param notification_resource:
         :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -66,26 +68,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
+        return self.create_notification_with_http_info(force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+    def create_notification_with_http_info(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
         """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_with_http_info(notification_resource, async_req=True)
+        >>> thread = api.create_notification_with_http_info(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param notification_resource:
         :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +111,15 @@
                  returns the request thread.
         :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -138,14 +143,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -158,15 +165,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -309,15 +316,15 @@
         _body_params = None
         if _params['notification_resource']:
             _body_params = _params['notification_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -585,15 +592,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NotificationResource",
         }
@@ -995,15 +1002,15 @@
         _body_params = None
         if _params['notification_resource']:
             _body_params = _params['notification_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -1283,15 +1290,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/ping_api.py` & `prowlarr-py-0.4.1/prowlarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/quality_profile_schema_api.py` & `prowlarr-py-0.4.1/prowlarr/api/quality_profile_schema_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "AppProfileResource",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/search_api.py` & `prowlarr-py-0.4.1/prowlarr/api/tag_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,81 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr, conlist
+from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
-from prowlarr.models.release_resource import ReleaseResource
+from prowlarr.models.tag_resource import TagResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class SearchApi(object):
+class TagApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_search(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
-        """create_search  # noqa: E501
+    def create_tag(self, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
+        """create_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_search(release_resource, async_req=True)
+        >>> thread = api.create_tag(tag_resource, async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
+        :param tag_resource:
+        :type tag_resource: TagResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: TagResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_search_with_http_info(release_resource, **kwargs)  # noqa: E501
+        return self.create_tag_with_http_info(tag_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_search_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
-        """create_search  # noqa: E501
+    def create_tag_with_http_info(self, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
+        """create_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_search_with_http_info(release_resource, async_req=True)
+        >>> thread = api.create_tag_with_http_info(tag_resource, async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
+        :param tag_resource:
+        :type tag_resource: TagResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'release_resource'
+            'tag_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,15 +126,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_search" % _key
+                    " to method create_tag" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -148,37 +148,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['release_resource']:
-            _body_params = _params['release_resource']
+        if _params['tag_resource']:
+            _body_params = _params['tag_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "TagResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search', 'POST',
+            '/api/v1/tag', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,55 +187,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_search_bulk(self, release_resource : Optional[conlist(ReleaseResource)] = None, **kwargs) -> ReleaseResource:  # noqa: E501
-        """create_search_bulk  # noqa: E501
+    def delete_tag(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_search_bulk(release_resource, async_req=True)
+        >>> thread = api.delete_tag(id, async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: List[ReleaseResource]
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_search_bulk_with_http_info(release_resource, **kwargs)  # noqa: E501
+        return self.delete_tag_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_search_bulk_with_http_info(self, release_resource : Optional[conlist(ReleaseResource)] = None, **kwargs):  # noqa: E501
-        """create_search_bulk  # noqa: E501
+    def delete_tag_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_search_bulk_with_http_info(release_resource, async_req=True)
+        >>> thread = api.delete_tag_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: List[ReleaseResource]
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -249,21 +249,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'release_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -274,59 +274,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_search_bulk" % _key
+                    " to method delete_tag" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['release_resource']:
-            _body_params = _params['release_resource']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "ReleaseResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/search/bulk', 'POST',
+            '/api/v1/tag/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -335,21 +322,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_search_by_id(self, id : StrictInt, **kwargs) -> ReleaseResource:  # noqa: E501
-        """get_search_by_id  # noqa: E501
+    def get_tag_by_id(self, id : StrictInt, **kwargs) -> TagResource:  # noqa: E501
+        """get_tag_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_search_by_id(id, async_req=True)
+        >>> thread = api.get_tag_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -359,27 +346,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: TagResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_search_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_tag_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_search_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_search_by_id  # noqa: E501
+    def get_tag_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_search_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_tag_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -397,15 +384,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -422,15 +409,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_search_by_id" % _key
+                    " to method get_tag_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -449,25 +436,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "TagResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search/{id}', 'GET',
+            '/api/v1/tag/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -476,75 +463,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_search(self, query : Optional[StrictStr] = None, type : Optional[StrictStr] = None, indexer_ids : Optional[conlist(StrictInt)] = None, categories : Optional[conlist(StrictInt)] = None, limit : Optional[StrictInt] = None, offset : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
-        """list_search  # noqa: E501
+    def list_tag(self, **kwargs) -> List[TagResource]:  # noqa: E501
+        """list_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_search(query, type, indexer_ids, categories, limit, offset, async_req=True)
+        >>> thread = api.list_tag(async_req=True)
         >>> result = thread.get()
 
-        :param query:
-        :type query: str
-        :param type:
-        :type type: str
-        :param indexer_ids:
-        :type indexer_ids: List[int]
-        :param categories:
-        :type categories: List[int]
-        :param limit:
-        :type limit: int
-        :param offset:
-        :type offset: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[ReleaseResource]
+        :rtype: List[TagResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_search_with_http_info(query, type, indexer_ids, categories, limit, offset, **kwargs)  # noqa: E501
+        return self.list_tag_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_search_with_http_info(self, query : Optional[StrictStr] = None, type : Optional[StrictStr] = None, indexer_ids : Optional[conlist(StrictInt)] = None, categories : Optional[conlist(StrictInt)] = None, limit : Optional[StrictInt] = None, offset : Optional[StrictInt] = None, **kwargs):  # noqa: E501
-        """list_search  # noqa: E501
+    def list_tag_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_search_with_http_info(query, type, indexer_ids, categories, limit, offset, async_req=True)
+        >>> thread = api.list_tag_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param query:
-        :type query: str
-        :param type:
-        :type type: str
-        :param indexer_ids:
-        :type indexer_ids: List[int]
-        :param categories:
-        :type categories: List[int]
-        :param limit:
-        :type limit: int
-        :param offset:
-        :type offset: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -558,26 +521,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TagResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'query',
-            'type',
-            'indexer_ids',
-            'categories',
-            'limit',
-            'offset'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -588,64 +545,205 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_search" % _key
+                    " to method list_tag" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('query') is not None:  # noqa: E501
-            _query_params.append(('Query', _params['query']))
-        if _params.get('type') is not None:  # noqa: E501
-            _query_params.append(('Type', _params['type']))
-        if _params.get('indexer_ids') is not None:  # noqa: E501
-            _query_params.append(('IndexerIds', _params['indexer_ids']))
-            _collection_formats['IndexerIds'] = 'multi'
-        if _params.get('categories') is not None:  # noqa: E501
-            _query_params.append(('Categories', _params['categories']))
-            _collection_formats['Categories'] = 'multi'
-        if _params.get('limit') is not None:  # noqa: E501
-            _query_params.append(('Limit', _params['limit']))
-        if _params.get('offset') is not None:  # noqa: E501
-            _query_params.append(('Offset', _params['offset']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "List[TagResource]",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/tag', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def update_tag(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
+        """update_tag  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_tag(id, tag_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param id: (required)
+        :type id: str
+        :param tag_resource:
+        :type tag_resource: TagResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: TagResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.update_tag_with_http_info(id, tag_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def update_tag_with_http_info(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
+        """update_tag  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_tag_with_http_info(id, tag_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param id: (required)
+        :type id: str
+        :param tag_resource:
+        :type tag_resource: TagResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'id',
+            'tag_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_tag" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['tag_resource']:
+            _body_params = _params['tag_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[ReleaseResource]",
+            '200': "TagResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/search', 'GET',
+            '/api/v1/tag/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/static_resource_api.py` & `prowlarr-py-0.4.1/prowlarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/api/system_api.py` & `prowlarr-py-0.4.1/prowlarr/api/system_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,15 +654,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "SystemResource",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/tag_api.py` & `prowlarr-py-0.4.1/prowlarr/api/search_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,81 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictInt, StrictStr, conlist
 
 from typing import List, Optional
 
-from prowlarr.models.tag_resource import TagResource
+from prowlarr.models.release_resource import ReleaseResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TagApi(object):
+class SearchApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_tag(self, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
-        """create_tag  # noqa: E501
+    def create_search(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
+        """create_search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_tag(tag_resource, async_req=True)
+        >>> thread = api.create_search(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param tag_resource:
-        :type tag_resource: TagResource
+        :param release_resource:
+        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: TagResource
+        :rtype: ReleaseResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_tag_with_http_info(tag_resource, **kwargs)  # noqa: E501
+        return self.create_search_with_http_info(release_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_tag_with_http_info(self, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
-        """create_tag  # noqa: E501
+    def create_search_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
+        """create_search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_tag_with_http_info(tag_resource, async_req=True)
+        >>> thread = api.create_search_with_http_info(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param tag_resource:
-        :type tag_resource: TagResource
+        :param release_resource:
+        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'tag_resource'
+            'release_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,15 +126,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_tag" % _key
+                    " to method create_search" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -148,37 +148,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['tag_resource']:
-            _body_params = _params['tag_resource']
+        if _params['release_resource']:
+            _body_params = _params['release_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "TagResource",
+            '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag', 'POST',
+            '/api/v1/search', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,55 +187,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_tag(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_tag  # noqa: E501
+    def create_search_bulk(self, release_resource : Optional[conlist(ReleaseResource)] = None, **kwargs) -> ReleaseResource:  # noqa: E501
+        """create_search_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_tag(id, async_req=True)
+        >>> thread = api.create_search_bulk(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param release_resource:
+        :type release_resource: List[ReleaseResource]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: ReleaseResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_tag_with_http_info(id, **kwargs)  # noqa: E501
+        return self.create_search_bulk_with_http_info(release_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_tag_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_tag  # noqa: E501
+    def create_search_bulk_with_http_info(self, release_resource : Optional[conlist(ReleaseResource)] = None, **kwargs):  # noqa: E501
+        """create_search_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_tag_with_http_info(id, async_req=True)
+        >>> thread = api.create_search_bulk_with_http_info(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param release_resource:
+        :type release_resource: List[ReleaseResource]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -249,21 +249,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'release_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -274,321 +274,59 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_tag" % _key
+                    " to method create_search_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
-        # process the query parameters
-        _query_params = []
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            '/api/v1/tag/{id}', 'DELETE',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def get_tag_by_id(self, id : StrictInt, **kwargs) -> TagResource:  # noqa: E501
-        """get_tag_by_id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_tag_by_id(id, async_req=True)
-        >>> result = thread.get()
-
-        :param id: (required)
-        :type id: int
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: TagResource
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_tag_by_id_with_http_info(id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def get_tag_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_tag_by_id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_tag_by_id_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param id: (required)
-        :type id: int
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'id'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_tag_by_id" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['release_resource']:
+            _body_params = _params['release_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {
-            '200': "TagResource",
-        }
-
-        return self.api_client.call_api(
-            '/api/v1/tag/{id}', 'GET',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def list_tag(self, **kwargs) -> List[TagResource]:  # noqa: E501
-        """list_tag  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.list_tag(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: List[TagResource]
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.list_tag_with_http_info(**kwargs)  # noqa: E501
-
-    @validate_arguments
-    def list_tag_with_http_info(self, **kwargs):  # noqa: E501
-        """list_tag  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.list_tag_with_http_info(async_req=True)
-        >>> result = thread.get()
-
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(List[TagResource], status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method list_tag" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-
-        # process the query parameters
-        _query_params = []
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[TagResource]",
+            '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag', 'GET',
+            '/api/v1/search/bulk', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -597,59 +335,75 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_tag(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
-        """update_tag  # noqa: E501
+    def list_search(self, query : Optional[StrictStr] = None, type : Optional[StrictStr] = None, indexer_ids : Optional[conlist(StrictInt)] = None, categories : Optional[conlist(StrictInt)] = None, limit : Optional[StrictInt] = None, offset : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
+        """list_search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_tag(id, tag_resource, async_req=True)
+        >>> thread = api.list_search(query, type, indexer_ids, categories, limit, offset, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
-        :param tag_resource:
-        :type tag_resource: TagResource
+        :param query:
+        :type query: str
+        :param type:
+        :type type: str
+        :param indexer_ids:
+        :type indexer_ids: List[int]
+        :param categories:
+        :type categories: List[int]
+        :param limit:
+        :type limit: int
+        :param offset:
+        :type offset: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: TagResource
+        :rtype: List[ReleaseResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_tag_with_http_info(id, tag_resource, **kwargs)  # noqa: E501
+        return self.list_search_with_http_info(query, type, indexer_ids, categories, limit, offset, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_tag_with_http_info(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
-        """update_tag  # noqa: E501
+    def list_search_with_http_info(self, query : Optional[StrictStr] = None, type : Optional[StrictStr] = None, indexer_ids : Optional[conlist(StrictInt)] = None, categories : Optional[conlist(StrictInt)] = None, limit : Optional[StrictInt] = None, offset : Optional[StrictInt] = None, **kwargs):  # noqa: E501
+        """list_search  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_tag_with_http_info(id, tag_resource, async_req=True)
+        >>> thread = api.list_search_with_http_info(query, type, indexer_ids, categories, limit, offset, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
-        :param tag_resource:
-        :type tag_resource: TagResource
+        :param query:
+        :type query: str
+        :param type:
+        :type type: str
+        :param indexer_ids:
+        :type indexer_ids: List[int]
+        :param categories:
+        :type categories: List[int]
+        :param limit:
+        :type limit: int
+        :param offset:
+        :type offset: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -663,22 +417,26 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'tag_resource'
+            'query',
+            'type',
+            'indexer_ids',
+            'categories',
+            'limit',
+            'offset'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -689,61 +447,64 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_tag" % _key
+                    " to method list_search" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('query') is not None:  # noqa: E501
+            _query_params.append(('Query', _params['query']))
+        if _params.get('type') is not None:  # noqa: E501
+            _query_params.append(('Type', _params['type']))
+        if _params.get('indexer_ids') is not None:  # noqa: E501
+            _query_params.append(('IndexerIds', _params['indexer_ids']))
+            _collection_formats['IndexerIds'] = 'multi'
+        if _params.get('categories') is not None:  # noqa: E501
+            _query_params.append(('Categories', _params['categories']))
+            _collection_formats['Categories'] = 'multi'
+        if _params.get('limit') is not None:  # noqa: E501
+            _query_params.append(('Limit', _params['limit']))
+        if _params.get('offset') is not None:  # noqa: E501
+            _query_params.append(('Offset', _params['offset']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['tag_resource']:
-            _body_params = _params['tag_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "TagResource",
+            '200': "List[ReleaseResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag/{id}', 'PUT',
+            '/api/v1/search', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/tag_details_api.py` & `prowlarr-py-0.4.1/prowlarr/api/ui_config_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,47 +13,181 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import List
+from typing import Optional
 
-from prowlarr.models.tag_details_resource import TagDetailsResource
+from prowlarr.models.ui_config_resource import UiConfigResource
 
 from prowlarr.api_client import ApiClient
 from prowlarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TagDetailsApi(object):
+class UiConfigApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_tag_detail_by_id(self, id : StrictInt, **kwargs) -> TagDetailsResource:  # noqa: E501
-        """get_tag_detail_by_id  # noqa: E501
+    def get_ui_config(self, **kwargs) -> UiConfigResource:  # noqa: E501
+        """get_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_detail_by_id(id, async_req=True)
+        >>> thread = api.get_ui_config(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: UiConfigResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.get_ui_config_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_ui_config_with_http_info(self, **kwargs):  # noqa: E501
+        """get_ui_config  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ui_config_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_ui_config" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "UiConfigResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/config/ui', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def get_ui_config_by_id(self, id : StrictInt, **kwargs) -> UiConfigResource:  # noqa: E501
+        """get_ui_config_by_id  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_ui_config_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -63,27 +197,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: TagDetailsResource
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_tag_detail_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_ui_config_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_tag_detail_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_tag_detail_by_id  # noqa: E501
+    def get_ui_config_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_ui_config_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_detail_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_ui_config_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -101,15 +235,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(TagDetailsResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -126,15 +260,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_tag_detail_by_id" % _key
+                    " to method get_ui_config_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -153,25 +287,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "TagDetailsResource",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag/detail/{id}', 'GET',
+            '/api/v1/config/ui/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,51 +314,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_tag_detail(self, **kwargs) -> List[TagDetailsResource]:  # noqa: E501
-        """list_tag_detail  # noqa: E501
+    def update_ui_config(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs) -> UiConfigResource:  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag_detail(async_req=True)
+        >>> thread = api.update_ui_config(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
+        :param ui_config_resource:
+        :type ui_config_resource: UiConfigResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[TagDetailsResource]
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_tag_detail_with_http_info(**kwargs)  # noqa: E501
+        return self.update_ui_config_with_http_info(id, ui_config_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_tag_detail_with_http_info(self, **kwargs):  # noqa: E501
-        """list_tag_detail  # noqa: E501
+    def update_ui_config_with_http_info(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs):  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag_detail_with_http_info(async_req=True)
+        >>> thread = api.update_ui_config_with_http_info(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: str
+        :param ui_config_resource:
+        :type ui_config_resource: UiConfigResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -238,20 +380,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[TagDetailsResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'id',
+            'ui_config_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -262,50 +406,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_tag_detail" % _key
+                    " to method update_ui_config" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['ui_config_resource']:
+            _body_params = _params['ui_config_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[TagDetailsResource]",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag/detail', 'GET',
+            '/api/v1/config/ui/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api/update_api.py` & `prowlarr-py-0.4.1/prowlarr/api/update_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,15 +144,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[UpdateResource]",
         }
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api_client.py` & `prowlarr-py-0.4.1/prowlarr/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'prowlarr-py/v0.4.0'
+        self.user_agent = 'prowlarr-py/v0.4.1'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `prowlarr-py-0.4.0/prowlarr/api_response.py` & `prowlarr-py-0.4.1/prowlarr/api_response.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/configuration.py` & `prowlarr-py-0.4.1/prowlarr/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.4.0'
+        sdkversion = '0.4.1'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `prowlarr-py-0.4.0/prowlarr/exceptions.py` & `prowlarr-py-0.4.1/prowlarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/__init__.py` & `prowlarr-py-0.4.1/prowlarr/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 
 from __future__ import absolute_import
 
 # import models into model package
 from prowlarr.models.api_info_resource import ApiInfoResource
 from prowlarr.models.app_profile_resource import AppProfileResource
+from prowlarr.models.application_bulk_resource import ApplicationBulkResource
 from prowlarr.models.application_resource import ApplicationResource
 from prowlarr.models.application_sync_level import ApplicationSyncLevel
 from prowlarr.models.apply_tags import ApplyTags
 from prowlarr.models.authentication_required_type import AuthenticationRequiredType
 from prowlarr.models.authentication_type import AuthenticationType
 from prowlarr.models.backup_resource import BackupResource
 from prowlarr.models.backup_type import BackupType
@@ -30,29 +31,30 @@
 from prowlarr.models.command_priority import CommandPriority
 from prowlarr.models.command_resource import CommandResource
 from prowlarr.models.command_status import CommandStatus
 from prowlarr.models.command_trigger import CommandTrigger
 from prowlarr.models.custom_filter_resource import CustomFilterResource
 from prowlarr.models.database_type import DatabaseType
 from prowlarr.models.development_config_resource import DevelopmentConfigResource
+from prowlarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from prowlarr.models.download_client_category import DownloadClientCategory
 from prowlarr.models.download_client_config_resource import DownloadClientConfigResource
 from prowlarr.models.download_client_resource import DownloadClientResource
 from prowlarr.models.download_protocol import DownloadProtocol
 from prowlarr.models.field import Field
 from prowlarr.models.health_check_result import HealthCheckResult
 from prowlarr.models.health_resource import HealthResource
 from prowlarr.models.history_event_type import HistoryEventType
 from prowlarr.models.history_resource import HistoryResource
 from prowlarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from prowlarr.models.host_config_resource import HostConfigResource
 from prowlarr.models.host_statistics import HostStatistics
+from prowlarr.models.indexer_bulk_resource import IndexerBulkResource
 from prowlarr.models.indexer_capability_resource import IndexerCapabilityResource
 from prowlarr.models.indexer_category import IndexerCategory
-from prowlarr.models.indexer_editor_resource import IndexerEditorResource
 from prowlarr.models.indexer_privacy import IndexerPrivacy
 from prowlarr.models.indexer_proxy_resource import IndexerProxyResource
 from prowlarr.models.indexer_resource import IndexerResource
 from prowlarr.models.indexer_statistics import IndexerStatistics
 from prowlarr.models.indexer_stats_resource import IndexerStatsResource
 from prowlarr.models.indexer_status_resource import IndexerStatusResource
 from prowlarr.models.localization_option import LocalizationOption
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/api_info_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/app_profile_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/app_profile_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/application_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/application_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/application_sync_level.py` & `prowlarr-py-0.4.1/prowlarr/models/application_sync_level.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/apply_tags.py` & `prowlarr-py-0.4.1/prowlarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/authentication_required_type.py` & `prowlarr-py-0.4.1/prowlarr/models/authentication_required_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/authentication_type.py` & `prowlarr-py-0.4.1/prowlarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/backup_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/backup_type.py` & `prowlarr-py-0.4.1/prowlarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/book_search_param.py` & `prowlarr-py-0.4.1/prowlarr/models/book_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/certificate_validation_type.py` & `prowlarr-py-0.4.1/prowlarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/command.py` & `prowlarr-py-0.4.1/prowlarr/models/command.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/command_priority.py` & `prowlarr-py-0.4.1/prowlarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/command_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/command_status.py` & `prowlarr-py-0.4.1/prowlarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/command_trigger.py` & `prowlarr-py-0.4.1/prowlarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/custom_filter_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/database_type.py` & `prowlarr-py-0.4.1/prowlarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/development_config_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/development_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/download_client_category.py` & `prowlarr-py-0.4.1/prowlarr/models/download_client_category.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/download_client_config_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/download_client_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/download_protocol.py` & `prowlarr-py-0.4.1/prowlarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/field.py` & `prowlarr-py-0.4.1/prowlarr/models/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,24 +28,25 @@
     Do not edit the class manually.
     """
     order: Optional[int]
     name: Optional[str]
     label: Optional[str]
     unit: Optional[str]
     help_text: Optional[str]
+    help_text_warning: Optional[str]
     help_link: Optional[str]
     value: Optional[object]
     type: Optional[str]
     advanced: Optional[bool]
     select_options: Optional[List]
     select_options_provider_action: Optional[str]
     section: Optional[str]
     hidden: Optional[str]
     placeholder: Optional[str]
-    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "placeholder"]
+    __properties = ["order", "name", "label", "unit", "helpText", "helpTextWarning", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "placeholder"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -89,14 +90,18 @@
         if self.unit is None:
             _dict['unit'] = None
 
         # set to None if help_text (nullable) is None
         if self.help_text is None:
             _dict['helpText'] = None
 
+        # set to None if help_text_warning (nullable) is None
+        if self.help_text_warning is None:
+            _dict['helpTextWarning'] = None
+
         # set to None if help_link (nullable) is None
         if self.help_link is None:
             _dict['helpLink'] = None
 
         # set to None if value (nullable) is None
         if self.value is None:
             _dict['value'] = None
@@ -138,14 +143,15 @@
 
         _obj = Field.parse_obj({
             "order": obj.get("order"),
             "name": obj.get("name"),
             "label": obj.get("label"),
             "unit": obj.get("unit"),
             "help_text": obj.get("helpText"),
+            "help_text_warning": obj.get("helpTextWarning"),
             "help_link": obj.get("helpLink"),
             "value": obj.get("value"),
             "type": obj.get("type"),
             "advanced": obj.get("advanced"),
             "select_options": [SelectOption.from_dict(_item) for _item in obj.get("selectOptions")] if obj.get("selectOptions") is not None else None,
             "select_options_provider_action": obj.get("selectOptionsProviderAction"),
             "section": obj.get("section"),
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/health_check_result.py` & `prowlarr-py-0.4.1/prowlarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/health_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/history_event_type.py` & `prowlarr-py-0.4.1/prowlarr/models/history_event_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/history_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/history_resource_paging_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/host_config_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/host_statistics.py` & `prowlarr-py-0.4.1/prowlarr/models/host_statistics.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_capability_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_capability_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_category.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_category.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_editor_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/log_file_resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,31 +12,30 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
-from typing import List, Optional
+from datetime import datetime
+from typing import Optional
 from pydantic import BaseModel
-from prowlarr.models.apply_tags import ApplyTags
 
-class IndexerEditorResource(BaseModel):
+class LogFileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    indexer_ids: Optional[List]
-    enable: Optional[bool]
-    app_profile_id: Optional[int]
-    tags: Optional[List]
-    apply_tags: Optional[ApplyTags]
-    __properties = ["indexerIds", "enable", "appProfileId", "tags", "applyTags"]
+    id: Optional[int]
+    filename: Optional[str]
+    last_write_time: Optional[datetime]
+    contents_url: Optional[str]
+    download_url: Optional[str]
+    __properties = ["id", "filename", "lastWriteTime", "contentsUrl", "downloadUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,53 +46,49 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> IndexerEditorResource:
-        """Create an instance of IndexerEditorResource from a JSON string"""
+    def from_json(cls, json_str: str) -> LogFileResource:
+        """Create an instance of LogFileResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if indexer_ids (nullable) is None
-        if self.indexer_ids is None:
-            _dict['indexerIds'] = None
-
-        # set to None if enable (nullable) is None
-        if self.enable is None:
-            _dict['enable'] = None
-
-        # set to None if app_profile_id (nullable) is None
-        if self.app_profile_id is None:
-            _dict['appProfileId'] = None
-
-        # set to None if tags (nullable) is None
-        if self.tags is None:
-            _dict['tags'] = None
+        # set to None if filename (nullable) is None
+        if self.filename is None:
+            _dict['filename'] = None
+
+        # set to None if contents_url (nullable) is None
+        if self.contents_url is None:
+            _dict['contentsUrl'] = None
+
+        # set to None if download_url (nullable) is None
+        if self.download_url is None:
+            _dict['downloadUrl'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> IndexerEditorResource:
-        """Create an instance of IndexerEditorResource from a dict"""
+    def from_dict(cls, obj: dict) -> LogFileResource:
+        """Create an instance of LogFileResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return IndexerEditorResource.parse_obj(obj)
+            return LogFileResource.parse_obj(obj)
 
-        _obj = IndexerEditorResource.parse_obj({
-            "indexer_ids": obj.get("indexerIds"),
-            "enable": obj.get("enable"),
-            "app_profile_id": obj.get("appProfileId"),
-            "tags": obj.get("tags"),
-            "apply_tags": obj.get("applyTags")
+        _obj = LogFileResource.parse_obj({
+            "id": obj.get("id"),
+            "filename": obj.get("filename"),
+            "last_write_time": obj.get("lastWriteTime"),
+            "contents_url": obj.get("contentsUrl"),
+            "download_url": obj.get("downloadUrl")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_privacy.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_privacy.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_proxy_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_proxy_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,18 +55,19 @@
     supports_redirect: Optional[bool]
     supports_pagination: Optional[bool]
     app_profile_id: Optional[int]
     protocol: Optional[DownloadProtocol]
     privacy: Optional[IndexerPrivacy]
     capabilities: Optional[IndexerCapabilityResource]
     priority: Optional[int]
+    download_client_id: Optional[int]
     added: Optional[datetime]
     status: Optional[IndexerStatusResource]
     sort_name: Optional[str]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "indexerUrls", "legacyUrls", "definitionName", "description", "language", "encoding", "enable", "redirect", "supportsRss", "supportsSearch", "supportsRedirect", "supportsPagination", "appProfileId", "protocol", "privacy", "capabilities", "priority", "added", "status", "sortName"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "indexerUrls", "legacyUrls", "definitionName", "description", "language", "encoding", "enable", "redirect", "supportsRss", "supportsSearch", "supportsRedirect", "supportsPagination", "appProfileId", "protocol", "privacy", "capabilities", "priority", "downloadClientId", "added", "status", "sortName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -209,13 +210,14 @@
             "supports_redirect": obj.get("supportsRedirect"),
             "supports_pagination": obj.get("supportsPagination"),
             "app_profile_id": obj.get("appProfileId"),
             "protocol": obj.get("protocol"),
             "privacy": obj.get("privacy"),
             "capabilities": IndexerCapabilityResource.from_dict(obj.get("capabilities")) if obj.get("capabilities") is not None else None,
             "priority": obj.get("priority"),
+            "download_client_id": obj.get("downloadClientId"),
             "added": obj.get("added"),
             "status": IndexerStatusResource.from_dict(obj.get("status")) if obj.get("status") is not None else None,
             "sort_name": obj.get("sortName")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_statistics.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_statistics.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_stats_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_stats_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/indexer_status_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/indexer_status_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/localization_option.py` & `prowlarr-py-0.4.1/prowlarr/models/localization_option.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/log_file_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/log_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,26 +16,29 @@
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 
-class LogFileResource(BaseModel):
+class LogResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    filename: Optional[str]
-    last_write_time: Optional[datetime]
-    contents_url: Optional[str]
-    download_url: Optional[str]
-    __properties = ["id", "filename", "lastWriteTime", "contentsUrl", "downloadUrl"]
+    time: Optional[datetime]
+    exception: Optional[str]
+    exception_type: Optional[str]
+    level: Optional[str]
+    logger: Optional[str]
+    message: Optional[str]
+    method: Optional[str]
+    __properties = ["id", "time", "exception", "exceptionType", "level", "logger", "message", "method"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -46,49 +49,64 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> LogFileResource:
-        """Create an instance of LogFileResource from a JSON string"""
+    def from_json(cls, json_str: str) -> LogResource:
+        """Create an instance of LogResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if filename (nullable) is None
-        if self.filename is None:
-            _dict['filename'] = None
-
-        # set to None if contents_url (nullable) is None
-        if self.contents_url is None:
-            _dict['contentsUrl'] = None
-
-        # set to None if download_url (nullable) is None
-        if self.download_url is None:
-            _dict['downloadUrl'] = None
+        # set to None if exception (nullable) is None
+        if self.exception is None:
+            _dict['exception'] = None
+
+        # set to None if exception_type (nullable) is None
+        if self.exception_type is None:
+            _dict['exceptionType'] = None
+
+        # set to None if level (nullable) is None
+        if self.level is None:
+            _dict['level'] = None
+
+        # set to None if logger (nullable) is None
+        if self.logger is None:
+            _dict['logger'] = None
+
+        # set to None if message (nullable) is None
+        if self.message is None:
+            _dict['message'] = None
+
+        # set to None if method (nullable) is None
+        if self.method is None:
+            _dict['method'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> LogFileResource:
-        """Create an instance of LogFileResource from a dict"""
+    def from_dict(cls, obj: dict) -> LogResource:
+        """Create an instance of LogResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return LogFileResource.parse_obj(obj)
+            return LogResource.parse_obj(obj)
 
-        _obj = LogFileResource.parse_obj({
+        _obj = LogResource.parse_obj({
             "id": obj.get("id"),
-            "filename": obj.get("filename"),
-            "last_write_time": obj.get("lastWriteTime"),
-            "contents_url": obj.get("contentsUrl"),
-            "download_url": obj.get("downloadUrl")
+            "time": obj.get("time"),
+            "exception": obj.get("exception"),
+            "exception_type": obj.get("exceptionType"),
+            "level": obj.get("level"),
+            "logger": obj.get("logger"),
+            "message": obj.get("message"),
+            "method": obj.get("method")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/log_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/select_option.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,33 +12,30 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import Optional
 from pydantic import BaseModel
 
-class LogResource(BaseModel):
+class SelectOption(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    time: Optional[datetime]
-    exception: Optional[str]
-    exception_type: Optional[str]
-    level: Optional[str]
-    logger: Optional[str]
-    message: Optional[str]
-    method: Optional[str]
-    __properties = ["id", "time", "exception", "exceptionType", "level", "logger", "message", "method"]
+    value: Optional[int]
+    name: Optional[str]
+    order: Optional[int]
+    hint: Optional[str]
+    parent_value: Optional[int]
+    __properties = ["value", "name", "order", "hint", "parentValue"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -49,64 +46,49 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> LogResource:
-        """Create an instance of LogResource from a JSON string"""
+    def from_json(cls, json_str: str) -> SelectOption:
+        """Create an instance of SelectOption from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if exception (nullable) is None
-        if self.exception is None:
-            _dict['exception'] = None
-
-        # set to None if exception_type (nullable) is None
-        if self.exception_type is None:
-            _dict['exceptionType'] = None
-
-        # set to None if level (nullable) is None
-        if self.level is None:
-            _dict['level'] = None
-
-        # set to None if logger (nullable) is None
-        if self.logger is None:
-            _dict['logger'] = None
-
-        # set to None if message (nullable) is None
-        if self.message is None:
-            _dict['message'] = None
-
-        # set to None if method (nullable) is None
-        if self.method is None:
-            _dict['method'] = None
+        # set to None if name (nullable) is None
+        if self.name is None:
+            _dict['name'] = None
+
+        # set to None if hint (nullable) is None
+        if self.hint is None:
+            _dict['hint'] = None
+
+        # set to None if parent_value (nullable) is None
+        if self.parent_value is None:
+            _dict['parentValue'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> LogResource:
-        """Create an instance of LogResource from a dict"""
+    def from_dict(cls, obj: dict) -> SelectOption:
+        """Create an instance of SelectOption from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return LogResource.parse_obj(obj)
+            return SelectOption.parse_obj(obj)
 
-        _obj = LogResource.parse_obj({
-            "id": obj.get("id"),
-            "time": obj.get("time"),
-            "exception": obj.get("exception"),
-            "exception_type": obj.get("exceptionType"),
-            "level": obj.get("level"),
-            "logger": obj.get("logger"),
-            "message": obj.get("message"),
-            "method": obj.get("method")
+        _obj = SelectOption.parse_obj({
+            "value": obj.get("value"),
+            "name": obj.get("name"),
+            "order": obj.get("order"),
+            "hint": obj.get("hint"),
+            "parent_value": obj.get("parentValue")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/log_resource_paging_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/movie_search_param.py` & `prowlarr-py-0.4.1/prowlarr/models/movie_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/music_search_param.py` & `prowlarr-py-0.4.1/prowlarr/models/music_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/notification_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/notification_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/paging_resource_filter.py` & `prowlarr-py-0.4.1/prowlarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/ping_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/provider_message.py` & `prowlarr-py-0.4.1/prowlarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/provider_message_type.py` & `prowlarr-py-0.4.1/prowlarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/proxy_type.py` & `prowlarr-py-0.4.1/prowlarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/release_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/release_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/runtime_mode.py` & `prowlarr-py-0.4.1/prowlarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/search_param.py` & `prowlarr-py-0.4.1/prowlarr/models/search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/select_option.py` & `prowlarr-py-0.4.1/prowlarr/models/task_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 
-class SelectOption(BaseModel):
+class TaskResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    value: Optional[int]
+    id: Optional[int]
     name: Optional[str]
-    order: Optional[int]
-    hint: Optional[str]
-    parent_value: Optional[int]
-    __properties = ["value", "name", "order", "hint", "parentValue"]
+    task_name: Optional[str]
+    interval: Optional[int]
+    last_execution: Optional[datetime]
+    last_start_time: Optional[datetime]
+    next_execution: Optional[datetime]
+    last_duration: Optional[str]
+    __properties = ["id", "name", "taskName", "interval", "lastExecution", "lastStartTime", "nextExecution", "lastDuration"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -46,49 +49,48 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> SelectOption:
-        """Create an instance of SelectOption from a JSON string"""
+    def from_json(cls, json_str: str) -> TaskResource:
+        """Create an instance of TaskResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # set to None if name (nullable) is None
         if self.name is None:
             _dict['name'] = None
 
-        # set to None if hint (nullable) is None
-        if self.hint is None:
-            _dict['hint'] = None
-
-        # set to None if parent_value (nullable) is None
-        if self.parent_value is None:
-            _dict['parentValue'] = None
+        # set to None if task_name (nullable) is None
+        if self.task_name is None:
+            _dict['taskName'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> SelectOption:
-        """Create an instance of SelectOption from a dict"""
+    def from_dict(cls, obj: dict) -> TaskResource:
+        """Create an instance of TaskResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return SelectOption.parse_obj(obj)
+            return TaskResource.parse_obj(obj)
 
-        _obj = SelectOption.parse_obj({
-            "value": obj.get("value"),
+        _obj = TaskResource.parse_obj({
+            "id": obj.get("id"),
             "name": obj.get("name"),
-            "order": obj.get("order"),
-            "hint": obj.get("hint"),
-            "parent_value": obj.get("parentValue")
+            "task_name": obj.get("taskName"),
+            "interval": obj.get("interval"),
+            "last_execution": obj.get("lastExecution"),
+            "last_start_time": obj.get("lastStartTime"),
+            "next_execution": obj.get("nextExecution"),
+            "last_duration": obj.get("lastDuration")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/sort_direction.py` & `prowlarr-py-0.4.1/prowlarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/system_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/tag_details_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/tag_details_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/tag_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/task_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/update_changes.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,33 +12,27 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
-from typing import Optional
+
+from typing import List, Optional
 from pydantic import BaseModel
 
-class TaskResource(BaseModel):
+class UpdateChanges(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    name: Optional[str]
-    task_name: Optional[str]
-    interval: Optional[int]
-    last_execution: Optional[datetime]
-    last_start_time: Optional[datetime]
-    next_execution: Optional[datetime]
-    last_duration: Optional[str]
-    __properties = ["id", "name", "taskName", "interval", "lastExecution", "lastStartTime", "nextExecution", "lastDuration"]
+    new: Optional[List]
+    fixed: Optional[List]
+    __properties = ["new", "fixed"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -49,48 +43,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TaskResource:
-        """Create an instance of TaskResource from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateChanges:
+        """Create an instance of UpdateChanges from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if name (nullable) is None
-        if self.name is None:
-            _dict['name'] = None
-
-        # set to None if task_name (nullable) is None
-        if self.task_name is None:
-            _dict['taskName'] = None
+        # set to None if new (nullable) is None
+        if self.new is None:
+            _dict['new'] = None
+
+        # set to None if fixed (nullable) is None
+        if self.fixed is None:
+            _dict['fixed'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TaskResource:
-        """Create an instance of TaskResource from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateChanges:
+        """Create an instance of UpdateChanges from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return TaskResource.parse_obj(obj)
+            return UpdateChanges.parse_obj(obj)
 
-        _obj = TaskResource.parse_obj({
-            "id": obj.get("id"),
-            "name": obj.get("name"),
-            "task_name": obj.get("taskName"),
-            "interval": obj.get("interval"),
-            "last_execution": obj.get("lastExecution"),
-            "last_start_time": obj.get("lastStartTime"),
-            "next_execution": obj.get("nextExecution"),
-            "last_duration": obj.get("lastDuration")
+        _obj = UpdateChanges.parse_obj({
+            "new": obj.get("new"),
+            "fixed": obj.get("fixed")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/tv_search_param.py` & `prowlarr-py-0.4.1/prowlarr/models/tv_search_param.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/ui_config_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/update_changes.py` & `prowlarr-py-0.4.1/prowlarr/models/user_agent_statistics.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel
 
-class UpdateChanges(BaseModel):
+class UserAgentStatistics(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    new: Optional[List]
-    fixed: Optional[List]
-    __properties = ["new", "fixed"]
+    user_agent: Optional[str]
+    number_of_queries: Optional[int]
+    number_of_grabs: Optional[int]
+    __properties = ["userAgent", "numberOfQueries", "numberOfGrabs"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -43,42 +44,39 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateChanges:
-        """Create an instance of UpdateChanges from a JSON string"""
+    def from_json(cls, json_str: str) -> UserAgentStatistics:
+        """Create an instance of UserAgentStatistics from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if new (nullable) is None
-        if self.new is None:
-            _dict['new'] = None
-
-        # set to None if fixed (nullable) is None
-        if self.fixed is None:
-            _dict['fixed'] = None
+        # set to None if user_agent (nullable) is None
+        if self.user_agent is None:
+            _dict['userAgent'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateChanges:
-        """Create an instance of UpdateChanges from a dict"""
+    def from_dict(cls, obj: dict) -> UserAgentStatistics:
+        """Create an instance of UserAgentStatistics from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateChanges.parse_obj(obj)
+            return UserAgentStatistics.parse_obj(obj)
 
-        _obj = UpdateChanges.parse_obj({
-            "new": obj.get("new"),
-            "fixed": obj.get("fixed")
+        _obj = UserAgentStatistics.parse_obj({
+            "user_agent": obj.get("userAgent"),
+            "number_of_queries": obj.get("numberOfQueries"),
+            "number_of_grabs": obj.get("numberOfGrabs")
         })
         return _obj
```

### Comparing `prowlarr-py-0.4.0/prowlarr/models/update_mechanism.py` & `prowlarr-py-0.4.1/prowlarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/models/update_resource.py` & `prowlarr-py-0.4.1/prowlarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr/rest.py` & `prowlarr-py-0.4.1/prowlarr/rest.py`

 * *Files identical despite different names*

### Comparing `prowlarr-py-0.4.0/prowlarr_py.egg-info/PKG-INFO` & `prowlarr-py-0.4.1/prowlarr_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prowlarr-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Prowlarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/prowlarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/prowlarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # prowlarr-py
 Prowlarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.4.0
+- Package version: 0.4.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -118,17 +118,19 @@
 *AppProfileApi* | [**delete_app_profile**](docs/AppProfileApi.md#delete_app_profile) | **DELETE** /api/v1/appprofile/{id} | 
 *AppProfileApi* | [**get_app_profile_by_id**](docs/AppProfileApi.md#get_app_profile_by_id) | **GET** /api/v1/appprofile/{id} | 
 *AppProfileApi* | [**list_app_profile**](docs/AppProfileApi.md#list_app_profile) | **GET** /api/v1/appprofile | 
 *AppProfileApi* | [**update_app_profile**](docs/AppProfileApi.md#update_app_profile) | **PUT** /api/v1/appprofile/{id} | 
 *ApplicationApi* | [**create_applications**](docs/ApplicationApi.md#create_applications) | **POST** /api/v1/applications | 
 *ApplicationApi* | [**create_applications_action_by_name**](docs/ApplicationApi.md#create_applications_action_by_name) | **POST** /api/v1/applications/action/{name} | 
 *ApplicationApi* | [**delete_applications**](docs/ApplicationApi.md#delete_applications) | **DELETE** /api/v1/applications/{id} | 
+*ApplicationApi* | [**delete_applications_bulk**](docs/ApplicationApi.md#delete_applications_bulk) | **DELETE** /api/v1/applications/bulk | 
 *ApplicationApi* | [**get_applications_by_id**](docs/ApplicationApi.md#get_applications_by_id) | **GET** /api/v1/applications/{id} | 
 *ApplicationApi* | [**list_applications**](docs/ApplicationApi.md#list_applications) | **GET** /api/v1/applications | 
 *ApplicationApi* | [**list_applications_schema**](docs/ApplicationApi.md#list_applications_schema) | **GET** /api/v1/applications/schema | 
+*ApplicationApi* | [**put_applications_bulk**](docs/ApplicationApi.md#put_applications_bulk) | **PUT** /api/v1/applications/bulk | 
 *ApplicationApi* | [**test_applications**](docs/ApplicationApi.md#test_applications) | **POST** /api/v1/applications/test | 
 *ApplicationApi* | [**testall_applications**](docs/ApplicationApi.md#testall_applications) | **POST** /api/v1/applications/testall | 
 *ApplicationApi* | [**update_applications**](docs/ApplicationApi.md#update_applications) | **PUT** /api/v1/applications/{id} | 
 *AuthenticationApi* | [**create_login**](docs/AuthenticationApi.md#create_login) | **POST** /login | 
 *AuthenticationApi* | [**get_logout**](docs/AuthenticationApi.md#get_logout) | **GET** /logout | 
 *BackupApi* | [**create_system_backup_restore_by_id**](docs/BackupApi.md#create_system_backup_restore_by_id) | **POST** /api/v1/system/backup/restore/{id} | 
 *BackupApi* | [**create_system_backup_restore_upload**](docs/BackupApi.md#create_system_backup_restore_upload) | **POST** /api/v1/system/backup/restore/upload | 
@@ -145,56 +147,56 @@
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v1/customfilter/{id} | 
 *DevelopmentConfigApi* | [**get_development_config**](docs/DevelopmentConfigApi.md#get_development_config) | **GET** /api/v1/config/development | 
 *DevelopmentConfigApi* | [**get_development_config_by_id**](docs/DevelopmentConfigApi.md#get_development_config_by_id) | **GET** /api/v1/config/development/{id} | 
 *DevelopmentConfigApi* | [**update_development_config**](docs/DevelopmentConfigApi.md#update_development_config) | **PUT** /api/v1/config/development/{id} | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v1/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v1/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v1/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v1/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v1/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_indexer**](docs/HistoryApi.md#list_history_indexer) | **GET** /api/v1/history/indexer | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v1/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v1/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v1/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v1/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v1/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v1/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v1/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v1/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v1/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v1/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v1/indexer/{id} | 
 *IndexerDefaultCategoriesApi* | [**list_indexer_categories**](docs/IndexerDefaultCategoriesApi.md#list_indexer_categories) | **GET** /api/v1/indexer/categories | 
-*IndexerEditorApi* | [**delete_indexer_editor**](docs/IndexerEditorApi.md#delete_indexer_editor) | **DELETE** /api/v1/indexer/editor | 
-*IndexerEditorApi* | [**put_indexer_editor**](docs/IndexerEditorApi.md#put_indexer_editor) | **PUT** /api/v1/indexer/editor | 
 *IndexerProxyApi* | [**create_indexer_proxy**](docs/IndexerProxyApi.md#create_indexer_proxy) | **POST** /api/v1/indexerproxy | 
 *IndexerProxyApi* | [**create_indexer_proxy_action_by_name**](docs/IndexerProxyApi.md#create_indexer_proxy_action_by_name) | **POST** /api/v1/indexerproxy/action/{name} | 
 *IndexerProxyApi* | [**delete_indexer_proxy**](docs/IndexerProxyApi.md#delete_indexer_proxy) | **DELETE** /api/v1/indexerproxy/{id} | 
 *IndexerProxyApi* | [**get_indexer_proxy_by_id**](docs/IndexerProxyApi.md#get_indexer_proxy_by_id) | **GET** /api/v1/indexerproxy/{id} | 
 *IndexerProxyApi* | [**list_indexer_proxy**](docs/IndexerProxyApi.md#list_indexer_proxy) | **GET** /api/v1/indexerproxy | 
 *IndexerProxyApi* | [**list_indexer_proxy_schema**](docs/IndexerProxyApi.md#list_indexer_proxy_schema) | **GET** /api/v1/indexerproxy/schema | 
 *IndexerProxyApi* | [**test_indexer_proxy**](docs/IndexerProxyApi.md#test_indexer_proxy) | **POST** /api/v1/indexerproxy/test | 
 *IndexerProxyApi* | [**testall_indexer_proxy**](docs/IndexerProxyApi.md#testall_indexer_proxy) | **POST** /api/v1/indexerproxy/testall | 
 *IndexerProxyApi* | [**update_indexer_proxy**](docs/IndexerProxyApi.md#update_indexer_proxy) | **PUT** /api/v1/indexerproxy/{id} | 
 *IndexerStatsApi* | [**get_indexer_stats**](docs/IndexerStatsApi.md#get_indexer_stats) | **GET** /api/v1/indexerstats | 
-*IndexerStatusApi* | [**get_indexer_status_by_id**](docs/IndexerStatusApi.md#get_indexer_status_by_id) | **GET** /api/v1/indexerstatus/{id} | 
 *IndexerStatusApi* | [**list_indexer_status**](docs/IndexerStatusApi.md#list_indexer_status) | **GET** /api/v1/indexerstatus | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v1/localization | 
 *LocalizationApi* | [**list_localization_options**](docs/LocalizationApi.md#list_localization_options) | **GET** /api/v1/localization/options | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v1/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v1/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v1/log/file | 
@@ -211,15 +213,14 @@
 *NotificationApi* | [**test_notification**](docs/NotificationApi.md#test_notification) | **POST** /api/v1/notification/test | 
 *NotificationApi* | [**testall_notification**](docs/NotificationApi.md#testall_notification) | **POST** /api/v1/notification/testall | 
 *NotificationApi* | [**update_notification**](docs/NotificationApi.md#update_notification) | **PUT** /api/v1/notification/{id} | 
 *PingApi* | [**get_ping**](docs/PingApi.md#get_ping) | **GET** /ping | 
 *QualityProfileSchemaApi* | [**get_appprofile_schema**](docs/QualityProfileSchemaApi.md#get_appprofile_schema) | **GET** /api/v1/appprofile/schema | 
 *SearchApi* | [**create_search**](docs/SearchApi.md#create_search) | **POST** /api/v1/search | 
 *SearchApi* | [**create_search_bulk**](docs/SearchApi.md#create_search_bulk) | **POST** /api/v1/search/bulk | 
-*SearchApi* | [**get_search_by_id**](docs/SearchApi.md#get_search_by_id) | **GET** /api/v1/search/{id} | 
 *SearchApi* | [**list_search**](docs/SearchApi.md#list_search) | **GET** /api/v1/search | 
 *StaticResourceApi* | [**get**](docs/StaticResourceApi.md#get) | **GET** / | 
 *StaticResourceApi* | [**get_by_path**](docs/StaticResourceApi.md#get_by_path) | **GET** /{path} | 
 *StaticResourceApi* | [**get_content_by_path**](docs/StaticResourceApi.md#get_content_by_path) | **GET** /content/{path} | 
 *StaticResourceApi* | [**get_login**](docs/StaticResourceApi.md#get_login) | **GET** /login | 
 *SystemApi* | [**create_system_restart**](docs/SystemApi.md#create_system_restart) | **POST** /api/v1/system/restart | 
 *SystemApi* | [**create_system_shutdown**](docs/SystemApi.md#create_system_shutdown) | **POST** /api/v1/system/shutdown | 
@@ -243,14 +244,15 @@
 *UpdateLogFileApi* | [**list_log_file_update**](docs/UpdateLogFileApi.md#list_log_file_update) | **GET** /api/v1/log/file/update | 
 
 
 ## Documentation For Models
 
  - [ApiInfoResource](docs/ApiInfoResource.md)
  - [AppProfileResource](docs/AppProfileResource.md)
+ - [ApplicationBulkResource](docs/ApplicationBulkResource.md)
  - [ApplicationResource](docs/ApplicationResource.md)
  - [ApplicationSyncLevel](docs/ApplicationSyncLevel.md)
  - [ApplyTags](docs/ApplyTags.md)
  - [AuthenticationRequiredType](docs/AuthenticationRequiredType.md)
  - [AuthenticationType](docs/AuthenticationType.md)
  - [BackupResource](docs/BackupResource.md)
  - [BackupType](docs/BackupType.md)
@@ -260,29 +262,30 @@
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientCategory](docs/DownloadClientCategory.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Field](docs/Field.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryEventType](docs/HistoryEventType.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [HostStatistics](docs/HostStatistics.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerCapabilityResource](docs/IndexerCapabilityResource.md)
  - [IndexerCategory](docs/IndexerCategory.md)
- - [IndexerEditorResource](docs/IndexerEditorResource.md)
  - [IndexerPrivacy](docs/IndexerPrivacy.md)
  - [IndexerProxyResource](docs/IndexerProxyResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IndexerStatistics](docs/IndexerStatistics.md)
  - [IndexerStatsResource](docs/IndexerStatsResource.md)
  - [IndexerStatusResource](docs/IndexerStatusResource.md)
  - [LocalizationOption](docs/LocalizationOption.md)
```

### Comparing `prowlarr-py-0.4.0/prowlarr_py.egg-info/SOURCES.txt` & `prowlarr-py-0.4.1/prowlarr_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 prowlarr/api/download_client_config_api.py
 prowlarr/api/file_system_api.py
 prowlarr/api/health_api.py
 prowlarr/api/history_api.py
 prowlarr/api/host_config_api.py
 prowlarr/api/indexer_api.py
 prowlarr/api/indexer_default_categories_api.py
-prowlarr/api/indexer_editor_api.py
 prowlarr/api/indexer_proxy_api.py
 prowlarr/api/indexer_stats_api.py
 prowlarr/api/indexer_status_api.py
 prowlarr/api/initialize_js_api.py
 prowlarr/api/localization_api.py
 prowlarr/api/log_api.py
 prowlarr/api/log_file_api.py
@@ -45,14 +44,15 @@
 prowlarr/api/task_api.py
 prowlarr/api/ui_config_api.py
 prowlarr/api/update_api.py
 prowlarr/api/update_log_file_api.py
 prowlarr/models/__init__.py
 prowlarr/models/api_info_resource.py
 prowlarr/models/app_profile_resource.py
+prowlarr/models/application_bulk_resource.py
 prowlarr/models/application_resource.py
 prowlarr/models/application_sync_level.py
 prowlarr/models/apply_tags.py
 prowlarr/models/authentication_required_type.py
 prowlarr/models/authentication_type.py
 prowlarr/models/backup_resource.py
 prowlarr/models/backup_type.py
@@ -62,29 +62,30 @@
 prowlarr/models/command_priority.py
 prowlarr/models/command_resource.py
 prowlarr/models/command_status.py
 prowlarr/models/command_trigger.py
 prowlarr/models/custom_filter_resource.py
 prowlarr/models/database_type.py
 prowlarr/models/development_config_resource.py
+prowlarr/models/download_client_bulk_resource.py
 prowlarr/models/download_client_category.py
 prowlarr/models/download_client_config_resource.py
 prowlarr/models/download_client_resource.py
 prowlarr/models/download_protocol.py
 prowlarr/models/field.py
 prowlarr/models/health_check_result.py
 prowlarr/models/health_resource.py
 prowlarr/models/history_event_type.py
 prowlarr/models/history_resource.py
 prowlarr/models/history_resource_paging_resource.py
 prowlarr/models/host_config_resource.py
 prowlarr/models/host_statistics.py
+prowlarr/models/indexer_bulk_resource.py
 prowlarr/models/indexer_capability_resource.py
 prowlarr/models/indexer_category.py
-prowlarr/models/indexer_editor_resource.py
 prowlarr/models/indexer_privacy.py
 prowlarr/models/indexer_proxy_resource.py
 prowlarr/models/indexer_resource.py
 prowlarr/models/indexer_statistics.py
 prowlarr/models/indexer_stats_resource.py
 prowlarr/models/indexer_status_resource.py
 prowlarr/models/localization_option.py
```

### Comparing `prowlarr-py-0.4.0/pyproject.toml` & `prowlarr-py-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 [project]
 name = "prowlarr-py"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
-    "urllib3 >= 1.25.3",
+    "urllib3>=1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
-    "pydantic>=1.10.2",
+    "pydantic~=1.10.11",
     "aenum"
 ]
 description = "Prowlarr API wrapper"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

