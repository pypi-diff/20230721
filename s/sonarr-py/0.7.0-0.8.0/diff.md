# Comparing `tmp/sonarr-py-0.7.0.tar.gz` & `tmp/sonarr-py-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonarr-py-0.7.0.tar", last modified: Wed May 17 06:52:10 2023, max compression
+gzip compressed data, was "sonarr-py-0.8.0.tar", last modified: Fri Jul 21 11:36:03 2023, max compression
```

## Comparing `sonarr-py-0.7.0.tar` & `sonarr-py-0.8.0.tar`

### file list

```diff
@@ -1,212 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    38463 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    38013 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.256320 sonarr-py-0.7.0/sonarr/
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.264320 sonarr-py-0.7.0/sonarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/auto_tagging_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23355 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30322 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35487 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53633 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/episode_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43090 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/episode_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52961 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31059 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52336 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/language_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12220 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/language_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52504 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    32710 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53176 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25201 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26584 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18949 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30902 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/rename_episode_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/season_pass_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31995 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/series_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29393 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/sonarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/add_series_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/alternate_title_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/authentication_required_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/auto_tagging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/auto_tagging_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episode_title_required_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/episodes_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language_profile_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/localization_language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/localization_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/manual_import_reprocess_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/parsed_episode_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/privacy_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/quality_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/release_episode_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rename_episode_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_pass_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_pass_series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/season_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/series_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/unmapped_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-17 06:51:54.000000 sonarr-py-0.7.0/sonarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 06:52:10.284321 sonarr-py-0.7.0/sonarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    38463 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 06:52:10.000000 sonarr-py-0.7.0/sonarr_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:03.185179 sonarr-py-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    38412 2023-07-21 11:36:03.185179 sonarr-py-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37962 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:36:03.185179 sonarr-py-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:03.161179 sonarr-py-0.8.0/sonarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:03.169179 sonarr-py-0.8.0/sonarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35382 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/auto_tagging_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23355 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30322 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35967 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36454 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67042 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19110 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27107 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/episode_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43090 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/episode_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27649 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66146 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31059 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65312 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30556 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/language_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/language_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14753 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19168 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53256 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32710 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53928 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25201 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20924 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13318 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30611 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30902 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7136 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/rename_episode_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23628 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/season_pass_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31995 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/series_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/series_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/series_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29393 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:03.181179 sonarr-py-0.8.0/sonarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/add_series_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/alternate_title_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/authentication_required_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/auto_tagging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/auto_tagging_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episode_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episode_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episode_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7213 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episode_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episode_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episode_title_required_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/episodes_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/import_list_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/language_profile_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/language_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/localization_language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/localization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/manual_import_reprocess_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7671 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7541 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/parsed_episode_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/privacy_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/quality_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/release_episode_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14151 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/rename_episode_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/season_pass_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/season_pass_series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/season_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/season_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/series_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/series_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/series_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/series_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/series_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/unmapped_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-21 11:35:48.000000 sonarr-py-0.8.0/sonarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:03.185179 sonarr-py-0.8.0/sonarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38412 2023-07-21 11:36:03.000000 sonarr-py-0.8.0/sonarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-07-21 11:36:03.000000 sonarr-py-0.8.0/sonarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:36:03.000000 sonarr-py-0.8.0/sonarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 11:36:03.000000 sonarr-py-0.8.0/sonarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 11:36:03.000000 sonarr-py-0.8.0/sonarr_py.egg-info/top_level.txt
```

### Comparing `sonarr-py-0.7.0/PKG-INFO` & `sonarr-py-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonarr-py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Sonarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/sonarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/sonarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,15 +12,15 @@
 
 # sonarr-py
 Sonarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.7.0
+- Package version: 0.8.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -137,32 +137,34 @@
 *CustomFilterApi* | [**delete_custom_filter**](docs/CustomFilterApi.md#delete_custom_filter) | **DELETE** /api/v3/customfilter/{id} | 
 *CustomFilterApi* | [**get_custom_filter_by_id**](docs/CustomFilterApi.md#get_custom_filter_by_id) | **GET** /api/v3/customfilter/{id} | 
 *CustomFilterApi* | [**list_custom_filter**](docs/CustomFilterApi.md#list_custom_filter) | **GET** /api/v3/customfilter | 
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v3/customfilter/{id} | 
 *CustomFormatApi* | [**create_custom_format**](docs/CustomFormatApi.md#create_custom_format) | **POST** /api/v3/customformat | 
 *CustomFormatApi* | [**delete_custom_format**](docs/CustomFormatApi.md#delete_custom_format) | **DELETE** /api/v3/customformat/{id} | 
 *CustomFormatApi* | [**get_custom_format_by_id**](docs/CustomFormatApi.md#get_custom_format_by_id) | **GET** /api/v3/customformat/{id} | 
-*CustomFormatApi* | [**get_custom_format_schema**](docs/CustomFormatApi.md#get_custom_format_schema) | **GET** /api/v3/customformat/schema | 
 *CustomFormatApi* | [**list_custom_format**](docs/CustomFormatApi.md#list_custom_format) | **GET** /api/v3/customformat | 
+*CustomFormatApi* | [**list_custom_format_schema**](docs/CustomFormatApi.md#list_custom_format_schema) | **GET** /api/v3/customformat/schema | 
 *CustomFormatApi* | [**update_custom_format**](docs/CustomFormatApi.md#update_custom_format) | **PUT** /api/v3/customformat/{id} | 
 *CutoffApi* | [**get_wanted_cutoff**](docs/CutoffApi.md#get_wanted_cutoff) | **GET** /api/v3/wanted/cutoff | 
 *CutoffApi* | [**get_wanted_cutoff_by_id**](docs/CutoffApi.md#get_wanted_cutoff_by_id) | **GET** /api/v3/wanted/cutoff/{id} | 
 *DelayProfileApi* | [**create_delay_profile**](docs/DelayProfileApi.md#create_delay_profile) | **POST** /api/v3/delayprofile | 
 *DelayProfileApi* | [**delete_delay_profile**](docs/DelayProfileApi.md#delete_delay_profile) | **DELETE** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v3/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**update_delay_profile_reorder**](docs/DelayProfileApi.md#update_delay_profile_reorder) | **PUT** /api/v3/delayprofile/reorder/{id} | 
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
 *EpisodeApi* | [**get_episode_by_id**](docs/EpisodeApi.md#get_episode_by_id) | **GET** /api/v3/episode/{id} | 
@@ -175,59 +177,60 @@
 *EpisodeFileApi* | [**list_episode_file**](docs/EpisodeFileApi.md#list_episode_file) | **GET** /api/v3/episodefile | 
 *EpisodeFileApi* | [**put_episode_file_bulk**](docs/EpisodeFileApi.md#put_episode_file_bulk) | **PUT** /api/v3/episodefile/bulk | 
 *EpisodeFileApi* | [**put_episode_file_editor**](docs/EpisodeFileApi.md#put_episode_file_editor) | **PUT** /api/v3/episodefile/editor | 
 *EpisodeFileApi* | [**update_episode_file**](docs/EpisodeFileApi.md#update_episode_file) | **PUT** /api/v3/episodefile/{id} | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v3/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v3/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v3/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v3/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v3/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v3/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v3/history | 
 *HistoryApi* | [**list_history_series**](docs/HistoryApi.md#list_history_series) | **GET** /api/v3/history/series | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v3/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v3/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v3/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v3/config/host/{id} | 
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
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v3/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v3/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v3/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v3/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v3/importlistexclusion/{id} | 
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
-*InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LanguageApi* | [**get_language_by_id**](docs/LanguageApi.md#get_language_by_id) | **GET** /api/v3/language/{id} | 
 *LanguageApi* | [**list_language**](docs/LanguageApi.md#list_language) | **GET** /api/v3/language | 
 *LanguageProfileApi* | [**create_language_profile**](docs/LanguageProfileApi.md#create_language_profile) | **POST** /api/v3/languageprofile | 
 *LanguageProfileApi* | [**delete_language_profile**](docs/LanguageProfileApi.md#delete_language_profile) | **DELETE** /api/v3/languageprofile/{id} | 
 *LanguageProfileApi* | [**get_language_profile_by_id**](docs/LanguageProfileApi.md#get_language_profile_by_id) | **GET** /api/v3/languageprofile/{id} | 
 *LanguageProfileApi* | [**list_language_profile**](docs/LanguageProfileApi.md#list_language_profile) | **GET** /api/v3/languageprofile | 
 *LanguageProfileApi* | [**update_language_profile**](docs/LanguageProfileApi.md#update_language_profile) | **PUT** /api/v3/languageprofile/{id} | 
 *LanguageProfileSchemaApi* | [**get_languageprofile_schema**](docs/LanguageProfileSchemaApi.md#get_languageprofile_schema) | **GET** /api/v3/languageprofile/schema | 
-*LanguageProfileSchemaApi* | [**get_languageprofile_schema_by_id**](docs/LanguageProfileSchemaApi.md#get_languageprofile_schema_by_id) | **GET** /api/v3/languageprofile/schema/{id} | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v3/localization | 
 *LocalizationApi* | [**get_localization_by_id**](docs/LocalizationApi.md#get_localization_by_id) | **GET** /api/v3/localization/{id} | 
 *LocalizationApi* | [**get_localization_language**](docs/LocalizationApi.md#get_localization_language) | **GET** /api/v3/localization/language | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v3/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v3/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v3/log/file | 
 *ManualImportApi* | [**create_manual_import**](docs/ManualImportApi.md#create_manual_import) | **POST** /api/v3/manualimport | 
@@ -271,31 +274,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v3/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v3/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v3/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v3/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v3/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v3/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v3/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v3/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v3/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v3/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v3/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v3/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v3/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v3/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v3/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v3/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v3/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v3/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v3/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v3/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v3/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v3/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v3/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v3/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v3/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v3/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v3/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v3/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v3/remotepathmapping/{id} | 
 *RenameEpisodeApi* | [**list_rename**](docs/RenameEpisodeApi.md#list_rename) | **GET** /api/v3/rename | 
 *RootFolderApi* | [**create_root_folder**](docs/RootFolderApi.md#create_root_folder) | **POST** /api/v3/rootfolder | 
@@ -360,14 +358,15 @@
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [EpisodeFileListResource](docs/EpisodeFileListResource.md)
  - [EpisodeFileResource](docs/EpisodeFileResource.md)
  - [EpisodeHistoryEventType](docs/EpisodeHistoryEventType.md)
  - [EpisodeResource](docs/EpisodeResource.md)
@@ -377,17 +376,19 @@
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [Language](docs/Language.md)
  - [LanguageProfileItemResource](docs/LanguageProfileItemResource.md)
  - [LanguageProfileResource](docs/LanguageProfileResource.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [LocalizationLanguageResource](docs/LocalizationLanguageResource.md)
```

### Comparing `sonarr-py-0.7.0/README.md` & `sonarr-py-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # sonarr-py
 Sonarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.7.0
+- Package version: 0.8.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -125,32 +125,34 @@
 *CustomFilterApi* | [**delete_custom_filter**](docs/CustomFilterApi.md#delete_custom_filter) | **DELETE** /api/v3/customfilter/{id} | 
 *CustomFilterApi* | [**get_custom_filter_by_id**](docs/CustomFilterApi.md#get_custom_filter_by_id) | **GET** /api/v3/customfilter/{id} | 
 *CustomFilterApi* | [**list_custom_filter**](docs/CustomFilterApi.md#list_custom_filter) | **GET** /api/v3/customfilter | 
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v3/customfilter/{id} | 
 *CustomFormatApi* | [**create_custom_format**](docs/CustomFormatApi.md#create_custom_format) | **POST** /api/v3/customformat | 
 *CustomFormatApi* | [**delete_custom_format**](docs/CustomFormatApi.md#delete_custom_format) | **DELETE** /api/v3/customformat/{id} | 
 *CustomFormatApi* | [**get_custom_format_by_id**](docs/CustomFormatApi.md#get_custom_format_by_id) | **GET** /api/v3/customformat/{id} | 
-*CustomFormatApi* | [**get_custom_format_schema**](docs/CustomFormatApi.md#get_custom_format_schema) | **GET** /api/v3/customformat/schema | 
 *CustomFormatApi* | [**list_custom_format**](docs/CustomFormatApi.md#list_custom_format) | **GET** /api/v3/customformat | 
+*CustomFormatApi* | [**list_custom_format_schema**](docs/CustomFormatApi.md#list_custom_format_schema) | **GET** /api/v3/customformat/schema | 
 *CustomFormatApi* | [**update_custom_format**](docs/CustomFormatApi.md#update_custom_format) | **PUT** /api/v3/customformat/{id} | 
 *CutoffApi* | [**get_wanted_cutoff**](docs/CutoffApi.md#get_wanted_cutoff) | **GET** /api/v3/wanted/cutoff | 
 *CutoffApi* | [**get_wanted_cutoff_by_id**](docs/CutoffApi.md#get_wanted_cutoff_by_id) | **GET** /api/v3/wanted/cutoff/{id} | 
 *DelayProfileApi* | [**create_delay_profile**](docs/DelayProfileApi.md#create_delay_profile) | **POST** /api/v3/delayprofile | 
 *DelayProfileApi* | [**delete_delay_profile**](docs/DelayProfileApi.md#delete_delay_profile) | **DELETE** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v3/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**update_delay_profile_reorder**](docs/DelayProfileApi.md#update_delay_profile_reorder) | **PUT** /api/v3/delayprofile/reorder/{id} | 
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
 *EpisodeApi* | [**get_episode_by_id**](docs/EpisodeApi.md#get_episode_by_id) | **GET** /api/v3/episode/{id} | 
@@ -163,59 +165,60 @@
 *EpisodeFileApi* | [**list_episode_file**](docs/EpisodeFileApi.md#list_episode_file) | **GET** /api/v3/episodefile | 
 *EpisodeFileApi* | [**put_episode_file_bulk**](docs/EpisodeFileApi.md#put_episode_file_bulk) | **PUT** /api/v3/episodefile/bulk | 
 *EpisodeFileApi* | [**put_episode_file_editor**](docs/EpisodeFileApi.md#put_episode_file_editor) | **PUT** /api/v3/episodefile/editor | 
 *EpisodeFileApi* | [**update_episode_file**](docs/EpisodeFileApi.md#update_episode_file) | **PUT** /api/v3/episodefile/{id} | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v3/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v3/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v3/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v3/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v3/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v3/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v3/history | 
 *HistoryApi* | [**list_history_series**](docs/HistoryApi.md#list_history_series) | **GET** /api/v3/history/series | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v3/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v3/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v3/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v3/config/host/{id} | 
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
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v3/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v3/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v3/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v3/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v3/importlistexclusion/{id} | 
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
-*InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LanguageApi* | [**get_language_by_id**](docs/LanguageApi.md#get_language_by_id) | **GET** /api/v3/language/{id} | 
 *LanguageApi* | [**list_language**](docs/LanguageApi.md#list_language) | **GET** /api/v3/language | 
 *LanguageProfileApi* | [**create_language_profile**](docs/LanguageProfileApi.md#create_language_profile) | **POST** /api/v3/languageprofile | 
 *LanguageProfileApi* | [**delete_language_profile**](docs/LanguageProfileApi.md#delete_language_profile) | **DELETE** /api/v3/languageprofile/{id} | 
 *LanguageProfileApi* | [**get_language_profile_by_id**](docs/LanguageProfileApi.md#get_language_profile_by_id) | **GET** /api/v3/languageprofile/{id} | 
 *LanguageProfileApi* | [**list_language_profile**](docs/LanguageProfileApi.md#list_language_profile) | **GET** /api/v3/languageprofile | 
 *LanguageProfileApi* | [**update_language_profile**](docs/LanguageProfileApi.md#update_language_profile) | **PUT** /api/v3/languageprofile/{id} | 
 *LanguageProfileSchemaApi* | [**get_languageprofile_schema**](docs/LanguageProfileSchemaApi.md#get_languageprofile_schema) | **GET** /api/v3/languageprofile/schema | 
-*LanguageProfileSchemaApi* | [**get_languageprofile_schema_by_id**](docs/LanguageProfileSchemaApi.md#get_languageprofile_schema_by_id) | **GET** /api/v3/languageprofile/schema/{id} | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v3/localization | 
 *LocalizationApi* | [**get_localization_by_id**](docs/LocalizationApi.md#get_localization_by_id) | **GET** /api/v3/localization/{id} | 
 *LocalizationApi* | [**get_localization_language**](docs/LocalizationApi.md#get_localization_language) | **GET** /api/v3/localization/language | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v3/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v3/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v3/log/file | 
 *ManualImportApi* | [**create_manual_import**](docs/ManualImportApi.md#create_manual_import) | **POST** /api/v3/manualimport | 
@@ -259,31 +262,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v3/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v3/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v3/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v3/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v3/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v3/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v3/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v3/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v3/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v3/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v3/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v3/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v3/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v3/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v3/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v3/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v3/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v3/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v3/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v3/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v3/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v3/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v3/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v3/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v3/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v3/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v3/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v3/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v3/remotepathmapping/{id} | 
 *RenameEpisodeApi* | [**list_rename**](docs/RenameEpisodeApi.md#list_rename) | **GET** /api/v3/rename | 
 *RootFolderApi* | [**create_root_folder**](docs/RootFolderApi.md#create_root_folder) | **POST** /api/v3/rootfolder | 
@@ -348,14 +346,15 @@
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [EpisodeFileListResource](docs/EpisodeFileListResource.md)
  - [EpisodeFileResource](docs/EpisodeFileResource.md)
  - [EpisodeHistoryEventType](docs/EpisodeHistoryEventType.md)
  - [EpisodeResource](docs/EpisodeResource.md)
@@ -365,17 +364,19 @@
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [Language](docs/Language.md)
  - [LanguageProfileItemResource](docs/LanguageProfileItemResource.md)
  - [LanguageProfileResource](docs/LanguageProfileResource.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [LocalizationLanguageResource](docs/LocalizationLanguageResource.md)
```

### Comparing `sonarr-py-0.7.0/pyproject.toml` & `sonarr-py-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 [project]
 name = "sonarr-py"
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
-    "urllib3 >= 1.25.3",
+    "urllib3>=1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
-    "pydantic>=1.10.2",
+    "pydantic~=1.10.11",
     "aenum"
 ]
 description = "Sonarr API wrapper"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `sonarr-py-0.7.0/sonarr/__init__.py` & `sonarr-py-0.8.0/sonarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 # x-release-please-end
 
 # import apis into sdk package
 from sonarr.api.api_info_api import ApiInfoApi
 from sonarr.api.authentication_api import AuthenticationApi
 from sonarr.api.auto_tagging_api import AutoTaggingApi
 from sonarr.api.backup_api import BackupApi
@@ -40,15 +40,14 @@
 from sonarr.api.health_api import HealthApi
 from sonarr.api.history_api import HistoryApi
 from sonarr.api.host_config_api import HostConfigApi
 from sonarr.api.import_list_api import ImportListApi
 from sonarr.api.import_list_exclusion_api import ImportListExclusionApi
 from sonarr.api.indexer_api import IndexerApi
 from sonarr.api.indexer_config_api import IndexerConfigApi
-from sonarr.api.initialize_js_api import InitializeJsApi
 from sonarr.api.language_api import LanguageApi
 from sonarr.api.language_profile_api import LanguageProfileApi
 from sonarr.api.language_profile_schema_api import LanguageProfileSchemaApi
 from sonarr.api.localization_api import LocalizationApi
 from sonarr.api.log_api import LogApi
 from sonarr.api.log_file_api import LogFileApi
 from sonarr.api.manual_import_api import ManualImportApi
@@ -117,14 +116,15 @@
 from sonarr.models.command_status import CommandStatus
 from sonarr.models.command_trigger import CommandTrigger
 from sonarr.models.custom_filter_resource import CustomFilterResource
 from sonarr.models.custom_format_resource import CustomFormatResource
 from sonarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from sonarr.models.delay_profile_resource import DelayProfileResource
 from sonarr.models.disk_space_resource import DiskSpaceResource
+from sonarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from sonarr.models.download_client_config_resource import DownloadClientConfigResource
 from sonarr.models.download_client_resource import DownloadClientResource
 from sonarr.models.download_protocol import DownloadProtocol
 from sonarr.models.episode_file_list_resource import EpisodeFileListResource
 from sonarr.models.episode_file_resource import EpisodeFileResource
 from sonarr.models.episode_history_event_type import EpisodeHistoryEventType
 from sonarr.models.episode_resource import EpisodeResource
@@ -134,17 +134,19 @@
 from sonarr.models.field import Field
 from sonarr.models.file_date_type import FileDateType
 from sonarr.models.health_check_result import HealthCheckResult
 from sonarr.models.health_resource import HealthResource
 from sonarr.models.history_resource import HistoryResource
 from sonarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from sonarr.models.host_config_resource import HostConfigResource
+from sonarr.models.import_list_bulk_resource import ImportListBulkResource
 from sonarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from sonarr.models.import_list_resource import ImportListResource
 from sonarr.models.import_list_type import ImportListType
+from sonarr.models.indexer_bulk_resource import IndexerBulkResource
 from sonarr.models.indexer_config_resource import IndexerConfigResource
 from sonarr.models.indexer_resource import IndexerResource
 from sonarr.models.language import Language
 from sonarr.models.language_profile_item_resource import LanguageProfileItemResource
 from sonarr.models.language_profile_resource import LanguageProfileResource
 from sonarr.models.language_resource import LanguageResource
 from sonarr.models.localization_language_resource import LocalizationLanguageResource
```

### Comparing `sonarr-py-0.7.0/sonarr/api/__init__.py` & `sonarr-py-0.8.0/sonarr/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from sonarr.api.health_api import HealthApi
 from sonarr.api.history_api import HistoryApi
 from sonarr.api.host_config_api import HostConfigApi
 from sonarr.api.import_list_api import ImportListApi
 from sonarr.api.import_list_exclusion_api import ImportListExclusionApi
 from sonarr.api.indexer_api import IndexerApi
 from sonarr.api.indexer_config_api import IndexerConfigApi
-from sonarr.api.initialize_js_api import InitializeJsApi
 from sonarr.api.language_api import LanguageApi
 from sonarr.api.language_profile_api import LanguageProfileApi
 from sonarr.api.language_profile_schema_api import LanguageProfileSchemaApi
 from sonarr.api.localization_api import LocalizationApi
 from sonarr.api.log_api import LogApi
 from sonarr.api.log_file_api import LogFileApi
 from sonarr.api.manual_import_api import ManualImportApi
```

### Comparing `sonarr-py-0.7.0/sonarr/api/api_info_api.py` & `sonarr-py-0.8.0/sonarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/authentication_api.py` & `sonarr-py-0.8.0/sonarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/auto_tagging_api.py` & `sonarr-py-0.8.0/sonarr/api/auto_tagging_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/backup_api.py` & `sonarr-py-0.8.0/sonarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/blocklist_api.py` & `sonarr-py-0.8.0/sonarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/calendar_api.py` & `sonarr-py-0.8.0/sonarr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/calendar_feed_api.py` & `sonarr-py-0.8.0/sonarr/api/calendar_feed_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/command_api.py` & `sonarr-py-0.8.0/sonarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/custom_filter_api.py` & `sonarr-py-0.8.0/sonarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/custom_format_api.py` & `sonarr-py-0.8.0/sonarr/api/custom_format_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from typing_extensions import Annotated
 
 from pydantic import StrictInt, StrictStr
 
 from typing import List, Optional
 
 from sonarr.models.custom_format_resource import CustomFormatResource
+from sonarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
@@ -463,21 +464,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_custom_format_schema(self, **kwargs) -> None:  # noqa: E501
-        """get_custom_format_schema  # noqa: E501
+    def list_custom_format(self, **kwargs) -> List[CustomFormatResource]:  # noqa: E501
+        """list_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_custom_format_schema(async_req=True)
+        >>> thread = api.list_custom_format(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -485,27 +486,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: List[CustomFormatResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_custom_format_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_custom_format_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_custom_format_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """get_custom_format_schema  # noqa: E501
+    def list_custom_format_with_http_info(self, **kwargs):  # noqa: E501
+        """list_custom_format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_custom_format_schema_with_http_info(async_req=True)
+        >>> thread = api.list_custom_format_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -521,15 +522,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(List[CustomFormatResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -545,15 +546,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_custom_format_schema" % _key
+                    " to method list_custom_format" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -568,21 +569,27 @@
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "List[CustomFormatResource]",
+        }
 
         return self.api_client.call_api(
-            '/api/v3/customformat/schema', 'GET',
+            '/api/v3/customformat', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -591,21 +598,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_custom_format(self, **kwargs) -> List[CustomFormatResource]:  # noqa: E501
-        """list_custom_format  # noqa: E501
+    def list_custom_format_schema(self, **kwargs) -> List[CustomFormatSpecificationSchema]:  # noqa: E501
+        """list_custom_format_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_custom_format(async_req=True)
+        >>> thread = api.list_custom_format_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -613,27 +620,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[CustomFormatResource]
+        :rtype: List[CustomFormatSpecificationSchema]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_custom_format_with_http_info(**kwargs)  # noqa: E501
+        return self.list_custom_format_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_custom_format_with_http_info(self, **kwargs):  # noqa: E501
-        """list_custom_format  # noqa: E501
+    def list_custom_format_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_custom_format_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_custom_format_with_http_info(async_req=True)
+        >>> thread = api.list_custom_format_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -649,15 +656,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[CustomFormatResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[CustomFormatSpecificationSchema], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -673,15 +680,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_custom_format" % _key
+                    " to method list_custom_format_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -704,19 +711,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[CustomFormatResource]",
+            '200': "List[CustomFormatSpecificationSchema]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/customformat', 'GET',
+            '/api/v3/customformat/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/cutoff_api.py` & `sonarr-py-0.8.0/sonarr/api/cutoff_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/delay_profile_api.py` & `sonarr-py-0.8.0/sonarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/disk_space_api.py` & `sonarr-py-0.8.0/sonarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/download_client_api.py` & `sonarr-py-0.8.0/sonarr/api/download_client_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from sonarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from sonarr.models.download_client_resource import DownloadClientResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
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
@@ -153,15 +161,15 @@
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
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
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
@@ -1271,15 +1576,15 @@
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
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
```

### Comparing `sonarr-py-0.7.0/sonarr/api/download_client_config_api.py` & `sonarr-py-0.8.0/sonarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/episode_api.py` & `sonarr-py-0.8.0/sonarr/api/episode_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/episode_file_api.py` & `sonarr-py-0.8.0/sonarr/api/episode_file_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/file_system_api.py` & `sonarr-py-0.8.0/sonarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/health_api.py` & `sonarr-py-0.8.0/sonarr/api/log_file_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,81 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import constr, validator
 
 from typing import List
 
-from sonarr.models.health_resource import HealthResource
+from sonarr.models.log_file_resource import LogFileResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class HealthApi(object):
+class LogFileApi(object):
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
+    def get_log_file_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
+        """get_log_file_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id(id, async_req=True)
+        >>> thread = api.get_log_file_by_filename(filename, async_req=True)
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
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_health_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_log_file_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_health_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_health_by_id  # noqa: E501
+    def get_log_file_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
+        """get_log_file_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_log_file_by_filename_with_http_info(filename, async_req=True)
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
+        :rtype: None
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
@@ -126,52 +126,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_health_by_id" % _key
+                    " to method get_log_file_by_filename" % _key
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
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "HealthResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/health/{id}', 'GET',
+            '/api/v3/log/file/{filename}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,21 +174,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_health(self, **kwargs) -> List[HealthResource]:  # noqa: E501
-        """list_health  # noqa: E501
+    def list_log_file(self, **kwargs) -> List[LogFileResource]:  # noqa: E501
+        """list_log_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health(async_req=True)
+        >>> thread = api.list_log_file(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -202,27 +196,27 @@
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
+        return self.list_log_file_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_health_with_http_info(self, **kwargs):  # noqa: E501
-        """list_health  # noqa: E501
+    def list_log_file_with_http_info(self, **kwargs):  # noqa: E501
+        """list_log_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health_with_http_info(async_req=True)
+        >>> thread = api.list_log_file_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -238,15 +232,15 @@
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
@@ -262,15 +256,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_health" % _key
+                    " to method list_log_file" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -293,19 +287,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[HealthResource]",
+            '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/health', 'GET',
+            '/api/v3/log/file', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/history_api.py` & `sonarr-py-0.8.0/sonarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/host_config_api.py` & `sonarr-py-0.8.0/sonarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/import_list_api.py` & `sonarr-py-0.8.0/sonarr/api/import_list_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from sonarr.models.import_list_bulk_resource import ImportListBulkResource
 from sonarr.models.import_list_resource import ImportListResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
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
@@ -153,15 +161,15 @@
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
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
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
@@ -1271,15 +1576,15 @@
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
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
```

### Comparing `sonarr-py-0.7.0/sonarr/api/import_list_exclusion_api.py` & `sonarr-py-0.8.0/sonarr/api/import_list_exclusion_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/indexer_api.py` & `sonarr-py-0.8.0/sonarr/api/notification_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,81 +13,85 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from sonarr.models.indexer_resource import IndexerResource
+from sonarr.models.notification_resource import NotificationResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class IndexerApi(object):
+class NotificationApi(object):
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
+    def create_notification(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+        """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer(indexer_resource, async_req=True)
+        >>> thread = api.create_notification(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
+        return self.create_notification_with_http_info(force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """create_indexer  # noqa: E501
+    def create_notification_with_http_info(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_with_http_info(indexer_resource, async_req=True)
+        >>> thread = api.create_notification_with_http_info(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'indexer_resource'
+            'force_save',
+            'notification_resource'
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
+                    " to method create_notification" % _key
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
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/indexer', 'POST',
+            '/api/v3/notification', 'POST',
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
+    def create_notification_action_by_name(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_notification_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_action_by_name(name, indexer_resource, async_req=True)
+        >>> thread = api.create_notification_action_by_name(name, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+        return self.create_notification_action_by_name_with_http_info(name, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_action_by_name_with_http_info(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """create_indexer_action_by_name  # noqa: E501
+    def create_notification_action_by_name_with_http_info(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """create_notification_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_action_by_name_with_http_info(name, indexer_resource, async_req=True)
+        >>> thread = api.create_notification_action_by_name_with_http_info(name, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+            'notification_resource'
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
+                    " to method create_notification_action_by_name" % _key
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
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/indexer/action/{name}', 'POST',
+            '/api/v3/notification/action/{name}', 'POST',
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
+    def delete_notification(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer(id, async_req=True)
+        >>> thread = api.delete_notification(id, async_req=True)
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
+        return self.delete_notification_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_indexer_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_indexer  # noqa: E501
+    def delete_notification_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_indexer_with_http_info(id, async_req=True)
+        >>> thread = api.delete_notification_with_http_info(id, async_req=True)
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
+                    " to method delete_notification" % _key
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
-            '/api/v3/indexer/{id}', 'DELETE',
+            '/api/v3/notification/{id}', 'DELETE',
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
+    def get_notification_by_id(self, id : StrictInt, **kwargs) -> NotificationResource:  # noqa: E501
+        """get_notification_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_by_id(id, async_req=True)
+        >>> thread = api.get_notification_by_id(id, async_req=True)
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
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_indexer_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_notification_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_indexer_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_indexer_by_id  # noqa: E501
+    def get_notification_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_notification_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_indexer_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_notification_by_id_with_http_info(id, async_req=True)
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
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
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
+                    " to method get_notification_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -591,19 +598,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/indexer/{id}', 'GET',
+            '/api/v3/notification/{id}', 'GET',
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
+    def list_notification(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
+        """list_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer(async_req=True)
+        >>> thread = api.list_notification(async_req=True)
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
+        :rtype: List[NotificationResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_with_http_info(**kwargs)  # noqa: E501
+        return self.list_notification_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer  # noqa: E501
+    def list_notification_with_http_info(self, **kwargs):  # noqa: E501
+        """list_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_with_http_info(async_req=True)
+        >>> thread = api.list_notification_with_http_info(async_req=True)
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
+        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
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
+                    " to method list_notification" % _key
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
+            '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/indexer', 'GET',
+            '/api/v3/notification', 'GET',
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
+    def list_notification_schema(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
+        """list_notification_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_schema(async_req=True)
+        >>> thread = api.list_notification_schema(async_req=True)
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
+        :rtype: List[NotificationResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_indexer_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_notification_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_indexer_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_indexer_schema  # noqa: E501
+    def list_notification_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_notification_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_indexer_schema_with_http_info(async_req=True)
+        >>> thread = api.list_notification_schema_with_http_info(async_req=True)
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
+        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
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
+                    " to method list_notification_schema" % _key
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
+            '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/indexer/schema', 'GET',
+            '/api/v3/notification/schema', 'GET',
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
+    def test_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
+        """test_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_indexer(indexer_resource, async_req=True)
+        >>> thread = api.test_notification(notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+        return self.test_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """test_indexer  # noqa: E501
+    def test_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """test_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_indexer_with_http_info(indexer_resource, async_req=True)
+        >>> thread = api.test_notification_with_http_info(notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+            'notification_resource'
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
+                    " to method test_notification" % _key
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
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/indexer/test', 'POST',
+            '/api/v3/notification/test', 'POST',
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
+    def testall_notification(self, **kwargs) -> None:  # noqa: E501
+        """testall_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_indexer(async_req=True)
+        >>> thread = api.testall_notification(async_req=True)
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
+        return self.testall_notification_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def testall_indexer_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_indexer  # noqa: E501
+    def testall_notification_with_http_info(self, **kwargs):  # noqa: E501
+        """testall_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_indexer_with_http_info(async_req=True)
+        >>> thread = api.testall_notification_with_http_info(async_req=True)
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
+                    " to method testall_notification" % _key
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
-            '/api/v3/indexer/testall', 'POST',
+            '/api/v3/notification/testall', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1150,59 +1157,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
-        """update_indexer  # noqa: E501
+    def update_notification(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+        """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer(id, indexer_resource, async_req=True)
+        >>> thread = api.update_notification(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_with_http_info(id, indexer_resource, **kwargs)  # noqa: E501
+        return self.update_notification_with_http_info(id, force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_with_http_info(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
-        """update_indexer  # noqa: E501
+    def update_notification_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_with_http_info(id, indexer_resource, async_req=True)
+        >>> thread = api.update_notification_with_http_info(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param indexer_resource:
-        :type indexer_resource: IndexerResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1216,22 +1227,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'indexer_resource'
+            'force_save',
+            'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1242,61 +1254,63 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_indexer" % _key
+                    " to method update_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
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
 
         # process the body parameter
         _body_params = None
-        if _params['indexer_resource']:
-            _body_params = _params['indexer_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "IndexerResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/indexer/{id}', 'PUT',
+            '/api/v3/notification/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/indexer_config_api.py` & `sonarr-py-0.8.0/sonarr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/initialize_js_api.py` & `sonarr-py-0.8.0/sonarr/api/quality_profile_schema_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
+from sonarr.models.quality_profile_resource import QualityProfileResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class InitializeJsApi(object):
+class QualityProfileSchemaApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_initialize_js(self, **kwargs) -> None:  # noqa: E501
-        """get_initialize_js  # noqa: E501
+    def get_qualityprofile_schema(self, **kwargs) -> QualityProfileResource:  # noqa: E501
+        """get_qualityprofile_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_initialize_js(async_req=True)
+        >>> thread = api.get_qualityprofile_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -56,27 +57,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: QualityProfileResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_initialize_js_with_http_info(**kwargs)  # noqa: E501
+        return self.get_qualityprofile_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_initialize_js_with_http_info(self, **kwargs):  # noqa: E501
-        """get_initialize_js  # noqa: E501
+    def get_qualityprofile_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """get_qualityprofile_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_initialize_js_with_http_info(async_req=True)
+        >>> thread = api.get_qualityprofile_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -92,15 +93,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(QualityProfileResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -116,15 +117,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_initialize_js" % _key
+                    " to method get_qualityprofile_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -139,21 +140,27 @@
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "QualityProfileResource",
+        }
 
         return self.api_client.call_api(
-            '/initialize.js', 'GET',
+            '/api/v3/qualityprofile/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/language_api.py` & `sonarr-py-0.8.0/sonarr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/language_profile_api.py` & `sonarr-py-0.8.0/sonarr/api/language_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/language_profile_schema_api.py` & `sonarr-py-0.8.0/sonarr/api/tag_details_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,73 +15,79 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
-from sonarr.models.language_profile_resource import LanguageProfileResource
+from typing import List
+
+from sonarr.models.tag_details_resource import TagDetailsResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class LanguageProfileSchemaApi(object):
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
-    def get_languageprofile_schema(self, **kwargs) -> LanguageProfileResource:  # noqa: E501
-        """get_languageprofile_schema  # noqa: E501
+    def get_tag_detail_by_id(self, id : StrictInt, **kwargs) -> TagDetailsResource:  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_languageprofile_schema(async_req=True)
+        >>> thread = api.get_tag_detail_by_id(id, async_req=True)
         >>> result = thread.get()
 
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
-        :rtype: LanguageProfileResource
+        :rtype: TagDetailsResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_languageprofile_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.get_tag_detail_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_languageprofile_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """get_languageprofile_schema  # noqa: E501
+    def get_tag_detail_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_languageprofile_schema_with_http_info(async_req=True)
+        >>> thread = api.get_tag_detail_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -95,20 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(LanguageProfileResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TagDetailsResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -119,23 +126,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_languageprofile_schema" % _key
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
 
@@ -150,19 +159,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "LanguageProfileResource",
+            '200': "TagDetailsResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/languageprofile/schema', 'GET',
+            '/api/v3/tag/detail/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -171,55 +180,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_languageprofile_schema_by_id(self, id : StrictInt, **kwargs) -> LanguageProfileResource:  # noqa: E501
-        """get_languageprofile_schema_by_id  # noqa: E501
+    def list_tag_detail(self, **kwargs) -> List[TagDetailsResource]:  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_languageprofile_schema_by_id(id, async_req=True)
+        >>> thread = api.list_tag_detail(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
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
-        :rtype: LanguageProfileResource
+        :rtype: List[TagDetailsResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_languageprofile_schema_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_tag_detail_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_languageprofile_schema_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_languageprofile_schema_by_id  # noqa: E501
+    def list_tag_detail_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_languageprofile_schema_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.list_tag_detail_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -233,21 +238,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(LanguageProfileResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TagDetailsResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -258,25 +262,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_languageprofile_schema_by_id" % _key
+                    " to method list_tag_detail" % _key
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
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -291,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "LanguageProfileResource",
+            '200': "List[TagDetailsResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/languageprofile/schema/{id}', 'GET',
+            '/api/v3/tag/detail', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/localization_api.py` & `sonarr-py-0.8.0/sonarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/log_api.py` & `sonarr-py-0.8.0/sonarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/log_file_api.py` & `sonarr-py-0.8.0/sonarr/api/missing_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,81 +13,86 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import constr, validator
+from pydantic import StrictBool, StrictInt
 
-from typing import List
+from typing import Optional
 
-from sonarr.models.log_file_resource import LogFileResource
+from sonarr.models.episode_resource import EpisodeResource
+from sonarr.models.episode_resource_paging_resource import EpisodeResourcePagingResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class LogFileApi(object):
+class MissingApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_log_file_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
-        """get_log_file_by_filename  # noqa: E501
+    def get_wanted_missing(self, include_series : Optional[StrictBool] = None, include_images : Optional[StrictBool] = None, **kwargs) -> EpisodeResourcePagingResource:  # noqa: E501
+        """get_wanted_missing  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_log_file_by_filename(filename, async_req=True)
+        >>> thread = api.get_wanted_missing(include_series, include_images, async_req=True)
         >>> result = thread.get()
 
-        :param filename: (required)
-        :type filename: str
+        :param include_series:
+        :type include_series: bool
+        :param include_images:
+        :type include_images: bool
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
+        :rtype: EpisodeResourcePagingResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_log_file_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
+        return self.get_wanted_missing_with_http_info(include_series, include_images, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_log_file_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
-        """get_log_file_by_filename  # noqa: E501
+    def get_wanted_missing_with_http_info(self, include_series : Optional[StrictBool] = None, include_images : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """get_wanted_missing  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_log_file_by_filename_with_http_info(filename, async_req=True)
+        >>> thread = api.get_wanted_missing_with_http_info(include_series, include_images, async_req=True)
         >>> result = thread.get()
 
-        :param filename: (required)
-        :type filename: str
+        :param include_series:
+        :type include_series: bool
+        :param include_images:
+        :type include_images: bool
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
-        :rtype: None
+        :rtype: tuple(EpisodeResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'filename'
+            'include_series',
+            'include_images'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,46 +132,54 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_log_file_by_filename" % _key
+                    " to method get_wanted_missing" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['filename']:
-            _path_params['filename'] = _params['filename']
 
         # process the query parameters
         _query_params = []
+        if _params.get('include_series') is not None:  # noqa: E501
+            _query_params.append(('includeSeries', _params['include_series']))
+        if _params.get('include_images') is not None:  # noqa: E501
+            _query_params.append(('includeImages', _params['include_images']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "EpisodeResourcePagingResource",
+        }
 
         return self.api_client.call_api(
-            '/api/v3/log/file/{filename}', 'GET',
+            '/api/v3/wanted/missing', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -174,51 +188,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_log_file(self, **kwargs) -> List[LogFileResource]:  # noqa: E501
-        """list_log_file  # noqa: E501
+    def get_wanted_missing_by_id(self, id : StrictInt, **kwargs) -> EpisodeResource:  # noqa: E501
+        """get_wanted_missing_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_log_file(async_req=True)
+        >>> thread = api.get_wanted_missing_by_id(id, async_req=True)
         >>> result = thread.get()
 
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
-        :rtype: List[LogFileResource]
+        :rtype: EpisodeResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_log_file_with_http_info(**kwargs)  # noqa: E501
+        return self.get_wanted_missing_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_log_file_with_http_info(self, **kwargs):  # noqa: E501
-        """list_log_file  # noqa: E501
+    def get_wanted_missing_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_wanted_missing_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_log_file_with_http_info(async_req=True)
+        >>> thread = api.get_wanted_missing_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -232,20 +250,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[LogFileResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(EpisodeResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -256,23 +275,25 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_log_file" % _key
+                    " to method get_wanted_missing_by_id" % _key
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
 
@@ -287,19 +308,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[LogFileResource]",
+            '200': "EpisodeResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/log/file', 'GET',
+            '/api/v3/wanted/missing/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/manual_import_api.py` & `sonarr-py-0.8.0/sonarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/media_cover_api.py` & `sonarr-py-0.8.0/sonarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/media_management_config_api.py` & `sonarr-py-0.8.0/sonarr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/metadata_api.py` & `sonarr-py-0.8.0/sonarr/api/metadata_api.py`

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
 
 from sonarr.models.metadata_resource import MetadataResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
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
@@ -153,15 +160,15 @@
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
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
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
@@ -1271,15 +1285,15 @@
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
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
```

### Comparing `sonarr-py-0.7.0/sonarr/api/missing_api.py` & `sonarr-py-0.8.0/sonarr/api/queue_action_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,86 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt
+from pydantic import StrictInt
 
 from typing import Optional
 
-from sonarr.models.episode_resource import EpisodeResource
-from sonarr.models.episode_resource_paging_resource import EpisodeResourcePagingResource
+from sonarr.models.queue_bulk_resource import QueueBulkResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class MissingApi(object):
+class QueueActionApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_wanted_missing(self, include_series : Optional[StrictBool] = None, include_images : Optional[StrictBool] = None, **kwargs) -> EpisodeResourcePagingResource:  # noqa: E501
-        """get_wanted_missing  # noqa: E501
+    def create_queue_grab_bulk(self, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_queue_grab_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_wanted_missing(include_series, include_images, async_req=True)
+        >>> thread = api.create_queue_grab_bulk(queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param include_series:
-        :type include_series: bool
-        :param include_images:
-        :type include_images: bool
+        :param queue_bulk_resource:
+        :type queue_bulk_resource: QueueBulkResource
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
-        :rtype: EpisodeResourcePagingResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_wanted_missing_with_http_info(include_series, include_images, **kwargs)  # noqa: E501
+        return self.create_queue_grab_bulk_with_http_info(queue_bulk_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_wanted_missing_with_http_info(self, include_series : Optional[StrictBool] = None, include_images : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """get_wanted_missing  # noqa: E501
+    def create_queue_grab_bulk_with_http_info(self, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
+        """create_queue_grab_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_wanted_missing_with_http_info(include_series, include_images, async_req=True)
+        >>> thread = api.create_queue_grab_bulk_with_http_info(queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param include_series:
-        :type include_series: bool
-        :param include_images:
-        :type include_images: bool
+        :param queue_bulk_resource:
+        :type queue_bulk_resource: QueueBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -106,22 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(EpisodeResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'include_series',
-            'include_images'
+            'queue_bulk_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -132,54 +126,53 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_wanted_missing" % _key
+                    " to method create_queue_grab_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('include_series') is not None:  # noqa: E501
-            _query_params.append(('includeSeries', _params['include_series']))
-        if _params.get('include_images') is not None:  # noqa: E501
-            _query_params.append(('includeImages', _params['include_images']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['queue_bulk_resource']:
+            _body_params = _params['queue_bulk_resource']
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "EpisodeResourcePagingResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/wanted/missing', 'GET',
+            '/api/v3/queue/grab/bulk', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -188,21 +181,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_wanted_missing_by_id(self, id : StrictInt, **kwargs) -> EpisodeResource:  # noqa: E501
-        """get_wanted_missing_by_id  # noqa: E501
+    def create_queue_grab_by_id(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """create_queue_grab_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_wanted_missing_by_id(id, async_req=True)
+        >>> thread = api.create_queue_grab_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -212,27 +205,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: EpisodeResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_wanted_missing_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.create_queue_grab_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_wanted_missing_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_wanted_missing_by_id  # noqa: E501
+    def create_queue_grab_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """create_queue_grab_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_wanted_missing_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.create_queue_grab_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -250,15 +243,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(EpisodeResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -275,15 +268,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_wanted_missing_by_id" % _key
+                    " to method create_queue_grab_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -300,27 +293,21 @@
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "EpisodeResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/wanted/missing/{id}', 'GET',
+            '/api/v3/queue/grab/{id}', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/naming_config_api.py` & `sonarr-py-0.8.0/sonarr/api/naming_config_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/notification_api.py` & `sonarr-py-0.8.0/sonarr/api/indexer_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,81 +13,86 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from sonarr.models.notification_resource import NotificationResource
+from sonarr.models.indexer_bulk_resource import IndexerBulkResource
+from sonarr.models.indexer_resource import IndexerResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class NotificationApi(object):
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
-    def create_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
-        """create_notification  # noqa: E501
+    def create_indexer(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification(notification_resource, async_req=True)
+        >>> thread = api.create_indexer(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-        :rtype: NotificationResource
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_with_http_info(force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """create_notification  # noqa: E501
+    def create_indexer_with_http_info(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_with_http_info(notification_resource, async_req=True)
+        >>> thread = api.create_indexer_with_http_info(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'notification_resource'
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
-                    " to method create_notification" % _key
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
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "NotificationResource",
+            '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/notification', 'POST',
+            '/api/v3/indexer', 'POST',
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
-    def create_notification_action_by_name(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_notification_action_by_name  # noqa: E501
+    def create_indexer_action_by_name(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_indexer_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_action_by_name(name, notification_resource, async_req=True)
+        >>> thread = api.create_indexer_action_by_name(name, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-        return self.create_notification_action_by_name_with_http_info(name, notification_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_action_by_name_with_http_info(name, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_notification_action_by_name_with_http_info(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """create_notification_action_by_name  # noqa: E501
+    def create_indexer_action_by_name_with_http_info(self, name : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """create_indexer_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_action_by_name_with_http_info(name, notification_resource, async_req=True)
+        >>> thread = api.create_indexer_action_by_name_with_http_info(name, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-            'notification_resource'
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
-                    " to method create_notification_action_by_name" % _key
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
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/notification/action/{name}', 'POST',
+            '/api/v3/indexer/action/{name}', 'POST',
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
-    def delete_notification(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_notification  # noqa: E501
+    def delete_indexer(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_notification(id, async_req=True)
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
-        return self.delete_notification_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_indexer_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_notification_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_notification  # noqa: E501
+    def delete_indexer_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_notification_with_http_info(id, async_req=True)
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
-                    " to method delete_notification" % _key
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
-            '/api/v3/notification/{id}', 'DELETE',
+            '/api/v3/indexer/{id}', 'DELETE',
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
-    def get_notification_by_id(self, id : StrictInt, **kwargs) -> NotificationResource:  # noqa: E501
-        """get_notification_by_id  # noqa: E501
+    def delete_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_indexer_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_notification_by_id(id, async_req=True)
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
-        :rtype: NotificationResource
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_notification_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_indexer_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_notification_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_notification_by_id  # noqa: E501
+    def get_indexer_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_indexer_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_notification_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_notification_by_id" % _key
+                    " to method get_indexer_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -591,19 +741,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "NotificationResource",
+            '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/notification/{id}', 'GET',
+            '/api/v3/indexer/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -612,21 +762,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_notification(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
-        """list_notification  # noqa: E501
+    def list_indexer(self, **kwargs) -> List[IndexerResource]:  # noqa: E501
+        """list_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_notification(async_req=True)
+        >>> thread = api.list_indexer(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -634,27 +784,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[NotificationResource]
+        :rtype: List[IndexerResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_notification_with_http_info(**kwargs)  # noqa: E501
+        return self.list_indexer_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_notification_with_http_info(self, **kwargs):  # noqa: E501
-        """list_notification  # noqa: E501
+    def list_indexer_with_http_info(self, **kwargs):  # noqa: E501
+        """list_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_notification_with_http_info(async_req=True)
+        >>> thread = api.list_indexer_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -670,15 +820,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[IndexerResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -694,15 +844,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_notification" % _key
+                    " to method list_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -725,19 +875,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[NotificationResource]",
+            '200': "List[IndexerResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/notification', 'GET',
+            '/api/v3/indexer', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -746,21 +896,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_notification_schema(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
-        """list_notification_schema  # noqa: E501
+    def list_indexer_schema(self, **kwargs) -> List[IndexerResource]:  # noqa: E501
+        """list_indexer_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_notification_schema(async_req=True)
+        >>> thread = api.list_indexer_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -768,27 +918,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[NotificationResource]
+        :rtype: List[IndexerResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_notification_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_indexer_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_notification_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_notification_schema  # noqa: E501
+    def list_indexer_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_indexer_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_notification_schema_with_http_info(async_req=True)
+        >>> thread = api.list_indexer_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -804,15 +954,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[IndexerResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -828,15 +978,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_notification_schema" % _key
+                    " to method list_indexer_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -859,19 +1009,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[NotificationResource]",
+            '200': "List[IndexerResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/notification/schema', 'GET',
+            '/api/v3/indexer/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -880,25 +1030,173 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def test_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
-        """test_notification  # noqa: E501
+    def put_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_notification(notification_resource, async_req=True)
+        >>> thread = api.put_indexer_bulk(indexer_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
+    def test_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
+        """test_indexer  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.test_indexer(indexer_resource, async_req=True)
+        >>> result = thread.get()
+
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
-        return self.test_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
+        return self.test_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """test_notification  # noqa: E501
+    def test_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """test_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_notification_with_http_info(notification_resource, async_req=True)
+        >>> thread = api.test_indexer_with_http_info(indexer_resource, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-            'notification_resource'
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
-                    " to method test_notification" % _key
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
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/notification/test', 'POST',
+            '/api/v3/indexer/test', 'POST',
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
-    def testall_notification(self, **kwargs) -> None:  # noqa: E501
-        """testall_notification  # noqa: E501
+    def testall_indexer(self, **kwargs) -> None:  # noqa: E501
+        """testall_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_notification(async_req=True)
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
-        return self.testall_notification_with_http_info(**kwargs)  # noqa: E501
+        return self.testall_indexer_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def testall_notification_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_notification  # noqa: E501
+    def testall_indexer_with_http_info(self, **kwargs):  # noqa: E501
+        """testall_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_notification_with_http_info(async_req=True)
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
-                    " to method testall_notification" % _key
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
-            '/api/v3/notification/testall', 'POST',
+            '/api/v3/indexer/testall', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1150,59 +1448,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_notification(self, id : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
-        """update_notification  # noqa: E501
+    def update_indexer(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification(id, notification_resource, async_req=True)
+        >>> thread = api.update_indexer(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-        :rtype: NotificationResource
+        :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_notification_with_http_info(id, notification_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_with_http_info(id, force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_notification_with_http_info(self, id : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """update_notification  # noqa: E501
+    def update_indexer_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+        """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification_with_http_info(id, notification_resource, async_req=True)
+        >>> thread = api.update_indexer_with_http_info(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
@@ -1216,22 +1518,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'notification_resource'
+            'force_save',
+            'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1242,61 +1545,63 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_notification" % _key
+                    " to method update_indexer" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
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
 
         # process the body parameter
         _body_params = None
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['indexer_resource']:
+            _body_params = _params['indexer_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "NotificationResource",
+            '200': "IndexerResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/notification/{id}', 'PUT',
+            '/api/v3/indexer/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/parse_api.py` & `sonarr-py-0.8.0/sonarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/ping_api.py` & `sonarr-py-0.8.0/sonarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/quality_definition_api.py` & `sonarr-py-0.8.0/sonarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/quality_profile_api.py` & `sonarr-py-0.8.0/sonarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/quality_profile_schema_api.py` & `sonarr-py-0.8.0/sonarr/api/language_profile_schema_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,43 +13,43 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from sonarr.models.quality_profile_resource import QualityProfileResource
+from sonarr.models.language_profile_resource import LanguageProfileResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QualityProfileSchemaApi(object):
+class LanguageProfileSchemaApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_qualityprofile_schema(self, **kwargs) -> QualityProfileResource:  # noqa: E501
-        """get_qualityprofile_schema  # noqa: E501
+    def get_languageprofile_schema(self, **kwargs) -> LanguageProfileResource:  # noqa: E501
+        """get_languageprofile_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_qualityprofile_schema(async_req=True)
+        >>> thread = api.get_languageprofile_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -57,27 +57,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: QualityProfileResource
+        :rtype: LanguageProfileResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_qualityprofile_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.get_languageprofile_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_qualityprofile_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """get_qualityprofile_schema  # noqa: E501
+    def get_languageprofile_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """get_languageprofile_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_qualityprofile_schema_with_http_info(async_req=True)
+        >>> thread = api.get_languageprofile_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -93,15 +93,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QualityProfileResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(LanguageProfileResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -117,15 +117,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_qualityprofile_schema" % _key
+                    " to method get_languageprofile_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -142,25 +142,25 @@
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
-            '200': "QualityProfileResource",
+            '200': "LanguageProfileResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/qualityprofile/schema', 'GET',
+            '/api/v3/languageprofile/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/queue_action_api.py` & `sonarr-py-0.8.0/sonarr/api/release_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,49 +15,49 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
-from typing import Optional
+from typing import List, Optional
 
-from sonarr.models.queue_bulk_resource import QueueBulkResource
+from sonarr.models.release_resource import ReleaseResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueActionApi(object):
+class ReleaseApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_queue_grab_bulk(self, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_queue_grab_bulk  # noqa: E501
+    def create_release(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_queue_grab_bulk(queue_bulk_resource, async_req=True)
+        >>> thread = api.create_release(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param queue_bulk_resource:
-        :type queue_bulk_resource: QueueBulkResource
+        :param release_resource:
+        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -66,28 +66,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_queue_grab_bulk_with_http_info(queue_bulk_resource, **kwargs)  # noqa: E501
+        return self.create_release_with_http_info(release_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_queue_grab_bulk_with_http_info(self, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
-        """create_queue_grab_bulk  # noqa: E501
+    def create_release_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
+        """create_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_queue_grab_bulk_with_http_info(queue_bulk_resource, async_req=True)
+        >>> thread = api.create_release_with_http_info(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param queue_bulk_resource:
-        :type queue_bulk_resource: QueueBulkResource
+        :param release_resource:
+        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -107,15 +107,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'queue_bulk_resource'
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
-                    " to method create_queue_grab_bulk" % _key
+                    " to method create_release" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -148,31 +148,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['queue_bulk_resource']:
-            _body_params = _params['queue_bulk_resource']
+        if _params['release_resource']:
+            _body_params = _params['release_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/queue/grab/bulk', 'POST',
+            '/api/v3/release', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -181,55 +181,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_queue_grab_by_id(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """create_queue_grab_by_id  # noqa: E501
+    def list_release(self, series_id : Optional[StrictInt] = None, episode_id : Optional[StrictInt] = None, season_number : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
+        """list_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_queue_grab_by_id(id, async_req=True)
+        >>> thread = api.list_release(series_id, episode_id, season_number, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param series_id:
+        :type series_id: int
+        :param episode_id:
+        :type episode_id: int
+        :param season_number:
+        :type season_number: int
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
+        :rtype: List[ReleaseResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_queue_grab_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_release_with_http_info(series_id, episode_id, season_number, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_queue_grab_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """create_queue_grab_by_id  # noqa: E501
+    def list_release_with_http_info(self, series_id : Optional[StrictInt] = None, episode_id : Optional[StrictInt] = None, season_number : Optional[StrictInt] = None, **kwargs):  # noqa: E501
+        """list_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_queue_grab_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.list_release_with_http_info(series_id, episode_id, season_number, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param series_id:
+        :type series_id: int
+        :param episode_id:
+        :type episode_id: int
+        :param season_number:
+        :type season_number: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -243,21 +251,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'series_id',
+            'episode_id',
+            'season_number'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -268,46 +278,56 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_queue_grab_by_id" % _key
+                    " to method list_release" % _key
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
+        if _params.get('series_id') is not None:  # noqa: E501
+            _query_params.append(('seriesId', _params['series_id']))
+        if _params.get('episode_id') is not None:  # noqa: E501
+            _query_params.append(('episodeId', _params['episode_id']))
+        if _params.get('season_number') is not None:  # noqa: E501
+            _query_params.append(('seasonNumber', _params['season_number']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "List[ReleaseResource]",
+        }
 
         return self.api_client.call_api(
-            '/api/v3/queue/grab/{id}', 'POST',
+            '/api/v3/release', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/queue_api.py` & `sonarr-py-0.8.0/sonarr/api/tag_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,57 +13,199 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import Optional
+from typing import List, Optional
 
-from sonarr.models.queue_bulk_resource import QueueBulkResource
-from sonarr.models.queue_resource import QueueResource
-from sonarr.models.queue_resource_paging_resource import QueueResourcePagingResource
+from sonarr.models.tag_resource import TagResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueApi(object):
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
-    def delete_queue(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
-        """delete_queue  # noqa: E501
+    def create_tag(self, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
+        """create_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue(id, remove_from_client, blocklist, async_req=True)
+        >>> thread = api.create_tag(tag_resource, async_req=True)
+        >>> result = thread.get()
+
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
+        return self.create_tag_with_http_info(tag_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def create_tag_with_http_info(self, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
+        """create_tag  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.create_tag_with_http_info(tag_resource, async_req=True)
+        >>> result = thread.get()
+
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
+                    " to method create_tag" % _key
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
+        if _params['tag_resource']:
+            _body_params = _params['tag_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
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
+            '200': "TagResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v3/tag', 'POST',
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
+    def delete_tag(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_tag  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_tag(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -72,32 +214,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_queue_with_http_info(id, remove_from_client, blocklist, **kwargs)  # noqa: E501
+        return self.delete_tag_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_queue_with_http_info(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """delete_queue  # noqa: E501
+    def delete_tag_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_with_http_info(id, remove_from_client, blocklist, async_req=True)
+        >>> thread = api.delete_tag_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -117,17 +255,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'remove_from_client',
-            'blocklist'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -138,32 +274,28 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_queue" % _key
+                    " to method delete_tag" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
-        if _params.get('remove_from_client') is not None:  # noqa: E501
-            _query_params.append(('removeFromClient', _params['remove_from_client']))
-        if _params.get('blocklist') is not None:  # noqa: E501
-            _query_params.append(('blocklist', _params['blocklist']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -173,15 +305,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/queue/{id}', 'DELETE',
+            '/api/v3/tag/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -190,63 +322,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_queue_bulk(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
-        """delete_queue_bulk  # noqa: E501
+    def get_tag_by_id(self, id : StrictInt, **kwargs) -> TagResource:  # noqa: E501
+        """get_tag_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_bulk(remove_from_client, blocklist, queue_bulk_resource, async_req=True)
+        >>> thread = api.get_tag_by_id(id, async_req=True)
         >>> result = thread.get()
 
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
-        :param queue_bulk_resource:
-        :type queue_bulk_resource: QueueBulkResource
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
+        :rtype: TagResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_queue_bulk_with_http_info(remove_from_client, blocklist, queue_bulk_resource, **kwargs)  # noqa: E501
+        return self.get_tag_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_queue_bulk_with_http_info(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
-        """delete_queue_bulk  # noqa: E501
+    def get_tag_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_bulk_with_http_info(remove_from_client, blocklist, queue_bulk_resource, async_req=True)
+        >>> thread = api.get_tag_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
-        :param queue_bulk_resource:
-        :type queue_bulk_resource: QueueBulkResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -260,23 +384,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'remove_from_client',
-            'blocklist',
-            'queue_bulk_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -287,57 +409,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_queue_bulk" % _key
+                    " to method get_tag_by_id" % _key
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
-        if _params.get('remove_from_client') is not None:  # noqa: E501
-            _query_params.append(('removeFromClient', _params['remove_from_client']))
-        if _params.get('blocklist') is not None:  # noqa: E501
-            _query_params.append(('blocklist', _params['blocklist']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['queue_bulk_resource']:
-            _body_params = _params['queue_bulk_resource']
 
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
+            '200': "TagResource",
+        }
 
         return self.api_client.call_api(
-            '/api/v3/queue/bulk', 'DELETE',
+            '/api/v3/tag/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -346,63 +463,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_queue(self, include_unknown_series_items : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode : Optional[StrictBool] = None, **kwargs) -> QueueResourcePagingResource:  # noqa: E501
-        """get_queue  # noqa: E501
+    def list_tag(self, **kwargs) -> List[TagResource]:  # noqa: E501
+        """list_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue(include_unknown_series_items, include_series, include_episode, async_req=True)
+        >>> thread = api.list_tag(async_req=True)
         >>> result = thread.get()
 
-        :param include_unknown_series_items:
-        :type include_unknown_series_items: bool
-        :param include_series:
-        :type include_series: bool
-        :param include_episode:
-        :type include_episode: bool
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
-        :rtype: QueueResourcePagingResource
+        :rtype: List[TagResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_with_http_info(include_unknown_series_items, include_series, include_episode, **kwargs)  # noqa: E501
+        return self.list_tag_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_with_http_info(self, include_unknown_series_items : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """get_queue  # noqa: E501
+    def list_tag_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_with_http_info(include_unknown_series_items, include_series, include_episode, async_req=True)
+        >>> thread = api.list_tag_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param include_unknown_series_items:
-        :type include_unknown_series_items: bool
-        :param include_series:
-        :type include_series: bool
-        :param include_episode:
-        :type include_episode: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -416,23 +521,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TagResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'include_unknown_series_items',
-            'include_series',
-            'include_episode'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -443,32 +545,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue" % _key
+                    " to method list_tag" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('include_unknown_series_items') is not None:  # noqa: E501
-            _query_params.append(('includeUnknownSeriesItems', _params['include_unknown_series_items']))
-        if _params.get('include_series') is not None:  # noqa: E501
-            _query_params.append(('includeSeries', _params['include_series']))
-        if _params.get('include_episode') is not None:  # noqa: E501
-            _query_params.append(('includeEpisode', _params['include_episode']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -480,19 +576,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueResourcePagingResource",
+            '200': "List[TagResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/queue', 'GET',
+            '/api/v3/tag', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -501,55 +597,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_queue_by_id(self, id : StrictInt, **kwargs) -> QueueResource:  # noqa: E501
-        """get_queue_by_id  # noqa: E501
+    def update_tag(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
+        """update_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_by_id(id, async_req=True)
+        >>> thread = api.update_tag(id, tag_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
-        :type id: int
+        :type id: str
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
-        :rtype: QueueResource
+        :rtype: TagResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.update_tag_with_http_info(id, tag_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_by_id  # noqa: E501
+    def update_tag_with_http_info(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
+        """update_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.update_tag_with_http_info(id, tag_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
-        :type id: int
+        :type id: str
+        :param tag_resource:
+        :type tag_resource: TagResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -563,21 +663,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'tag_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -588,15 +689,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_by_id" % _key
+                    " to method update_tag" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -612,28 +713,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['tag_resource']:
+            _body_params = _params['tag_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
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
-            '200': "QueueResource",
+            '200': "TagResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/queue/{id}', 'GET',
+            '/api/v3/tag/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/queue_details_api.py` & `sonarr-py-0.8.0/sonarr/api/task_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,47 +13,47 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt, conlist
+from pydantic import StrictInt
 
-from typing import List, Optional
+from typing import List
 
-from sonarr.models.queue_resource import QueueResource
+from sonarr.models.task_resource import TaskResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueDetailsApi(object):
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
-    def get_queue_details_by_id(self, id : StrictInt, **kwargs) -> QueueResource:  # noqa: E501
-        """get_queue_details_by_id  # noqa: E501
+    def get_system_task_by_id(self, id : StrictInt, **kwargs) -> TaskResource:  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_details_by_id(id, async_req=True)
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
-        :rtype: QueueResource
+        :rtype: TaskResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_details_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_system_task_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_details_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_details_by_id  # noqa: E501
+    def get_system_task_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_details_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(QueueResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_queue_details_by_id" % _key
+                    " to method get_system_task_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -159,19 +159,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueResource",
+            '200': "TaskResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/queue/details/{id}', 'GET',
+            '/api/v3/system/task/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,67 +180,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_queue_details(self, series_id : Optional[StrictInt] = None, episode_ids : Optional[conlist(StrictInt)] = None, include_series : Optional[StrictBool] = None, include_episode : Optional[StrictBool] = None, **kwargs) -> List[QueueResource]:  # noqa: E501
-        """list_queue_details  # noqa: E501
+    def list_system_task(self, **kwargs) -> List[TaskResource]:  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_queue_details(series_id, episode_ids, include_series, include_episode, async_req=True)
+        >>> thread = api.list_system_task(async_req=True)
         >>> result = thread.get()
 
-        :param series_id:
-        :type series_id: int
-        :param episode_ids:
-        :type episode_ids: List[int]
-        :param include_series:
-        :type include_series: bool
-        :param include_episode:
-        :type include_episode: bool
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
-        :rtype: List[QueueResource]
+        :rtype: List[TaskResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_queue_details_with_http_info(series_id, episode_ids, include_series, include_episode, **kwargs)  # noqa: E501
+        return self.list_system_task_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_queue_details_with_http_info(self, series_id : Optional[StrictInt] = None, episode_ids : Optional[conlist(StrictInt)] = None, include_series : Optional[StrictBool] = None, include_episode : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """list_queue_details  # noqa: E501
+    def list_system_task_with_http_info(self, **kwargs):  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_queue_details_with_http_info(series_id, episode_ids, include_series, include_episode, async_req=True)
+        >>> thread = api.list_system_task_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param series_id:
-        :type series_id: int
-        :param episode_ids:
-        :type episode_ids: List[int]
-        :param include_series:
-        :type include_series: bool
-        :param include_episode:
-        :type include_episode: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -254,24 +238,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[QueueResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TaskResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'series_id',
-            'episode_ids',
-            'include_series',
-            'include_episode'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -282,59 +262,50 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_queue_details" % _key
+                    " to method list_system_task" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('series_id') is not None:  # noqa: E501
-            _query_params.append(('seriesId', _params['series_id']))
-        if _params.get('episode_ids') is not None:  # noqa: E501
-            _query_params.append(('episodeIds', _params['episode_ids']))
-            _collection_formats['episodeIds'] = 'multi'
-        if _params.get('include_series') is not None:  # noqa: E501
-            _query_params.append(('includeSeries', _params['include_series']))
-        if _params.get('include_episode') is not None:  # noqa: E501
-            _query_params.append(('includeEpisode', _params['include_episode']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[QueueResource]",
+            '200': "List[TaskResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/queue/details', 'GET',
+            '/api/v3/system/task', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/queue_status_api.py` & `sonarr-py-0.8.0/sonarr/api/update_log_file_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,75 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import constr, validator
 
-from sonarr.models.queue_status_resource import QueueStatusResource
+from typing import List
+
+from sonarr.models.log_file_resource import LogFileResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueStatusApi(object):
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
-    def get_queue_status(self, **kwargs) -> QueueStatusResource:  # noqa: E501
-        """get_queue_status  # noqa: E501
+    def get_log_file_update_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
+        """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status(async_req=True)
+        >>> thread = api.get_log_file_update_by_filename(filename, async_req=True)
         >>> result = thread.get()
 
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
-        :rtype: QueueStatusResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_status_with_http_info(**kwargs)  # noqa: E501
+        return self.get_log_file_update_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_status_with_http_info(self, **kwargs):  # noqa: E501
-        """get_queue_status  # noqa: E501
+    def get_log_file_update_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
+        """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status_with_http_info(async_req=True)
+        >>> thread = api.get_log_file_update_by_filename_with_http_info(filename, async_req=True)
         >>> result = thread.get()
 
+        :param filename: (required)
+        :type filename: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -95,20 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueStatusResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
+            'filename'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -119,50 +126,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_status" % _key
+                    " to method get_log_file_update_by_filename" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['filename']:
+            _path_params['filename'] = _params['filename']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "QueueStatusResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/queue/status', 'GET',
+            '/api/v3/log/file/update/{filename}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -171,55 +174,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_queue_status_by_id(self, id : StrictInt, **kwargs) -> QueueStatusResource:  # noqa: E501
-        """get_queue_status_by_id  # noqa: E501
+    def list_log_file_update(self, **kwargs) -> List[LogFileResource]:  # noqa: E501
+        """list_log_file_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status_by_id(id, async_req=True)
+        >>> thread = api.list_log_file_update(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
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
-        :rtype: QueueStatusResource
+        :rtype: List[LogFileResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_status_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_log_file_update_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_status_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_status_by_id  # noqa: E501
+    def list_log_file_update_with_http_info(self, **kwargs):  # noqa: E501
+        """list_log_file_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.list_log_file_update_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -233,21 +232,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueStatusResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[LogFileResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -258,25 +256,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_status_by_id" % _key
+                    " to method list_log_file_update" % _key
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
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -291,19 +287,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueStatusResource",
+            '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v3/queue/status/{id}', 'GET',
+            '/api/v3/log/file/update', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/release_api.py` & `sonarr-py-0.8.0/sonarr/api/ui_config_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,81 +13,77 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import List, Optional
+from typing import Optional
 
-from sonarr.models.release_resource import ReleaseResource
+from sonarr.models.ui_config_resource import UiConfigResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ReleaseApi(object):
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
-    def create_release(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_release  # noqa: E501
+    def get_ui_config(self, **kwargs) -> UiConfigResource:  # noqa: E501
+        """get_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release(release_resource, async_req=True)
+        >>> thread = api.get_ui_config(async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
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
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_release_with_http_info(release_resource, **kwargs)  # noqa: E501
+        return self.get_ui_config_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_release_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
-        """create_release  # noqa: E501
+    def get_ui_config_with_http_info(self, **kwargs):  # noqa: E501
+        """get_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release_with_http_info(release_resource, async_req=True)
+        >>> thread = api.get_ui_config_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +97,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'release_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,15 +121,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_release" % _key
+                    " to method get_ui_config" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -148,31 +143,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['release_resource']:
-            _body_params = _params['release_resource']
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "UiConfigResource",
+        }
 
         return self.api_client.call_api(
-            '/api/v3/release', 'POST',
+            '/api/v3/config/ui', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -181,21 +173,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_release_by_id(self, id : StrictInt, **kwargs) -> ReleaseResource:  # noqa: E501
-        """get_release_by_id  # noqa: E501
+    def get_ui_config_by_id(self, id : StrictInt, **kwargs) -> UiConfigResource:  # noqa: E501
+        """get_ui_config_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_by_id(id, async_req=True)
+        >>> thread = api.get_ui_config_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -205,27 +197,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_release_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_ui_config_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_release_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_release_by_id  # noqa: E501
+    def get_ui_config_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_ui_config_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_ui_config_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -243,15 +235,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -268,15 +260,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_release_by_id" % _key
+                    " to method get_ui_config_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -301,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/release/{id}', 'GET',
+            '/api/v3/config/ui/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -322,63 +314,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_release(self, series_id : Optional[StrictInt] = None, episode_id : Optional[StrictInt] = None, season_number : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
-        """list_release  # noqa: E501
+    def update_ui_config(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs) -> UiConfigResource:  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_release(series_id, episode_id, season_number, async_req=True)
+        >>> thread = api.update_ui_config(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
-        :param series_id:
-        :type series_id: int
-        :param episode_id:
-        :type episode_id: int
-        :param season_number:
-        :type season_number: int
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
-        :rtype: List[ReleaseResource]
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_release_with_http_info(series_id, episode_id, season_number, **kwargs)  # noqa: E501
+        return self.update_ui_config_with_http_info(id, ui_config_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_release_with_http_info(self, series_id : Optional[StrictInt] = None, episode_id : Optional[StrictInt] = None, season_number : Optional[StrictInt] = None, **kwargs):  # noqa: E501
-        """list_release  # noqa: E501
+    def update_ui_config_with_http_info(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs):  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_release_with_http_info(series_id, episode_id, season_number, async_req=True)
+        >>> thread = api.update_ui_config_with_http_info(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
-        :param series_id:
-        :type series_id: int
-        :param episode_id:
-        :type episode_id: int
-        :param season_number:
-        :type season_number: int
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
@@ -392,23 +380,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'series_id',
-            'episode_id',
-            'season_number'
+            'id',
+            'ui_config_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -419,56 +406,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_release" % _key
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
-        if _params.get('series_id') is not None:  # noqa: E501
-            _query_params.append(('seriesId', _params['series_id']))
-        if _params.get('episode_id') is not None:  # noqa: E501
-            _query_params.append(('episodeId', _params['episode_id']))
-        if _params.get('season_number') is not None:  # noqa: E501
-            _query_params.append(('seasonNumber', _params['season_number']))
 
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
-            ['application/json'])  # noqa: E501
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
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
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/release', 'GET',
+            '/api/v3/config/ui/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/release_profile_api.py` & `sonarr-py-0.8.0/sonarr/api/release_profile_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/remote_path_mapping_api.py` & `sonarr-py-0.8.0/sonarr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/rename_episode_api.py` & `sonarr-py-0.8.0/sonarr/api/rename_episode_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/root_folder_api.py` & `sonarr-py-0.8.0/sonarr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/season_pass_api.py` & `sonarr-py-0.8.0/sonarr/api/season_pass_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/series_api.py` & `sonarr-py-0.8.0/sonarr/api/series_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/series_editor_api.py` & `sonarr-py-0.8.0/sonarr/api/series_editor_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/series_import_api.py` & `sonarr-py-0.8.0/sonarr/api/series_import_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/series_lookup_api.py` & `sonarr-py-0.8.0/sonarr/api/series_lookup_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/static_resource_api.py` & `sonarr-py-0.8.0/sonarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/system_api.py` & `sonarr-py-0.8.0/sonarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api/tag_api.py` & `sonarr-py-0.8.0/sonarr/api/queue_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,199 +13,56 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt
 
-from typing import List, Optional
+from typing import Optional
 
-from sonarr.models.tag_resource import TagResource
+from sonarr.models.queue_bulk_resource import QueueBulkResource
+from sonarr.models.queue_resource_paging_resource import QueueResourcePagingResource
 
 from sonarr.api_client import ApiClient
 from sonarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TagApi(object):
+class QueueApi(object):
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
+    def delete_queue(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+        """delete_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_tag(tag_resource, async_req=True)
-        >>> result = thread.get()
-
-        :param tag_resource:
-        :type tag_resource: TagResource
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
-        return self.create_tag_with_http_info(tag_resource, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def create_tag_with_http_info(self, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
-        """create_tag  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.create_tag_with_http_info(tag_resource, async_req=True)
-        >>> result = thread.get()
-
-        :param tag_resource:
-        :type tag_resource: TagResource
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
-            'tag_resource'
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
-                    " to method create_tag" % _key
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
-        if _params['tag_resource']:
-            _body_params = _params['tag_resource']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {
-            '200': "TagResource",
-        }
-
-        return self.api_client.call_api(
-            '/api/v3/tag', 'POST',
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
-    def delete_tag(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_tag  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.delete_tag(id, async_req=True)
+        >>> thread = api.delete_queue(id, remove_from_client, blocklist, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -214,28 +71,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_tag_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_queue_with_http_info(id, remove_from_client, blocklist, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_tag_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_tag  # noqa: E501
+    def delete_queue_with_http_info(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """delete_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_tag_with_http_info(id, async_req=True)
+        >>> thread = api.delete_queue_with_http_info(id, remove_from_client, blocklist, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -255,15 +116,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'remove_from_client',
+            'blocklist'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -274,28 +137,32 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_tag" % _key
+                    " to method delete_queue" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('remove_from_client') is not None:  # noqa: E501
+            _query_params.append(('removeFromClient', _params['remove_from_client']))
+        if _params.get('blocklist') is not None:  # noqa: E501
+            _query_params.append(('blocklist', _params['blocklist']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -305,15 +172,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/tag/{id}', 'DELETE',
+            '/api/v3/queue/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -322,55 +189,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_tag_by_id(self, id : StrictInt, **kwargs) -> TagResource:  # noqa: E501
-        """get_tag_by_id  # noqa: E501
+    def delete_queue_bulk(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_queue_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_by_id(id, async_req=True)
+        >>> thread = api.delete_queue_bulk(remove_from_client, blocklist, queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
+        :param queue_bulk_resource:
+        :type queue_bulk_resource: QueueBulkResource
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
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_tag_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_queue_bulk_with_http_info(remove_from_client, blocklist, queue_bulk_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_tag_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_tag_by_id  # noqa: E501
+    def delete_queue_bulk_with_http_info(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_queue_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.delete_queue_bulk_with_http_info(remove_from_client, blocklist, queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
+        :param queue_bulk_resource:
+        :type queue_bulk_resource: QueueBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -384,21 +259,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'remove_from_client',
+            'blocklist',
+            'queue_bulk_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -409,52 +286,57 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_tag_by_id" % _key
+                    " to method delete_queue_bulk" % _key
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
+        if _params.get('remove_from_client') is not None:  # noqa: E501
+            _query_params.append(('removeFromClient', _params['remove_from_client']))
+        if _params.get('blocklist') is not None:  # noqa: E501
+            _query_params.append(('blocklist', _params['blocklist']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['queue_bulk_resource']:
+            _body_params = _params['queue_bulk_resource']
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "TagResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v3/tag/{id}', 'GET',
+            '/api/v3/queue/bulk', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -463,51 +345,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_tag(self, **kwargs) -> List[TagResource]:  # noqa: E501
-        """list_tag  # noqa: E501
+    def get_queue(self, include_unknown_series_items : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode : Optional[StrictBool] = None, **kwargs) -> QueueResourcePagingResource:  # noqa: E501
+        """get_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag(async_req=True)
+        >>> thread = api.get_queue(include_unknown_series_items, include_series, include_episode, async_req=True)
         >>> result = thread.get()
 
+        :param include_unknown_series_items:
+        :type include_unknown_series_items: bool
+        :param include_series:
+        :type include_series: bool
+        :param include_episode:
+        :type include_episode: bool
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
-        :rtype: List[TagResource]
+        :rtype: QueueResourcePagingResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_tag_with_http_info(**kwargs)  # noqa: E501
+        return self.get_queue_with_http_info(include_unknown_series_items, include_series, include_episode, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_tag_with_http_info(self, **kwargs):  # noqa: E501
-        """list_tag  # noqa: E501
+    def get_queue_with_http_info(self, include_unknown_series_items : Optional[StrictBool] = None, include_series : Optional[StrictBool] = None, include_episode : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """get_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag_with_http_info(async_req=True)
+        >>> thread = api.get_queue_with_http_info(include_unknown_series_items, include_series, include_episode, async_req=True)
         >>> result = thread.get()
 
+        :param include_unknown_series_items:
+        :type include_unknown_series_items: bool
+        :param include_series:
+        :type include_series: bool
+        :param include_episode:
+        :type include_episode: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -521,20 +415,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[TagResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(QueueResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'include_unknown_series_items',
+            'include_series',
+            'include_episode'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -545,26 +442,32 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_tag" % _key
+                    " to method get_queue" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('include_unknown_series_items') is not None:  # noqa: E501
+            _query_params.append(('includeUnknownSeriesItems', _params['include_unknown_series_items']))
+        if _params.get('include_series') is not None:  # noqa: E501
+            _query_params.append(('includeSeries', _params['include_series']))
+        if _params.get('include_episode') is not None:  # noqa: E501
+            _query_params.append(('includeEpisode', _params['include_episode']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -576,174 +479,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[TagResource]",
-        }
-
-        return self.api_client.call_api(
-            '/api/v3/tag', 'GET',
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
-    def update_tag(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
-        """update_tag  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_tag(id, tag_resource, async_req=True)
-        >>> result = thread.get()
-
-        :param id: (required)
-        :type id: str
-        :param tag_resource:
-        :type tag_resource: TagResource
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
-        return self.update_tag_with_http_info(id, tag_resource, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def update_tag_with_http_info(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
-        """update_tag  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_tag_with_http_info(id, tag_resource, async_req=True)
-        >>> result = thread.get()
-
-        :param id: (required)
-        :type id: str
-        :param tag_resource:
-        :type tag_resource: TagResource
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
-            'id',
-            'tag_resource'
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
-                    " to method update_tag" % _key
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
-        if _params['tag_resource']:
-            _body_params = _params['tag_resource']
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {
-            '200': "TagResource",
+            '200': "QueueResourcePagingResource",
         }
 
         return self.api_client.call_api(
-            '/api/v3/tag/{id}', 'PUT',
+            '/api/v3/queue', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `sonarr-py-0.7.0/sonarr/api/update_api.py` & `sonarr-py-0.8.0/sonarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/api_client.py` & `sonarr-py-0.8.0/sonarr/api_client.py`

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
-        self.user_agent = 'sonarr-py/v0.7.0'
+        self.user_agent = 'sonarr-py/v0.8.0'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `sonarr-py-0.7.0/sonarr/api_response.py` & `sonarr-py-0.8.0/sonarr/api_response.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/configuration.py` & `sonarr-py-0.8.0/sonarr/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.7.0'
+        sdkversion = '0.8.0'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `sonarr-py-0.7.0/sonarr/exceptions.py` & `sonarr-py-0.8.0/sonarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/__init__.py` & `sonarr-py-0.8.0/sonarr/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from sonarr.models.command_status import CommandStatus
 from sonarr.models.command_trigger import CommandTrigger
 from sonarr.models.custom_filter_resource import CustomFilterResource
 from sonarr.models.custom_format_resource import CustomFormatResource
 from sonarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from sonarr.models.delay_profile_resource import DelayProfileResource
 from sonarr.models.disk_space_resource import DiskSpaceResource
+from sonarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from sonarr.models.download_client_config_resource import DownloadClientConfigResource
 from sonarr.models.download_client_resource import DownloadClientResource
 from sonarr.models.download_protocol import DownloadProtocol
 from sonarr.models.episode_file_list_resource import EpisodeFileListResource
 from sonarr.models.episode_file_resource import EpisodeFileResource
 from sonarr.models.episode_history_event_type import EpisodeHistoryEventType
 from sonarr.models.episode_resource import EpisodeResource
@@ -52,17 +53,19 @@
 from sonarr.models.field import Field
 from sonarr.models.file_date_type import FileDateType
 from sonarr.models.health_check_result import HealthCheckResult
 from sonarr.models.health_resource import HealthResource
 from sonarr.models.history_resource import HistoryResource
 from sonarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from sonarr.models.host_config_resource import HostConfigResource
+from sonarr.models.import_list_bulk_resource import ImportListBulkResource
 from sonarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from sonarr.models.import_list_resource import ImportListResource
 from sonarr.models.import_list_type import ImportListType
+from sonarr.models.indexer_bulk_resource import IndexerBulkResource
 from sonarr.models.indexer_config_resource import IndexerConfigResource
 from sonarr.models.indexer_resource import IndexerResource
 from sonarr.models.language import Language
 from sonarr.models.language_profile_item_resource import LanguageProfileItemResource
 from sonarr.models.language_profile_resource import LanguageProfileResource
 from sonarr.models.language_resource import LanguageResource
 from sonarr.models.localization_language_resource import LocalizationLanguageResource
```

### Comparing `sonarr-py-0.7.0/sonarr/models/add_series_options.py` & `sonarr-py-0.8.0/sonarr/models/add_series_options.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/alternate_title_resource.py` & `sonarr-py-0.8.0/sonarr/models/alternate_title_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/apply_tags.py` & `sonarr-py-0.8.0/sonarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/authentication_required_type.py` & `sonarr-py-0.8.0/sonarr/models/authentication_required_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/authentication_type.py` & `sonarr-py-0.8.0/sonarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/auto_tagging_resource.py` & `sonarr-py-0.8.0/sonarr/models/auto_tagging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/auto_tagging_specification_schema.py` & `sonarr-py-0.8.0/sonarr/models/auto_tagging_specification_schema.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/backup_resource.py` & `sonarr-py-0.8.0/sonarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/backup_type.py` & `sonarr-py-0.8.0/sonarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/blocklist_bulk_resource.py` & `sonarr-py-0.8.0/sonarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/blocklist_resource.py` & `sonarr-py-0.8.0/sonarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/blocklist_resource_paging_resource.py` & `sonarr-py-0.8.0/sonarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/certificate_validation_type.py` & `sonarr-py-0.8.0/sonarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/command.py` & `sonarr-py-0.8.0/sonarr/models/command.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/command_priority.py` & `sonarr-py-0.8.0/sonarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/command_resource.py` & `sonarr-py-0.8.0/sonarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/command_result.py` & `sonarr-py-0.8.0/sonarr/models/command_result.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/command_status.py` & `sonarr-py-0.8.0/sonarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/command_trigger.py` & `sonarr-py-0.8.0/sonarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/custom_filter_resource.py` & `sonarr-py-0.8.0/sonarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/custom_format_resource.py` & `sonarr-py-0.8.0/sonarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/custom_format_specification_schema.py` & `sonarr-py-0.8.0/sonarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/delay_profile_resource.py` & `sonarr-py-0.8.0/sonarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/disk_space_resource.py` & `sonarr-py-0.8.0/sonarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/download_client_config_resource.py` & `sonarr-py-0.8.0/sonarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/download_client_resource.py` & `sonarr-py-0.8.0/sonarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/download_protocol.py` & `sonarr-py-0.8.0/sonarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/episode_file_list_resource.py` & `sonarr-py-0.8.0/sonarr/models/episode_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/episode_file_resource.py` & `sonarr-py-0.8.0/sonarr/models/episode_file_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,17 +38,18 @@
     size: Optional[int]
     date_added: Optional[datetime]
     scene_name: Optional[str]
     release_group: Optional[str]
     languages: Optional[List]
     quality: Optional[QualityModel]
     custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     media_info: Optional[MediaInfoResource]
     quality_cutoff_not_met: Optional[bool]
-    __properties = ["id", "seriesId", "seasonNumber", "relativePath", "path", "size", "dateAdded", "sceneName", "releaseGroup", "languages", "quality", "customFormats", "mediaInfo", "qualityCutoffNotMet"]
+    __properties = ["id", "seriesId", "seasonNumber", "relativePath", "path", "size", "dateAdded", "sceneName", "releaseGroup", "languages", "quality", "customFormats", "customFormatScore", "mediaInfo", "qualityCutoffNotMet"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -137,12 +138,13 @@
             "size": obj.get("size"),
             "date_added": obj.get("dateAdded"),
             "scene_name": obj.get("sceneName"),
             "release_group": obj.get("releaseGroup"),
             "languages": [Language.from_dict(_item) for _item in obj.get("languages")] if obj.get("languages") is not None else None,
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "media_info": MediaInfoResource.from_dict(obj.get("mediaInfo")) if obj.get("mediaInfo") is not None else None,
             "quality_cutoff_not_met": obj.get("qualityCutoffNotMet")
         })
         return _obj
```

### Comparing `sonarr-py-0.7.0/sonarr/models/episode_history_event_type.py` & `sonarr-py-0.8.0/sonarr/models/episode_history_event_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/episode_resource.py` & `sonarr-py-0.8.0/sonarr/models/episode_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/episode_resource_paging_resource.py` & `sonarr-py-0.8.0/sonarr/models/episode_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/episode_title_required_type.py` & `sonarr-py-0.8.0/sonarr/models/episode_title_required_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/episodes_monitored_resource.py` & `sonarr-py-0.8.0/sonarr/models/episodes_monitored_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/field.py` & `sonarr-py-0.8.0/sonarr/models/field.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,26 @@
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
     privacy: Optional[PrivacyLevel]
     placeholder: Optional[str]
-    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "privacy", "placeholder"]
+    __properties = ["order", "name", "label", "unit", "helpText", "helpTextWarning", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "privacy", "placeholder"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -91,14 +92,18 @@
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
@@ -140,14 +145,15 @@
 
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

### Comparing `sonarr-py-0.7.0/sonarr/models/file_date_type.py` & `sonarr-py-0.8.0/sonarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/health_check_result.py` & `sonarr-py-0.8.0/sonarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/health_resource.py` & `sonarr-py-0.8.0/sonarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/history_resource.py` & `sonarr-py-0.8.0/sonarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/history_resource_paging_resource.py` & `sonarr-py-0.8.0/sonarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/host_config_resource.py` & `sonarr-py-0.8.0/sonarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/import_list_exclusion_resource.py` & `sonarr-py-0.8.0/sonarr/models/import_list_exclusion_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/import_list_resource.py` & `sonarr-py-0.8.0/sonarr/models/import_list_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/import_list_type.py` & `sonarr-py-0.8.0/sonarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/indexer_config_resource.py` & `sonarr-py-0.8.0/sonarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/indexer_resource.py` & `sonarr-py-0.8.0/sonarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/language.py` & `sonarr-py-0.8.0/sonarr/models/language.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/language_profile_item_resource.py` & `sonarr-py-0.8.0/sonarr/models/language_profile_item_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/language_profile_resource.py` & `sonarr-py-0.8.0/sonarr/models/language_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/language_resource.py` & `sonarr-py-0.8.0/sonarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/localization_language_resource.py` & `sonarr-py-0.8.0/sonarr/models/localization_language_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/localization_resource.py` & `sonarr-py-0.8.0/sonarr/models/localization_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/log_file_resource.py` & `sonarr-py-0.8.0/sonarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/log_resource.py` & `sonarr-py-0.8.0/sonarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/log_resource_paging_resource.py` & `sonarr-py-0.8.0/sonarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/manual_import_reprocess_resource.py` & `sonarr-py-0.8.0/sonarr/models/manual_import_reprocess_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/manual_import_resource.py` & `sonarr-py-0.8.0/sonarr/models/manual_import_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
     episode_file_id: Optional[int]
     release_group: Optional[str]
     quality: Optional[QualityModel]
     languages: Optional[List]
     quality_weight: Optional[int]
     download_id: Optional[str]
     custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     rejections: Optional[List]
-    __properties = ["id", "path", "relativePath", "folderName", "name", "size", "series", "seasonNumber", "episodes", "episodeFileId", "releaseGroup", "quality", "languages", "qualityWeight", "downloadId", "customFormats", "rejections"]
+    __properties = ["id", "path", "relativePath", "folderName", "name", "size", "series", "seasonNumber", "episodes", "episodeFileId", "releaseGroup", "quality", "languages", "qualityWeight", "downloadId", "customFormats", "customFormatScore", "rejections"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -184,11 +185,12 @@
             "episode_file_id": obj.get("episodeFileId"),
             "release_group": obj.get("releaseGroup"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "languages": [Language.from_dict(_item) for _item in obj.get("languages")] if obj.get("languages") is not None else None,
             "quality_weight": obj.get("qualityWeight"),
             "download_id": obj.get("downloadId"),
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "rejections": [Rejection.from_dict(_item) for _item in obj.get("rejections")] if obj.get("rejections") is not None else None
         })
         return _obj
```

### Comparing `sonarr-py-0.7.0/sonarr/models/media_cover.py` & `sonarr-py-0.8.0/sonarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/media_cover_types.py` & `sonarr-py-0.8.0/sonarr/models/rescan_after_refresh_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,25 +15,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class MediaCoverTypes(str, Enum):
+class RescanAfterRefreshType(str, Enum):
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
+    ALWAYS = 'always'
+    AFTERMANUAL = 'afterManual'
+    NEVER = 'never'
```

### Comparing `sonarr-py-0.7.0/sonarr/models/media_info_resource.py` & `sonarr-py-0.8.0/sonarr/models/media_info_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/media_management_config_resource.py` & `sonarr-py-0.8.0/sonarr/models/media_management_config_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,18 +42,20 @@
     set_permissions_linux: Optional[bool]
     chmod_folder: Optional[str]
     chown_group: Optional[str]
     episode_title_required: Optional[EpisodeTitleRequiredType]
     skip_free_space_check_when_importing: Optional[bool]
     minimum_free_space_when_importing: Optional[int]
     copy_using_hardlinks: Optional[bool]
+    use_script_import: Optional[bool]
+    script_import_path: Optional[str]
     import_extra_files: Optional[bool]
     extra_file_extensions: Optional[str]
     enable_media_info: Optional[bool]
-    __properties = ["id", "autoUnmonitorPreviouslyDownloadedEpisodes", "recycleBin", "recycleBinCleanupDays", "downloadPropersAndRepacks", "createEmptySeriesFolders", "deleteEmptyFolders", "fileDate", "rescanAfterRefresh", "setPermissionsLinux", "chmodFolder", "chownGroup", "episodeTitleRequired", "skipFreeSpaceCheckWhenImporting", "minimumFreeSpaceWhenImporting", "copyUsingHardlinks", "importExtraFiles", "extraFileExtensions", "enableMediaInfo"]
+    __properties = ["id", "autoUnmonitorPreviouslyDownloadedEpisodes", "recycleBin", "recycleBinCleanupDays", "downloadPropersAndRepacks", "createEmptySeriesFolders", "deleteEmptyFolders", "fileDate", "rescanAfterRefresh", "setPermissionsLinux", "chmodFolder", "chownGroup", "episodeTitleRequired", "skipFreeSpaceCheckWhenImporting", "minimumFreeSpaceWhenImporting", "copyUsingHardlinks", "useScriptImport", "scriptImportPath", "importExtraFiles", "extraFileExtensions", "enableMediaInfo"]
 
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
@@ -118,13 +124,15 @@
             "set_permissions_linux": obj.get("setPermissionsLinux"),
             "chmod_folder": obj.get("chmodFolder"),
             "chown_group": obj.get("chownGroup"),
             "episode_title_required": obj.get("episodeTitleRequired"),
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

### Comparing `sonarr-py-0.7.0/sonarr/models/metadata_resource.py` & `sonarr-py-0.8.0/sonarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/monitor_types.py` & `sonarr-py-0.8.0/sonarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/monitoring_options.py` & `sonarr-py-0.8.0/sonarr/models/monitoring_options.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/naming_config_resource.py` & `sonarr-py-0.8.0/sonarr/models/naming_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/notification_resource.py` & `sonarr-py-0.8.0/sonarr/models/notification_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/paging_resource_filter.py` & `sonarr-py-0.8.0/sonarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/parse_resource.py` & `sonarr-py-0.8.0/sonarr/models/queue_resource_paging_resource.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,30 +15,32 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from sonarr.models.episode_resource import EpisodeResource
-from sonarr.models.parsed_episode_info import ParsedEpisodeInfo
-from sonarr.models.series_resource import SeriesResource
+from sonarr.models.paging_resource_filter import PagingResourceFilter
+from sonarr.models.queue_resource import QueueResource
+from sonarr.models.sort_direction import SortDirection
 
-class ParseResource(BaseModel):
+class QueueResourcePagingResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    id: Optional[int]
-    title: Optional[str]
-    parsed_episode_info: Optional[ParsedEpisodeInfo]
-    series: Optional[SeriesResource]
-    episodes: Optional[List]
-    __properties = ["id", "title", "parsedEpisodeInfo", "series", "episodes"]
+    page: Optional[int]
+    page_size: Optional[int]
+    sort_key: Optional[str]
+    sort_direction: Optional[SortDirection]
+    filters: Optional[List]
+    total_records: Optional[int]
+    records: Optional[List]
+    __properties = ["page", "pageSize", "sortKey", "sortDirection", "filters", "totalRecords", "records"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -49,58 +51,65 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> ParseResource:
-        """Create an instance of ParseResource from a JSON string"""
+    def from_json(cls, json_str: str) -> QueueResourcePagingResource:
+        """Create an instance of QueueResourcePagingResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of parsed_episode_info
-        if self.parsed_episode_info:
-            _dict['parsedEpisodeInfo'] = self.parsed_episode_info.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of series
-        if self.series:
-            _dict['series'] = self.series.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in episodes (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in filters (list)
         _items = []
-        if self.episodes:
-            for _item in self.episodes:
+        if self.filters:
+            for _item in self.filters:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['episodes'] = _items
-        # set to None if title (nullable) is None
-        if self.title is None:
-            _dict['title'] = None
-
-        # set to None if episodes (nullable) is None
-        if self.episodes is None:
-            _dict['episodes'] = None
+            _dict['filters'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in records (list)
+        _items = []
+        if self.records:
+            for _item in self.records:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['records'] = _items
+        # set to None if sort_key (nullable) is None
+        if self.sort_key is None:
+            _dict['sortKey'] = None
+
+        # set to None if filters (nullable) is None
+        if self.filters is None:
+            _dict['filters'] = None
+
+        # set to None if records (nullable) is None
+        if self.records is None:
+            _dict['records'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> ParseResource:
-        """Create an instance of ParseResource from a dict"""
+    def from_dict(cls, obj: dict) -> QueueResourcePagingResource:
+        """Create an instance of QueueResourcePagingResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return ParseResource.parse_obj(obj)
+            return QueueResourcePagingResource.parse_obj(obj)
 
-        _obj = ParseResource.parse_obj({
-            "id": obj.get("id"),
-            "title": obj.get("title"),
-            "parsed_episode_info": ParsedEpisodeInfo.from_dict(obj.get("parsedEpisodeInfo")) if obj.get("parsedEpisodeInfo") is not None else None,
-            "series": SeriesResource.from_dict(obj.get("series")) if obj.get("series") is not None else None,
-            "episodes": [EpisodeResource.from_dict(_item) for _item in obj.get("episodes")] if obj.get("episodes") is not None else None
+        _obj = QueueResourcePagingResource.parse_obj({
+            "page": obj.get("page"),
+            "page_size": obj.get("pageSize"),
+            "sort_key": obj.get("sortKey"),
+            "sort_direction": obj.get("sortDirection"),
+            "filters": [PagingResourceFilter.from_dict(_item) for _item in obj.get("filters")] if obj.get("filters") is not None else None,
+            "total_records": obj.get("totalRecords"),
+            "records": [QueueResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
         })
         return _obj
```

### Comparing `sonarr-py-0.7.0/sonarr/models/parsed_episode_info.py` & `sonarr-py-0.8.0/sonarr/models/parsed_episode_info.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/ping_resource.py` & `sonarr-py-0.8.0/sonarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/privacy_level.py` & `sonarr-py-0.8.0/sonarr/models/privacy_level.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/profile_format_item_resource.py` & `sonarr-py-0.8.0/sonarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/proper_download_types.py` & `sonarr-py-0.8.0/sonarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/provider_message.py` & `sonarr-py-0.8.0/sonarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/provider_message_type.py` & `sonarr-py-0.8.0/sonarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/proxy_type.py` & `sonarr-py-0.8.0/sonarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/quality.py` & `sonarr-py-0.8.0/sonarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/quality_definition_resource.py` & `sonarr-py-0.8.0/sonarr/models/quality_definition_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/quality_model.py` & `sonarr-py-0.8.0/sonarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/quality_profile_quality_item_resource.py` & `sonarr-py-0.8.0/sonarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/quality_profile_resource.py` & `sonarr-py-0.8.0/sonarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/quality_source.py` & `sonarr-py-0.8.0/sonarr/models/quality_source.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/queue_bulk_resource.py` & `sonarr-py-0.8.0/sonarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/queue_resource.py` & `sonarr-py-0.8.0/sonarr/models/queue_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     episode_id: Optional[int]
     season_number: Optional[int]
     series: Optional[SeriesResource]
     episode: Optional[EpisodeResource]
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
@@ -56,15 +57,15 @@
     error_message: Optional[str]
     download_id: Optional[str]
     protocol: Optional[DownloadProtocol]
     download_client: Optional[str]
     indexer: Optional[str]
     output_path: Optional[str]
     episode_has_file: Optional[bool]
-    __properties = ["id", "seriesId", "episodeId", "seasonNumber", "series", "episode", "languages", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "episodeHasFile"]
+    __properties = ["id", "seriesId", "episodeId", "seasonNumber", "series", "episode", "languages", "quality", "customFormats", "customFormatScore", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "episodeHasFile"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -192,14 +193,15 @@
             "episode_id": obj.get("episodeId"),
             "season_number": obj.get("seasonNumber"),
             "series": SeriesResource.from_dict(obj.get("series")) if obj.get("series") is not None else None,
             "episode": EpisodeResource.from_dict(obj.get("episode")) if obj.get("episode") is not None else None,
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

### Comparing `sonarr-py-0.7.0/sonarr/models/queue_resource_paging_resource.py` & `sonarr-py-0.8.0/sonarr/models/parse_resource.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,32 +15,35 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel
-from sonarr.models.paging_resource_filter import PagingResourceFilter
-from sonarr.models.queue_resource import QueueResource
-from sonarr.models.sort_direction import SortDirection
+from sonarr.models.custom_format_resource import CustomFormatResource
+from sonarr.models.episode_resource import EpisodeResource
+from sonarr.models.language import Language
+from sonarr.models.parsed_episode_info import ParsedEpisodeInfo
+from sonarr.models.series_resource import SeriesResource
 
-class QueueResourcePagingResource(BaseModel):
+class ParseResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
-    page: Optional[int]
-    page_size: Optional[int]
-    sort_key: Optional[str]
-    sort_direction: Optional[SortDirection]
-    filters: Optional[List]
-    total_records: Optional[int]
-    records: Optional[List]
-    __properties = ["page", "pageSize", "sortKey", "sortDirection", "filters", "totalRecords", "records"]
+    id: Optional[int]
+    title: Optional[str]
+    parsed_episode_info: Optional[ParsedEpisodeInfo]
+    series: Optional[SeriesResource]
+    episodes: Optional[List]
+    languages: Optional[List]
+    custom_formats: Optional[List]
+    custom_format_score: Optional[int]
+    __properties = ["id", "title", "parsedEpisodeInfo", "series", "episodes", "languages", "customFormats", "customFormatScore"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -51,65 +54,83 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> QueueResourcePagingResource:
-        """Create an instance of QueueResourcePagingResource from a JSON string"""
+    def from_json(cls, json_str: str) -> ParseResource:
+        """Create an instance of ParseResource from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in filters (list)
+        # override the default output from pydantic by calling `to_dict()` of parsed_episode_info
+        if self.parsed_episode_info:
+            _dict['parsedEpisodeInfo'] = self.parsed_episode_info.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of series
+        if self.series:
+            _dict['series'] = self.series.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in episodes (list)
         _items = []
-        if self.filters:
-            for _item in self.filters:
+        if self.episodes:
+            for _item in self.episodes:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['filters'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in records (list)
+            _dict['episodes'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in languages (list)
         _items = []
-        if self.records:
-            for _item in self.records:
+        if self.languages:
+            for _item in self.languages:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['records'] = _items
-        # set to None if sort_key (nullable) is None
-        if self.sort_key is None:
-            _dict['sortKey'] = None
-
-        # set to None if filters (nullable) is None
-        if self.filters is None:
-            _dict['filters'] = None
-
-        # set to None if records (nullable) is None
-        if self.records is None:
-            _dict['records'] = None
+            _dict['languages'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in custom_formats (list)
+        _items = []
+        if self.custom_formats:
+            for _item in self.custom_formats:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['customFormats'] = _items
+        # set to None if title (nullable) is None
+        if self.title is None:
+            _dict['title'] = None
+
+        # set to None if episodes (nullable) is None
+        if self.episodes is None:
+            _dict['episodes'] = None
+
+        # set to None if languages (nullable) is None
+        if self.languages is None:
+            _dict['languages'] = None
+
+        # set to None if custom_formats (nullable) is None
+        if self.custom_formats is None:
+            _dict['customFormats'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> QueueResourcePagingResource:
-        """Create an instance of QueueResourcePagingResource from a dict"""
+    def from_dict(cls, obj: dict) -> ParseResource:
+        """Create an instance of ParseResource from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return QueueResourcePagingResource.parse_obj(obj)
+            return ParseResource.parse_obj(obj)
 
-        _obj = QueueResourcePagingResource.parse_obj({
-            "page": obj.get("page"),
-            "page_size": obj.get("pageSize"),
-            "sort_key": obj.get("sortKey"),
-            "sort_direction": obj.get("sortDirection"),
-            "filters": [PagingResourceFilter.from_dict(_item) for _item in obj.get("filters")] if obj.get("filters") is not None else None,
-            "total_records": obj.get("totalRecords"),
-            "records": [QueueResource.from_dict(_item) for _item in obj.get("records")] if obj.get("records") is not None else None
+        _obj = ParseResource.parse_obj({
+            "id": obj.get("id"),
+            "title": obj.get("title"),
+            "parsed_episode_info": ParsedEpisodeInfo.from_dict(obj.get("parsedEpisodeInfo")) if obj.get("parsedEpisodeInfo") is not None else None,
+            "series": SeriesResource.from_dict(obj.get("series")) if obj.get("series") is not None else None,
+            "episodes": [EpisodeResource.from_dict(_item) for _item in obj.get("episodes")] if obj.get("episodes") is not None else None,
+            "languages": [Language.from_dict(_item) for _item in obj.get("languages")] if obj.get("languages") is not None else None,
+            "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore")
         })
         return _obj
```

### Comparing `sonarr-py-0.7.0/sonarr/models/queue_status_resource.py` & `sonarr-py-0.8.0/sonarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/ratings.py` & `sonarr-py-0.8.0/sonarr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/rejection.py` & `sonarr-py-0.8.0/sonarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/rejection_type.py` & `sonarr-py-0.8.0/sonarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/release_episode_resource.py` & `sonarr-py-0.8.0/sonarr/models/release_episode_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/release_profile_resource.py` & `sonarr-py-0.8.0/sonarr/models/release_profile_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Any, List, Optional
+from typing import List, Optional
 from pydantic import BaseModel
 
 class ReleaseProfileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     name: Optional[str]
     enabled: Optional[bool]
-    required: Optional[object]
-    ignored: Optional[object]
+    required: Optional[List]
+    ignored: Optional[List]
     indexer_id: Optional[int]
     tags: Optional[List]
     __properties = ["id", "name", "enabled", "required", "ignored", "indexerId", "tags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `sonarr-py-0.7.0/sonarr/models/release_resource.py` & `sonarr-py-0.8.0/sonarr/models/release_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/remote_path_mapping_resource.py` & `sonarr-py-0.8.0/sonarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/rename_episode_resource.py` & `sonarr-py-0.8.0/sonarr/models/rename_episode_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/rescan_after_refresh_type.py` & `sonarr-py-0.8.0/sonarr/models/tracked_download_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class RescanAfterRefreshType(str, Enum):
+class TrackedDownloadStatus(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    ALWAYS = 'always'
-    AFTERMANUAL = 'afterManual'
-    NEVER = 'never'
+    OK = 'ok'
+    WARNING = 'warning'
+    ERROR = 'error'
```

### Comparing `sonarr-py-0.7.0/sonarr/models/revision.py` & `sonarr-py-0.8.0/sonarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/root_folder_resource.py` & `sonarr-py-0.8.0/sonarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/runtime_mode.py` & `sonarr-py-0.8.0/sonarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/season_pass_resource.py` & `sonarr-py-0.8.0/sonarr/models/season_pass_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/season_pass_series_resource.py` & `sonarr-py-0.8.0/sonarr/models/season_pass_series_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/season_resource.py` & `sonarr-py-0.8.0/sonarr/models/season_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/season_statistics_resource.py` & `sonarr-py-0.8.0/sonarr/models/season_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/select_option.py` & `sonarr-py-0.8.0/sonarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/series_editor_resource.py` & `sonarr-py-0.8.0/sonarr/models/series_editor_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/series_resource.py` & `sonarr-py-0.8.0/sonarr/models/series_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/series_statistics_resource.py` & `sonarr-py-0.8.0/sonarr/models/series_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/series_status_type.py` & `sonarr-py-0.8.0/sonarr/models/series_status_type.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/series_title_info.py` & `sonarr-py-0.8.0/sonarr/models/series_title_info.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/series_types.py` & `sonarr-py-0.8.0/sonarr/models/series_types.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/sort_direction.py` & `sonarr-py-0.8.0/sonarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/system_resource.py` & `sonarr-py-0.8.0/sonarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/tag_details_resource.py` & `sonarr-py-0.8.0/sonarr/models/tag_details_resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,17 +29,18 @@
     id: Optional[int]
     label: Optional[str]
     delay_profile_ids: Optional[List]
     import_list_ids: Optional[List]
     notification_ids: Optional[List]
     restriction_ids: Optional[List]
     indexer_ids: Optional[List]
+    download_client_ids: Optional[List]
     auto_tag_ids: Optional[List]
     series_ids: Optional[List]
-    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "indexerIds", "autoTagIds", "seriesIds"]
+    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "indexerIds", "downloadClientIds", "autoTagIds", "seriesIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -84,14 +85,18 @@
         if self.restriction_ids is None:
             _dict['restrictionIds'] = None
 
         # set to None if indexer_ids (nullable) is None
         if self.indexer_ids is None:
             _dict['indexerIds'] = None
 
+        # set to None if download_client_ids (nullable) is None
+        if self.download_client_ids is None:
+            _dict['downloadClientIds'] = None
+
         # set to None if auto_tag_ids (nullable) is None
         if self.auto_tag_ids is None:
             _dict['autoTagIds'] = None
 
         # set to None if series_ids (nullable) is None
         if self.series_ids is None:
             _dict['seriesIds'] = None
@@ -111,12 +116,13 @@
             "id": obj.get("id"),
             "label": obj.get("label"),
             "delay_profile_ids": obj.get("delayProfileIds"),
             "import_list_ids": obj.get("importListIds"),
             "notification_ids": obj.get("notificationIds"),
             "restriction_ids": obj.get("restrictionIds"),
             "indexer_ids": obj.get("indexerIds"),
+            "download_client_ids": obj.get("downloadClientIds"),
             "auto_tag_ids": obj.get("autoTagIds"),
             "series_ids": obj.get("seriesIds")
         })
         return _obj
```

### Comparing `sonarr-py-0.7.0/sonarr/models/tag_resource.py` & `sonarr-py-0.8.0/sonarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/task_resource.py` & `sonarr-py-0.8.0/sonarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/tracked_download_state.py` & `sonarr-py-0.8.0/sonarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/tracked_download_status.py` & `sonarr-py-0.8.0/sonarr/models/update_mechanism.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class TrackedDownloadStatus(str, Enum):
+class UpdateMechanism(str, Enum):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
 
-    OK = 'ok'
-    WARNING = 'warning'
-    ERROR = 'error'
+    BUILTIN = 'builtIn'
+    SCRIPT = 'script'
+    EXTERNAL = 'external'
+    APT = 'apt'
+    DOCKER = 'docker'
```

### Comparing `sonarr-py-0.7.0/sonarr/models/tracked_download_status_message.py` & `sonarr-py-0.8.0/sonarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/ui_config_resource.py` & `sonarr-py-0.8.0/sonarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/unmapped_folder.py` & `sonarr-py-0.8.0/sonarr/models/unmapped_folder.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/update_changes.py` & `sonarr-py-0.8.0/sonarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/models/update_mechanism.py` & `sonarr-py-0.8.0/sonarr/models/media_cover_types.py`

 * *Files 19% similar despite different names*

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

### Comparing `sonarr-py-0.7.0/sonarr/models/update_resource.py` & `sonarr-py-0.8.0/sonarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr/rest.py` & `sonarr-py-0.8.0/sonarr/rest.py`

 * *Files identical despite different names*

### Comparing `sonarr-py-0.7.0/sonarr_py.egg-info/PKG-INFO` & `sonarr-py-0.8.0/sonarr_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonarr-py
-Version: 0.7.0
+Version: 0.8.0
 Summary: Sonarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/sonarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/sonarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -12,15 +12,15 @@
 
 # sonarr-py
 Sonarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.7.0
+- Package version: 0.8.0
 
 [comment]: # (x-release-please-end)
 - API version: 3.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -137,32 +137,34 @@
 *CustomFilterApi* | [**delete_custom_filter**](docs/CustomFilterApi.md#delete_custom_filter) | **DELETE** /api/v3/customfilter/{id} | 
 *CustomFilterApi* | [**get_custom_filter_by_id**](docs/CustomFilterApi.md#get_custom_filter_by_id) | **GET** /api/v3/customfilter/{id} | 
 *CustomFilterApi* | [**list_custom_filter**](docs/CustomFilterApi.md#list_custom_filter) | **GET** /api/v3/customfilter | 
 *CustomFilterApi* | [**update_custom_filter**](docs/CustomFilterApi.md#update_custom_filter) | **PUT** /api/v3/customfilter/{id} | 
 *CustomFormatApi* | [**create_custom_format**](docs/CustomFormatApi.md#create_custom_format) | **POST** /api/v3/customformat | 
 *CustomFormatApi* | [**delete_custom_format**](docs/CustomFormatApi.md#delete_custom_format) | **DELETE** /api/v3/customformat/{id} | 
 *CustomFormatApi* | [**get_custom_format_by_id**](docs/CustomFormatApi.md#get_custom_format_by_id) | **GET** /api/v3/customformat/{id} | 
-*CustomFormatApi* | [**get_custom_format_schema**](docs/CustomFormatApi.md#get_custom_format_schema) | **GET** /api/v3/customformat/schema | 
 *CustomFormatApi* | [**list_custom_format**](docs/CustomFormatApi.md#list_custom_format) | **GET** /api/v3/customformat | 
+*CustomFormatApi* | [**list_custom_format_schema**](docs/CustomFormatApi.md#list_custom_format_schema) | **GET** /api/v3/customformat/schema | 
 *CustomFormatApi* | [**update_custom_format**](docs/CustomFormatApi.md#update_custom_format) | **PUT** /api/v3/customformat/{id} | 
 *CutoffApi* | [**get_wanted_cutoff**](docs/CutoffApi.md#get_wanted_cutoff) | **GET** /api/v3/wanted/cutoff | 
 *CutoffApi* | [**get_wanted_cutoff_by_id**](docs/CutoffApi.md#get_wanted_cutoff_by_id) | **GET** /api/v3/wanted/cutoff/{id} | 
 *DelayProfileApi* | [**create_delay_profile**](docs/DelayProfileApi.md#create_delay_profile) | **POST** /api/v3/delayprofile | 
 *DelayProfileApi* | [**delete_delay_profile**](docs/DelayProfileApi.md#delete_delay_profile) | **DELETE** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**get_delay_profile_by_id**](docs/DelayProfileApi.md#get_delay_profile_by_id) | **GET** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v3/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v3/delayprofile/{id} | 
 *DelayProfileApi* | [**update_delay_profile_reorder**](docs/DelayProfileApi.md#update_delay_profile_reorder) | **PUT** /api/v3/delayprofile/reorder/{id} | 
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
 *EpisodeApi* | [**get_episode_by_id**](docs/EpisodeApi.md#get_episode_by_id) | **GET** /api/v3/episode/{id} | 
@@ -175,59 +177,60 @@
 *EpisodeFileApi* | [**list_episode_file**](docs/EpisodeFileApi.md#list_episode_file) | **GET** /api/v3/episodefile | 
 *EpisodeFileApi* | [**put_episode_file_bulk**](docs/EpisodeFileApi.md#put_episode_file_bulk) | **PUT** /api/v3/episodefile/bulk | 
 *EpisodeFileApi* | [**put_episode_file_editor**](docs/EpisodeFileApi.md#put_episode_file_editor) | **PUT** /api/v3/episodefile/editor | 
 *EpisodeFileApi* | [**update_episode_file**](docs/EpisodeFileApi.md#update_episode_file) | **PUT** /api/v3/episodefile/{id} | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v3/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v3/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v3/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v3/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v3/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v3/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v3/history | 
 *HistoryApi* | [**list_history_series**](docs/HistoryApi.md#list_history_series) | **GET** /api/v3/history/series | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v3/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v3/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v3/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v3/config/host/{id} | 
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
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v3/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v3/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v3/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v3/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v3/importlistexclusion/{id} | 
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
-*InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
 *LanguageApi* | [**get_language_by_id**](docs/LanguageApi.md#get_language_by_id) | **GET** /api/v3/language/{id} | 
 *LanguageApi* | [**list_language**](docs/LanguageApi.md#list_language) | **GET** /api/v3/language | 
 *LanguageProfileApi* | [**create_language_profile**](docs/LanguageProfileApi.md#create_language_profile) | **POST** /api/v3/languageprofile | 
 *LanguageProfileApi* | [**delete_language_profile**](docs/LanguageProfileApi.md#delete_language_profile) | **DELETE** /api/v3/languageprofile/{id} | 
 *LanguageProfileApi* | [**get_language_profile_by_id**](docs/LanguageProfileApi.md#get_language_profile_by_id) | **GET** /api/v3/languageprofile/{id} | 
 *LanguageProfileApi* | [**list_language_profile**](docs/LanguageProfileApi.md#list_language_profile) | **GET** /api/v3/languageprofile | 
 *LanguageProfileApi* | [**update_language_profile**](docs/LanguageProfileApi.md#update_language_profile) | **PUT** /api/v3/languageprofile/{id} | 
 *LanguageProfileSchemaApi* | [**get_languageprofile_schema**](docs/LanguageProfileSchemaApi.md#get_languageprofile_schema) | **GET** /api/v3/languageprofile/schema | 
-*LanguageProfileSchemaApi* | [**get_languageprofile_schema_by_id**](docs/LanguageProfileSchemaApi.md#get_languageprofile_schema_by_id) | **GET** /api/v3/languageprofile/schema/{id} | 
 *LocalizationApi* | [**get_localization**](docs/LocalizationApi.md#get_localization) | **GET** /api/v3/localization | 
 *LocalizationApi* | [**get_localization_by_id**](docs/LocalizationApi.md#get_localization_by_id) | **GET** /api/v3/localization/{id} | 
 *LocalizationApi* | [**get_localization_language**](docs/LocalizationApi.md#get_localization_language) | **GET** /api/v3/localization/language | 
 *LogApi* | [**get_log**](docs/LogApi.md#get_log) | **GET** /api/v3/log | 
 *LogFileApi* | [**get_log_file_by_filename**](docs/LogFileApi.md#get_log_file_by_filename) | **GET** /api/v3/log/file/{filename} | 
 *LogFileApi* | [**list_log_file**](docs/LogFileApi.md#list_log_file) | **GET** /api/v3/log/file | 
 *ManualImportApi* | [**create_manual_import**](docs/ManualImportApi.md#create_manual_import) | **POST** /api/v3/manualimport | 
@@ -271,31 +274,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v3/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v3/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v3/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v3/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v3/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v3/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v3/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v3/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v3/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v3/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v3/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v3/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v3/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v3/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v3/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v3/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v3/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v3/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v3/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v3/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v3/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v3/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v3/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v3/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v3/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v3/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v3/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v3/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v3/remotepathmapping/{id} | 
 *RenameEpisodeApi* | [**list_rename**](docs/RenameEpisodeApi.md#list_rename) | **GET** /api/v3/rename | 
 *RootFolderApi* | [**create_root_folder**](docs/RootFolderApi.md#create_root_folder) | **POST** /api/v3/rootfolder | 
@@ -360,14 +358,15 @@
  - [CommandStatus](docs/CommandStatus.md)
  - [CommandTrigger](docs/CommandTrigger.md)
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [EpisodeFileListResource](docs/EpisodeFileListResource.md)
  - [EpisodeFileResource](docs/EpisodeFileResource.md)
  - [EpisodeHistoryEventType](docs/EpisodeHistoryEventType.md)
  - [EpisodeResource](docs/EpisodeResource.md)
@@ -377,17 +376,19 @@
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [Language](docs/Language.md)
  - [LanguageProfileItemResource](docs/LanguageProfileItemResource.md)
  - [LanguageProfileResource](docs/LanguageProfileResource.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [LocalizationLanguageResource](docs/LocalizationLanguageResource.md)
```

### Comparing `sonarr-py-0.7.0/sonarr_py.egg-info/SOURCES.txt` & `sonarr-py-0.8.0/sonarr_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 sonarr/api/health_api.py
 sonarr/api/history_api.py
 sonarr/api/host_config_api.py
 sonarr/api/import_list_api.py
 sonarr/api/import_list_exclusion_api.py
 sonarr/api/indexer_api.py
 sonarr/api/indexer_config_api.py
-sonarr/api/initialize_js_api.py
 sonarr/api/language_api.py
 sonarr/api/language_profile_api.py
 sonarr/api/language_profile_schema_api.py
 sonarr/api/localization_api.py
 sonarr/api/log_api.py
 sonarr/api/log_file_api.py
 sonarr/api/manual_import_api.py
@@ -96,14 +95,15 @@
 sonarr/models/command_status.py
 sonarr/models/command_trigger.py
 sonarr/models/custom_filter_resource.py
 sonarr/models/custom_format_resource.py
 sonarr/models/custom_format_specification_schema.py
 sonarr/models/delay_profile_resource.py
 sonarr/models/disk_space_resource.py
+sonarr/models/download_client_bulk_resource.py
 sonarr/models/download_client_config_resource.py
 sonarr/models/download_client_resource.py
 sonarr/models/download_protocol.py
 sonarr/models/episode_file_list_resource.py
 sonarr/models/episode_file_resource.py
 sonarr/models/episode_history_event_type.py
 sonarr/models/episode_resource.py
@@ -113,17 +113,19 @@
 sonarr/models/field.py
 sonarr/models/file_date_type.py
 sonarr/models/health_check_result.py
 sonarr/models/health_resource.py
 sonarr/models/history_resource.py
 sonarr/models/history_resource_paging_resource.py
 sonarr/models/host_config_resource.py
+sonarr/models/import_list_bulk_resource.py
 sonarr/models/import_list_exclusion_resource.py
 sonarr/models/import_list_resource.py
 sonarr/models/import_list_type.py
+sonarr/models/indexer_bulk_resource.py
 sonarr/models/indexer_config_resource.py
 sonarr/models/indexer_resource.py
 sonarr/models/language.py
 sonarr/models/language_profile_item_resource.py
 sonarr/models/language_profile_resource.py
 sonarr/models/language_resource.py
 sonarr/models/localization_language_resource.py
```

