# Comparing `tmp/whisparr-py-0.2.2.tar.gz` & `tmp/whisparr-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisparr-py-0.2.2.tar", last modified: Mon Mar 27 14:24:41 2023, max compression
+gzip compressed data, was "whisparr-py-0.3.0.tar", last modified: Fri Jul 21 11:34:58 2023, max compression
```

## Comparing `whisparr-py-0.2.2.tar` & `whisparr-py-0.3.0.tar`

### file list

```diff
@@ -1,215 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:41.470728 whisparr-py-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37790 2023-03-27 14:24:41.470728 whisparr-py-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37312 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 14:24:41.470728 whisparr-py-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:41.418727 whisparr-py-0.2.2/whisparr/
--rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:41.430727 whisparr-py-0.2.2/whisparr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/alternative_title_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/credit_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35520 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53860 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19143 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/extra_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25841 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36651 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/import_exclusions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53188 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/import_list_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/import_list_movies_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52563 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/indexer_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19201 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52731 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/metadata_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30068 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/movie_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/movie_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36985 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/movie_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/movie_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/movie_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29130 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53403 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25234 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26160 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30997 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/rename_movie_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30291 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/restriction_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29523 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29537 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18042 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:41.466728 whisparr-py-0.2.2/whisparr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/add_movie_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/add_movie_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/alternative_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/alternative_title_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/collection_movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/collection_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/collection_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/colon_replacement_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/credit_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/credit_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/extra_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/extra_file_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/import_exclusions_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/import_list_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6284 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/indexer_flag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/manual_import_reprocess_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/metadata_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    12221 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_runtime_format_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/movie_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/parsed_movie_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/rating_child.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/rating_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/rename_movie_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/restriction_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/source_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/tmdb_country_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/unmapped_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-03-27 14:24:23.000000 whisparr-py-0.2.2/whisparr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 14:24:41.470728 whisparr-py-0.2.2/whisparr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37790 2023-03-27 14:24:41.000000 whisparr-py-0.2.2/whisparr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-03-27 14:24:41.000000 whisparr-py-0.2.2/whisparr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 14:24:41.000000 whisparr-py-0.2.2/whisparr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-27 14:24:41.000000 whisparr-py-0.2.2/whisparr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 14:24:41.000000 whisparr-py-0.2.2/whisparr_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:34:58.334758 whisparr-py-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38803 2023-07-21 11:34:58.334758 whisparr-py-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    38325 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:34:58.334758 whisparr-py-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:34:58.294755 whisparr-py-0.3.0/whisparr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:34:58.310756 whisparr-py-0.3.0/whisparr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/alternative_title_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6156 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22488 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23735 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23477 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12802 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/credit_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35520 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30452 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67166 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19143 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/extra_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11943 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25841 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18588 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36651 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/import_exclusions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66270 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18911 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/import_list_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/import_list_movies_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65436 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6355 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/indexer_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11833 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14378 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19201 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53378 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/metadata_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31426 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/movie_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/movie_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36985 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/movie_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/movie_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23018 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/movie_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29130 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54050 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25234 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30644 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26160 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12877 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30997 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/rename_movie_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30291 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/restriction_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26851 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29523 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12011 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18410 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29651 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18220 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:34:58.330757 whisparr-py-0.3.0/whisparr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/add_movie_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/add_movie_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/alternative_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/alternative_title_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/collection_movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/collection_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/collection_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/colon_replacement_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/credit_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/credit_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/extra_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/extra_file_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/import_exclusions_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/import_list_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/import_list_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/indexer_flag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/manual_import_reprocess_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/metadata_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12228 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_runtime_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/movie_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/parsed_movie_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/rating_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/rating_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9444 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/rename_movie_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/restriction_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/source_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/tmdb_country_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/unmapped_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-21 11:34:41.000000 whisparr-py-0.3.0/whisparr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:34:58.330757 whisparr-py-0.3.0/whisparr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38803 2023-07-21 11:34:58.000000 whisparr-py-0.3.0/whisparr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7532 2023-07-21 11:34:58.000000 whisparr-py-0.3.0/whisparr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:34:58.000000 whisparr-py-0.3.0/whisparr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 11:34:58.000000 whisparr-py-0.3.0/whisparr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 11:34:58.000000 whisparr-py-0.3.0/whisparr_py.egg-info/top_level.txt
```

### Comparing `whisparr-py-0.2.2/LICENSE` & `whisparr-py-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/PKG-INFO` & `whisparr-py-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisparr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Radarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/whisparr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/whisparr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # whisparr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
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
@@ -358,40 +364,44 @@
  - [CollectionMovieResource](docs/CollectionMovieResource.md)
  - [CollectionResource](docs/CollectionResource.md)
  - [CollectionUpdateResource](docs/CollectionUpdateResource.md)
  - [ColonReplacementFormat](docs/ColonReplacementFormat.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CreditResource](docs/CreditResource.md)
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

### Comparing `whisparr-py-0.2.2/README.md` & `whisparr-py-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # whisparr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -143,17 +143,19 @@
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
@@ -174,31 +176,35 @@
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
@@ -345,40 +351,44 @@
  - [CollectionMovieResource](docs/CollectionMovieResource.md)
  - [CollectionResource](docs/CollectionResource.md)
  - [CollectionUpdateResource](docs/CollectionUpdateResource.md)
  - [ColonReplacementFormat](docs/ColonReplacementFormat.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CreditResource](docs/CreditResource.md)
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

### Comparing `whisparr-py-0.2.2/pyproject.toml` & `whisparr-py-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 [project]
 name = "whisparr-py"
-version = "0.2.2"
+version = "0.3.0"
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

### Comparing `whisparr-py-0.2.2/whisparr/__init__.py` & `whisparr-py-0.3.0/whisparr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 # x-release-please-end
 
 # import apis into sdk package
 from whisparr.api.alternative_title_api import AlternativeTitleApi
 from whisparr.api.api_info_api import ApiInfoApi
 from whisparr.api.authentication_api import AuthenticationApi
 from whisparr.api.backup_api import BackupApi
@@ -114,40 +114,44 @@
 from whisparr.models.collection_movie_resource import CollectionMovieResource
 from whisparr.models.collection_resource import CollectionResource
 from whisparr.models.collection_update_resource import CollectionUpdateResource
 from whisparr.models.colon_replacement_format import ColonReplacementFormat
 from whisparr.models.command import Command
 from whisparr.models.command_priority import CommandPriority
 from whisparr.models.command_resource import CommandResource
+from whisparr.models.command_result import CommandResult
 from whisparr.models.command_status import CommandStatus
 from whisparr.models.command_trigger import CommandTrigger
 from whisparr.models.credit_resource import CreditResource
 from whisparr.models.credit_type import CreditType
 from whisparr.models.custom_filter_resource import CustomFilterResource
 from whisparr.models.custom_format_resource import CustomFormatResource
 from whisparr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from whisparr.models.database_type import DatabaseType
 from whisparr.models.delay_profile_resource import DelayProfileResource
 from whisparr.models.disk_space_resource import DiskSpaceResource
+from whisparr.models.download_client_bulk_resource import DownloadClientBulkResource
 from whisparr.models.download_client_config_resource import DownloadClientConfigResource
 from whisparr.models.download_client_resource import DownloadClientResource
 from whisparr.models.download_protocol import DownloadProtocol
 from whisparr.models.extra_file_resource import ExtraFileResource
 from whisparr.models.extra_file_type import ExtraFileType
 from whisparr.models.field import Field
 from whisparr.models.file_date_type import FileDateType
 from whisparr.models.health_check_result import HealthCheckResult
 from whisparr.models.health_resource import HealthResource
 from whisparr.models.history_resource import HistoryResource
 from whisparr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from whisparr.models.host_config_resource import HostConfigResource
 from whisparr.models.import_exclusions_resource import ImportExclusionsResource
+from whisparr.models.import_list_bulk_resource import ImportListBulkResource
 from whisparr.models.import_list_config_resource import ImportListConfigResource
 from whisparr.models.import_list_resource import ImportListResource
 from whisparr.models.import_list_type import ImportListType
+from whisparr.models.indexer_bulk_resource import IndexerBulkResource
 from whisparr.models.indexer_config_resource import IndexerConfigResource
 from whisparr.models.indexer_flag_resource import IndexerFlagResource
 from whisparr.models.indexer_resource import IndexerResource
 from whisparr.models.language import Language
 from whisparr.models.language_resource import LanguageResource
 from whisparr.models.log_file_resource import LogFileResource
 from whisparr.models.log_resource import LogResource
```

### Comparing `whisparr-py-0.2.2/whisparr/api/__init__.py` & `whisparr-py-0.3.0/whisparr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/alternative_title_api.py` & `whisparr-py-0.3.0/whisparr/api/alternative_title_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/api_info_api.py` & `whisparr-py-0.3.0/whisparr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/authentication_api.py` & `whisparr-py-0.3.0/whisparr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/backup_api.py` & `whisparr-py-0.3.0/whisparr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/blocklist_api.py` & `whisparr-py-0.3.0/whisparr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/calendar_api.py` & `whisparr-py-0.3.0/whisparr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/calendar_feed_api.py` & `whisparr-py-0.3.0/whisparr/api/calendar_feed_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,29 +38,29 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_feed_v3_calendar_radarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+    def get_feed_v3_calendar_radarr_ics(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tags : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """get_feed_v3_calendar_radarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_feed_v3_calendar_radarr_ics(past_days, future_days, tag_list, unmonitored, async_req=True)
+        >>> thread = api.get_feed_v3_calendar_radarr_ics(past_days, future_days, tags, unmonitored, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
-        :param tag_list:
-        :type tag_list: str
+        :param tags:
+        :type tags: str
         :param unmonitored:
         :type unmonitored: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -71,32 +71,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, **kwargs)  # noqa: E501
+        return self.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tags, unmonitored, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_feed_v3_calendar_radarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tag_list : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+    def get_feed_v3_calendar_radarr_ics_with_http_info(self, past_days : Optional[StrictInt] = None, future_days : Optional[StrictInt] = None, tags : Optional[StrictStr] = None, unmonitored : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """get_feed_v3_calendar_radarr_ics  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tag_list, unmonitored, async_req=True)
+        >>> thread = api.get_feed_v3_calendar_radarr_ics_with_http_info(past_days, future_days, tags, unmonitored, async_req=True)
         >>> result = thread.get()
 
         :param past_days:
         :type past_days: int
         :param future_days:
         :type future_days: int
-        :param tag_list:
-        :type tag_list: str
+        :param tags:
+        :type tags: str
         :param unmonitored:
         :type unmonitored: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -120,15 +120,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'past_days',
             'future_days',
-            'tag_list',
+            'tags',
             'unmonitored'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -156,16 +156,16 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('past_days') is not None:  # noqa: E501
             _query_params.append(('pastDays', _params['past_days']))
         if _params.get('future_days') is not None:  # noqa: E501
             _query_params.append(('futureDays', _params['future_days']))
-        if _params.get('tag_list') is not None:  # noqa: E501
-            _query_params.append(('tagList', _params['tag_list']))
+        if _params.get('tags') is not None:  # noqa: E501
+            _query_params.append(('tags', _params['tags']))
         if _params.get('unmonitored') is not None:  # noqa: E501
             _query_params.append(('unmonitored', _params['unmonitored']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
```

### Comparing `whisparr-py-0.2.2/whisparr/api/collection_api.py` & `whisparr-py-0.3.0/whisparr/api/collection_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/command_api.py` & `whisparr-py-0.3.0/whisparr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/credit_api.py` & `whisparr-py-0.3.0/whisparr/api/credit_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/custom_filter_api.py` & `whisparr-py-0.3.0/whisparr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/custom_format_api.py` & `whisparr-py-0.3.0/whisparr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/delay_profile_api.py` & `whisparr-py-0.3.0/whisparr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/disk_space_api.py` & `whisparr-py-0.3.0/whisparr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/download_client_api.py` & `whisparr-py-0.3.0/whisparr/api/download_client_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from whisparr.models.download_client_bulk_resource import DownloadClientBulkResource
 from whisparr.models.download_client_resource import DownloadClientResource
 
 from whisparr.api_client import ApiClient
 from whisparr.exceptions import (  # noqa: F401
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
@@ -1150,25 +1448,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_download_client(self, id : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
+    def update_download_client(self, id : StrictStr, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
         """update_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client(id, download_client_resource, async_req=True)
+        >>> thread = api.update_download_client(id, force_save, download_client_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param download_client_resource:
         :type download_client_resource: DownloadClientResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1479,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: DownloadClientResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_download_client_with_http_info(id, download_client_resource, **kwargs)  # noqa: E501
+        return self.update_download_client_with_http_info(id, force_save, download_client_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_download_client_with_http_info(self, id : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
+    def update_download_client_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
         """update_download_client  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client_with_http_info(id, download_client_resource, async_req=True)
+        >>> thread = api.update_download_client_with_http_info(id, force_save, download_client_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param download_client_resource:
         :type download_client_resource: DownloadClientResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1525,15 @@
         :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'download_client_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1559,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1576,20 @@
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

### Comparing `whisparr-py-0.2.2/whisparr/api/download_client_config_api.py` & `whisparr-py-0.3.0/whisparr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/extra_file_api.py` & `whisparr-py-0.3.0/whisparr/api/extra_file_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/file_system_api.py` & `whisparr-py-0.3.0/whisparr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/health_api.py` & `whisparr-py-0.3.0/whisparr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/history_api.py` & `whisparr-py-0.3.0/whisparr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/host_config_api.py` & `whisparr-py-0.3.0/whisparr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/import_exclusions_api.py` & `whisparr-py-0.3.0/whisparr/api/import_exclusions_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/import_list_api.py` & `whisparr-py-0.3.0/whisparr/api/import_list_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from whisparr.models.import_list_bulk_resource import ImportListBulkResource
 from whisparr.models.import_list_resource import ImportListResource
 
 from whisparr.api_client import ApiClient
 from whisparr.exceptions import (  # noqa: F401
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
@@ -1150,25 +1448,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_import_list(self, id : StrictStr, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+    def update_import_list(self, id : StrictStr, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
         """update_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_import_list(id, import_list_resource, async_req=True)
+        >>> thread = api.update_import_list(id, force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1479,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ImportListResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_import_list_with_http_info(id, import_list_resource, **kwargs)  # noqa: E501
+        return self.update_import_list_with_http_info(id, force_save, import_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_import_list_with_http_info(self, id : StrictStr, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
+    def update_import_list_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
         """update_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_import_list_with_http_info(id, import_list_resource, async_req=True)
+        >>> thread = api.update_import_list_with_http_info(id, force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1525,15 @@
         :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'import_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1559,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1576,20 @@
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

### Comparing `whisparr-py-0.2.2/whisparr/api/import_list_config_api.py` & `whisparr-py-0.3.0/whisparr/api/import_list_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/import_list_movies_api.py` & `whisparr-py-0.3.0/whisparr/api/import_list_movies_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/indexer_api.py` & `whisparr-py-0.3.0/whisparr/api/indexer_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from whisparr.models.indexer_bulk_resource import IndexerBulkResource
 from whisparr.models.indexer_resource import IndexerResource
 
 from whisparr.api_client import ApiClient
 from whisparr.exceptions import (  # noqa: F401
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
@@ -1150,25 +1448,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+    def update_indexer(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
         """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer(id, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1479,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_with_http_info(id, indexer_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_with_http_info(id, force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_with_http_info(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+    def update_indexer_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
         """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_with_http_info(id, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer_with_http_info(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1525,15 @@
         :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1559,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1576,20 @@
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

### Comparing `whisparr-py-0.2.2/whisparr/api/indexer_config_api.py` & `whisparr-py-0.3.0/whisparr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/indexer_flag_api.py` & `whisparr-py-0.3.0/whisparr/api/indexer_flag_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/initialize_js_api.py` & `whisparr-py-0.3.0/whisparr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/language_api.py` & `whisparr-py-0.3.0/whisparr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/localization_api.py` & `whisparr-py-0.3.0/whisparr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/log_api.py` & `whisparr-py-0.3.0/whisparr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/log_file_api.py` & `whisparr-py-0.3.0/whisparr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/manual_import_api.py` & `whisparr-py-0.3.0/whisparr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/media_cover_api.py` & `whisparr-py-0.3.0/whisparr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/media_management_config_api.py` & `whisparr-py-0.3.0/whisparr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/metadata_api.py` & `whisparr-py-0.3.0/whisparr/api/metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from whisparr.models.metadata_resource import MetadataResource
 
 from whisparr.api_client import ApiClient
 from whisparr.exceptions import (  # noqa: F401
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
@@ -1150,25 +1157,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_metadata(self, id : StrictStr, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
+    def update_metadata(self, id : StrictStr, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
         """update_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_metadata(id, metadata_resource, async_req=True)
+        >>> thread = api.update_metadata(id, force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1188,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MetadataResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_metadata_with_http_info(id, metadata_resource, **kwargs)  # noqa: E501
+        return self.update_metadata_with_http_info(id, force_save, metadata_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_metadata_with_http_info(self, id : StrictStr, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
+    def update_metadata_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
         """update_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_metadata_with_http_info(id, metadata_resource, async_req=True)
+        >>> thread = api.update_metadata_with_http_info(id, force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1234,15 @@
         :rtype: tuple(MetadataResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'metadata_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1268,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1285,20 @@
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

### Comparing `whisparr-py-0.2.2/whisparr/api/metadata_config_api.py` & `whisparr-py-0.3.0/whisparr/api/metadata_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/movie_api.py` & `whisparr-py-0.3.0/whisparr/api/movie_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from whisparr.models.movie_resource import MovieResource
 
 from whisparr.api_client import ApiClient
 from whisparr.exceptions import (  # noqa: F401
@@ -187,25 +187,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_movie(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_movie(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_movie(id, async_req=True)
+        >>> thread = api.delete_movie(id, delete_files, add_import_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_exclusion:
+        :type add_import_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -214,28 +218,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_movie_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_movie_with_http_info(id, delete_files, add_import_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_movie_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_movie_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_movie_with_http_info(id, async_req=True)
+        >>> thread = api.delete_movie_with_http_info(id, delete_files, add_import_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_exclusion:
+        :type add_import_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -255,15 +263,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'delete_files',
+            'add_import_exclusion'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -288,14 +298,18 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('delete_files') is not None:  # noqa: E501
+            _query_params.append(('deleteFiles', _params['delete_files']))
+        if _params.get('add_import_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportExclusion', _params['add_import_exclusion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -604,25 +618,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_movie(self, id : StrictStr, movie_resource : Optional[MovieResource] = None, **kwargs) -> MovieResource:  # noqa: E501
+    def update_movie(self, id : StrictStr, move_files : Optional[StrictBool] = None, movie_resource : Optional[MovieResource] = None, **kwargs) -> MovieResource:  # noqa: E501
         """update_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_movie(id, movie_resource, async_req=True)
+        >>> thread = api.update_movie(id, move_files, movie_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param movie_resource:
         :type movie_resource: MovieResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -633,28 +649,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MovieResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_movie_with_http_info(id, movie_resource, **kwargs)  # noqa: E501
+        return self.update_movie_with_http_info(id, move_files, movie_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_movie_with_http_info(self, id : StrictStr, movie_resource : Optional[MovieResource] = None, **kwargs):  # noqa: E501
+    def update_movie_with_http_info(self, id : StrictStr, move_files : Optional[StrictBool] = None, movie_resource : Optional[MovieResource] = None, **kwargs):  # noqa: E501
         """update_movie  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_movie_with_http_info(id, movie_resource, async_req=True)
+        >>> thread = api.update_movie_with_http_info(id, move_files, movie_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param movie_resource:
         :type movie_resource: MovieResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -677,14 +695,15 @@
         :rtype: tuple(MovieResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'move_files',
             'movie_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -710,14 +729,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('move_files') is not None:  # noqa: E501
+            _query_params.append(('moveFiles', _params['move_files']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `whisparr-py-0.2.2/whisparr/api/movie_editor_api.py` & `whisparr-py-0.3.0/whisparr/api/movie_editor_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/movie_file_api.py` & `whisparr-py-0.3.0/whisparr/api/movie_file_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/movie_import_api.py` & `whisparr-py-0.3.0/whisparr/api/movie_import_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/movie_lookup_api.py` & `whisparr-py-0.3.0/whisparr/api/movie_lookup_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/naming_config_api.py` & `whisparr-py-0.3.0/whisparr/api/naming_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/notification_api.py` & `whisparr-py-0.3.0/whisparr/api/notification_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from whisparr.models.notification_resource import NotificationResource
 
 from whisparr.api_client import ApiClient
 from whisparr.exceptions import (  # noqa: F401
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
@@ -1150,25 +1157,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_notification(self, id : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+    def update_notification(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
         """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification(id, notification_resource, async_req=True)
+        >>> thread = api.update_notification(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param notification_resource:
         :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1188,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_notification_with_http_info(id, notification_resource, **kwargs)  # noqa: E501
+        return self.update_notification_with_http_info(id, force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_notification_with_http_info(self, id : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+    def update_notification_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
         """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification_with_http_info(id, notification_resource, async_req=True)
+        >>> thread = api.update_notification_with_http_info(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param notification_resource:
         :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1234,15 @@
         :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1268,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1285,20 @@
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

### Comparing `whisparr-py-0.2.2/whisparr/api/parse_api.py` & `whisparr-py-0.3.0/whisparr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/ping_api.py` & `whisparr-py-0.3.0/whisparr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/quality_definition_api.py` & `whisparr-py-0.3.0/whisparr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/quality_profile_api.py` & `whisparr-py-0.3.0/whisparr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/quality_profile_schema_api.py` & `whisparr-py-0.3.0/whisparr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/queue_action_api.py` & `whisparr-py-0.3.0/whisparr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/queue_api.py` & `whisparr-py-0.3.0/whisparr/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/queue_details_api.py` & `whisparr-py-0.3.0/whisparr/api/queue_details_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/queue_status_api.py` & `whisparr-py-0.3.0/whisparr/api/queue_status_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/release_api.py` & `whisparr-py-0.3.0/whisparr/api/release_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/release_push_api.py` & `whisparr-py-0.3.0/whisparr/api/release_push_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/remote_path_mapping_api.py` & `whisparr-py-0.3.0/whisparr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/rename_movie_api.py` & `whisparr-py-0.3.0/whisparr/api/rename_movie_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/restriction_api.py` & `whisparr-py-0.3.0/whisparr/api/restriction_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/root_folder_api.py` & `whisparr-py-0.3.0/whisparr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/static_resource_api.py` & `whisparr-py-0.3.0/whisparr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/system_api.py` & `whisparr-py-0.3.0/whisparr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/tag_api.py` & `whisparr-py-0.3.0/whisparr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/tag_details_api.py` & `whisparr-py-0.3.0/whisparr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/task_api.py` & `whisparr-py-0.3.0/whisparr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/ui_config_api.py` & `whisparr-py-0.3.0/whisparr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/update_api.py` & `whisparr-py-0.3.0/whisparr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api/update_log_file_api.py` & `whisparr-py-0.3.0/whisparr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/api_client.py` & `whisparr-py-0.3.0/whisparr/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'whisparr-py/v0.2.2'
+        self.user_agent = 'whisparr-py/v0.3.0'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
@@ -187,14 +187,18 @@
 
         # auth setting
         self.update_params_for_auth(
             header_params, query_params, auth_settings,
             resource_path, method, body,
             request_auth=_request_auth)
 
+        # request timeout
+        if not _request_timeout:
+            _request_timeout = config.request_timeout
+
         # body
         if body:
             body = self.sanitize_for_serialization(body)
 
         # request url
         if _host is None:
             url = self.configuration.host + resource_path
```

### Comparing `whisparr-py-0.2.2/whisparr/configuration.py` & `whisparr-py-0.3.0/whisparr/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
       and data received from the server, independent of any validation performed by
       the server side. If the input data does not satisfy the JSON schema validation
       rules specified in the OpenAPI document, an exception is raised.
       If disabled_client_side_validations is set, structural validation is
       disabled. This can be useful to troubleshoot data validation problem, such as
       when the OpenAPI document validation rules do not match the actual API data
       received by the server.
+    :param request_timeout: Default request timeout.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
@@ -105,14 +106,15 @@
     _default = None
 
     def __init__(self, host=None,
                  api_key=None, api_key_prefix=None,
                  username=None, password=None,
                  discard_unknown_keys=False,
                  disabled_client_side_validations="",
+                 request_timeout=None,
                  server_index=None, server_variables=None,
                  server_operation_index=None, server_operation_variables=None,
                  ssl_ca_cert=None,
                  ):
         """Constructor
         """
         self._base_path = "http://localhost:7878" if host is None else host
@@ -147,14 +149,17 @@
         """Username for HTTP basic authentication
         """
         self.password = password
         """Password for HTTP basic authentication
         """
         self.discard_unknown_keys = discard_unknown_keys
         self.disabled_client_side_validations = disabled_client_side_validations
+        self.request_timeout = request_timeout
+        """Request Timeout
+        """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("whisparr")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
@@ -421,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.2.2'
+        sdkversion = '0.3.0'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `whisparr-py-0.2.2/whisparr/exceptions.py` & `whisparr-py-0.3.0/whisparr/exceptions.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/__init__.py` & `whisparr-py-0.3.0/whisparr/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,40 +31,44 @@
 from whisparr.models.collection_movie_resource import CollectionMovieResource
 from whisparr.models.collection_resource import CollectionResource
 from whisparr.models.collection_update_resource import CollectionUpdateResource
 from whisparr.models.colon_replacement_format import ColonReplacementFormat
 from whisparr.models.command import Command
 from whisparr.models.command_priority import CommandPriority
 from whisparr.models.command_resource import CommandResource
+from whisparr.models.command_result import CommandResult
 from whisparr.models.command_status import CommandStatus
 from whisparr.models.command_trigger import CommandTrigger
 from whisparr.models.credit_resource import CreditResource
 from whisparr.models.credit_type import CreditType
 from whisparr.models.custom_filter_resource import CustomFilterResource
 from whisparr.models.custom_format_resource import CustomFormatResource
 from whisparr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from whisparr.models.database_type import DatabaseType
 from whisparr.models.delay_profile_resource import DelayProfileResource
 from whisparr.models.disk_space_resource import DiskSpaceResource
+from whisparr.models.download_client_bulk_resource import DownloadClientBulkResource
 from whisparr.models.download_client_config_resource import DownloadClientConfigResource
 from whisparr.models.download_client_resource import DownloadClientResource
 from whisparr.models.download_protocol import DownloadProtocol
 from whisparr.models.extra_file_resource import ExtraFileResource
 from whisparr.models.extra_file_type import ExtraFileType
 from whisparr.models.field import Field
 from whisparr.models.file_date_type import FileDateType
 from whisparr.models.health_check_result import HealthCheckResult
 from whisparr.models.health_resource import HealthResource
 from whisparr.models.history_resource import HistoryResource
 from whisparr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from whisparr.models.host_config_resource import HostConfigResource
 from whisparr.models.import_exclusions_resource import ImportExclusionsResource
+from whisparr.models.import_list_bulk_resource import ImportListBulkResource
 from whisparr.models.import_list_config_resource import ImportListConfigResource
 from whisparr.models.import_list_resource import ImportListResource
 from whisparr.models.import_list_type import ImportListType
+from whisparr.models.indexer_bulk_resource import IndexerBulkResource
 from whisparr.models.indexer_config_resource import IndexerConfigResource
 from whisparr.models.indexer_flag_resource import IndexerFlagResource
 from whisparr.models.indexer_resource import IndexerResource
 from whisparr.models.language import Language
 from whisparr.models.language_resource import LanguageResource
 from whisparr.models.log_file_resource import LogFileResource
 from whisparr.models.log_resource import LogResource
```

### Comparing `whisparr-py-0.2.2/whisparr/models/add_movie_method.py` & `whisparr-py-0.3.0/whisparr/models/add_movie_method.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/add_movie_options.py` & `whisparr-py-0.3.0/whisparr/models/add_movie_options.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/alternative_title.py` & `whisparr-py-0.3.0/whisparr/models/alternative_title.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/alternative_title_resource.py` & `whisparr-py-0.3.0/whisparr/models/alternative_title_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/api_info_resource.py` & `whisparr-py-0.3.0/whisparr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/apply_tags.py` & `whisparr-py-0.3.0/whisparr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/authentication_type.py` & `whisparr-py-0.3.0/whisparr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/backup_resource.py` & `whisparr-py-0.3.0/whisparr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/backup_type.py` & `whisparr-py-0.3.0/whisparr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/blocklist_bulk_resource.py` & `whisparr-py-0.3.0/whisparr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/blocklist_resource.py` & `whisparr-py-0.3.0/whisparr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/blocklist_resource_paging_resource.py` & `whisparr-py-0.3.0/whisparr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/certificate_validation_type.py` & `whisparr-py-0.3.0/whisparr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/collection_movie_resource.py` & `whisparr-py-0.3.0/whisparr/models/collection_movie_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/collection_resource.py` & `whisparr-py-0.3.0/whisparr/models/collection_resource.py`

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

### Comparing `whisparr-py-0.2.2/whisparr/models/collection_update_resource.py` & `whisparr-py-0.3.0/whisparr/models/collection_update_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/colon_replacement_format.py` & `whisparr-py-0.3.0/whisparr/models/colon_replacement_format.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/command.py` & `whisparr-py-0.3.0/whisparr/models/command.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/command_priority.py` & `whisparr-py-0.3.0/whisparr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/command_resource.py` & `whisparr-py-0.3.0/whisparr/models/command_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel
 from whisparr.models.command import Command
 from whisparr.models.command_priority import CommandPriority
+from whisparr.models.command_result import CommandResult
 from whisparr.models.command_status import CommandStatus
 from whisparr.models.command_trigger import CommandTrigger
 
 class CommandResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -33,26 +34,27 @@
     id: Optional[int]
     name: Optional[str]
     command_name: Optional[str]
     message: Optional[str]
     body: Optional[Command]
     priority: Optional[CommandPriority]
     status: Optional[CommandStatus]
+    result: Optional[CommandResult]
     queued: Optional[datetime]
     started: Optional[datetime]
     ended: Optional[datetime]
     duration: Optional[str]
     exception: Optional[str]
     trigger: Optional[CommandTrigger]
     client_user_agent: Optional[str]
     state_change_time: Optional[datetime]
     send_updates_to_client: Optional[bool]
     update_scheduled_task: Optional[bool]
     last_execution_time: Optional[datetime]
-    __properties = ["id", "name", "commandName", "message", "body", "priority", "status", "queued", "started", "ended", "duration", "exception", "trigger", "clientUserAgent", "stateChangeTime", "sendUpdatesToClient", "updateScheduledTask", "lastExecutionTime"]
+    __properties = ["id", "name", "commandName", "message", "body", "priority", "status", "result", "queued", "started", "ended", "duration", "exception", "trigger", "clientUserAgent", "stateChangeTime", "sendUpdatesToClient", "updateScheduledTask", "lastExecutionTime"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -131,14 +133,15 @@
             "id": obj.get("id"),
             "name": obj.get("name"),
             "command_name": obj.get("commandName"),
             "message": obj.get("message"),
             "body": Command.from_dict(obj.get("body")) if obj.get("body") is not None else None,
             "priority": obj.get("priority"),
             "status": obj.get("status"),
+            "result": obj.get("result"),
             "queued": obj.get("queued"),
             "started": obj.get("started"),
             "ended": obj.get("ended"),
             "duration": obj.get("duration"),
             "exception": obj.get("exception"),
             "trigger": obj.get("trigger"),
             "client_user_agent": obj.get("clientUserAgent"),
```

### Comparing `whisparr-py-0.2.2/whisparr/models/command_status.py` & `whisparr-py-0.3.0/whisparr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/command_trigger.py` & `whisparr-py-0.3.0/whisparr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/credit_resource.py` & `whisparr-py-0.3.0/whisparr/models/credit_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/credit_type.py` & `whisparr-py-0.3.0/whisparr/models/credit_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/custom_filter_resource.py` & `whisparr-py-0.3.0/whisparr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/custom_format_resource.py` & `whisparr-py-0.3.0/whisparr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/custom_format_specification_schema.py` & `whisparr-py-0.3.0/whisparr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/database_type.py` & `whisparr-py-0.3.0/whisparr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/delay_profile_resource.py` & `whisparr-py-0.3.0/whisparr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/disk_space_resource.py` & `whisparr-py-0.3.0/whisparr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/download_client_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/download_client_resource.py` & `whisparr-py-0.3.0/whisparr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/download_protocol.py` & `whisparr-py-0.3.0/whisparr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/extra_file_resource.py` & `whisparr-py-0.3.0/whisparr/models/extra_file_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/extra_file_type.py` & `whisparr-py-0.3.0/whisparr/models/extra_file_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/field.py` & `whisparr-py-0.3.0/whisparr/models/field.py`

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

### Comparing `whisparr-py-0.2.2/whisparr/models/file_date_type.py` & `whisparr-py-0.3.0/whisparr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/health_check_result.py` & `whisparr-py-0.3.0/whisparr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/health_resource.py` & `whisparr-py-0.3.0/whisparr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/history_resource.py` & `whisparr-py-0.3.0/whisparr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/history_resource_paging_resource.py` & `whisparr-py-0.3.0/whisparr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/host_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/import_exclusions_resource.py` & `whisparr-py-0.3.0/whisparr/models/import_exclusions_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/import_list_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/import_list_config_resource.py`

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

### Comparing `whisparr-py-0.2.2/whisparr/models/import_list_resource.py` & `whisparr-py-0.3.0/whisparr/models/import_list_resource.py`

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

### Comparing `whisparr-py-0.2.2/whisparr/models/import_list_type.py` & `whisparr-py-0.3.0/whisparr/models/import_list_type.py`

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

### Comparing `whisparr-py-0.2.2/whisparr/models/indexer_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/indexer_flag_resource.py` & `whisparr-py-0.3.0/whisparr/models/indexer_flag_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/indexer_resource.py` & `whisparr-py-0.3.0/whisparr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/language.py` & `whisparr-py-0.3.0/whisparr/models/language.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/language_resource.py` & `whisparr-py-0.3.0/whisparr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/log_file_resource.py` & `whisparr-py-0.3.0/whisparr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/log_resource.py` & `whisparr-py-0.3.0/whisparr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/log_resource_paging_resource.py` & `whisparr-py-0.3.0/whisparr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/manual_import_reprocess_resource.py` & `whisparr-py-0.3.0/whisparr/models/manual_import_reprocess_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/manual_import_resource.py` & `whisparr-py-0.3.0/whisparr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/media_cover.py` & `whisparr-py-0.3.0/whisparr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/media_cover_types.py` & `whisparr-py-0.3.0/whisparr/models/update_mechanism.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,25 +15,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MediaCoverTypes(str, Enum):
+class UpdateMechanism(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    UNKNOWN = 'unknown'
-    POSTER = 'poster'
-    BANNER = 'banner'
-    FANART = 'fanart'
-    SCREENSHOT = 'screenshot'
-    HEADSHOT = 'headshot'
+    BUILTIN = 'builtIn'
+    SCRIPT = 'script'
+    EXTERNAL = 'external'
+    APT = 'apt'
+    DOCKER = 'docker'
```

### Comparing `whisparr-py-0.2.2/whisparr/models/media_info_resource.py` & `whisparr-py-0.3.0/whisparr/models/media_info_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 
 class MediaInfoResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
```

### Comparing `whisparr-py-0.2.2/whisparr/models/media_management_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/media_management_config_resource.py`

 * *Files 12% similar despite different names*

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

### Comparing `whisparr-py-0.2.2/whisparr/models/metadata_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/metadata_config_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/metadata_resource.py` & `whisparr-py-0.3.0/whisparr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/modifier.py` & `whisparr-py-0.3.0/whisparr/models/modifier.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/monitor_types.py` & `whisparr-py-0.3.0/whisparr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_collection.py` & `whisparr-py-0.3.0/whisparr/models/movie_collection.py`

 * *Files 2% similar despite different names*

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

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_editor_resource.py` & `whisparr-py-0.3.0/whisparr/models/movie_editor_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_file_list_resource.py` & `whisparr-py-0.3.0/whisparr/models/movie_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_file_resource.py` & `whisparr-py-0.3.0/whisparr/models/movie_file_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_history_event_type.py` & `whisparr-py-0.3.0/whisparr/models/movie_history_event_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_metadata.py` & `whisparr-py-0.3.0/whisparr/models/movie_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from whisparr.models.alternative_title import AlternativeTitle
 from whisparr.models.language import Language
 from whisparr.models.media_cover import MediaCover
 from whisparr.models.movie_status_type import MovieStatusType
 from whisparr.models.movie_translation import MovieTranslation
 from whisparr.models.ratings import Ratings
```

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_resource.py` & `whisparr-py-0.3.0/whisparr/models/movie_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from whisparr.models.add_movie_options import AddMovieOptions
 from whisparr.models.alternative_title_resource import AlternativeTitleResource
 from whisparr.models.language import Language
 from whisparr.models.media_cover import MediaCover
 from whisparr.models.movie_collection import MovieCollection
 from whisparr.models.movie_file_resource import MovieFileResource
```

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_runtime_format_type.py` & `whisparr-py-0.3.0/whisparr/models/movie_runtime_format_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_status_type.py` & `whisparr-py-0.3.0/whisparr/models/movie_status_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/movie_translation.py` & `whisparr-py-0.3.0/whisparr/models/movie_translation.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/naming_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/naming_config_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/notification_resource.py` & `whisparr-py-0.3.0/whisparr/models/notification_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,28 +44,32 @@
     on_upgrade: Optional[bool]
     on_rename: Optional[bool]
     on_movie_added: Optional[bool]
     on_movie_delete: Optional[bool]
     on_movie_file_delete: Optional[bool]
     on_movie_file_delete_for_upgrade: Optional[bool]
     on_health_issue: Optional[bool]
+    on_health_restored: Optional[bool]
     on_application_update: Optional[bool]
+    on_manual_interaction_required: Optional[bool]
     supports_on_grab: Optional[bool]
     supports_on_download: Optional[bool]
     supports_on_upgrade: Optional[bool]
     supports_on_rename: Optional[bool]
     supports_on_movie_added: Optional[bool]
     supports_on_movie_delete: Optional[bool]
     supports_on_movie_file_delete: Optional[bool]
     supports_on_movie_file_delete_for_upgrade: Optional[bool]
     supports_on_health_issue: Optional[bool]
+    supports_on_health_restored: Optional[bool]
     supports_on_application_update: Optional[bool]
+    supports_on_manual_interaction_required: Optional[bool]
     include_health_warnings: Optional[bool]
     test_command: Optional[str]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onDownload", "onUpgrade", "onRename", "onMovieAdded", "onMovieDelete", "onMovieFileDelete", "onMovieFileDeleteForUpgrade", "onHealthIssue", "onApplicationUpdate", "supportsOnGrab", "supportsOnDownload", "supportsOnUpgrade", "supportsOnRename", "supportsOnMovieAdded", "supportsOnMovieDelete", "supportsOnMovieFileDelete", "supportsOnMovieFileDeleteForUpgrade", "supportsOnHealthIssue", "supportsOnApplicationUpdate", "includeHealthWarnings", "testCommand"]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "link", "onGrab", "onDownload", "onUpgrade", "onRename", "onMovieAdded", "onMovieDelete", "onMovieFileDelete", "onMovieFileDeleteForUpgrade", "onHealthIssue", "onHealthRestored", "onApplicationUpdate", "onManualInteractionRequired", "supportsOnGrab", "supportsOnDownload", "supportsOnUpgrade", "supportsOnRename", "supportsOnMovieAdded", "supportsOnMovieDelete", "supportsOnMovieFileDelete", "supportsOnMovieFileDeleteForUpgrade", "supportsOnHealthIssue", "supportsOnHealthRestored", "supportsOnApplicationUpdate", "supportsOnManualInteractionRequired", "includeHealthWarnings", "testCommand"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -175,23 +179,27 @@
             "on_upgrade": obj.get("onUpgrade"),
             "on_rename": obj.get("onRename"),
             "on_movie_added": obj.get("onMovieAdded"),
             "on_movie_delete": obj.get("onMovieDelete"),
             "on_movie_file_delete": obj.get("onMovieFileDelete"),
             "on_movie_file_delete_for_upgrade": obj.get("onMovieFileDeleteForUpgrade"),
             "on_health_issue": obj.get("onHealthIssue"),
+            "on_health_restored": obj.get("onHealthRestored"),
             "on_application_update": obj.get("onApplicationUpdate"),
+            "on_manual_interaction_required": obj.get("onManualInteractionRequired"),
             "supports_on_grab": obj.get("supportsOnGrab"),
             "supports_on_download": obj.get("supportsOnDownload"),
             "supports_on_upgrade": obj.get("supportsOnUpgrade"),
             "supports_on_rename": obj.get("supportsOnRename"),
             "supports_on_movie_added": obj.get("supportsOnMovieAdded"),
             "supports_on_movie_delete": obj.get("supportsOnMovieDelete"),
             "supports_on_movie_file_delete": obj.get("supportsOnMovieFileDelete"),
             "supports_on_movie_file_delete_for_upgrade": obj.get("supportsOnMovieFileDeleteForUpgrade"),
             "supports_on_health_issue": obj.get("supportsOnHealthIssue"),
+            "supports_on_health_restored": obj.get("supportsOnHealthRestored"),
             "supports_on_application_update": obj.get("supportsOnApplicationUpdate"),
+            "supports_on_manual_interaction_required": obj.get("supportsOnManualInteractionRequired"),
             "include_health_warnings": obj.get("includeHealthWarnings"),
             "test_command": obj.get("testCommand")
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/paging_resource_filter.py` & `whisparr-py-0.3.0/whisparr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/parse_resource.py` & `whisparr-py-0.3.0/whisparr/models/quality_definition_resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,30 +13,32 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
-from whisparr.models.movie_resource import MovieResource
-from whisparr.models.parsed_movie_info import ParsedMovieInfo
+from whisparr.models.quality import Quality
 
-class ParseResource(BaseModel):
+class QualityDefinitionResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
+    quality: Optional[Quality]
     title: Optional[str]
-    parsed_movie_info: Optional[ParsedMovieInfo]
-    movie: Optional[MovieResource]
-    __properties = ["id", "title", "parsedMovieInfo", "movie"]
+    weight: Optional[int]
+    min_size: Optional[float]
+    max_size: Optional[float]
+    preferred_size: Optional[float]
+    __properties = ["id", "quality", "title", "weight", "minSize", "maxSize", "preferredSize"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -47,46 +49,58 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ParseResource:
-        """Create an instance of ParseResource from a JSON string"""
+    def from_json(cls, json_str: str) -> QualityDefinitionResource:
+        """Create an instance of QualityDefinitionResource from a JSON string"""
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
+        # override the default output from pydantic by calling `to_dict()` of quality
+        if self.quality:
+            _dict['quality'] = self.quality.to_dict()
         # set to None if title (nullable) is None
         if self.title is None:
             _dict['title'] = None
 
+        # set to None if min_size (nullable) is None
+        if self.min_size is None:
+            _dict['minSize'] = None
+
+        # set to None if max_size (nullable) is None
+        if self.max_size is None:
+            _dict['maxSize'] = None
+
+        # set to None if preferred_size (nullable) is None
+        if self.preferred_size is None:
+            _dict['preferredSize'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ParseResource:
-        """Create an instance of ParseResource from a dict"""
+    def from_dict(cls, obj: dict) -> QualityDefinitionResource:
+        """Create an instance of QualityDefinitionResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ParseResource.parse_obj(obj)
+            return QualityDefinitionResource.parse_obj(obj)
 
-        _obj = ParseResource.parse_obj({
+        _obj = QualityDefinitionResource.parse_obj({
             "id": obj.get("id"),
+            "quality": Quality.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "title": obj.get("title"),
-            "parsed_movie_info": ParsedMovieInfo.from_dict(obj.get("parsedMovieInfo")) if obj.get("parsedMovieInfo") is not None else None,
-            "movie": MovieResource.from_dict(obj.get("movie")) if obj.get("movie") is not None else None
+            "weight": obj.get("weight"),
+            "min_size": obj.get("minSize"),
+            "max_size": obj.get("maxSize"),
+            "preferred_size": obj.get("preferredSize")
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/parsed_movie_info.py` & `whisparr-py-0.3.0/whisparr/models/parsed_movie_info.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/ping_resource.py` & `whisparr-py-0.3.0/whisparr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/profile_format_item_resource.py` & `whisparr-py-0.3.0/whisparr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/proper_download_types.py` & `whisparr-py-0.3.0/whisparr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/provider_message.py` & `whisparr-py-0.3.0/whisparr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/provider_message_type.py` & `whisparr-py-0.3.0/whisparr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/proxy_type.py` & `whisparr-py-0.3.0/whisparr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/quality.py` & `whisparr-py-0.3.0/whisparr/models/quality.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/quality_definition_resource.py` & `whisparr-py-0.3.0/whisparr/models/quality_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,29 +16,25 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
 from whisparr.models.quality import Quality
+from whisparr.models.revision import Revision
 
-class QualityDefinitionResource(BaseModel):
+class QualityModel(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
     quality: Optional[Quality]
-    title: Optional[str]
-    weight: Optional[int]
-    min_size: Optional[float]
-    max_size: Optional[float]
-    preferred_size: Optional[float]
-    __properties = ["id", "quality", "title", "weight", "minSize", "maxSize", "preferredSize"]
+    revision: Optional[Revision]
+    __properties = ["quality", "revision"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -49,58 +45,40 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QualityDefinitionResource:
-        """Create an instance of QualityDefinitionResource from a JSON string"""
+    def from_json(cls, json_str: str) -> QualityModel:
+        """Create an instance of QualityModel from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of quality
         if self.quality:
             _dict['quality'] = self.quality.to_dict()
-        # set to None if title (nullable) is None
-        if self.title is None:
-            _dict['title'] = None
-
-        # set to None if min_size (nullable) is None
-        if self.min_size is None:
-            _dict['minSize'] = None
-
-        # set to None if max_size (nullable) is None
-        if self.max_size is None:
-            _dict['maxSize'] = None
-
-        # set to None if preferred_size (nullable) is None
-        if self.preferred_size is None:
-            _dict['preferredSize'] = None
-
+        # override the default output from pydantic by calling `to_dict()` of revision
+        if self.revision:
+            _dict['revision'] = self.revision.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QualityDefinitionResource:
-        """Create an instance of QualityDefinitionResource from a dict"""
+    def from_dict(cls, obj: dict) -> QualityModel:
+        """Create an instance of QualityModel from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QualityDefinitionResource.parse_obj(obj)
+            return QualityModel.parse_obj(obj)
 
-        _obj = QualityDefinitionResource.parse_obj({
-            "id": obj.get("id"),
+        _obj = QualityModel.parse_obj({
             "quality": Quality.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
-            "title": obj.get("title"),
-            "weight": obj.get("weight"),
-            "min_size": obj.get("minSize"),
-            "max_size": obj.get("maxSize"),
-            "preferred_size": obj.get("preferredSize")
+            "revision": Revision.from_dict(obj.get("revision")) if obj.get("revision") is not None else None
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/quality_model.py` & `whisparr-py-0.3.0/whisparr/models/queue_bulk_resource.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,28 +13,25 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
-from whisparr.models.quality import Quality
-from whisparr.models.revision import Revision
 
-class QualityModel(BaseModel):
+class QueueBulkResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    quality: Optional[Quality]
-    revision: Optional[Revision]
-    __properties = ["quality", "revision"]
+    ids: Optional[List]
+    __properties = ["ids"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -45,40 +42,37 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QualityModel:
-        """Create an instance of QualityModel from a JSON string"""
+    def from_json(cls, json_str: str) -> QueueBulkResource:
+        """Create an instance of QueueBulkResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of quality
-        if self.quality:
-            _dict['quality'] = self.quality.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of revision
-        if self.revision:
-            _dict['revision'] = self.revision.to_dict()
+        # set to None if ids (nullable) is None
+        if self.ids is None:
+            _dict['ids'] = None
+
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QualityModel:
-        """Create an instance of QualityModel from a dict"""
+    def from_dict(cls, obj: dict) -> QueueBulkResource:
+        """Create an instance of QueueBulkResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QualityModel.parse_obj(obj)
+            return QueueBulkResource.parse_obj(obj)
 
-        _obj = QualityModel.parse_obj({
-            "quality": Quality.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
-            "revision": Revision.from_dict(obj.get("revision")) if obj.get("revision") is not None else None
+        _obj = QueueBulkResource.parse_obj({
+            "ids": obj.get("ids")
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/quality_profile_quality_item_resource.py` & `whisparr-py-0.3.0/whisparr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/quality_profile_resource.py` & `whisparr-py-0.3.0/whisparr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/queue_bulk_resource.py` & `whisparr-py-0.3.0/whisparr/models/tag_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
+from typing import Optional
 from pydantic import BaseModel
 
-class QueueBulkResource(BaseModel):
+class TagResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    ids: Optional[List]
-    __properties = ["ids"]
+    id: Optional[int]
+    label: Optional[str]
+    __properties = ["id", "label"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -42,37 +43,38 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QueueBulkResource:
-        """Create an instance of QueueBulkResource from a JSON string"""
+    def from_json(cls, json_str: str) -> TagResource:
+        """Create an instance of TagResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if ids (nullable) is None
-        if self.ids is None:
-            _dict['ids'] = None
+        # set to None if label (nullable) is None
+        if self.label is None:
+            _dict['label'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QueueBulkResource:
-        """Create an instance of QueueBulkResource from a dict"""
+    def from_dict(cls, obj: dict) -> TagResource:
+        """Create an instance of TagResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QueueBulkResource.parse_obj(obj)
+            return TagResource.parse_obj(obj)
 
-        _obj = QueueBulkResource.parse_obj({
-            "ids": obj.get("ids")
+        _obj = TagResource.parse_obj({
+            "id": obj.get("id"),
+            "label": obj.get("label")
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/queue_resource.py` & `whisparr-py-0.3.0/whisparr/models/queue_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from whisparr.models.custom_format_resource import CustomFormatResource
 from whisparr.models.download_protocol import DownloadProtocol
 from whisparr.models.language import Language
 from whisparr.models.movie_resource import MovieResource
 from whisparr.models.quality_model import QualityModel
 from whisparr.models.tracked_download_state import TrackedDownloadState
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

### Comparing `whisparr-py-0.2.2/whisparr/models/queue_resource_paging_resource.py` & `whisparr-py-0.3.0/whisparr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/queue_status_resource.py` & `whisparr-py-0.3.0/whisparr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/rating_child.py` & `whisparr-py-0.3.0/whisparr/models/rating_child.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import Optional, Union
 from pydantic import BaseModel
 from whisparr.models.rating_type import RatingType
 
 class RatingChild(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `whisparr-py-0.2.2/whisparr/models/rating_type.py` & `whisparr-py-0.3.0/whisparr/models/rating_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/ratings.py` & `whisparr-py-0.3.0/whisparr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/rejection.py` & `whisparr-py-0.3.0/whisparr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/rejection_type.py` & `whisparr-py-0.3.0/whisparr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/release_resource.py` & `whisparr-py-0.3.0/whisparr/models/release_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import List, Optional
+from typing import List, Optional, Union
 from pydantic import BaseModel
 from whisparr.models.custom_format_resource import CustomFormatResource
 from whisparr.models.download_protocol import DownloadProtocol
 from whisparr.models.language import Language
 from whisparr.models.quality_model import QualityModel
 
 class ReleaseResource(BaseModel):
```

### Comparing `whisparr-py-0.2.2/whisparr/models/remote_path_mapping_resource.py` & `whisparr-py-0.3.0/whisparr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/rename_movie_resource.py` & `whisparr-py-0.3.0/whisparr/models/rename_movie_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/rescan_after_refresh_type.py` & `whisparr-py-0.3.0/whisparr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/restriction_resource.py` & `whisparr-py-0.3.0/whisparr/models/restriction_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/revision.py` & `whisparr-py-0.3.0/whisparr/models/revision.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/root_folder_resource.py` & `whisparr-py-0.3.0/whisparr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/runtime_mode.py` & `whisparr-py-0.3.0/whisparr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/select_option.py` & `whisparr-py-0.3.0/whisparr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/sort_direction.py` & `whisparr-py-0.3.0/whisparr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/source.py` & `whisparr-py-0.3.0/whisparr/models/source.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/source_type.py` & `whisparr-py-0.3.0/whisparr/models/source_type.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/system_resource.py` & `whisparr-py-0.3.0/whisparr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/tag_details_resource.py` & `whisparr-py-0.3.0/whisparr/models/tag_details_resource.py`

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

### Comparing `whisparr-py-0.2.2/whisparr/models/tag_resource.py` & `whisparr-py-0.3.0/whisparr/models/unmapped_folder.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel
 
-class TagResource(BaseModel):
+class UnmappedFolder(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    label: Optional[str]
-    __properties = ["id", "label"]
+    name: Optional[str]
+    path: Optional[str]
+    __properties = ["name", "path"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -43,38 +43,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> TagResource:
-        """Create an instance of TagResource from a JSON string"""
+    def from_json(cls, json_str: str) -> UnmappedFolder:
+        """Create an instance of UnmappedFolder from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # set to None if label (nullable) is None
-        if self.label is None:
-            _dict['label'] = None
+        # set to None if name (nullable) is None
+        if self.name is None:
+            _dict['name'] = None
+
+        # set to None if path (nullable) is None
+        if self.path is None:
+            _dict['path'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> TagResource:
-        """Create an instance of TagResource from a dict"""
+    def from_dict(cls, obj: dict) -> UnmappedFolder:
+        """Create an instance of UnmappedFolder from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return TagResource.parse_obj(obj)
+            return UnmappedFolder.parse_obj(obj)
 
-        _obj = TagResource.parse_obj({
-            "id": obj.get("id"),
-            "label": obj.get("label")
+        _obj = UnmappedFolder.parse_obj({
+            "name": obj.get("name"),
+            "path": obj.get("path")
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/task_resource.py` & `whisparr-py-0.3.0/whisparr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/tmdb_country_code.py` & `whisparr-py-0.3.0/whisparr/models/tmdb_country_code.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/tracked_download_state.py` & `whisparr-py-0.3.0/whisparr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/tracked_download_status.py` & `whisparr-py-0.3.0/whisparr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/tracked_download_status_message.py` & `whisparr-py-0.3.0/whisparr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/ui_config_resource.py` & `whisparr-py-0.3.0/whisparr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/models/unmapped_folder.py` & `whisparr-py-0.3.0/whisparr/models/update_changes.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
 
-class UnmappedFolder(BaseModel):
+class UpdateChanges(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    name: Optional[str]
-    path: Optional[str]
-    __properties = ["name", "path"]
+    new: Optional[List]
+    fixed: Optional[List]
+    __properties = ["new", "fixed"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -43,42 +43,42 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UnmappedFolder:
-        """Create an instance of UnmappedFolder from a JSON string"""
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
-        # set to None if path (nullable) is None
-        if self.path is None:
-            _dict['path'] = None
+        # set to None if new (nullable) is None
+        if self.new is None:
+            _dict['new'] = None
+
+        # set to None if fixed (nullable) is None
+        if self.fixed is None:
+            _dict['fixed'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UnmappedFolder:
-        """Create an instance of UnmappedFolder from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateChanges:
+        """Create an instance of UpdateChanges from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UnmappedFolder.parse_obj(obj)
+            return UpdateChanges.parse_obj(obj)
 
-        _obj = UnmappedFolder.parse_obj({
-            "name": obj.get("name"),
-            "path": obj.get("path")
+        _obj = UpdateChanges.parse_obj({
+            "new": obj.get("new"),
+            "fixed": obj.get("fixed")
         })
         return _obj
```

### Comparing `whisparr-py-0.2.2/whisparr/models/update_mechanism.py` & `whisparr-py-0.3.0/whisparr/models/media_cover_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,24 +15,26 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class UpdateMechanism(str, Enum):
+class MediaCoverTypes(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    BUILTIN = 'builtIn'
-    SCRIPT = 'script'
-    EXTERNAL = 'external'
-    APT = 'apt'
-    DOCKER = 'docker'
+    UNKNOWN = 'unknown'
+    POSTER = 'poster'
+    BANNER = 'banner'
+    FANART = 'fanart'
+    SCREENSHOT = 'screenshot'
+    HEADSHOT = 'headshot'
+    CLEARLOGO = 'clearlogo'
```

### Comparing `whisparr-py-0.2.2/whisparr/models/update_resource.py` & `whisparr-py-0.3.0/whisparr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr/rest.py` & `whisparr-py-0.3.0/whisparr/rest.py`

 * *Files identical despite different names*

### Comparing `whisparr-py-0.2.2/whisparr_py.egg-info/PKG-INFO` & `whisparr-py-0.3.0/whisparr_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisparr-py
-Version: 0.2.2
+Version: 0.3.0
 Summary: Radarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/whisparr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/whisparr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # whisparr-py
 Radarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.2.2
+- Package version: 0.3.0
 
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
@@ -358,40 +364,44 @@
  - [CollectionMovieResource](docs/CollectionMovieResource.md)
  - [CollectionResource](docs/CollectionResource.md)
  - [CollectionUpdateResource](docs/CollectionUpdateResource.md)
  - [ColonReplacementFormat](docs/ColonReplacementFormat.md)
  - [Command](docs/Command.md)
  - [CommandPriority](docs/CommandPriority.md)
  - [CommandResource](docs/CommandResource.md)
+ - [CommandResult](docs/CommandResult.md)
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CreditResource](docs/CreditResource.md)
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

### Comparing `whisparr-py-0.2.2/whisparr_py.egg-info/SOURCES.txt` & `whisparr-py-0.3.0/whisparr_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 whisparr/__init__.py
 whisparr/api_client.py
+whisparr/api_response.py
 whisparr/configuration.py
 whisparr/exceptions.py
 whisparr/rest.py
 whisparr/api/__init__.py
 whisparr/api/alternative_title_api.py
 whisparr/api/api_info_api.py
 whisparr/api/authentication_api.py
@@ -93,40 +94,44 @@
 whisparr/models/collection_movie_resource.py
 whisparr/models/collection_resource.py
 whisparr/models/collection_update_resource.py
 whisparr/models/colon_replacement_format.py
 whisparr/models/command.py
 whisparr/models/command_priority.py
 whisparr/models/command_resource.py
+whisparr/models/command_result.py
 whisparr/models/command_status.py
 whisparr/models/command_trigger.py
 whisparr/models/credit_resource.py
 whisparr/models/credit_type.py
 whisparr/models/custom_filter_resource.py
 whisparr/models/custom_format_resource.py
 whisparr/models/custom_format_specification_schema.py
 whisparr/models/database_type.py
 whisparr/models/delay_profile_resource.py
 whisparr/models/disk_space_resource.py
+whisparr/models/download_client_bulk_resource.py
 whisparr/models/download_client_config_resource.py
 whisparr/models/download_client_resource.py
 whisparr/models/download_protocol.py
 whisparr/models/extra_file_resource.py
 whisparr/models/extra_file_type.py
 whisparr/models/field.py
 whisparr/models/file_date_type.py
 whisparr/models/health_check_result.py
 whisparr/models/health_resource.py
 whisparr/models/history_resource.py
 whisparr/models/history_resource_paging_resource.py
 whisparr/models/host_config_resource.py
 whisparr/models/import_exclusions_resource.py
+whisparr/models/import_list_bulk_resource.py
 whisparr/models/import_list_config_resource.py
 whisparr/models/import_list_resource.py
 whisparr/models/import_list_type.py
+whisparr/models/indexer_bulk_resource.py
 whisparr/models/indexer_config_resource.py
 whisparr/models/indexer_flag_resource.py
 whisparr/models/indexer_resource.py
 whisparr/models/language.py
 whisparr/models/language_resource.py
 whisparr/models/log_file_resource.py
 whisparr/models/log_resource.py
```

