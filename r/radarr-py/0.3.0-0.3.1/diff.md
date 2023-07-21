# Comparing `tmp/radarr-py-0.3.0.tar.gz` & `tmp/radarr-py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radarr-py-0.3.0.tar", last modified: Mon May 29 06:42:04 2023, max compression
+gzip compressed data, was "radarr-py-0.3.1.tar", last modified: Fri Jul 21 10:21:46 2023, max compression
```

## Comparing `radarr-py-0.3.0.tar` & `radarr-py-0.3.1.tar`

### file list

```diff
@@ -1,217 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.660362 radarr-py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:41:42.000000 radarr-py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-05-29 06:42:04.660362 radarr-py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37334 2023-05-29 06:41:42.000000 radarr-py-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 06:41:42.000000 radarr-py-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.620361 radarr-py-0.3.0/radarr/
--rw-r--r--   0 runner    (1001) docker     (123)    12302 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.632362 radarr-py-0.3.0/radarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/alternative_title_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23725 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/credit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54263 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/extra_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25831 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36645 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_exclusions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53591 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_list_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/import_list_movies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52966 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/indexer_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53134 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/metadata_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31420 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36977 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/movie_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29122 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53806 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26150 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/rename_movie_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/restriction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.656362 radarr-py-0.3.0/radarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/add_movie_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/add_movie_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/alternative_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/alternative_title_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/collection_movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/collection_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/collection_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/colon_replacement_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/credit_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/credit_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/extra_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/extra_file_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_exclusions_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_list_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/indexer_flag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/manual_import_reprocess_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/metadata_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_runtime_format_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/movie_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/parsed_movie_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rating_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rating_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rename_movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/restriction_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/source_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tmdb_country_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/unmapped_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-29 06:41:42.000000 radarr-py-0.3.0/radarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:42:04.660362 radarr-py-0.3.0/radarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37806 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 06:42:04.000000 radarr-py-0.3.0/radarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:42:04.660362 radarr-py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 06:41:42.000000 radarr-py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:46.665054 radarr-py-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-21 10:21:27.000000 radarr-py-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38777 2023-07-21 10:21:46.665054 radarr-py-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38305 2023-07-21 10:21:27.000000 radarr-py-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 10:21:27.000000 radarr-py-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:46.621052 radarr-py-0.3.1/radarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:46.637053 radarr-py-0.3.1/radarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/alternative_title_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23725 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12796 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/credit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67158 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/extra_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25831 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36645 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/import_exclusions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66262 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18905 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/import_list_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/import_list_movies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65428 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/indexer_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53372 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18752 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/metadata_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31420 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/movie_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/movie_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36977 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/movie_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/movie_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23012 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/movie_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29122 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54044 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26150 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12883 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18200 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12871 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/rename_movie_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30285 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/restriction_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23717 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:46.661054 radarr-py-0.3.1/radarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/add_movie_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/add_movie_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/alternative_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/alternative_title_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/collection_movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/collection_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/collection_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/colon_replacement_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/credit_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/credit_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/extra_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/extra_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/import_exclusions_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/import_list_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/import_list_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/indexer_flag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/manual_import_reprocess_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/metadata_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10220 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_runtime_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/movie_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/parsed_movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/rating_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/rating_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9436 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/rename_movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/restriction_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/source_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/tmdb_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/unmapped_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-21 10:21:27.000000 radarr-py-0.3.1/radarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 10:21:46.665054 radarr-py-0.3.1/radarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38777 2023-07-21 10:21:46.000000 radarr-py-0.3.1/radarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-21 10:21:46.000000 radarr-py-0.3.1/radarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 10:21:46.000000 radarr-py-0.3.1/radarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 10:21:46.000000 radarr-py-0.3.1/radarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 10:21:46.000000 radarr-py-0.3.1/radarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 10:21:46.665054 radarr-py-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 10:21:27.000000 radarr-py-0.3.1/setup.py
```

### Comparing `radarr-py-0.3.0/LICENSE` & `radarr-py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/PKG-INFO` & `radarr-py-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radarr-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Radarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/radarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/radarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # radarr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.3.1
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -156,17 +156,19 @@
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v3/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v3/delayprofile/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v3/diskspace | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v3/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v3/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v3/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v3/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v3/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v3/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v3/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v3/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v3/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v3/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v3/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v3/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v3/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v3/config/downloadclient/{id} | 
 *ExtraFileApi* | [**list_extra_file**](docs/ExtraFileApi.md#list_extra_file) | **GET** /api/v3/extrafile | 
@@ -187,31 +189,35 @@
 *ImportExclusionsApi* | [**delete_exclusions**](docs/ImportExclusionsApi.md#delete_exclusions) | **DELETE** /api/v3/exclusions/{id} | 
 *ImportExclusionsApi* | [**get_exclusions_by_id**](docs/ImportExclusionsApi.md#get_exclusions_by_id) | **GET** /api/v3/exclusions/{id} | 
 *ImportExclusionsApi* | [**list_exclusions**](docs/ImportExclusionsApi.md#list_exclusions) | **GET** /api/v3/exclusions | 
 *ImportExclusionsApi* | [**update_exclusions**](docs/ImportExclusionsApi.md#update_exclusions) | **PUT** /api/v3/exclusions/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v3/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v3/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v3/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v3/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v3/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v3/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v3/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v3/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v3/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v3/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v3/importlist/{id} | 
 *ImportListConfigApi* | [**get_import_list_config**](docs/ImportListConfigApi.md#get_import_list_config) | **GET** /api/v3/config/importlist | 
 *ImportListConfigApi* | [**get_import_list_config_by_id**](docs/ImportListConfigApi.md#get_import_list_config_by_id) | **GET** /api/v3/config/importlist/{id} | 
 *ImportListConfigApi* | [**update_import_list_config**](docs/ImportListConfigApi.md#update_import_list_config) | **PUT** /api/v3/config/importlist/{id} | 
 *ImportListMoviesApi* | [**create_importlist_movie**](docs/ImportListMoviesApi.md#create_importlist_movie) | **POST** /api/v3/importlist/movie | 
 *ImportListMoviesApi* | [**get_importlist_movie**](docs/ImportListMoviesApi.md#get_importlist_movie) | **GET** /api/v3/importlist/movie | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v3/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v3/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v3/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v3/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v3/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v3/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v3/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v3/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v3/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v3/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v3/indexer/{id} | 
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v3/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v3/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v3/config/indexer/{id} | 
 *IndexerFlagApi* | [**list_indexer_flag**](docs/IndexerFlagApi.md#list_indexer_flag) | **GET** /api/v3/indexerflag | 
@@ -369,30 +375,33 @@
  - [CreditType](docs/CreditType.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [ExtraFileResource](docs/ExtraFileResource.md)
  - [ExtraFileType](docs/ExtraFileType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ImportExclusionsResource](docs/ImportExclusionsResource.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListConfigResource](docs/ImportListConfigResource.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerFlagResource](docs/IndexerFlagResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [Language](docs/Language.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
```

### Comparing `radarr-py-0.3.0/README.md` & `radarr-py-0.3.1/radarr_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: radarr-py
+Version: 0.3.1
+Summary: Radarr API wrapper
+Project-URL: Homepage, https://github.com/devopsarr/radarr-py
+Project-URL: Bug Tracker, https://github.com/devopsarr/radarr-py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # radarr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.3.1
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -143,17 +156,19 @@
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v3/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v3/delayprofile/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v3/diskspace | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v3/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v3/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v3/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v3/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v3/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v3/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v3/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v3/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v3/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v3/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v3/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v3/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v3/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v3/config/downloadclient/{id} | 
 *ExtraFileApi* | [**list_extra_file**](docs/ExtraFileApi.md#list_extra_file) | **GET** /api/v3/extrafile | 
@@ -174,31 +189,35 @@
 *ImportExclusionsApi* | [**delete_exclusions**](docs/ImportExclusionsApi.md#delete_exclusions) | **DELETE** /api/v3/exclusions/{id} | 
 *ImportExclusionsApi* | [**get_exclusions_by_id**](docs/ImportExclusionsApi.md#get_exclusions_by_id) | **GET** /api/v3/exclusions/{id} | 
 *ImportExclusionsApi* | [**list_exclusions**](docs/ImportExclusionsApi.md#list_exclusions) | **GET** /api/v3/exclusions | 
 *ImportExclusionsApi* | [**update_exclusions**](docs/ImportExclusionsApi.md#update_exclusions) | **PUT** /api/v3/exclusions/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v3/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v3/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v3/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v3/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v3/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v3/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v3/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v3/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v3/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v3/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v3/importlist/{id} | 
 *ImportListConfigApi* | [**get_import_list_config**](docs/ImportListConfigApi.md#get_import_list_config) | **GET** /api/v3/config/importlist | 
 *ImportListConfigApi* | [**get_import_list_config_by_id**](docs/ImportListConfigApi.md#get_import_list_config_by_id) | **GET** /api/v3/config/importlist/{id} | 
 *ImportListConfigApi* | [**update_import_list_config**](docs/ImportListConfigApi.md#update_import_list_config) | **PUT** /api/v3/config/importlist/{id} | 
 *ImportListMoviesApi* | [**create_importlist_movie**](docs/ImportListMoviesApi.md#create_importlist_movie) | **POST** /api/v3/importlist/movie | 
 *ImportListMoviesApi* | [**get_importlist_movie**](docs/ImportListMoviesApi.md#get_importlist_movie) | **GET** /api/v3/importlist/movie | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v3/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v3/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v3/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v3/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v3/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v3/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v3/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v3/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v3/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v3/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v3/indexer/{id} | 
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v3/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v3/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v3/config/indexer/{id} | 
 *IndexerFlagApi* | [**list_indexer_flag**](docs/IndexerFlagApi.md#list_indexer_flag) | **GET** /api/v3/indexerflag | 
@@ -356,30 +375,33 @@
  - [CreditType](docs/CreditType.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [ExtraFileResource](docs/ExtraFileResource.md)
  - [ExtraFileType](docs/ExtraFileType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ImportExclusionsResource](docs/ImportExclusionsResource.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListConfigResource](docs/ImportListConfigResource.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerFlagResource](docs/IndexerFlagResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [Language](docs/Language.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
```

### Comparing `radarr-py-0.3.0/pyproject.toml` & `radarr-py-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 [project]
 name = "radarr-py"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
-    "urllib3 >= 1.25.3",
+    "urllib3>=1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
-    "pydantic>=1.10.2",
+    "pydantic~=1.10.11",
     "aenum"
 ]
 description = "Radarr API wrapper"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `radarr-py-0.3.0/radarr/__init__.py` & `radarr-py-0.3.1/radarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 # x-release-please-end
 
 # import apis into sdk package
 from radarr.api.alternative_title_api import AlternativeTitleApi
 from radarr.api.api_info_api import ApiInfoApi
 from radarr.api.authentication_api import AuthenticationApi
 from radarr.api.backup_api import BackupApi
@@ -125,30 +125,33 @@
 from radarr.models.credit_type import CreditType
 from radarr.models.custom_filter_resource import CustomFilterResource
 from radarr.models.custom_format_resource import CustomFormatResource
 from radarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from radarr.models.database_type import DatabaseType
 from radarr.models.delay_profile_resource import DelayProfileResource
 from radarr.models.disk_space_resource import DiskSpaceResource
+from radarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from radarr.models.download_client_config_resource import DownloadClientConfigResource
 from radarr.models.download_client_resource import DownloadClientResource
 from radarr.models.download_protocol import DownloadProtocol
 from radarr.models.extra_file_resource import ExtraFileResource
 from radarr.models.extra_file_type import ExtraFileType
 from radarr.models.field import Field
 from radarr.models.file_date_type import FileDateType
 from radarr.models.health_check_result import HealthCheckResult
 from radarr.models.health_resource import HealthResource
 from radarr.models.history_resource import HistoryResource
 from radarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from radarr.models.host_config_resource import HostConfigResource
 from radarr.models.import_exclusions_resource import ImportExclusionsResource
+from radarr.models.import_list_bulk_resource import ImportListBulkResource
 from radarr.models.import_list_config_resource import ImportListConfigResource
 from radarr.models.import_list_resource import ImportListResource
 from radarr.models.import_list_type import ImportListType
+from radarr.models.indexer_bulk_resource import IndexerBulkResource
 from radarr.models.indexer_config_resource import IndexerConfigResource
 from radarr.models.indexer_flag_resource import IndexerFlagResource
 from radarr.models.indexer_resource import IndexerResource
 from radarr.models.language import Language
 from radarr.models.language_resource import LanguageResource
 from radarr.models.log_file_resource import LogFileResource
 from radarr.models.log_resource import LogResource
```

### Comparing `radarr-py-0.3.0/radarr/api/__init__.py` & `radarr-py-0.3.1/radarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/alternative_title_api.py` & `radarr-py-0.3.1/radarr/api/alternative_title_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/api_info_api.py` & `radarr-py-0.3.1/radarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/authentication_api.py` & `radarr-py-0.3.1/radarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/backup_api.py` & `radarr-py-0.3.1/radarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/blocklist_api.py` & `radarr-py-0.3.1/radarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/calendar_api.py` & `radarr-py-0.3.1/radarr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/calendar_feed_api.py` & `radarr-py-0.3.1/radarr/api/calendar_feed_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/collection_api.py` & `radarr-py-0.3.1/radarr/api/collection_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/command_api.py` & `radarr-py-0.3.1/radarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/credit_api.py` & `radarr-py-0.3.1/radarr/api/credit_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/custom_filter_api.py` & `radarr-py-0.3.1/radarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/custom_format_api.py` & `radarr-py-0.3.1/radarr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/delay_profile_api.py` & `radarr-py-0.3.1/radarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/disk_space_api.py` & `radarr-py-0.3.1/radarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/download_client_api.py` & `radarr-py-0.3.1/radarr/api/download_client_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from radarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from radarr.models.download_client_resource import DownloadClientResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
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
@@ -153,20 +161,20 @@
         # process the body parameter
         _body_params = None
         if _params['download_client_resource']:
             _body_params = _params['download_client_resource']
 
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
+            '/api/v3/downloadclient/bulk', 'DELETE',
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
+            '/api/v3/downloadclient/bulk', 'PUT',
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
@@ -1278,20 +1576,20 @@
         # process the body parameter
         _body_params = None
         if _params['download_client_resource']:
             _body_params = _params['download_client_resource']
 
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

### Comparing `radarr-py-0.3.0/radarr/api/download_client_config_api.py` & `radarr-py-0.3.1/radarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/extra_file_api.py` & `radarr-py-0.3.1/radarr/api/extra_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/file_system_api.py` & `radarr-py-0.3.1/radarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/health_api.py` & `radarr-py-0.3.1/radarr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/history_api.py` & `radarr-py-0.3.1/radarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/host_config_api.py` & `radarr-py-0.3.1/radarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/import_exclusions_api.py` & `radarr-py-0.3.1/radarr/api/import_exclusions_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/import_list_api.py` & `radarr-py-0.3.1/radarr/api/import_list_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from radarr.models.import_list_bulk_resource import ImportListBulkResource
 from radarr.models.import_list_resource import ImportListResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -39,23 +40,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_import_list(self, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+    def create_import_list(self, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
         """create_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_import_list(import_list_resource, async_req=True)
+        >>> thread = api.create_import_list(force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
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
         :rtype: ImportListResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_import_list_with_http_info(import_list_resource, **kwargs)  # noqa: E501
+        return self.create_import_list_with_http_info(force_save, import_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_import_list_with_http_info(self, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
+    def create_import_list_with_http_info(self, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
         """create_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_import_list_with_http_info(import_list_resource, async_req=True)
+        >>> thread = api.create_import_list_with_http_info(force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +112,15 @@
                  returns the request thread.
         :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'import_list_resource'
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
@@ -153,20 +161,20 @@
         # process the body parameter
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
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
@@ -309,15 +317,15 @@
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
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
+    def delete_import_list_bulk(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_import_list_bulk(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
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
+        return self.delete_import_list_bulk_with_http_info(import_list_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_import_list_bulk_with_http_info(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_import_list_bulk_with_http_info(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
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
+            'import_list_bulk_resource'
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
+                    " to method delete_import_list_bulk" % _key
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
+        if _params['import_list_bulk_resource']:
+            _body_params = _params['import_list_bulk_resource']
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
+            '/api/v3/importlist/bulk', 'DELETE',
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
     def get_import_list_by_id(self, id : StrictInt, **kwargs) -> ImportListResource:  # noqa: E501
         """get_import_list_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_import_list_by_id(id, async_req=True)
@@ -880,14 +1030,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def put_import_list_bulk(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+        """put_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_import_list_bulk(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
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
+        :rtype: ImportListResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.put_import_list_bulk_with_http_info(import_list_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_import_list_bulk_with_http_info(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs):  # noqa: E501
+        """put_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_import_list_bulk_with_http_info(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
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
+        :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'import_list_bulk_resource'
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
+                    " to method put_import_list_bulk" % _key
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
+        if _params['import_list_bulk_resource']:
+            _body_params = _params['import_list_bulk_resource']
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
+            '200': "ImportListResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v3/importlist/bulk', 'PUT',
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
     def test_import_list(self, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> None:  # noqa: E501
         """test_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.test_import_list(import_list_resource, async_req=True)
@@ -1278,20 +1576,20 @@
         # process the body parameter
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
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

### Comparing `radarr-py-0.3.0/radarr/api/import_list_config_api.py` & `radarr-py-0.3.1/radarr/api/import_list_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/import_list_movies_api.py` & `radarr-py-0.3.1/radarr/api/import_list_movies_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/indexer_api.py` & `radarr-py-0.3.1/radarr/api/indexer_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from radarr.models.indexer_bulk_resource import IndexerBulkResource
 from radarr.models.indexer_resource import IndexerResource
 
 from radarr.api_client import ApiClient
 from radarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -39,23 +40,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+    def create_indexer(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
         """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer(indexer_resource, async_req=True)
+        >>> thread = api.create_indexer(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
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
         :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_with_http_info(force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+    def create_indexer_with_http_info(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
         """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_with_http_info(indexer_resource, async_req=True)
+        >>> thread = api.create_indexer_with_http_info(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +112,15 @@
                  returns the request thread.
         :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'indexer_resource'
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
@@ -153,20 +161,20 @@
         # process the body parameter
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
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
@@ -309,15 +317,15 @@
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
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
+    def delete_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
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
+            '/api/v3/indexer/bulk', 'DELETE',
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
     def get_indexer_by_id(self, id : StrictInt, **kwargs) -> IndexerResource:  # noqa: E501
         """get_indexer_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_indexer_by_id(id, async_req=True)
@@ -880,14 +1030,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def put_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_indexer_bulk(indexer_bulk_resource, async_req=True)
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
+        :rtype: IndexerResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.put_indexer_bulk_with_http_info(indexer_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_indexer_bulk_with_http_info(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs):  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_indexer_bulk_with_http_info(indexer_bulk_resource, async_req=True)
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
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
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
+                    " to method put_indexer_bulk" % _key
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
+            '200': "IndexerResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v3/indexer/bulk', 'PUT',
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
     def test_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
         """test_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.test_indexer(indexer_resource, async_req=True)
@@ -1278,20 +1576,20 @@
         # process the body parameter
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
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

### Comparing `radarr-py-0.3.0/radarr/api/indexer_config_api.py` & `radarr-py-0.3.1/radarr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/indexer_flag_api.py` & `radarr-py-0.3.1/radarr/api/indexer_flag_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/initialize_js_api.py` & `radarr-py-0.3.1/radarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/language_api.py` & `radarr-py-0.3.1/radarr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/localization_api.py` & `radarr-py-0.3.1/radarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/log_api.py` & `radarr-py-0.3.1/radarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/log_file_api.py` & `radarr-py-0.3.1/radarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/manual_import_api.py` & `radarr-py-0.3.1/radarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/media_cover_api.py` & `radarr-py-0.3.1/radarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/media_management_config_api.py` & `radarr-py-0.3.1/radarr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/metadata_api.py` & `radarr-py-0.3.1/radarr/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,23 +39,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_metadata(self, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
+    def create_metadata(self, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
         """create_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_metadata(metadata_resource, async_req=True)
+        >>> thread = api.create_metadata(force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
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
         :rtype: MetadataResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_metadata_with_http_info(metadata_resource, **kwargs)  # noqa: E501
+        return self.create_metadata_with_http_info(force_save, metadata_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_metadata_with_http_info(self, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
+    def create_metadata_with_http_info(self, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
         """create_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_metadata_with_http_info(metadata_resource, async_req=True)
+        >>> thread = api.create_metadata_with_http_info(force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +111,15 @@
                  returns the request thread.
         :rtype: tuple(MetadataResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'metadata_resource'
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
@@ -153,20 +160,20 @@
         # process the body parameter
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
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
@@ -309,15 +316,15 @@
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
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
@@ -1278,20 +1285,20 @@
         # process the body parameter
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
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

### Comparing `radarr-py-0.3.0/radarr/api/metadata_config_api.py` & `radarr-py-0.3.1/radarr/api/metadata_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/movie_api.py` & `radarr-py-0.3.1/radarr/api/movie_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/movie_editor_api.py` & `radarr-py-0.3.1/radarr/api/movie_editor_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/movie_file_api.py` & `radarr-py-0.3.1/radarr/api/movie_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/movie_import_api.py` & `radarr-py-0.3.1/radarr/api/movie_import_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/movie_lookup_api.py` & `radarr-py-0.3.1/radarr/api/movie_lookup_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/naming_config_api.py` & `radarr-py-0.3.1/radarr/api/naming_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/notification_api.py` & `radarr-py-0.3.1/radarr/api/notification_api.py`

 * *Files 1% similar despite different names*

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
@@ -153,20 +160,20 @@
         # process the body parameter
         _body_params = None
         if _params['notification_resource']:
             _body_params = _params['notification_resource']
 
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
@@ -1278,20 +1285,20 @@
         # process the body parameter
         _body_params = None
         if _params['notification_resource']:
             _body_params = _params['notification_resource']
 
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

### Comparing `radarr-py-0.3.0/radarr/api/parse_api.py` & `radarr-py-0.3.1/radarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/ping_api.py` & `radarr-py-0.3.1/radarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/quality_definition_api.py` & `radarr-py-0.3.1/radarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/quality_profile_api.py` & `radarr-py-0.3.1/radarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/quality_profile_schema_api.py` & `radarr-py-0.3.1/radarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/queue_action_api.py` & `radarr-py-0.3.1/radarr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/queue_api.py` & `radarr-py-0.3.1/radarr/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/queue_details_api.py` & `radarr-py-0.3.1/radarr/api/queue_details_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/queue_status_api.py` & `radarr-py-0.3.1/radarr/api/queue_status_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/release_api.py` & `radarr-py-0.3.1/radarr/api/release_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/release_push_api.py` & `radarr-py-0.3.1/radarr/api/release_push_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/remote_path_mapping_api.py` & `radarr-py-0.3.1/radarr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/rename_movie_api.py` & `radarr-py-0.3.1/radarr/api/rename_movie_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/restriction_api.py` & `radarr-py-0.3.1/radarr/api/restriction_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/root_folder_api.py` & `radarr-py-0.3.1/radarr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/static_resource_api.py` & `radarr-py-0.3.1/radarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/system_api.py` & `radarr-py-0.3.1/radarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/tag_api.py` & `radarr-py-0.3.1/radarr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/tag_details_api.py` & `radarr-py-0.3.1/radarr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/task_api.py` & `radarr-py-0.3.1/radarr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/ui_config_api.py` & `radarr-py-0.3.1/radarr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/update_api.py` & `radarr-py-0.3.1/radarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api/update_log_file_api.py` & `radarr-py-0.3.1/radarr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/api_client.py` & `radarr-py-0.3.1/radarr/api_client.py`

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
-        self.user_agent = 'radarr-py/v0.3.0'
+        self.user_agent = 'radarr-py/v0.3.1'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `radarr-py-0.3.0/radarr/api_response.py` & `radarr-py-0.3.1/radarr/api_response.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/configuration.py` & `radarr-py-0.3.1/radarr/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.3.0'
+        sdkversion = '0.3.1'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `radarr-py-0.3.0/radarr/exceptions.py` & `radarr-py-0.3.1/radarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/__init__.py` & `radarr-py-0.3.1/radarr/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,33 @@
 from radarr.models.credit_type import CreditType
 from radarr.models.custom_filter_resource import CustomFilterResource
 from radarr.models.custom_format_resource import CustomFormatResource
 from radarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from radarr.models.database_type import DatabaseType
 from radarr.models.delay_profile_resource import DelayProfileResource
 from radarr.models.disk_space_resource import DiskSpaceResource
+from radarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from radarr.models.download_client_config_resource import DownloadClientConfigResource
 from radarr.models.download_client_resource import DownloadClientResource
 from radarr.models.download_protocol import DownloadProtocol
 from radarr.models.extra_file_resource import ExtraFileResource
 from radarr.models.extra_file_type import ExtraFileType
 from radarr.models.field import Field
 from radarr.models.file_date_type import FileDateType
 from radarr.models.health_check_result import HealthCheckResult
 from radarr.models.health_resource import HealthResource
 from radarr.models.history_resource import HistoryResource
 from radarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from radarr.models.host_config_resource import HostConfigResource
 from radarr.models.import_exclusions_resource import ImportExclusionsResource
+from radarr.models.import_list_bulk_resource import ImportListBulkResource
 from radarr.models.import_list_config_resource import ImportListConfigResource
 from radarr.models.import_list_resource import ImportListResource
 from radarr.models.import_list_type import ImportListType
+from radarr.models.indexer_bulk_resource import IndexerBulkResource
 from radarr.models.indexer_config_resource import IndexerConfigResource
 from radarr.models.indexer_flag_resource import IndexerFlagResource
 from radarr.models.indexer_resource import IndexerResource
 from radarr.models.language import Language
 from radarr.models.language_resource import LanguageResource
 from radarr.models.log_file_resource import LogFileResource
 from radarr.models.log_resource import LogResource
```

### Comparing `radarr-py-0.3.0/radarr/models/add_movie_method.py` & `radarr-py-0.3.1/radarr/models/add_movie_method.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/add_movie_options.py` & `radarr-py-0.3.1/radarr/models/add_movie_options.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/alternative_title.py` & `radarr-py-0.3.1/radarr/models/alternative_title.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/alternative_title_resource.py` & `radarr-py-0.3.1/radarr/models/alternative_title_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/api_info_resource.py` & `radarr-py-0.3.1/radarr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/apply_tags.py` & `radarr-py-0.3.1/radarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/authentication_type.py` & `radarr-py-0.3.1/radarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/backup_resource.py` & `radarr-py-0.3.1/radarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/backup_type.py` & `radarr-py-0.3.1/radarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/blocklist_bulk_resource.py` & `radarr-py-0.3.1/radarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/blocklist_resource.py` & `radarr-py-0.3.1/radarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/blocklist_resource_paging_resource.py` & `radarr-py-0.3.1/radarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/certificate_validation_type.py` & `radarr-py-0.3.1/radarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/collection_movie_resource.py` & `radarr-py-0.3.1/radarr/models/collection_movie_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/collection_resource.py` & `radarr-py-0.3.1/radarr/models/collection_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,17 @@
     overview: Optional[str]
     monitored: Optional[bool]
     root_folder_path: Optional[str]
     quality_profile_id: Optional[int]
     search_on_add: Optional[bool]
     minimum_availability: Optional[MovieStatusType]
     movies: Optional[List]
-    __properties = ["id", "title", "sortTitle", "tmdbId", "images", "overview", "monitored", "rootFolderPath", "qualityProfileId", "searchOnAdd", "minimumAvailability", "movies"]
+    missing_movies: Optional[int]
+    tags: Optional[List]
+    __properties = ["id", "title", "sortTitle", "tmdbId", "images", "overview", "monitored", "rootFolderPath", "qualityProfileId", "searchOnAdd", "minimumAvailability", "movies", "missingMovies", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -104,14 +106,18 @@
         if self.root_folder_path is None:
             _dict['rootFolderPath'] = None
 
         # set to None if movies (nullable) is None
         if self.movies is None:
             _dict['movies'] = None
 
+        # set to None if tags (nullable) is None
+        if self.tags is None:
+            _dict['tags'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> CollectionResource:
         """Create an instance of CollectionResource from a dict"""
         if obj is None:
             return None
@@ -127,11 +133,13 @@
             "images": [MediaCover.from_dict(_item) for _item in obj.get("images")] if obj.get("images") is not None else None,
             "overview": obj.get("overview"),
             "monitored": obj.get("monitored"),
             "root_folder_path": obj.get("rootFolderPath"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "search_on_add": obj.get("searchOnAdd"),
             "minimum_availability": obj.get("minimumAvailability"),
-            "movies": [CollectionMovieResource.from_dict(_item) for _item in obj.get("movies")] if obj.get("movies") is not None else None
+            "movies": [CollectionMovieResource.from_dict(_item) for _item in obj.get("movies")] if obj.get("movies") is not None else None,
+            "missing_movies": obj.get("missingMovies"),
+            "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/collection_update_resource.py` & `radarr-py-0.3.1/radarr/models/collection_update_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/colon_replacement_format.py` & `radarr-py-0.3.1/radarr/models/colon_replacement_format.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/command.py` & `radarr-py-0.3.1/radarr/models/command.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/command_priority.py` & `radarr-py-0.3.1/radarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/command_resource.py` & `radarr-py-0.3.1/radarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/command_result.py` & `radarr-py-0.3.1/radarr/models/command_result.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/command_status.py` & `radarr-py-0.3.1/radarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/command_trigger.py` & `radarr-py-0.3.1/radarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/credit_resource.py` & `radarr-py-0.3.1/radarr/models/credit_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/credit_type.py` & `radarr-py-0.3.1/radarr/models/credit_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/custom_filter_resource.py` & `radarr-py-0.3.1/radarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/custom_format_resource.py` & `radarr-py-0.3.1/radarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/custom_format_specification_schema.py` & `radarr-py-0.3.1/radarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/database_type.py` & `radarr-py-0.3.1/radarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/delay_profile_resource.py` & `radarr-py-0.3.1/radarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/disk_space_resource.py` & `radarr-py-0.3.1/radarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/download_client_config_resource.py` & `radarr-py-0.3.1/radarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/download_client_resource.py` & `radarr-py-0.3.1/radarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/download_protocol.py` & `radarr-py-0.3.1/radarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/extra_file_resource.py` & `radarr-py-0.3.1/radarr/models/extra_file_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/extra_file_type.py` & `radarr-py-0.3.1/radarr/models/extra_file_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/field.py` & `radarr-py-0.3.1/radarr/models/field.py`

 * *Files 12% similar despite different names*

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

### Comparing `radarr-py-0.3.0/radarr/models/file_date_type.py` & `radarr-py-0.3.1/radarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/health_check_result.py` & `radarr-py-0.3.1/radarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/health_resource.py` & `radarr-py-0.3.1/radarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/history_resource.py` & `radarr-py-0.3.1/radarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/history_resource_paging_resource.py` & `radarr-py-0.3.1/radarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/host_config_resource.py` & `radarr-py-0.3.1/radarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/import_exclusions_resource.py` & `radarr-py-0.3.1/radarr/models/import_exclusions_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/import_list_config_resource.py` & `radarr-py-0.3.1/radarr/models/import_list_config_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,17 @@
 class ImportListConfigResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    import_list_sync_interval: Optional[int]
     list_sync_level: Optional[str]
     import_exclusions: Optional[str]
-    __properties = ["id", "importListSyncInterval", "listSyncLevel", "importExclusions"]
+    __properties = ["id", "listSyncLevel", "importExclusions"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -76,13 +75,12 @@
             return None
 
         if type(obj) is not dict:
             return ImportListConfigResource.parse_obj(obj)
 
         _obj = ImportListConfigResource.parse_obj({
             "id": obj.get("id"),
-            "import_list_sync_interval": obj.get("importListSyncInterval"),
             "list_sync_level": obj.get("listSyncLevel"),
             "import_exclusions": obj.get("importExclusions")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/import_list_resource.py` & `radarr-py-0.3.1/radarr/models/import_list_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
     monitor: Optional[MonitorTypes]
     root_folder_path: Optional[str]
     quality_profile_id: Optional[int]
     search_on_add: Optional[bool]
     minimum_availability: Optional[MovieStatusType]
     list_type: Optional[ImportListType]
     list_order: Optional[int]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enabled", "enableAuto", "monitor", "rootFolderPath", "qualityProfileId", "searchOnAdd", "minimumAvailability", "listType", "listOrder"]
+    min_refresh_interval: Optional[str]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enabled", "enableAuto", "monitor", "rootFolderPath", "qualityProfileId", "searchOnAdd", "minimumAvailability", "listType", "listOrder", "minRefreshInterval"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -158,11 +159,12 @@
             "enable_auto": obj.get("enableAuto"),
             "monitor": obj.get("monitor"),
             "root_folder_path": obj.get("rootFolderPath"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "search_on_add": obj.get("searchOnAdd"),
             "minimum_availability": obj.get("minimumAvailability"),
             "list_type": obj.get("listType"),
-            "list_order": obj.get("listOrder")
+            "list_order": obj.get("listOrder"),
+            "min_refresh_interval": obj.get("minRefreshInterval")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/import_list_type.py` & `radarr-py-0.3.1/radarr/models/import_list_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,10 +30,11 @@
     allowed enum values
     """
 
     PROGRAM = 'program'
     TMDB = 'tmdb'
     TRAKT = 'trakt'
     PLEX = 'plex'
+    SIMKL = 'simkl'
     OTHER = 'other'
     ADVANCED = 'advanced'
```

### Comparing `radarr-py-0.3.0/radarr/models/indexer_config_resource.py` & `radarr-py-0.3.1/radarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/indexer_flag_resource.py` & `radarr-py-0.3.1/radarr/models/indexer_flag_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/indexer_resource.py` & `radarr-py-0.3.1/radarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/language.py` & `radarr-py-0.3.1/radarr/models/language.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/language_resource.py` & `radarr-py-0.3.1/radarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/log_file_resource.py` & `radarr-py-0.3.1/radarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/log_resource.py` & `radarr-py-0.3.1/radarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/log_resource_paging_resource.py` & `radarr-py-0.3.1/radarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/manual_import_reprocess_resource.py` & `radarr-py-0.3.1/radarr/models/manual_import_reprocess_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/manual_import_resource.py` & `radarr-py-0.3.1/radarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/media_cover.py` & `radarr-py-0.3.1/radarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/media_cover_types.py` & `radarr-py-0.3.1/radarr/models/media_cover_types.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/media_info_resource.py` & `radarr-py-0.3.1/radarr/models/media_info_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/media_management_config_resource.py` & `radarr-py-0.3.1/radarr/models/media_management_config_resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,18 +42,20 @@
     paths_default_static: Optional[bool]
     set_permissions_linux: Optional[bool]
     chmod_folder: Optional[str]
     chown_group: Optional[str]
     skip_free_space_check_when_importing: Optional[bool]
     minimum_free_space_when_importing: Optional[int]
     copy_using_hardlinks: Optional[bool]
+    use_script_import: Optional[bool]
+    script_import_path: Optional[str]
     import_extra_files: Optional[bool]
     extra_file_extensions: Optional[str]
     enable_media_info: Optional[bool]
-    __properties = ["id", "autoUnmonitorPreviouslyDownloadedMovies", "recycleBin", "recycleBinCleanupDays", "downloadPropersAndRepacks", "createEmptyMovieFolders", "deleteEmptyFolders", "fileDate", "rescanAfterRefresh", "autoRenameFolders", "pathsDefaultStatic", "setPermissionsLinux", "chmodFolder", "chownGroup", "skipFreeSpaceCheckWhenImporting", "minimumFreeSpaceWhenImporting", "copyUsingHardlinks", "importExtraFiles", "extraFileExtensions", "enableMediaInfo"]
+    __properties = ["id", "autoUnmonitorPreviouslyDownloadedMovies", "recycleBin", "recycleBinCleanupDays", "downloadPropersAndRepacks", "createEmptyMovieFolders", "deleteEmptyFolders", "fileDate", "rescanAfterRefresh", "autoRenameFolders", "pathsDefaultStatic", "setPermissionsLinux", "chmodFolder", "chownGroup", "skipFreeSpaceCheckWhenImporting", "minimumFreeSpaceWhenImporting", "copyUsingHardlinks", "useScriptImport", "scriptImportPath", "importExtraFiles", "extraFileExtensions", "enableMediaInfo"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -86,14 +88,18 @@
         if self.chmod_folder is None:
             _dict['chmodFolder'] = None
 
         # set to None if chown_group (nullable) is None
         if self.chown_group is None:
             _dict['chownGroup'] = None
 
+        # set to None if script_import_path (nullable) is None
+        if self.script_import_path is None:
+            _dict['scriptImportPath'] = None
+
         # set to None if extra_file_extensions (nullable) is None
         if self.extra_file_extensions is None:
             _dict['extraFileExtensions'] = None
 
         return _dict
 
     @classmethod
@@ -119,13 +125,15 @@
             "paths_default_static": obj.get("pathsDefaultStatic"),
             "set_permissions_linux": obj.get("setPermissionsLinux"),
             "chmod_folder": obj.get("chmodFolder"),
             "chown_group": obj.get("chownGroup"),
             "skip_free_space_check_when_importing": obj.get("skipFreeSpaceCheckWhenImporting"),
             "minimum_free_space_when_importing": obj.get("minimumFreeSpaceWhenImporting"),
             "copy_using_hardlinks": obj.get("copyUsingHardlinks"),
+            "use_script_import": obj.get("useScriptImport"),
+            "script_import_path": obj.get("scriptImportPath"),
             "import_extra_files": obj.get("importExtraFiles"),
             "extra_file_extensions": obj.get("extraFileExtensions"),
             "enable_media_info": obj.get("enableMediaInfo")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/metadata_config_resource.py` & `radarr-py-0.3.1/radarr/models/metadata_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/metadata_resource.py` & `radarr-py-0.3.1/radarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/modifier.py` & `radarr-py-0.3.1/radarr/models/modifier.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/monitor_types.py` & `radarr-py-0.3.1/radarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_collection.py` & `radarr-py-0.3.1/radarr/models/movie_collection.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
     root_folder_path: Optional[str]
     search_on_add: Optional[bool]
     minimum_availability: Optional[MovieStatusType]
     last_info_sync: Optional[datetime]
     images: Optional[List]
     added: Optional[datetime]
     movies: Optional[List]
-    __properties = ["id", "title", "cleanTitle", "sortTitle", "tmdbId", "overview", "monitored", "qualityProfileId", "rootFolderPath", "searchOnAdd", "minimumAvailability", "lastInfoSync", "images", "added", "movies"]
+    tags: Optional[List]
+    __properties = ["id", "title", "cleanTitle", "sortTitle", "tmdbId", "overview", "monitored", "qualityProfileId", "rootFolderPath", "searchOnAdd", "minimumAvailability", "lastInfoSync", "images", "added", "movies", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -115,14 +116,18 @@
         if self.images is None:
             _dict['images'] = None
 
         # set to None if movies (nullable) is None
         if self.movies is None:
             _dict['movies'] = None
 
+        # set to None if tags (nullable) is None
+        if self.tags is None:
+            _dict['tags'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> MovieCollection:
         """Create an instance of MovieCollection from a dict"""
         if obj is None:
             return None
@@ -141,11 +146,12 @@
             "quality_profile_id": obj.get("qualityProfileId"),
             "root_folder_path": obj.get("rootFolderPath"),
             "search_on_add": obj.get("searchOnAdd"),
             "minimum_availability": obj.get("minimumAvailability"),
             "last_info_sync": obj.get("lastInfoSync"),
             "images": [MediaCover.from_dict(_item) for _item in obj.get("images")] if obj.get("images") is not None else None,
             "added": obj.get("added"),
-            "movies": [MovieMetadata.from_dict(_item) for _item in obj.get("movies")] if obj.get("movies") is not None else None
+            "movies": [MovieMetadata.from_dict(_item) for _item in obj.get("movies")] if obj.get("movies") is not None else None,
+            "tags": obj.get("tags")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/movie_editor_resource.py` & `radarr-py-0.3.1/radarr/models/movie_editor_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_file_list_resource.py` & `radarr-py-0.3.1/radarr/models/movie_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_file_resource.py` & `radarr-py-0.3.1/radarr/models/movie_file_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_history_event_type.py` & `radarr-py-0.3.1/radarr/models/movie_history_event_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_metadata.py` & `radarr-py-0.3.1/radarr/models/movie_metadata.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_resource.py` & `radarr-py-0.3.1/radarr/models/movie_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_runtime_format_type.py` & `radarr-py-0.3.1/radarr/models/movie_runtime_format_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_status_type.py` & `radarr-py-0.3.1/radarr/models/movie_status_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/movie_translation.py` & `radarr-py-0.3.1/radarr/models/movie_translation.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/naming_config_resource.py` & `radarr-py-0.3.1/radarr/models/naming_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/notification_resource.py` & `radarr-py-0.3.1/radarr/models/notification_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/paging_resource_filter.py` & `radarr-py-0.3.1/radarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/parse_resource.py` & `radarr-py-0.3.1/radarr/models/queue_status_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
-from radarr.models.movie_resource import MovieResource
-from radarr.models.parsed_movie_info import ParsedMovieInfo
 
-class ParseResource(BaseModel):
+class QueueStatusResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    title: Optional[str]
-    parsed_movie_info: Optional[ParsedMovieInfo]
-    movie: Optional[MovieResource]
-    __properties = ["id", "title", "parsedMovieInfo", "movie"]
+    total_count: Optional[int]
+    count: Optional[int]
+    unknown_count: Optional[int]
+    errors: Optional[bool]
+    warnings: Optional[bool]
+    unknown_errors: Optional[bool]
+    unknown_warnings: Optional[bool]
+    __properties = ["id", "totalCount", "count", "unknownCount", "errors", "warnings", "unknownErrors", "unknownWarnings"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,46 +49,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ParseResource:
-        """Create an instance of ParseResource from a JSON string"""
+    def from_json(cls, json_str: str) -> QueueStatusResource:
+        """Create an instance of QueueStatusResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of parsed_movie_info
-        if self.parsed_movie_info:
-            _dict['parsedMovieInfo'] = self.parsed_movie_info.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of movie
-        if self.movie:
-            _dict['movie'] = self.movie.to_dict()
-        # set to None if title (nullable) is None
-        if self.title is None:
-            _dict['title'] = None
-
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ParseResource:
-        """Create an instance of ParseResource from a dict"""
+    def from_dict(cls, obj: dict) -> QueueStatusResource:
+        """Create an instance of QueueStatusResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ParseResource.parse_obj(obj)
+            return QueueStatusResource.parse_obj(obj)
 
-        _obj = ParseResource.parse_obj({
+        _obj = QueueStatusResource.parse_obj({
             "id": obj.get("id"),
-            "title": obj.get("title"),
-            "parsed_movie_info": ParsedMovieInfo.from_dict(obj.get("parsedMovieInfo")) if obj.get("parsedMovieInfo") is not None else None,
-            "movie": MovieResource.from_dict(obj.get("movie")) if obj.get("movie") is not None else None
+            "total_count": obj.get("totalCount"),
+            "count": obj.get("count"),
+            "unknown_count": obj.get("unknownCount"),
+            "errors": obj.get("errors"),
+            "warnings": obj.get("warnings"),
+            "unknown_errors": obj.get("unknownErrors"),
+            "unknown_warnings": obj.get("unknownWarnings")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/parsed_movie_info.py` & `radarr-py-0.3.1/radarr/models/parsed_movie_info.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/ping_resource.py` & `radarr-py-0.3.1/radarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/profile_format_item_resource.py` & `radarr-py-0.3.1/radarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/proper_download_types.py` & `radarr-py-0.3.1/radarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/provider_message.py` & `radarr-py-0.3.1/radarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/provider_message_type.py` & `radarr-py-0.3.1/radarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/proxy_type.py` & `radarr-py-0.3.1/radarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/quality.py` & `radarr-py-0.3.1/radarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/quality_definition_resource.py` & `radarr-py-0.3.1/radarr/models/quality_definition_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/quality_model.py` & `radarr-py-0.3.1/radarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/quality_profile_quality_item_resource.py` & `radarr-py-0.3.1/radarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/quality_profile_resource.py` & `radarr-py-0.3.1/radarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/queue_bulk_resource.py` & `radarr-py-0.3.1/radarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/queue_resource.py` & `radarr-py-0.3.1/radarr/models/queue_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     """
     id: Optional[int]
     movie_id: Optional[int]
     movie: Optional[MovieResource]
     languages: Optional[List]
     quality: Optional[QualityModel]
     custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     size: Optional[float]
     title: Optional[str]
     sizeleft: Optional[float]
     timeleft: Optional[str]
     estimated_completion_time: Optional[datetime]
     status: Optional[str]
     tracked_download_status: Optional[TrackedDownloadStatus]
@@ -51,15 +52,15 @@
     status_messages: Optional[List]
     error_message: Optional[str]
     download_id: Optional[str]
     protocol: Optional[DownloadProtocol]
     download_client: Optional[str]
     indexer: Optional[str]
     output_path: Optional[str]
-    __properties = ["id", "movieId", "movie", "languages", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath"]
+    __properties = ["id", "movieId", "movie", "languages", "quality", "customFormats", "customFormatScore", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -173,14 +174,15 @@
         _obj = QueueResource.parse_obj({
             "id": obj.get("id"),
             "movie_id": obj.get("movieId"),
             "movie": MovieResource.from_dict(obj.get("movie")) if obj.get("movie") is not None else None,
             "languages": [Language.from_dict(_item) for _item in obj.get("languages")] if obj.get("languages") is not None else None,
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "size": obj.get("size"),
             "title": obj.get("title"),
             "sizeleft": obj.get("sizeleft"),
             "timeleft": obj.get("timeleft"),
             "estimated_completion_time": obj.get("estimatedCompletionTime"),
             "status": obj.get("status"),
             "tracked_download_status": obj.get("trackedDownloadStatus"),
```

### Comparing `radarr-py-0.3.0/radarr/models/queue_resource_paging_resource.py` & `radarr-py-0.3.1/radarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/queue_status_resource.py` & `radarr-py-0.3.1/radarr/models/task_resource.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 
-class QueueStatusResource(BaseModel):
+class TaskResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
-    total_count: Optional[int]
-    count: Optional[int]
-    unknown_count: Optional[int]
-    errors: Optional[bool]
-    warnings: Optional[bool]
-    unknown_errors: Optional[bool]
-    unknown_warnings: Optional[bool]
-    __properties = ["id", "totalCount", "count", "unknownCount", "errors", "warnings", "unknownErrors", "unknownWarnings"]
+    name: Optional[str]
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
@@ -49,40 +49,48 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QueueStatusResource:
-        """Create an instance of QueueStatusResource from a JSON string"""
+    def from_json(cls, json_str: str) -> TaskResource:
+        """Create an instance of TaskResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # set to None if name (nullable) is None
+        if self.name is None:
+            _dict['name'] = None
+
+        # set to None if task_name (nullable) is None
+        if self.task_name is None:
+            _dict['taskName'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QueueStatusResource:
-        """Create an instance of QueueStatusResource from a dict"""
+    def from_dict(cls, obj: dict) -> TaskResource:
+        """Create an instance of TaskResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QueueStatusResource.parse_obj(obj)
+            return TaskResource.parse_obj(obj)
 
-        _obj = QueueStatusResource.parse_obj({
+        _obj = TaskResource.parse_obj({
             "id": obj.get("id"),
-            "total_count": obj.get("totalCount"),
-            "count": obj.get("count"),
-            "unknown_count": obj.get("unknownCount"),
-            "errors": obj.get("errors"),
-            "warnings": obj.get("warnings"),
-            "unknown_errors": obj.get("unknownErrors"),
-            "unknown_warnings": obj.get("unknownWarnings")
+            "name": obj.get("name"),
+            "task_name": obj.get("taskName"),
+            "interval": obj.get("interval"),
+            "last_execution": obj.get("lastExecution"),
+            "last_start_time": obj.get("lastStartTime"),
+            "next_execution": obj.get("nextExecution"),
+            "last_duration": obj.get("lastDuration")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/rating_child.py` & `radarr-py-0.3.1/radarr/models/rating_child.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/rating_type.py` & `radarr-py-0.3.1/radarr/models/rating_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/ratings.py` & `radarr-py-0.3.1/radarr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/rejection.py` & `radarr-py-0.3.1/radarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/rejection_type.py` & `radarr-py-0.3.1/radarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/release_resource.py` & `radarr-py-0.3.1/radarr/models/release_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/remote_path_mapping_resource.py` & `radarr-py-0.3.1/radarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/rename_movie_resource.py` & `radarr-py-0.3.1/radarr/models/rename_movie_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/rescan_after_refresh_type.py` & `radarr-py-0.3.1/radarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/restriction_resource.py` & `radarr-py-0.3.1/radarr/models/restriction_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/revision.py` & `radarr-py-0.3.1/radarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/root_folder_resource.py` & `radarr-py-0.3.1/radarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/runtime_mode.py` & `radarr-py-0.3.1/radarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/select_option.py` & `radarr-py-0.3.1/radarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/sort_direction.py` & `radarr-py-0.3.1/radarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/source.py` & `radarr-py-0.3.1/radarr/models/source.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/source_type.py` & `radarr-py-0.3.1/radarr/models/source_type.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/system_resource.py` & `radarr-py-0.3.1/radarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/tag_details_resource.py` & `radarr-py-0.3.1/radarr/models/tag_details_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     label: Optional[str]
     delay_profile_ids: Optional[List]
     notification_ids: Optional[List]
     restriction_ids: Optional[List]
     import_list_ids: Optional[List]
     movie_ids: Optional[List]
     indexer_ids: Optional[List]
-    __properties = ["id", "label", "delayProfileIds", "notificationIds", "restrictionIds", "importListIds", "movieIds", "indexerIds"]
+    download_client_ids: Optional[List]
+    __properties = ["id", "label", "delayProfileIds", "notificationIds", "restrictionIds", "importListIds", "movieIds", "indexerIds", "downloadClientIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -87,14 +88,18 @@
         if self.movie_ids is None:
             _dict['movieIds'] = None
 
         # set to None if indexer_ids (nullable) is None
         if self.indexer_ids is None:
             _dict['indexerIds'] = None
 
+        # set to None if download_client_ids (nullable) is None
+        if self.download_client_ids is None:
+            _dict['downloadClientIds'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> TagDetailsResource:
         """Create an instance of TagDetailsResource from a dict"""
         if obj is None:
             return None
@@ -106,11 +111,12 @@
             "id": obj.get("id"),
             "label": obj.get("label"),
             "delay_profile_ids": obj.get("delayProfileIds"),
             "notification_ids": obj.get("notificationIds"),
             "restriction_ids": obj.get("restrictionIds"),
             "import_list_ids": obj.get("importListIds"),
             "movie_ids": obj.get("movieIds"),
-            "indexer_ids": obj.get("indexerIds")
+            "indexer_ids": obj.get("indexerIds"),
+            "download_client_ids": obj.get("downloadClientIds")
         })
         return _obj
```

### Comparing `radarr-py-0.3.0/radarr/models/tag_resource.py` & `radarr-py-0.3.1/radarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/task_resource.py` & `radarr-py-0.3.1/radarr/models/update_changes.py`

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

### Comparing `radarr-py-0.3.0/radarr/models/tmdb_country_code.py` & `radarr-py-0.3.1/radarr/models/tmdb_country_code.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/tracked_download_state.py` & `radarr-py-0.3.1/radarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/tracked_download_status.py` & `radarr-py-0.3.1/radarr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/tracked_download_status_message.py` & `radarr-py-0.3.1/radarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/ui_config_resource.py` & `radarr-py-0.3.1/radarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/unmapped_folder.py` & `radarr-py-0.3.1/radarr/models/unmapped_folder.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/update_mechanism.py` & `radarr-py-0.3.1/radarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/models/update_resource.py` & `radarr-py-0.3.1/radarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr/rest.py` & `radarr-py-0.3.1/radarr/rest.py`

 * *Files identical despite different names*

### Comparing `radarr-py-0.3.0/radarr_py.egg-info/PKG-INFO` & `radarr-py-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: radarr-py
-Version: 0.3.0
-Summary: Radarr API wrapper
-Project-URL: Homepage, https://github.com/devopsarr/radarr-py
-Project-URL: Bug Tracker, https://github.com/devopsarr/radarr-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # radarr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.3.1
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -156,17 +143,19 @@
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v3/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v3/delayprofile/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v3/diskspace | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v3/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v3/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v3/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v3/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v3/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v3/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v3/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v3/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v3/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v3/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v3/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v3/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v3/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v3/config/downloadclient/{id} | 
 *ExtraFileApi* | [**list_extra_file**](docs/ExtraFileApi.md#list_extra_file) | **GET** /api/v3/extrafile | 
@@ -187,31 +176,35 @@
 *ImportExclusionsApi* | [**delete_exclusions**](docs/ImportExclusionsApi.md#delete_exclusions) | **DELETE** /api/v3/exclusions/{id} | 
 *ImportExclusionsApi* | [**get_exclusions_by_id**](docs/ImportExclusionsApi.md#get_exclusions_by_id) | **GET** /api/v3/exclusions/{id} | 
 *ImportExclusionsApi* | [**list_exclusions**](docs/ImportExclusionsApi.md#list_exclusions) | **GET** /api/v3/exclusions | 
 *ImportExclusionsApi* | [**update_exclusions**](docs/ImportExclusionsApi.md#update_exclusions) | **PUT** /api/v3/exclusions/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v3/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v3/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v3/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v3/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v3/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v3/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v3/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v3/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v3/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v3/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v3/importlist/{id} | 
 *ImportListConfigApi* | [**get_import_list_config**](docs/ImportListConfigApi.md#get_import_list_config) | **GET** /api/v3/config/importlist | 
 *ImportListConfigApi* | [**get_import_list_config_by_id**](docs/ImportListConfigApi.md#get_import_list_config_by_id) | **GET** /api/v3/config/importlist/{id} | 
 *ImportListConfigApi* | [**update_import_list_config**](docs/ImportListConfigApi.md#update_import_list_config) | **PUT** /api/v3/config/importlist/{id} | 
 *ImportListMoviesApi* | [**create_importlist_movie**](docs/ImportListMoviesApi.md#create_importlist_movie) | **POST** /api/v3/importlist/movie | 
 *ImportListMoviesApi* | [**get_importlist_movie**](docs/ImportListMoviesApi.md#get_importlist_movie) | **GET** /api/v3/importlist/movie | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v3/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v3/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v3/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v3/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v3/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v3/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v3/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v3/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v3/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v3/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v3/indexer/{id} | 
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v3/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v3/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v3/config/indexer/{id} | 
 *IndexerFlagApi* | [**list_indexer_flag**](docs/IndexerFlagApi.md#list_indexer_flag) | **GET** /api/v3/indexerflag | 
@@ -369,30 +362,33 @@
  - [CreditType](docs/CreditType.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [ExtraFileResource](docs/ExtraFileResource.md)
  - [ExtraFileType](docs/ExtraFileType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ImportExclusionsResource](docs/ImportExclusionsResource.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListConfigResource](docs/ImportListConfigResource.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerFlagResource](docs/IndexerFlagResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [Language](docs/Language.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
```

### Comparing `radarr-py-0.3.0/radarr_py.egg-info/SOURCES.txt` & `radarr-py-0.3.1/radarr_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,30 +105,33 @@
 radarr/models/credit_type.py
 radarr/models/custom_filter_resource.py
 radarr/models/custom_format_resource.py
 radarr/models/custom_format_specification_schema.py
 radarr/models/database_type.py
 radarr/models/delay_profile_resource.py
 radarr/models/disk_space_resource.py
+radarr/models/download_client_bulk_resource.py
 radarr/models/download_client_config_resource.py
 radarr/models/download_client_resource.py
 radarr/models/download_protocol.py
 radarr/models/extra_file_resource.py
 radarr/models/extra_file_type.py
 radarr/models/field.py
 radarr/models/file_date_type.py
 radarr/models/health_check_result.py
 radarr/models/health_resource.py
 radarr/models/history_resource.py
 radarr/models/history_resource_paging_resource.py
 radarr/models/host_config_resource.py
 radarr/models/import_exclusions_resource.py
+radarr/models/import_list_bulk_resource.py
 radarr/models/import_list_config_resource.py
 radarr/models/import_list_resource.py
 radarr/models/import_list_type.py
+radarr/models/indexer_bulk_resource.py
 radarr/models/indexer_config_resource.py
 radarr/models/indexer_flag_resource.py
 radarr/models/indexer_resource.py
 radarr/models/language.py
 radarr/models/language_resource.py
 radarr/models/log_file_resource.py
 radarr/models/log_resource.py
```

