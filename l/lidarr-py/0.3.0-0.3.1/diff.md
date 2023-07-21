# Comparing `tmp/lidarr-py-0.3.0.tar.gz` & `tmp/lidarr-py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidarr-py-0.3.0.tar", last modified: Mon May 29 06:41:55 2023, max compression
+gzip compressed data, was "lidarr-py-0.3.1.tar", last modified: Fri Jul 21 11:35:51 2023, max compression
```

## Comparing `lidarr-py-0.3.0.tar` & `lidarr-py-0.3.1.tar`

### file list

```diff
@@ -1,251 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39897 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.272012 lidarr-py-0.3.0/lidarr/
--rw-r--r--   0 runner    (1001) docker     (123)    14710 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.288012 lidarr-py-0.3.0/lidarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38749 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/album_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/album_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/album_studio_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31554 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/artist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/artist_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/artist_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17838 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23471 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30446 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36254 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    54263 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19199 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11937 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28885 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53591 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52966 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18756 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53134 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/metadata_provider_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30583 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53806 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27560 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12044 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12841 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30991 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/rename_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/retag_track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26845 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29517 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/track_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37824 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/track_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18466 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/lidarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/add_album_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/add_artist_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_add_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_studio_artist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/album_studio_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/albums_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/allow_fingerprinting.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_metadata_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/artist_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/entity_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/i_custom_format_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/iso_country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/manual_import_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/medium_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/member.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_provider_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/new_item_monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/parsed_album_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/parsed_track_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/primary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_format_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_release_status_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_release_status_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/release_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rename_track_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/retag_track_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/secondary_album_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tag_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/track_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/models/write_audio_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/lidarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/lidarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40369 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 06:41:55.000000 lidarr-py-0.3.0/lidarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:41:55.320011 lidarr-py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-29 06:41:30.000000 lidarr-py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:51.182645 lidarr-py-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-07-21 11:35:51.182645 lidarr-py-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40199 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:51.126643 lidarr-py-0.3.1/lidarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:51.142644 lidarr-py-0.3.1/lidarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38749 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/album_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/album_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6872 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/album_studio_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31554 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/artist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/artist_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/artist_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12688 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30349 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35514 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36254 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67069 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19137 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28885 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18582 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66173 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65339 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11800 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19195 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53283 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30734 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/metadata_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/metadata_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19253 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/metadata_provider_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12618 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30583 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53955 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25228 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12253 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21822 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30638 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30929 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/rename_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/retag_track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30192 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21832 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26818 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29420 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12027 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/track_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37824 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/track_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11932 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29639 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:51.178645 lidarr-py-0.3.1/lidarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10768 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/add_album_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/add_artist_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_add_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_release_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_release_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_studio_artist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/album_studio_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/albums_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/allow_fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_metadata_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/artist_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/command_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/entity_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/i_custom_format_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/import_list_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/import_list_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/iso_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/localization_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/manual_import_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/media_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/medium_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/metadata_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/metadata_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/metadata_provider_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/new_item_monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/parsed_album_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/parsed_track_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/primary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_format_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_primary_album_type_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_primary_album_type_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_release_status_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_release_status_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_secondary_album_type_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/profile_secondary_album_type_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_profile_quality_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8909 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/release_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/rename_track_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/retag_track_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/secondary_album_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/tag_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6699 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track_file_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4965 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/track_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/models/write_audio_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/lidarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:51.178645 lidarr-py-0.3.1/lidarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40671 2023-07-21 11:35:51.000000 lidarr-py-0.3.1/lidarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-07-21 11:35:51.000000 lidarr-py-0.3.1/lidarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:35:51.000000 lidarr-py-0.3.1/lidarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 11:35:51.000000 lidarr-py-0.3.1/lidarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 11:35:51.000000 lidarr-py-0.3.1/lidarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:35:51.182645 lidarr-py-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-21 11:35:36.000000 lidarr-py-0.3.1/setup.py
```

### Comparing `lidarr-py-0.3.0/LICENSE` & `lidarr-py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/PKG-INFO` & `lidarr-py-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidarr-py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lidarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/lidarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/lidarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # lidarr-py
 Lidarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.3.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -166,55 +166,60 @@
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v1/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**update_delay_profile_reorder**](docs/DelayProfileApi.md#update_delay_profile_reorder) | **PUT** /api/v1/delayprofile/reorder/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v1/diskspace | 
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
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_artist**](docs/HistoryApi.md#list_history_artist) | **GET** /api/v1/history/artist | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v1/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v1/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v1/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v1/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v1/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v1/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v1/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v1/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v1/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v1/importlist/{id} | 
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v1/importlistexclusion/{id} | 
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
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v1/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v1/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v1/config/indexer/{id} | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
@@ -275,31 +280,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v1/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v1/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v1/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v1/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v1/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v1/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v1/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v1/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v1/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v1/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v1/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v1/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v1/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v1/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v1/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v1/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v1/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v1/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v1/remotepathmapping/{id} | 
 *RenameTrackApi* | [**list_rename**](docs/RenameTrackApi.md#list_rename) | **GET** /api/v1/rename | 
 *RetagTrackApi* | [**list_retag**](docs/RetagTrackApi.md#list_retag) | **GET** /api/v1/retag | 
@@ -388,35 +388,39 @@
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [EntityHistoryEventType](docs/EntityHistoryEventType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
+ - [LocalizationResource](docs/LocalizationResource.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
  - [LogResourcePagingResource](docs/LogResourcePagingResource.md)
  - [ManualImportResource](docs/ManualImportResource.md)
  - [ManualImportUpdateResource](docs/ManualImportUpdateResource.md)
  - [MediaCover](docs/MediaCover.md)
  - [MediaCoverTypes](docs/MediaCoverTypes.md)
```

### Comparing `lidarr-py-0.3.0/README.md` & `lidarr-py-0.3.1/lidarr_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: lidarr-py
+Version: 0.3.1
+Summary: Lidarr API wrapper
+Project-URL: Homepage, https://github.com/devopsarr/lidarr-py
+Project-URL: Bug Tracker, https://github.com/devopsarr/lidarr-py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # lidarr-py
 Lidarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.3.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -153,55 +166,60 @@
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v1/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**update_delay_profile_reorder**](docs/DelayProfileApi.md#update_delay_profile_reorder) | **PUT** /api/v1/delayprofile/reorder/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v1/diskspace | 
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
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_artist**](docs/HistoryApi.md#list_history_artist) | **GET** /api/v1/history/artist | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v1/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v1/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v1/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v1/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v1/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v1/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v1/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v1/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v1/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v1/importlist/{id} | 
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v1/importlistexclusion/{id} | 
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
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v1/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v1/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v1/config/indexer/{id} | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
@@ -262,31 +280,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v1/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v1/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v1/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v1/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v1/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v1/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v1/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v1/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v1/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v1/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v1/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v1/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v1/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v1/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v1/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v1/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v1/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v1/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v1/remotepathmapping/{id} | 
 *RenameTrackApi* | [**list_rename**](docs/RenameTrackApi.md#list_rename) | **GET** /api/v1/rename | 
 *RetagTrackApi* | [**list_retag**](docs/RetagTrackApi.md#list_retag) | **GET** /api/v1/retag | 
@@ -375,35 +388,39 @@
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [EntityHistoryEventType](docs/EntityHistoryEventType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
+ - [LocalizationResource](docs/LocalizationResource.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
  - [LogResourcePagingResource](docs/LogResourcePagingResource.md)
  - [ManualImportResource](docs/ManualImportResource.md)
  - [ManualImportUpdateResource](docs/ManualImportUpdateResource.md)
  - [MediaCover](docs/MediaCover.md)
  - [MediaCoverTypes](docs/MediaCoverTypes.md)
```

### Comparing `lidarr-py-0.3.0/lidarr/__init__.py` & `lidarr-py-0.3.1/lidarr/__init__.py`

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
 from lidarr.api.album_api import AlbumApi
 from lidarr.api.album_lookup_api import AlbumLookupApi
 from lidarr.api.album_studio_api import AlbumStudioApi
 from lidarr.api.api_info_api import ApiInfoApi
@@ -143,35 +143,39 @@
 from lidarr.models.custom_filter_resource import CustomFilterResource
 from lidarr.models.custom_format import CustomFormat
 from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from lidarr.models.database_type import DatabaseType
 from lidarr.models.delay_profile_resource import DelayProfileResource
 from lidarr.models.disk_space_resource import DiskSpaceResource
+from lidarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from lidarr.models.download_client_config_resource import DownloadClientConfigResource
 from lidarr.models.download_client_resource import DownloadClientResource
 from lidarr.models.download_protocol import DownloadProtocol
 from lidarr.models.entity_history_event_type import EntityHistoryEventType
 from lidarr.models.field import Field
 from lidarr.models.file_date_type import FileDateType
 from lidarr.models.health_check_result import HealthCheckResult
 from lidarr.models.health_resource import HealthResource
 from lidarr.models.history_resource import HistoryResource
 from lidarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from lidarr.models.host_config_resource import HostConfigResource
 from lidarr.models.i_custom_format_specification import ICustomFormatSpecification
+from lidarr.models.import_list_bulk_resource import ImportListBulkResource
 from lidarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from lidarr.models.import_list_monitor_type import ImportListMonitorType
 from lidarr.models.import_list_resource import ImportListResource
 from lidarr.models.import_list_type import ImportListType
+from lidarr.models.indexer_bulk_resource import IndexerBulkResource
 from lidarr.models.indexer_config_resource import IndexerConfigResource
 from lidarr.models.indexer_resource import IndexerResource
 from lidarr.models.iso_country import IsoCountry
 from lidarr.models.language_resource import LanguageResource
 from lidarr.models.links import Links
+from lidarr.models.localization_resource import LocalizationResource
 from lidarr.models.log_file_resource import LogFileResource
 from lidarr.models.log_resource import LogResource
 from lidarr.models.log_resource_paging_resource import LogResourcePagingResource
 from lidarr.models.manual_import_resource import ManualImportResource
 from lidarr.models.manual_import_update_resource import ManualImportUpdateResource
 from lidarr.models.media_cover import MediaCover
 from lidarr.models.media_cover_types import MediaCoverTypes
```

### Comparing `lidarr-py-0.3.0/lidarr/api/__init__.py` & `lidarr-py-0.3.1/lidarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/album_api.py` & `lidarr-py-0.3.1/lidarr/api/album_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/album_lookup_api.py` & `lidarr-py-0.3.1/lidarr/api/album_lookup_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/album_studio_api.py` & `lidarr-py-0.3.1/lidarr/api/album_studio_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/api_info_api.py` & `lidarr-py-0.3.1/lidarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/artist_api.py` & `lidarr-py-0.3.1/lidarr/api/artist_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/artist_editor_api.py` & `lidarr-py-0.3.1/lidarr/api/artist_editor_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/artist_lookup_api.py` & `lidarr-py-0.3.1/lidarr/api/artist_lookup_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/authentication_api.py` & `lidarr-py-0.3.1/lidarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/backup_api.py` & `lidarr-py-0.3.1/lidarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/blocklist_api.py` & `lidarr-py-0.3.1/lidarr/api/blocklist_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -424,15 +424,15 @@
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
             '200': "BlocklistResourcePagingResource",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/calendar_api.py` & `lidarr-py-0.3.1/lidarr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/calendar_feed_api.py` & `lidarr-py-0.3.1/lidarr/api/calendar_feed_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/command_api.py` & `lidarr-py-0.3.1/lidarr/api/command_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,20 +153,20 @@
         # process the body parameter
         _body_params = None
         if _params['command_resource']:
             _body_params = _params['command_resource']
 
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
@@ -570,15 +570,15 @@
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
             '200': "List[CommandResource]",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/custom_filter_api.py` & `lidarr-py-0.3.1/lidarr/api/custom_filter_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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
@@ -570,15 +570,15 @@
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
             '200': "List[CustomFilterResource]",
         }
@@ -723,15 +723,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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

### Comparing `lidarr-py-0.3.0/lidarr/api/custom_format_api.py` & `lidarr-py-0.3.1/lidarr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/cutoff_api.py` & `lidarr-py-0.3.1/lidarr/api/cutoff_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
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
             '200': "AlbumResourcePagingResource",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/delay_profile_api.py` & `lidarr-py-0.3.1/lidarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/disk_space_api.py` & `lidarr-py-0.3.1/lidarr/api/disk_space_api.py`

 * *Files 1% similar despite different names*

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
             '200': "List[DiskSpaceResource]",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/download_client_api.py` & `lidarr-py-0.3.1/lidarr/api/notification_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,77 +17,81 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from lidarr.models.download_client_resource import DownloadClientResource
+from lidarr.models.notification_resource import NotificationResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class DownloadClientApi(object):
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
-    def create_download_client(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
-        """create_download_client  # noqa: E501
+    def create_notification(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+        """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client(download_client_resource, async_req=True)
+        >>> thread = api.create_notification(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-        :rtype: DownloadClientResource
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_download_client_with_http_info(download_client_resource, **kwargs)  # noqa: E501
+        return self.create_notification_with_http_info(force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_download_client_with_http_info(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """create_download_client  # noqa: E501
+    def create_notification_with_http_info(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_with_http_info(download_client_resource, async_req=True)
+        >>> thread = api.create_notification_with_http_info(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'download_client_resource'
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
-                    " to method create_download_client" % _key
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
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
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
-            '200': "DownloadClientResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient', 'POST',
+            '/api/v1/notification', 'POST',
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
-    def create_download_client_action_by_name(self, name : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_download_client_action_by_name  # noqa: E501
+    def create_notification_action_by_name(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_notification_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_action_by_name(name, download_client_resource, async_req=True)
+        >>> thread = api.create_notification_action_by_name(name, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-        return self.create_download_client_action_by_name_with_http_info(name, download_client_resource, **kwargs)  # noqa: E501
+        return self.create_notification_action_by_name_with_http_info(name, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_download_client_action_by_name_with_http_info(self, name : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """create_download_client_action_by_name  # noqa: E501
+    def create_notification_action_by_name_with_http_info(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """create_notification_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_action_by_name_with_http_info(name, download_client_resource, async_req=True)
+        >>> thread = api.create_notification_action_by_name_with_http_info(name, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-            'download_client_resource'
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
-                    " to method create_download_client_action_by_name" % _key
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
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
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
-            '/api/v1/downloadclient/action/{name}', 'POST',
+            '/api/v1/notification/action/{name}', 'POST',
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
-    def delete_download_client(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_download_client  # noqa: E501
+    def delete_notification(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_download_client(id, async_req=True)
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
-        return self.delete_download_client_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_notification_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_download_client_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_download_client  # noqa: E501
+    def delete_notification_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_download_client_with_http_info(id, async_req=True)
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
-                    " to method delete_download_client" % _key
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
-            '/api/v1/downloadclient/{id}', 'DELETE',
+            '/api/v1/notification/{id}', 'DELETE',
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
-    def get_download_client_by_id(self, id : StrictInt, **kwargs) -> DownloadClientResource:  # noqa: E501
-        """get_download_client_by_id  # noqa: E501
+    def get_notification_by_id(self, id : StrictInt, **kwargs) -> NotificationResource:  # noqa: E501
+        """get_notification_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_download_client_by_id(id, async_req=True)
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
-        :rtype: DownloadClientResource
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_download_client_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_notification_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_download_client_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_download_client_by_id  # noqa: E501
+    def get_notification_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_notification_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_download_client_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_download_client_by_id" % _key
+                    " to method get_notification_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -591,19 +598,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "DownloadClientResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/{id}', 'GET',
+            '/api/v1/notification/{id}', 'GET',
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
-    def list_download_client(self, **kwargs) -> List[DownloadClientResource]:  # noqa: E501
-        """list_download_client  # noqa: E501
+    def list_notification(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
+        """list_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client(async_req=True)
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
-        :rtype: List[DownloadClientResource]
+        :rtype: List[NotificationResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_download_client_with_http_info(**kwargs)  # noqa: E501
+        return self.list_notification_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_download_client_with_http_info(self, **kwargs):  # noqa: E501
-        """list_download_client  # noqa: E501
+    def list_notification_with_http_info(self, **kwargs):  # noqa: E501
+        """list_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client_with_http_info(async_req=True)
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
-        :rtype: tuple(List[DownloadClientResource], status_code(int), headers(HTTPHeaderDict))
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
-                    " to method list_download_client" % _key
+                    " to method list_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -719,25 +726,25 @@
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
-            '200': "List[DownloadClientResource]",
+            '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient', 'GET',
+            '/api/v1/notification', 'GET',
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
-    def list_download_client_schema(self, **kwargs) -> List[DownloadClientResource]:  # noqa: E501
-        """list_download_client_schema  # noqa: E501
+    def list_notification_schema(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
+        """list_notification_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client_schema(async_req=True)
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
-        :rtype: List[DownloadClientResource]
+        :rtype: List[NotificationResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_download_client_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_notification_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_download_client_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_download_client_schema  # noqa: E501
+    def list_notification_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_notification_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client_schema_with_http_info(async_req=True)
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
-        :rtype: tuple(List[DownloadClientResource], status_code(int), headers(HTTPHeaderDict))
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
-                    " to method list_download_client_schema" % _key
+                    " to method list_notification_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -853,25 +860,25 @@
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
-            '200': "List[DownloadClientResource]",
+            '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/schema', 'GET',
+            '/api/v1/notification/schema', 'GET',
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
-    def test_download_client(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> None:  # noqa: E501
-        """test_download_client  # noqa: E501
+    def test_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
+        """test_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_download_client(download_client_resource, async_req=True)
+        >>> thread = api.test_notification(notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-        return self.test_download_client_with_http_info(download_client_resource, **kwargs)  # noqa: E501
+        return self.test_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_download_client_with_http_info(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """test_download_client  # noqa: E501
+    def test_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """test_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_download_client_with_http_info(download_client_resource, async_req=True)
+        >>> thread = api.test_notification_with_http_info(notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-            'download_client_resource'
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
-                    " to method test_download_client" % _key
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
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
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
-            '/api/v1/downloadclient/test', 'POST',
+            '/api/v1/notification/test', 'POST',
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
-    def testall_download_client(self, **kwargs) -> None:  # noqa: E501
-        """testall_download_client  # noqa: E501
+    def testall_notification(self, **kwargs) -> None:  # noqa: E501
+        """testall_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_download_client(async_req=True)
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
-        return self.testall_download_client_with_http_info(**kwargs)  # noqa: E501
+        return self.testall_notification_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def testall_download_client_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_download_client  # noqa: E501
+    def testall_notification_with_http_info(self, **kwargs):  # noqa: E501
+        """testall_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_download_client_with_http_info(async_req=True)
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
-                    " to method testall_download_client" % _key
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
-            '/api/v1/downloadclient/testall', 'POST',
+            '/api/v1/notification/testall', 'POST',
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
-    def update_download_client(self, id : StrictStr, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
-        """update_download_client  # noqa: E501
+    def update_notification(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+        """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client(id, force_save, download_client_resource, async_req=True)
+        >>> thread = api.update_notification(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
         :param force_save:
         :type force_save: bool
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
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
-        :rtype: DownloadClientResource
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_download_client_with_http_info(id, force_save, download_client_resource, **kwargs)  # noqa: E501
+        return self.update_notification_with_http_info(id, force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_download_client_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """update_download_client  # noqa: E501
+    def update_notification_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client_with_http_info(id, force_save, download_client_resource, async_req=True)
+        >>> thread = api.update_notification_with_http_info(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
         :param force_save:
         :type force_save: bool
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
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
-        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
             'force_save',
-            'download_client_resource'
+            'notification_resource'
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
-                    " to method update_download_client" % _key
+                    " to method update_notification" % _key
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
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
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
-            '200': "DownloadClientResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/{id}', 'PUT',
+            '/api/v1/notification/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/download_client_config_api.py` & `lidarr-py-0.3.1/lidarr/api/download_client_config_api.py`

 * *Files 1% similar despite different names*

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
             '200': "DownloadClientConfigResource",
         }
@@ -440,15 +440,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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

### Comparing `lidarr-py-0.3.0/lidarr/api/file_system_api.py` & `lidarr-py-0.3.1/lidarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/health_api.py` & `lidarr-py-0.3.1/lidarr/api/language_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import List
 
-from lidarr.models.health_resource import HealthResource
+from lidarr.models.language_resource import LanguageResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class HealthApi(object):
+class LanguageApi(object):
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
+    def get_language_by_id(self, id : StrictInt, **kwargs) -> LanguageResource:  # noqa: E501
+        """get_language_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id(id, async_req=True)
+        >>> thread = api.get_language_by_id(id, async_req=True)
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
-        :rtype: HealthResource
+        :rtype: LanguageResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_health_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_language_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_health_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_health_by_id  # noqa: E501
+    def get_language_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_language_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_language_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(HealthResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(LanguageResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_health_by_id" % _key
+                    " to method get_language_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -159,19 +159,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "HealthResource",
+            '200': "LanguageResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/health/{id}', 'GET',
+            '/api/v1/language/{id}', 'GET',
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
+    def list_language(self, **kwargs) -> List[LanguageResource]:  # noqa: E501
+        """list_language  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health(async_req=True)
+        >>> thread = api.list_language(async_req=True)
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
+        :rtype: List[LanguageResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_health_with_http_info(**kwargs)  # noqa: E501
+        return self.list_language_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_health_with_http_info(self, **kwargs):  # noqa: E501
-        """list_health  # noqa: E501
+    def list_language_with_http_info(self, **kwargs):  # noqa: E501
+        """list_language  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health_with_http_info(async_req=True)
+        >>> thread = api.list_language_with_http_info(async_req=True)
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
+        :rtype: tuple(List[LanguageResource], status_code(int), headers(HTTPHeaderDict))
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
+                    " to method list_language" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -293,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[HealthResource]",
+            '200': "List[LanguageResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/health', 'GET',
+            '/api/v1/language', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/history_api.py` & `lidarr-py-0.3.1/lidarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/host_config_api.py` & `lidarr-py-0.3.1/lidarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/import_list_api.py` & `lidarr-py-0.3.1/lidarr/api/import_list_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from lidarr.models.import_list_bulk_resource import ImportListBulkResource
 from lidarr.models.import_list_resource import ImportListResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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
+            '/api/v1/importlist/bulk', 'DELETE',
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
@@ -719,15 +869,15 @@
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
             '200': "List[ImportListResource]",
         }
@@ -853,15 +1003,15 @@
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
             '200': "List[ImportListResource]",
         }
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
+            '/api/v1/importlist/bulk', 'PUT',
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
@@ -995,15 +1293,15 @@
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

### Comparing `lidarr-py-0.3.0/lidarr/api/import_list_exclusion_api.py` & `lidarr-py-0.3.1/lidarr/api/import_list_exclusion_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/indexer_api.py` & `lidarr-py-0.3.1/lidarr/api/indexer_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from lidarr.models.indexer_bulk_resource import IndexerBulkResource
 from lidarr.models.indexer_resource import IndexerResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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
     def get_indexer_by_id(self, id : StrictInt, **kwargs) -> IndexerResource:  # noqa: E501
         """get_indexer_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_indexer_by_id(id, async_req=True)
@@ -719,15 +869,15 @@
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
             '200': "List[IndexerResource]",
         }
@@ -853,15 +1003,15 @@
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
             '200': "List[IndexerResource]",
         }
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
+            '/api/v1/indexer/bulk', 'PUT',
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
@@ -995,15 +1293,15 @@
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

### Comparing `lidarr-py-0.3.0/lidarr/api/indexer_config_api.py` & `lidarr-py-0.3.1/lidarr/api/indexer_config_api.py`

 * *Files 2% similar despite different names*

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
             '200': "IndexerConfigResource",
         }
@@ -440,15 +440,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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

### Comparing `lidarr-py-0.3.0/lidarr/api/initialize_js_api.py` & `lidarr-py-0.3.1/lidarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/language_api.py` & `lidarr-py-0.3.1/lidarr/api/tag_details_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import List
 
-from lidarr.models.language_resource import LanguageResource
+from lidarr.models.tag_details_resource import TagDetailsResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class LanguageApi(object):
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
-    def get_language_by_id(self, id : StrictInt, **kwargs) -> LanguageResource:  # noqa: E501
-        """get_language_by_id  # noqa: E501
+    def get_tag_detail_by_id(self, id : StrictInt, **kwargs) -> TagDetailsResource:  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_language_by_id(id, async_req=True)
+        >>> thread = api.get_tag_detail_by_id(id, async_req=True)
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
-        :rtype: LanguageResource
+        :rtype: TagDetailsResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_language_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_tag_detail_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_language_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_language_by_id  # noqa: E501
+    def get_tag_detail_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_language_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_tag_detail_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(LanguageResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TagDetailsResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_language_by_id" % _key
+                    " to method get_tag_detail_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -159,19 +159,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "LanguageResource",
+            '200': "TagDetailsResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/language/{id}', 'GET',
+            '/api/v1/tag/detail/{id}', 'GET',
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
-    def list_language(self, **kwargs) -> List[LanguageResource]:  # noqa: E501
-        """list_language  # noqa: E501
+    def list_tag_detail(self, **kwargs) -> List[TagDetailsResource]:  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_language(async_req=True)
+        >>> thread = api.list_tag_detail(async_req=True)
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
-        :rtype: List[LanguageResource]
+        :rtype: List[TagDetailsResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_language_with_http_info(**kwargs)  # noqa: E501
+        return self.list_tag_detail_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_language_with_http_info(self, **kwargs):  # noqa: E501
-        """list_language  # noqa: E501
+    def list_tag_detail_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_language_with_http_info(async_req=True)
+        >>> thread = api.list_tag_detail_with_http_info(async_req=True)
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
-        :rtype: tuple(List[LanguageResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TagDetailsResource], status_code(int), headers(HTTPHeaderDict))
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
-                    " to method list_language" % _key
+                    " to method list_tag_detail" % _key
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
-            '200': "List[LanguageResource]",
+            '200': "List[TagDetailsResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/language', 'GET',
+            '/api/v1/tag/detail', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/localization_api.py` & `lidarr-py-0.3.1/lidarr/api/parse_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,72 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
+from pydantic import StrictStr
+
+from typing import Optional
+
+from lidarr.models.parse_resource import ParseResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class LocalizationApi(object):
+class ParseApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_localization(self, **kwargs) -> str:  # noqa: E501
-        """get_localization  # noqa: E501
+    def get_parse(self, title : Optional[StrictStr] = None, **kwargs) -> ParseResource:  # noqa: E501
+        """get_parse  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_localization(async_req=True)
+        >>> thread = api.get_parse(title, async_req=True)
         >>> result = thread.get()
 
+        :param title:
+        :type title: str
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
-        :rtype: str
+        :rtype: ParseResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_localization_with_http_info(**kwargs)  # noqa: E501
+        return self.get_parse_with_http_info(title, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_localization_with_http_info(self, **kwargs):  # noqa: E501
-        """get_localization  # noqa: E501
+    def get_parse_with_http_info(self, title : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+        """get_parse  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_localization_with_http_info(async_req=True)
+        >>> thread = api.get_parse_with_http_info(title, async_req=True)
         >>> result = thread.get()
 
+        :param title:
+        :type title: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -92,20 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(str, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ParseResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'title'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -116,50 +126,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_localization" % _key
+                    " to method get_parse" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('title') is not None:  # noqa: E501
+            _query_params.append(('title', _params['title']))
 
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
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "str",
+            '200': "ParseResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/localization', 'GET',
+            '/api/v1/parse', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/log_api.py` & `lidarr-py-0.3.1/lidarr/api/log_api.py`

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
             '200': "LogResourcePagingResource",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/log_file_api.py` & `lidarr-py-0.3.1/lidarr/api/log_file_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
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

### Comparing `lidarr-py-0.3.0/lidarr/api/manual_import_api.py` & `lidarr-py-0.3.1/lidarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/media_cover_api.py` & `lidarr-py-0.3.1/lidarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/media_management_config_api.py` & `lidarr-py-0.3.1/lidarr/api/media_management_config_api.py`

 * *Files 1% similar despite different names*

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
             '200': "MediaManagementConfigResource",
         }
@@ -440,15 +440,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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

### Comparing `lidarr-py-0.3.0/lidarr/api/metadata_api.py` & `lidarr-py-0.3.1/lidarr/api/metadata_api.py`

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
@@ -719,15 +726,15 @@
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
             '200': "List[MetadataResource]",
         }
@@ -853,15 +860,15 @@
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
             '200': "List[MetadataResource]",
         }
@@ -995,15 +1002,15 @@
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

### Comparing `lidarr-py-0.3.0/lidarr/api/metadata_profile_api.py` & `lidarr-py-0.3.1/lidarr/api/metadata_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/metadata_profile_schema_api.py` & `lidarr-py-0.3.1/lidarr/api/metadata_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/metadata_provider_config_api.py` & `lidarr-py-0.3.1/lidarr/api/metadata_provider_config_api.py`

 * *Files 0% similar despite different names*

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
             '200': "MetadataProviderConfigResource",
         }
@@ -440,15 +440,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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

### Comparing `lidarr-py-0.3.0/lidarr/api/missing_api.py` & `lidarr-py-0.3.1/lidarr/api/missing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
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
             '200': "AlbumResourcePagingResource",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/naming_config_api.py` & `lidarr-py-0.3.1/lidarr/api/naming_config_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/notification_api.py` & `lidarr-py-0.3.1/lidarr/api/track_file_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,81 +13,82 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr, conlist
 
 from typing import List, Optional
 
-from lidarr.models.notification_resource import NotificationResource
+from lidarr.models.track_file_list_resource import TrackFileListResource
+from lidarr.models.track_file_resource import TrackFileResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class NotificationApi(object):
+class TrackFileApi(object):
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
+    def delete_track_file(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_track_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification(notification_resource, async_req=True)
+        >>> thread = api.delete_track_file(id, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
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
-        :rtype: NotificationResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
+        return self.delete_track_file_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """create_notification  # noqa: E501
+    def delete_track_file_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_track_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_with_http_info(notification_resource, async_req=True)
+        >>> thread = api.delete_track_file_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +102,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'notification_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,59 +127,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_notification" % _key
+                    " to method delete_track_file" % _key
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
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
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
-            '200': "NotificationResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/notification', 'POST',
+            '/api/v1/trackfile/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,27 +175,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_notification_action_by_name(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_notification_action_by_name  # noqa: E501
+    def delete_track_file_bulk(self, track_file_list_resource : Optional[TrackFileListResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_track_file_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_action_by_name(name, notification_resource, async_req=True)
+        >>> thread = api.delete_track_file_bulk(track_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param name: (required)
-        :type name: str
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param track_file_list_resource:
+        :type track_file_list_resource: TrackFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -216,30 +202,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_notification_action_by_name_with_http_info(name, notification_resource, **kwargs)  # noqa: E501
+        return self.delete_track_file_bulk_with_http_info(track_file_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_notification_action_by_name_with_http_info(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """create_notification_action_by_name  # noqa: E501
+    def delete_track_file_bulk_with_http_info(self, track_file_list_resource : Optional[TrackFileListResource] = None, **kwargs):  # noqa: E501
+        """delete_track_file_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_notification_action_by_name_with_http_info(name, notification_resource, async_req=True)
+        >>> thread = api.delete_track_file_bulk_with_http_info(track_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param name: (required)
-        :type name: str
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param track_file_list_resource:
+        :type track_file_list_resource: TrackFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -259,16 +243,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'name',
-            'notification_resource'
+            'track_file_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -279,55 +262,53 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_notification_action_by_name" % _key
+                    " to method delete_track_file_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['name']:
-            _path_params['name'] = _params['name']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['track_file_list_resource']:
+            _body_params = _params['track_file_list_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/notification/action/{name}', 'POST',
+            '/api/v1/trackfile/bulk', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -336,21 +317,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_notification(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_notification  # noqa: E501
+    def get_track_file_by_id(self, id : StrictInt, **kwargs) -> TrackFileResource:  # noqa: E501
+        """get_track_file_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_notification(id, async_req=True)
+        >>> thread = api.get_track_file_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -360,27 +341,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: TrackFileResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_notification_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_track_file_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_notification_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_notification  # noqa: E501
+    def get_track_file_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_track_file_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_notification_with_http_info(id, async_req=True)
+        >>> thread = api.get_track_file_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -398,15 +379,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(TrackFileResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -423,15 +404,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_notification" % _key
+                    " to method get_track_file_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -448,296 +429,27 @@
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            '/api/v1/notification/{id}', 'DELETE',
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
-    def get_notification_by_id(self, id : StrictInt, **kwargs) -> NotificationResource:  # noqa: E501
-        """get_notification_by_id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_notification_by_id(id, async_req=True)
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
-        :rtype: NotificationResource
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_notification_by_id_with_http_info(id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def get_notification_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_notification_by_id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_notification_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_notification_by_id" % _key
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
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {
-            '200': "NotificationResource",
-        }
-
-        return self.api_client.call_api(
-            '/api/v1/notification/{id}', 'GET',
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
-    def list_notification(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
-        """list_notification  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.list_notification(async_req=True)
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
-        :rtype: List[NotificationResource]
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.list_notification_with_http_info(**kwargs)  # noqa: E501
-
-    @validate_arguments
-    def list_notification_with_http_info(self, **kwargs):  # noqa: E501
-        """list_notification  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.list_notification_with_http_info(async_req=True)
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
-        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
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
-                    " to method list_notification" % _key
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
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[NotificationResource]",
+            '200': "TrackFileResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/notification', 'GET',
+            '/api/v1/trackfile/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -746,51 +458,67 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_notification_schema(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
-        """list_notification_schema  # noqa: E501
+    def list_track_file(self, artist_id : Optional[StrictInt] = None, track_file_ids : Optional[conlist(StrictInt)] = None, album_id : Optional[conlist(StrictInt)] = None, unmapped : Optional[StrictBool] = None, **kwargs) -> List[TrackFileResource]:  # noqa: E501
+        """list_track_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_notification_schema(async_req=True)
+        >>> thread = api.list_track_file(artist_id, track_file_ids, album_id, unmapped, async_req=True)
         >>> result = thread.get()
 
+        :param artist_id:
+        :type artist_id: int
+        :param track_file_ids:
+        :type track_file_ids: List[int]
+        :param album_id:
+        :type album_id: List[int]
+        :param unmapped:
+        :type unmapped: bool
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
-        :rtype: List[NotificationResource]
+        :rtype: List[TrackFileResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_notification_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_track_file_with_http_info(artist_id, track_file_ids, album_id, unmapped, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_notification_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_notification_schema  # noqa: E501
+    def list_track_file_with_http_info(self, artist_id : Optional[StrictInt] = None, track_file_ids : Optional[conlist(StrictInt)] = None, album_id : Optional[conlist(StrictInt)] = None, unmapped : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """list_track_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_notification_schema_with_http_info(async_req=True)
+        >>> thread = api.list_track_file_with_http_info(artist_id, track_file_ids, album_id, unmapped, async_req=True)
         >>> result = thread.get()
 
+        :param artist_id:
+        :type artist_id: int
+        :param track_file_ids:
+        :type track_file_ids: List[int]
+        :param album_id:
+        :type album_id: List[int]
+        :param unmapped:
+        :type unmapped: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -804,20 +532,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TrackFileResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'artist_id',
+            'track_file_ids',
+            'album_id',
+            'unmapped'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -828,26 +560,36 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_notification_schema" % _key
+                    " to method list_track_file" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('artist_id') is not None:  # noqa: E501
+            _query_params.append(('artistId', _params['artist_id']))
+        if _params.get('track_file_ids') is not None:  # noqa: E501
+            _query_params.append(('trackFileIds', _params['track_file_ids']))
+            _collection_formats['trackFileIds'] = 'multi'
+        if _params.get('album_id') is not None:  # noqa: E501
+            _query_params.append(('albumId', _params['album_id']))
+            _collection_formats['albumId'] = 'multi'
+        if _params.get('unmapped') is not None:  # noqa: E501
+            _query_params.append(('unmapped', _params['unmapped']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -859,19 +601,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[NotificationResource]",
+            '200': "List[TrackFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/notification/schema', 'GET',
+            '/api/v1/trackfile', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -880,25 +622,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def test_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
-        """test_notification  # noqa: E501
+    def put_track_file_editor(self, track_file_list_resource : Optional[TrackFileListResource] = None, **kwargs) -> None:  # noqa: E501
+        """put_track_file_editor  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_notification(notification_resource, async_req=True)
+        >>> thread = api.put_track_file_editor(track_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param track_file_list_resource:
+        :type track_file_list_resource: TrackFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -907,28 +649,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.test_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
+        return self.put_track_file_editor_with_http_info(track_file_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """test_notification  # noqa: E501
+    def put_track_file_editor_with_http_info(self, track_file_list_resource : Optional[TrackFileListResource] = None, **kwargs):  # noqa: E501
+        """put_track_file_editor  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_notification_with_http_info(notification_resource, async_req=True)
+        >>> thread = api.put_track_file_editor_with_http_info(track_file_list_resource, async_req=True)
         >>> result = thread.get()
 
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param track_file_list_resource:
+        :type track_file_list_resource: TrackFileListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -948,15 +690,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'notification_resource'
+            'track_file_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -967,15 +709,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method test_notification" % _key
+                    " to method put_track_file_editor" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -989,159 +731,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['track_file_list_resource']:
+            _body_params = _params['track_file_list_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
                 ['application/json', 'text/json', 'application/*+json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/notification/test', 'POST',
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
-    def testall_notification(self, **kwargs) -> None:  # noqa: E501
-        """testall_notification  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.testall_notification(async_req=True)
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
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.testall_notification_with_http_info(**kwargs)  # noqa: E501
-
-    @validate_arguments
-    def testall_notification_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_notification  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.testall_notification_with_http_info(async_req=True)
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
-        :rtype: None
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
-                    " to method testall_notification" % _key
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
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            '/api/v1/notification/testall', 'POST',
+            '/api/v1/trackfile/editor', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1150,63 +764,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_notification(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
-        """update_notification  # noqa: E501
+    def update_track_file(self, id : StrictStr, track_file_resource : Optional[TrackFileResource] = None, **kwargs) -> TrackFileResource:  # noqa: E501
+        """update_track_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification(id, force_save, notification_resource, async_req=True)
+        >>> thread = api.update_track_file(id, track_file_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param force_save:
-        :type force_save: bool
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param track_file_resource:
+        :type track_file_resource: TrackFileResource
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
+        :rtype: TrackFileResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_notification_with_http_info(id, force_save, notification_resource, **kwargs)  # noqa: E501
+        return self.update_track_file_with_http_info(id, track_file_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_notification_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
-        """update_notification  # noqa: E501
+    def update_track_file_with_http_info(self, id : StrictStr, track_file_resource : Optional[TrackFileResource] = None, **kwargs):  # noqa: E501
+        """update_track_file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_notification_with_http_info(id, force_save, notification_resource, async_req=True)
+        >>> thread = api.update_track_file_with_http_info(id, track_file_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param force_save:
-        :type force_save: bool
-        :param notification_resource:
-        :type notification_resource: NotificationResource
+        :param track_file_resource:
+        :type track_file_resource: TrackFileResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1220,23 +830,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TrackFileResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'force_save',
-            'notification_resource'
+            'track_file_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1247,42 +856,40 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_notification" % _key
+                    " to method update_track_file" % _key
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
-        if _params.get('force_save') is not None:  # noqa: E501
-            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['notification_resource']:
-            _body_params = _params['notification_resource']
+        if _params['track_file_resource']:
+            _body_params = _params['track_file_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1291,19 +898,19 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "NotificationResource",
+            '200': "TrackFileResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/notification/{id}', 'PUT',
+            '/api/v1/trackfile/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/parse_api.py` & `lidarr-py-0.3.1/lidarr/api/ping_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,81 +13,73 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictStr
-
-from typing import Optional
-
-from lidarr.models.parse_resource import ParseResource
+from lidarr.models.ping_resource import PingResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ParseApi(object):
+class PingApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_parse(self, title : Optional[StrictStr] = None, **kwargs) -> ParseResource:  # noqa: E501
-        """get_parse  # noqa: E501
+    def get_ping(self, **kwargs) -> PingResource:  # noqa: E501
+        """get_ping  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_parse(title, async_req=True)
+        >>> thread = api.get_ping(async_req=True)
         >>> result = thread.get()
 
-        :param title:
-        :type title: str
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
-        :rtype: ParseResource
+        :rtype: PingResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_parse_with_http_info(title, **kwargs)  # noqa: E501
+        return self.get_ping_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_parse_with_http_info(self, title : Optional[StrictStr] = None, **kwargs):  # noqa: E501
-        """get_parse  # noqa: E501
+    def get_ping_with_http_info(self, **kwargs):  # noqa: E501
+        """get_ping  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_parse_with_http_info(title, async_req=True)
+        >>> thread = api.get_ping_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param title:
-        :type title: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +93,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ParseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(PingResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'title'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,52 +117,50 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_parse" % _key
+                    " to method get_ping" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('title') is not None:  # noqa: E501
-            _query_params.append(('title', _params['title']))
 
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
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ParseResource",
+            '200': "PingResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/parse', 'GET',
+            '/ping', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/ping_api.py` & `lidarr-py-0.3.1/lidarr/api/update_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,43 +13,45 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from lidarr.models.ping_resource import PingResource
+from typing import List
+
+from lidarr.models.update_resource import UpdateResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class PingApi(object):
+class UpdateApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_ping(self, **kwargs) -> PingResource:  # noqa: E501
-        """get_ping  # noqa: E501
+    def list_update(self, **kwargs) -> List[UpdateResource]:  # noqa: E501
+        """list_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_ping(async_req=True)
+        >>> thread = api.list_update(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -57,27 +59,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: PingResource
+        :rtype: List[UpdateResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_ping_with_http_info(**kwargs)  # noqa: E501
+        return self.list_update_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_ping_with_http_info(self, **kwargs):  # noqa: E501
-        """get_ping  # noqa: E501
+    def list_update_with_http_info(self, **kwargs):  # noqa: E501
+        """list_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_ping_with_http_info(async_req=True)
+        >>> thread = api.list_update_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -93,15 +95,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(PingResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[UpdateResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -117,15 +119,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_ping" % _key
+                    " to method list_update" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -148,19 +150,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "PingResource",
+            '200': "List[UpdateResource]",
         }
 
         return self.api_client.call_api(
-            '/ping', 'GET',
+            '/api/v1/update', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/quality_definition_api.py` & `lidarr-py-0.3.1/lidarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/quality_profile_api.py` & `lidarr-py-0.3.1/lidarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/quality_profile_schema_api.py` & `lidarr-py-0.3.1/lidarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/queue_action_api.py` & `lidarr-py-0.3.1/lidarr/api/queue_action_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         _body_params = None
         if _params['queue_bulk_resource']:
             _body_params = _params['queue_bulk_resource']
 
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
```

### Comparing `lidarr-py-0.3.0/lidarr/api/queue_api.py` & `lidarr-py-0.3.1/lidarr/api/tag_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,59 +13,199 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import Optional
+from typing import List, Optional
 
-from lidarr.models.queue_bulk_resource import QueueBulkResource
-from lidarr.models.queue_resource import QueueResource
-from lidarr.models.queue_resource_paging_resource import QueueResourcePagingResource
+from lidarr.models.tag_resource import TagResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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
-    def delete_queue(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
-        """delete_queue  # noqa: E501
+    def create_tag(self, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
+        """create_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue(id, remove_from_client, blocklist, skip_re_download, async_req=True)
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
+            '/api/v1/tag', 'POST',
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
-        :param skip_re_download:
-        :type skip_re_download: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -74,34 +214,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_queue_with_http_info(id, remove_from_client, blocklist, skip_re_download, **kwargs)  # noqa: E501
+        return self.delete_tag_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_queue_with_http_info(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """delete_queue  # noqa: E501
+    def delete_tag_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_with_http_info(id, remove_from_client, blocklist, skip_re_download, async_req=True)
+        >>> thread = api.delete_tag_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
-        :param skip_re_download:
-        :type skip_re_download: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -121,18 +255,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'remove_from_client',
-            'blocklist',
-            'skip_re_download'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -143,34 +274,28 @@
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
-        if _params.get('skip_re_download') is not None:  # noqa: E501
-            _query_params.append(('skipReDownload', _params['skip_re_download']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -180,15 +305,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/queue/{id}', 'DELETE',
+            '/api/v1/tag/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -197,67 +322,55 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_queue_bulk(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
-        """delete_queue_bulk  # noqa: E501
+    def get_tag_by_id(self, id : StrictInt, **kwargs) -> TagResource:  # noqa: E501
+        """get_tag_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_bulk(remove_from_client, blocklist, skip_re_download, queue_bulk_resource, async_req=True)
+        >>> thread = api.get_tag_by_id(id, async_req=True)
         >>> result = thread.get()
 
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
-        :param skip_re_download:
-        :type skip_re_download: bool
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
-        return self.delete_queue_bulk_with_http_info(remove_from_client, blocklist, skip_re_download, queue_bulk_resource, **kwargs)  # noqa: E501
+        return self.get_tag_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_queue_bulk_with_http_info(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_re_download : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
-        """delete_queue_bulk  # noqa: E501
+    def get_tag_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_queue_bulk_with_http_info(remove_from_client, blocklist, skip_re_download, queue_bulk_resource, async_req=True)
+        >>> thread = api.get_tag_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param remove_from_client:
-        :type remove_from_client: bool
-        :param blocklist:
-        :type blocklist: bool
-        :param skip_re_download:
-        :type skip_re_download: bool
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
@@ -271,24 +384,21 @@
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
-            'skip_re_download',
-            'queue_bulk_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -299,59 +409,52 @@
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
-        if _params.get('skip_re_download') is not None:  # noqa: E501
-            _query_params.append(('skipReDownload', _params['skip_re_download']))
 
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
+            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "TagResource",
+        }
 
         return self.api_client.call_api(
-            '/api/v1/queue/bulk', 'DELETE',
+            '/api/v1/tag/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -360,63 +463,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_queue(self, include_unknown_artist_items : Optional[StrictBool] = None, include_artist : Optional[StrictBool] = None, include_album : Optional[StrictBool] = None, **kwargs) -> QueueResourcePagingResource:  # noqa: E501
-        """get_queue  # noqa: E501
+    def list_tag(self, **kwargs) -> List[TagResource]:  # noqa: E501
+        """list_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue(include_unknown_artist_items, include_artist, include_album, async_req=True)
+        >>> thread = api.list_tag(async_req=True)
         >>> result = thread.get()
 
-        :param include_unknown_artist_items:
-        :type include_unknown_artist_items: bool
-        :param include_artist:
-        :type include_artist: bool
-        :param include_album:
-        :type include_album: bool
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
-        return self.get_queue_with_http_info(include_unknown_artist_items, include_artist, include_album, **kwargs)  # noqa: E501
+        return self.list_tag_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_with_http_info(self, include_unknown_artist_items : Optional[StrictBool] = None, include_artist : Optional[StrictBool] = None, include_album : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """get_queue  # noqa: E501
+    def list_tag_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_with_http_info(include_unknown_artist_items, include_artist, include_album, async_req=True)
+        >>> thread = api.list_tag_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param include_unknown_artist_items:
-        :type include_unknown_artist_items: bool
-        :param include_artist:
-        :type include_artist: bool
-        :param include_album:
-        :type include_album: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -430,23 +521,20 @@
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
-            'include_unknown_artist_items',
-            'include_artist',
-            'include_album'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -457,56 +545,50 @@
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
-        if _params.get('include_unknown_artist_items') is not None:  # noqa: E501
-            _query_params.append(('includeUnknownArtistItems', _params['include_unknown_artist_items']))
-        if _params.get('include_artist') is not None:  # noqa: E501
-            _query_params.append(('includeArtist', _params['include_artist']))
-        if _params.get('include_album') is not None:  # noqa: E501
-            _query_params.append(('includeAlbum', _params['include_album']))
 
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
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueResourcePagingResource",
+            '200': "List[TagResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue', 'GET',
+            '/api/v1/tag', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -515,55 +597,59 @@
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
@@ -577,21 +663,22 @@
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
@@ -602,15 +689,15 @@
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
@@ -626,28 +713,37 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['tag_resource']:
+            _body_params = _params['tag_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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
-            '200': "QueueResource",
+            '200': "TagResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/{id}', 'GET',
+            '/api/v1/tag/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/queue_details_api.py` & `lidarr-py-0.3.1/lidarr/api/track_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,47 +13,47 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt, conlist
+from pydantic import StrictInt, conlist
 
 from typing import List, Optional
 
-from lidarr.models.queue_resource import QueueResource
+from lidarr.models.track_resource import TrackResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueDetailsApi(object):
+class TrackApi(object):
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
+    def get_track_by_id(self, id : StrictInt, **kwargs) -> TrackResource:  # noqa: E501
+        """get_track_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_details_by_id(id, async_req=True)
+        >>> thread = api.get_track_by_id(id, async_req=True)
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
+        :rtype: TrackResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_details_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_track_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_details_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_details_by_id  # noqa: E501
+    def get_track_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_track_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_details_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_track_by_id_with_http_info(id, async_req=True)
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
+        :rtype: tuple(TrackResource, status_code(int), headers(HTTPHeaderDict))
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
+                    " to method get_track_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -159,19 +159,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueResource",
+            '200': "TrackResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/details/{id}', 'GET',
+            '/api/v1/track/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,67 +180,67 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_queue_details(self, artist_id : Optional[StrictInt] = None, album_ids : Optional[conlist(StrictInt)] = None, include_artist : Optional[StrictBool] = None, include_album : Optional[StrictBool] = None, **kwargs) -> List[QueueResource]:  # noqa: E501
-        """list_queue_details  # noqa: E501
+    def list_track(self, artist_id : Optional[StrictInt] = None, album_id : Optional[StrictInt] = None, album_release_id : Optional[StrictInt] = None, track_ids : Optional[conlist(StrictInt)] = None, **kwargs) -> List[TrackResource]:  # noqa: E501
+        """list_track  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_queue_details(artist_id, album_ids, include_artist, include_album, async_req=True)
+        >>> thread = api.list_track(artist_id, album_id, album_release_id, track_ids, async_req=True)
         >>> result = thread.get()
 
         :param artist_id:
         :type artist_id: int
-        :param album_ids:
-        :type album_ids: List[int]
-        :param include_artist:
-        :type include_artist: bool
-        :param include_album:
-        :type include_album: bool
+        :param album_id:
+        :type album_id: int
+        :param album_release_id:
+        :type album_release_id: int
+        :param track_ids:
+        :type track_ids: List[int]
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
+        :rtype: List[TrackResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_queue_details_with_http_info(artist_id, album_ids, include_artist, include_album, **kwargs)  # noqa: E501
+        return self.list_track_with_http_info(artist_id, album_id, album_release_id, track_ids, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_queue_details_with_http_info(self, artist_id : Optional[StrictInt] = None, album_ids : Optional[conlist(StrictInt)] = None, include_artist : Optional[StrictBool] = None, include_album : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """list_queue_details  # noqa: E501
+    def list_track_with_http_info(self, artist_id : Optional[StrictInt] = None, album_id : Optional[StrictInt] = None, album_release_id : Optional[StrictInt] = None, track_ids : Optional[conlist(StrictInt)] = None, **kwargs):  # noqa: E501
+        """list_track  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_queue_details_with_http_info(artist_id, album_ids, include_artist, include_album, async_req=True)
+        >>> thread = api.list_track_with_http_info(artist_id, album_id, album_release_id, track_ids, async_req=True)
         >>> result = thread.get()
 
         :param artist_id:
         :type artist_id: int
-        :param album_ids:
-        :type album_ids: List[int]
-        :param include_artist:
-        :type include_artist: bool
-        :param include_album:
-        :type include_album: bool
+        :param album_id:
+        :type album_id: int
+        :param album_release_id:
+        :type album_release_id: int
+        :param track_ids:
+        :type track_ids: List[int]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -254,24 +254,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[QueueResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TrackResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'artist_id',
-            'album_ids',
-            'include_artist',
-            'include_album'
+            'album_id',
+            'album_release_id',
+            'track_ids'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -282,35 +282,35 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_queue_details" % _key
+                    " to method list_track" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
         if _params.get('artist_id') is not None:  # noqa: E501
             _query_params.append(('artistId', _params['artist_id']))
-        if _params.get('album_ids') is not None:  # noqa: E501
-            _query_params.append(('albumIds', _params['album_ids']))
-            _collection_formats['albumIds'] = 'multi'
-        if _params.get('include_artist') is not None:  # noqa: E501
-            _query_params.append(('includeArtist', _params['include_artist']))
-        if _params.get('include_album') is not None:  # noqa: E501
-            _query_params.append(('includeAlbum', _params['include_album']))
+        if _params.get('album_id') is not None:  # noqa: E501
+            _query_params.append(('albumId', _params['album_id']))
+        if _params.get('album_release_id') is not None:  # noqa: E501
+            _query_params.append(('albumReleaseId', _params['album_release_id']))
+        if _params.get('track_ids') is not None:  # noqa: E501
+            _query_params.append(('trackIds', _params['track_ids']))
+            _collection_formats['trackIds'] = 'multi'
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -322,19 +322,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[QueueResource]",
+            '200': "List[TrackResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/details', 'GET',
+            '/api/v1/track', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/queue_status_api.py` & `lidarr-py-0.3.1/lidarr/api/update_log_file_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,75 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import constr, validator
 
-from lidarr.models.queue_status_resource import QueueStatusResource
+from typing import List
+
+from lidarr.models.log_file_resource import LogFileResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "QueueStatusResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/queue/status', 'GET',
+            '/api/v1/log/file/update/{filename}', 'GET',
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
 
@@ -285,25 +281,25 @@
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
-            '200': "QueueStatusResource",
+            '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/status/{id}', 'GET',
+            '/api/v1/log/file/update', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/release_api.py` & `lidarr-py-0.3.1/lidarr/api/ui_config_api.py`

 * *Files 12% similar despite different names*

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
 
-from lidarr.models.release_resource import ReleaseResource
+from lidarr.models.ui_config_resource import UiConfigResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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
-    def create_release(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
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
-        :rtype: ReleaseResource
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
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
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
@@ -148,37 +143,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['release_resource']:
-            _body_params = _params['release_resource']
 
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
-            '200': "ReleaseResource",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release', 'POST',
+            '/api/v1/config/ui', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,21 +173,21 @@
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
@@ -211,27 +197,27 @@
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
@@ -249,15 +235,15 @@
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
@@ -274,15 +260,15 @@
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
@@ -307,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release/{id}', 'GET',
+            '/api/v1/config/ui/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -328,59 +314,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_release(self, album_id : Optional[StrictInt] = None, artist_id : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
-        """list_release  # noqa: E501
+    def update_ui_config(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs) -> UiConfigResource:  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_release(album_id, artist_id, async_req=True)
+        >>> thread = api.update_ui_config(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
-        :param album_id:
-        :type album_id: int
-        :param artist_id:
-        :type artist_id: int
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
-        return self.list_release_with_http_info(album_id, artist_id, **kwargs)  # noqa: E501
+        return self.update_ui_config_with_http_info(id, ui_config_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_release_with_http_info(self, album_id : Optional[StrictInt] = None, artist_id : Optional[StrictInt] = None, **kwargs):  # noqa: E501
-        """list_release  # noqa: E501
+    def update_ui_config_with_http_info(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs):  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_release_with_http_info(album_id, artist_id, async_req=True)
+        >>> thread = api.update_ui_config_with_http_info(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
-        :param album_id:
-        :type album_id: int
-        :param artist_id:
-        :type artist_id: int
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
@@ -394,22 +380,22 @@
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
-            'album_id',
-            'artist_id'
+            'id',
+            'ui_config_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -420,54 +406,61 @@
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
-        if _params.get('album_id') is not None:  # noqa: E501
-            _query_params.append(('albumId', _params['album_id']))
-        if _params.get('artist_id') is not None:  # noqa: E501
-            _query_params.append(('artistId', _params['artist_id']))
 
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
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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
-            '200': "List[ReleaseResource]",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release', 'GET',
+            '/api/v1/config/ui/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/release_profile_api.py` & `lidarr-py-0.3.1/lidarr/api/release_profile_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/release_push_api.py` & `lidarr-py-0.3.1/lidarr/api/release_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,45 +15,45 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
-from typing import Optional
+from typing import List, Optional
 
 from lidarr.models.release_resource import ReleaseResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ReleasePushApi(object):
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
-    def create_release_push(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
-        """create_release_push  # noqa: E501
+    def create_release(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
+        """create_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release_push(release_resource, async_req=True)
+        >>> thread = api.create_release(release_resource, async_req=True)
         >>> result = thread.get()
 
         :param release_resource:
         :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -66,24 +66,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ReleaseResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_release_push_with_http_info(release_resource, **kwargs)  # noqa: E501
+        return self.create_release_with_http_info(release_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_release_push_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
-        """create_release_push  # noqa: E501
+    def create_release_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
+        """create_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release_push_with_http_info(release_resource, async_req=True)
+        >>> thread = api.create_release_with_http_info(release_resource, async_req=True)
         >>> result = thread.get()
 
         :param release_resource:
         :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -126,15 +126,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_release_push" % _key
+                    " to method create_release" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -170,15 +170,15 @@
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release/push', 'POST',
+            '/api/v1/release', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,55 +187,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_release_push_by_id(self, id : StrictInt, **kwargs) -> ReleaseResource:  # noqa: E501
-        """get_release_push_by_id  # noqa: E501
+    def list_release(self, album_id : Optional[StrictInt] = None, artist_id : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
+        """list_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_push_by_id(id, async_req=True)
+        >>> thread = api.list_release(album_id, artist_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param album_id:
+        :type album_id: int
+        :param artist_id:
+        :type artist_id: int
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
+        :rtype: List[ReleaseResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_release_push_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_release_with_http_info(album_id, artist_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_release_push_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_release_push_by_id  # noqa: E501
+    def list_release_with_http_info(self, album_id : Optional[StrictInt] = None, artist_id : Optional[StrictInt] = None, **kwargs):  # noqa: E501
+        """list_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_push_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.list_release_with_http_info(album_id, artist_id, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param album_id:
+        :type album_id: int
+        :param artist_id:
+        :type artist_id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -249,21 +253,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'album_id',
+            'artist_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -274,28 +279,30 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_release_push_by_id" % _key
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
+        if _params.get('album_id') is not None:  # noqa: E501
+            _query_params.append(('albumId', _params['album_id']))
+        if _params.get('artist_id') is not None:  # noqa: E501
+            _query_params.append(('artistId', _params['artist_id']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -307,19 +314,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "List[ReleaseResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release/push/{id}', 'GET',
+            '/api/v1/release', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/remote_path_mapping_api.py` & `lidarr-py-0.3.1/lidarr/api/remote_path_mapping_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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
@@ -570,15 +570,15 @@
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
             '200': "List[RemotePathMappingResource]",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/rename_track_api.py` & `lidarr-py-0.3.1/lidarr/api/rename_track_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/retag_track_api.py` & `lidarr-py-0.3.1/lidarr/api/retag_track_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/root_folder_api.py` & `lidarr-py-0.3.1/lidarr/api/root_folder_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
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
@@ -570,15 +570,15 @@
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
             '200': "List[RootFolderResource]",
         }
```

### Comparing `lidarr-py-0.3.0/lidarr/api/search_api.py` & `lidarr-py-0.3.1/lidarr/api/search_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/static_resource_api.py` & `lidarr-py-0.3.1/lidarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/api/system_api.py` & `lidarr-py-0.3.1/lidarr/api/system_api.py`

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

### Comparing `lidarr-py-0.3.0/lidarr/api/tag_api.py` & `lidarr-py-0.3.1/lidarr/api/queue_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,199 +13,58 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt
 
-from typing import List, Optional
+from typing import Optional
 
-from lidarr.models.tag_resource import TagResource
+from lidarr.models.queue_bulk_resource import QueueBulkResource
+from lidarr.models.queue_resource_paging_resource import QueueResourcePagingResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
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
+    def delete_queue(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_redownload : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
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
-                ['application/json', 'text/json', 'application/*+json']))
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
-            '/api/v1/tag', 'POST',
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
+        >>> thread = api.delete_queue(id, remove_from_client, blocklist, skip_redownload, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
+        :param skip_redownload:
+        :type skip_redownload: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -214,28 +73,34 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_tag_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_queue_with_http_info(id, remove_from_client, blocklist, skip_redownload, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_tag_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_tag  # noqa: E501
+    def delete_queue_with_http_info(self, id : StrictInt, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_redownload : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """delete_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_tag_with_http_info(id, async_req=True)
+        >>> thread = api.delete_queue_with_http_info(id, remove_from_client, blocklist, skip_redownload, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
+        :param skip_redownload:
+        :type skip_redownload: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -255,15 +120,18 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'remove_from_client',
+            'blocklist',
+            'skip_redownload'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -274,28 +142,34 @@
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
+        if _params.get('skip_redownload') is not None:  # noqa: E501
+            _query_params.append(('skipRedownload', _params['skip_redownload']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -305,15 +179,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/tag/{id}', 'DELETE',
+            '/api/v1/queue/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -322,192 +196,67 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_tag_by_id(self, id : StrictInt, **kwargs) -> TagResource:  # noqa: E501
-        """get_tag_by_id  # noqa: E501
+    def delete_queue_bulk(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_redownload : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_queue_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_by_id(id, async_req=True)
+        >>> thread = api.delete_queue_bulk(remove_from_client, blocklist, skip_redownload, queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
+        :param skip_redownload:
+        :type skip_redownload: bool
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
-
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
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_tag_with_http_info(**kwargs)  # noqa: E501
+        return self.delete_queue_bulk_with_http_info(remove_from_client, blocklist, skip_redownload, queue_bulk_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_tag_with_http_info(self, **kwargs):  # noqa: E501
-        """list_tag  # noqa: E501
+    def delete_queue_bulk_with_http_info(self, remove_from_client : Optional[StrictBool] = None, blocklist : Optional[StrictBool] = None, skip_redownload : Optional[StrictBool] = None, queue_bulk_resource : Optional[QueueBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_queue_bulk  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag_with_http_info(async_req=True)
+        >>> thread = api.delete_queue_bulk_with_http_info(remove_from_client, blocklist, skip_redownload, queue_bulk_resource, async_req=True)
         >>> result = thread.get()
 
+        :param remove_from_client:
+        :type remove_from_client: bool
+        :param blocklist:
+        :type blocklist: bool
+        :param skip_redownload:
+        :type skip_redownload: bool
+        :param queue_bulk_resource:
+        :type queue_bulk_resource: QueueBulkResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -521,20 +270,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[TagResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
+            'remove_from_client',
+            'blocklist',
+            'skip_redownload',
+            'queue_bulk_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -545,50 +298,59 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_tag" % _key
+                    " to method delete_queue_bulk" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('remove_from_client') is not None:  # noqa: E501
+            _query_params.append(('removeFromClient', _params['remove_from_client']))
+        if _params.get('blocklist') is not None:  # noqa: E501
+            _query_params.append(('blocklist', _params['blocklist']))
+        if _params.get('skip_redownload') is not None:  # noqa: E501
+            _query_params.append(('skipRedownload', _params['skip_redownload']))
 
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
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "List[TagResource]",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/tag', 'GET',
+            '/api/v1/queue/bulk', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -597,59 +359,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_tag(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs) -> TagResource:  # noqa: E501
-        """update_tag  # noqa: E501
+    def get_queue(self, include_unknown_artist_items : Optional[StrictBool] = None, include_artist : Optional[StrictBool] = None, include_album : Optional[StrictBool] = None, **kwargs) -> QueueResourcePagingResource:  # noqa: E501
+        """get_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_tag(id, tag_resource, async_req=True)
+        >>> thread = api.get_queue(include_unknown_artist_items, include_artist, include_album, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
-        :param tag_resource:
-        :type tag_resource: TagResource
+        :param include_unknown_artist_items:
+        :type include_unknown_artist_items: bool
+        :param include_artist:
+        :type include_artist: bool
+        :param include_album:
+        :type include_album: bool
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
+        :rtype: QueueResourcePagingResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_tag_with_http_info(id, tag_resource, **kwargs)  # noqa: E501
+        return self.get_queue_with_http_info(include_unknown_artist_items, include_artist, include_album, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_tag_with_http_info(self, id : StrictStr, tag_resource : Optional[TagResource] = None, **kwargs):  # noqa: E501
-        """update_tag  # noqa: E501
+    def get_queue_with_http_info(self, include_unknown_artist_items : Optional[StrictBool] = None, include_artist : Optional[StrictBool] = None, include_album : Optional[StrictBool] = None, **kwargs):  # noqa: E501
+        """get_queue  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_tag_with_http_info(id, tag_resource, async_req=True)
+        >>> thread = api.get_queue_with_http_info(include_unknown_artist_items, include_artist, include_album, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: str
-        :param tag_resource:
-        :type tag_resource: TagResource
+        :param include_unknown_artist_items:
+        :type include_unknown_artist_items: bool
+        :param include_artist:
+        :type include_artist: bool
+        :param include_album:
+        :type include_album: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -663,22 +429,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(TagResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(QueueResourcePagingResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'tag_resource'
+            'include_unknown_artist_items',
+            'include_artist',
+            'include_album'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -689,61 +456,56 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_tag" % _key
+                    " to method get_queue" % _key
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
+        if _params.get('include_unknown_artist_items') is not None:  # noqa: E501
+            _query_params.append(('includeUnknownArtistItems', _params['include_unknown_artist_items']))
+        if _params.get('include_artist') is not None:  # noqa: E501
+            _query_params.append(('includeArtist', _params['include_artist']))
+        if _params.get('include_album') is not None:  # noqa: E501
+            _query_params.append(('includeAlbum', _params['include_album']))
 
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
+            '200': "QueueResourcePagingResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag/{id}', 'PUT',
+            '/api/v1/queue', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/tag_details_api.py` & `lidarr-py-0.3.1/lidarr/api/task_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import List
 
-from lidarr.models.tag_details_resource import TagDetailsResource
+from lidarr.models.task_resource import TaskResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class TagDetailsApi(object):
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
-    def get_tag_detail_by_id(self, id : StrictInt, **kwargs) -> TagDetailsResource:  # noqa: E501
-        """get_tag_detail_by_id  # noqa: E501
+    def get_system_task_by_id(self, id : StrictInt, **kwargs) -> TaskResource:  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_detail_by_id(id, async_req=True)
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
-        :rtype: TagDetailsResource
+        :rtype: TaskResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_tag_detail_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_system_task_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_tag_detail_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_tag_detail_by_id  # noqa: E501
+    def get_system_task_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_tag_detail_by_id_with_http_info(id, async_req=True)
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
-        :rtype: tuple(TagDetailsResource, status_code(int), headers(HTTPHeaderDict))
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
-                    " to method get_tag_detail_by_id" % _key
+                    " to method get_system_task_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -159,19 +159,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "TagDetailsResource",
+            '200': "TaskResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag/detail/{id}', 'GET',
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
-    def list_tag_detail(self, **kwargs) -> List[TagDetailsResource]:  # noqa: E501
-        """list_tag_detail  # noqa: E501
+    def list_system_task(self, **kwargs) -> List[TaskResource]:  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag_detail(async_req=True)
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
-        :rtype: List[TagDetailsResource]
+        :rtype: List[TaskResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_tag_detail_with_http_info(**kwargs)  # noqa: E501
+        return self.list_system_task_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_tag_detail_with_http_info(self, **kwargs):  # noqa: E501
-        """list_tag_detail  # noqa: E501
+    def list_system_task_with_http_info(self, **kwargs):  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_tag_detail_with_http_info(async_req=True)
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
-        :rtype: tuple(List[TagDetailsResource], status_code(int), headers(HTTPHeaderDict))
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
-                    " to method list_tag_detail" % _key
+                    " to method list_system_task" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -293,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[TagDetailsResource]",
+            '200': "List[TaskResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/tag/detail', 'GET',
+            '/api/v1/system/task', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api/update_api.py` & `lidarr-py-0.3.1/lidarr/api/health_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,43 +15,43 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from typing import List
 
-from lidarr.models.update_resource import UpdateResource
+from lidarr.models.health_resource import HealthResource
 
 from lidarr.api_client import ApiClient
 from lidarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class UpdateApi(object):
+class HealthApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def list_update(self, **kwargs) -> List[UpdateResource]:  # noqa: E501
-        """list_update  # noqa: E501
+    def list_health(self, **kwargs) -> List[HealthResource]:  # noqa: E501
+        """list_health  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_update(async_req=True)
+        >>> thread = api.list_health(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -59,27 +59,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[UpdateResource]
+        :rtype: List[HealthResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_update_with_http_info(**kwargs)  # noqa: E501
+        return self.list_health_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_update_with_http_info(self, **kwargs):  # noqa: E501
-        """list_update  # noqa: E501
+    def list_health_with_http_info(self, **kwargs):  # noqa: E501
+        """list_health  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_update_with_http_info(async_req=True)
+        >>> thread = api.list_health_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -95,15 +95,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[UpdateResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[HealthResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -119,15 +119,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_update" % _key
+                    " to method list_health" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -144,25 +144,25 @@
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
-            '200': "List[UpdateResource]",
+            '200': "List[HealthResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/update', 'GET',
+            '/api/v1/health', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `lidarr-py-0.3.0/lidarr/api_client.py` & `lidarr-py-0.3.1/lidarr/api_client.py`

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
-        self.user_agent = 'lidarr-py/v0.3.0'
+        self.user_agent = 'lidarr-py/v0.3.1'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `lidarr-py-0.3.0/lidarr/api_response.py` & `lidarr-py-0.3.1/lidarr/api_response.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/configuration.py` & `lidarr-py-0.3.1/lidarr/configuration.py`

 * *Files 0% similar despite different names*

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
                "Version of the API: 1.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `lidarr-py-0.3.0/lidarr/exceptions.py` & `lidarr-py-0.3.1/lidarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/__init__.py` & `lidarr-py-0.3.1/lidarr/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,35 +58,39 @@
 from lidarr.models.custom_filter_resource import CustomFilterResource
 from lidarr.models.custom_format import CustomFormat
 from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from lidarr.models.database_type import DatabaseType
 from lidarr.models.delay_profile_resource import DelayProfileResource
 from lidarr.models.disk_space_resource import DiskSpaceResource
+from lidarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from lidarr.models.download_client_config_resource import DownloadClientConfigResource
 from lidarr.models.download_client_resource import DownloadClientResource
 from lidarr.models.download_protocol import DownloadProtocol
 from lidarr.models.entity_history_event_type import EntityHistoryEventType
 from lidarr.models.field import Field
 from lidarr.models.file_date_type import FileDateType
 from lidarr.models.health_check_result import HealthCheckResult
 from lidarr.models.health_resource import HealthResource
 from lidarr.models.history_resource import HistoryResource
 from lidarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from lidarr.models.host_config_resource import HostConfigResource
 from lidarr.models.i_custom_format_specification import ICustomFormatSpecification
+from lidarr.models.import_list_bulk_resource import ImportListBulkResource
 from lidarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from lidarr.models.import_list_monitor_type import ImportListMonitorType
 from lidarr.models.import_list_resource import ImportListResource
 from lidarr.models.import_list_type import ImportListType
+from lidarr.models.indexer_bulk_resource import IndexerBulkResource
 from lidarr.models.indexer_config_resource import IndexerConfigResource
 from lidarr.models.indexer_resource import IndexerResource
 from lidarr.models.iso_country import IsoCountry
 from lidarr.models.language_resource import LanguageResource
 from lidarr.models.links import Links
+from lidarr.models.localization_resource import LocalizationResource
 from lidarr.models.log_file_resource import LogFileResource
 from lidarr.models.log_resource import LogResource
 from lidarr.models.log_resource_paging_resource import LogResourcePagingResource
 from lidarr.models.manual_import_resource import ManualImportResource
 from lidarr.models.manual_import_update_resource import ManualImportUpdateResource
 from lidarr.models.media_cover import MediaCover
 from lidarr.models.media_cover_types import MediaCoverTypes
```

### Comparing `lidarr-py-0.3.0/lidarr/models/add_album_options.py` & `lidarr-py-0.3.1/lidarr/models/add_album_options.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/add_artist_options.py` & `lidarr-py-0.3.1/lidarr/models/add_artist_options.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album.py` & `lidarr-py-0.3.1/lidarr/models/album.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_add_type.py` & `lidarr-py-0.3.1/lidarr/models/album_add_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/album_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_list_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/album_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_release.py` & `lidarr-py-0.3.1/lidarr/models/album_release.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_release_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/album_release_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_release_list_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/album_release_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_release_resource.py` & `lidarr-py-0.3.1/lidarr/models/album_release_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_resource.py` & `lidarr-py-0.3.1/lidarr/models/album_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_resource_paging_resource.py` & `lidarr-py-0.3.1/lidarr/models/album_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_statistics_resource.py` & `lidarr-py-0.3.1/lidarr/models/album_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_studio_artist_resource.py` & `lidarr-py-0.3.1/lidarr/models/album_studio_artist_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/album_studio_resource.py` & `lidarr-py-0.3.1/lidarr/models/album_studio_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/albums_monitored_resource.py` & `lidarr-py-0.3.1/lidarr/models/albums_monitored_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/allow_fingerprinting.py` & `lidarr-py-0.3.1/lidarr/models/allow_fingerprinting.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/apply_tags.py` & `lidarr-py-0.3.1/lidarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist.py` & `lidarr-py-0.3.1/lidarr/models/artist.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_editor_resource.py` & `lidarr-py-0.3.1/lidarr/models/artist_editor_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/artist_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_metadata.py` & `lidarr-py-0.3.1/lidarr/models/artist_metadata.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_metadata_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/artist_metadata_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_resource.py` & `lidarr-py-0.3.1/lidarr/models/artist_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_statistics_resource.py` & `lidarr-py-0.3.1/lidarr/models/artist_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_status_type.py` & `lidarr-py-0.3.1/lidarr/models/artist_status_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/artist_title_info.py` & `lidarr-py-0.3.1/lidarr/models/artist_title_info.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/authentication_type.py` & `lidarr-py-0.3.1/lidarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/backup_resource.py` & `lidarr-py-0.3.1/lidarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/backup_type.py` & `lidarr-py-0.3.1/lidarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/blocklist_bulk_resource.py` & `lidarr-py-0.3.1/lidarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/blocklist_resource.py` & `lidarr-py-0.3.1/lidarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/blocklist_resource_paging_resource.py` & `lidarr-py-0.3.1/lidarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/certificate_validation_type.py` & `lidarr-py-0.3.1/lidarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/command.py` & `lidarr-py-0.3.1/lidarr/models/command.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/command_priority.py` & `lidarr-py-0.3.1/lidarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/command_resource.py` & `lidarr-py-0.3.1/lidarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/command_result.py` & `lidarr-py-0.3.1/lidarr/models/command_result.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/command_status.py` & `lidarr-py-0.3.1/lidarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/command_trigger.py` & `lidarr-py-0.3.1/lidarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/custom_filter_resource.py` & `lidarr-py-0.3.1/lidarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/custom_format.py` & `lidarr-py-0.3.1/lidarr/models/custom_format.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/custom_format_resource.py` & `lidarr-py-0.3.1/lidarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/custom_format_specification_schema.py` & `lidarr-py-0.3.1/lidarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/database_type.py` & `lidarr-py-0.3.1/lidarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/delay_profile_resource.py` & `lidarr-py-0.3.1/lidarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/disk_space_resource.py` & `lidarr-py-0.3.1/lidarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/download_client_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/download_client_resource.py` & `lidarr-py-0.3.1/lidarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/download_protocol.py` & `lidarr-py-0.3.1/lidarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/entity_history_event_type.py` & `lidarr-py-0.3.1/lidarr/models/entity_history_event_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/field.py` & `lidarr-py-0.3.1/lidarr/models/field.py`

 * *Files 5% similar despite different names*

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

### Comparing `lidarr-py-0.3.0/lidarr/models/file_date_type.py` & `lidarr-py-0.3.1/lidarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/health_check_result.py` & `lidarr-py-0.3.1/lidarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/health_resource.py` & `lidarr-py-0.3.1/lidarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/history_resource.py` & `lidarr-py-0.3.1/lidarr/models/history_resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,23 +35,24 @@
     id: Optional[int]
     album_id: Optional[int]
     artist_id: Optional[int]
     track_id: Optional[int]
     source_title: Optional[str]
     quality: Optional[QualityModel]
     custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     quality_cutoff_not_met: Optional[bool]
     var_date: Optional[datetime]
     download_id: Optional[str]
     event_type: Optional[EntityHistoryEventType]
     data: Optional[Dict]
     album: Optional[AlbumResource]
     artist: Optional[ArtistResource]
     track: Optional[TrackResource]
-    __properties = ["id", "albumId", "artistId", "trackId", "sourceTitle", "quality", "customFormats", "qualityCutoffNotMet", "date", "downloadId", "eventType", "data", "album", "artist", "track"]
+    __properties = ["id", "albumId", "artistId", "trackId", "sourceTitle", "quality", "customFormats", "customFormatScore", "qualityCutoffNotMet", "date", "downloadId", "eventType", "data", "album", "artist", "track"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -126,14 +127,15 @@
             "id": obj.get("id"),
             "album_id": obj.get("albumId"),
             "artist_id": obj.get("artistId"),
             "track_id": obj.get("trackId"),
             "source_title": obj.get("sourceTitle"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "quality_cutoff_not_met": obj.get("qualityCutoffNotMet"),
             "var_date": obj.get("date"),
             "download_id": obj.get("downloadId"),
             "event_type": obj.get("eventType"),
             "data": obj.get("data"),
             "album": AlbumResource.from_dict(obj.get("album")) if obj.get("album") is not None else None,
             "artist": ArtistResource.from_dict(obj.get("artist")) if obj.get("artist") is not None else None,
```

### Comparing `lidarr-py-0.3.0/lidarr/models/history_resource_paging_resource.py` & `lidarr-py-0.3.1/lidarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/host_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/i_custom_format_specification.py` & `lidarr-py-0.3.1/lidarr/models/i_custom_format_specification.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/import_list_exclusion_resource.py` & `lidarr-py-0.3.1/lidarr/models/import_list_exclusion_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/import_list_monitor_type.py` & `lidarr-py-0.3.1/lidarr/models/import_list_monitor_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/import_list_resource.py` & `lidarr-py-0.3.1/lidarr/models/import_list_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,16 @@
     should_search: Optional[bool]
     root_folder_path: Optional[str]
     monitor_new_items: Optional[NewItemMonitorTypes]
     quality_profile_id: Optional[int]
     metadata_profile_id: Optional[int]
     list_type: Optional[ImportListType]
     list_order: Optional[int]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enableAutomaticAdd", "shouldMonitor", "shouldMonitorExisting", "shouldSearch", "rootFolderPath", "monitorNewItems", "qualityProfileId", "metadataProfileId", "listType", "listOrder"]
+    min_refresh_interval: Optional[str]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enableAutomaticAdd", "shouldMonitor", "shouldMonitorExisting", "shouldSearch", "rootFolderPath", "monitorNewItems", "qualityProfileId", "metadataProfileId", "listType", "listOrder", "minRefreshInterval"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -160,11 +161,12 @@
             "should_monitor_existing": obj.get("shouldMonitorExisting"),
             "should_search": obj.get("shouldSearch"),
             "root_folder_path": obj.get("rootFolderPath"),
             "monitor_new_items": obj.get("monitorNewItems"),
             "quality_profile_id": obj.get("qualityProfileId"),
             "metadata_profile_id": obj.get("metadataProfileId"),
             "list_type": obj.get("listType"),
-            "list_order": obj.get("listOrder")
+            "list_order": obj.get("listOrder"),
+            "min_refresh_interval": obj.get("minRefreshInterval")
         })
         return _obj
```

### Comparing `lidarr-py-0.3.0/lidarr/models/import_list_type.py` & `lidarr-py-0.3.1/lidarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/indexer_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/indexer_resource.py` & `lidarr-py-0.3.1/lidarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/iso_country.py` & `lidarr-py-0.3.1/lidarr/models/iso_country.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/language_resource.py` & `lidarr-py-0.3.1/lidarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/links.py` & `lidarr-py-0.3.1/lidarr/models/links.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/log_file_resource.py` & `lidarr-py-0.3.1/lidarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/log_resource.py` & `lidarr-py-0.3.1/lidarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/log_resource_paging_resource.py` & `lidarr-py-0.3.1/lidarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/manual_import_resource.py` & `lidarr-py-0.3.1/lidarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/manual_import_update_resource.py` & `lidarr-py-0.3.1/lidarr/models/manual_import_update_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/media_cover.py` & `lidarr-py-0.3.1/lidarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/media_cover_types.py` & `lidarr-py-0.3.1/lidarr/models/media_cover_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/media_info_model.py` & `lidarr-py-0.3.1/lidarr/models/media_info_model.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/media_info_resource.py` & `lidarr-py-0.3.1/lidarr/models/media_info_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/media_management_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/media_management_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/medium.py` & `lidarr-py-0.3.1/lidarr/models/medium.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/medium_resource.py` & `lidarr-py-0.3.1/lidarr/models/medium_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/member.py` & `lidarr-py-0.3.1/lidarr/models/member.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/metadata_profile.py` & `lidarr-py-0.3.1/lidarr/models/metadata_profile.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/metadata_profile_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/metadata_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/metadata_profile_resource.py` & `lidarr-py-0.3.1/lidarr/models/metadata_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/metadata_provider_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/metadata_provider_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/metadata_resource.py` & `lidarr-py-0.3.1/lidarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/monitor_types.py` & `lidarr-py-0.3.1/lidarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/monitoring_options.py` & `lidarr-py-0.3.1/lidarr/models/monitoring_options.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/naming_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/naming_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/new_item_monitor_types.py` & `lidarr-py-0.3.1/lidarr/models/new_item_monitor_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/notification_resource.py` & `lidarr-py-0.3.1/lidarr/models/notification_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/paging_resource_filter.py` & `lidarr-py-0.3.1/lidarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/parse_resource.py` & `lidarr-py-0.3.1/lidarr/models/parse_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/parsed_album_info.py` & `lidarr-py-0.3.1/lidarr/models/parsed_album_info.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/parsed_track_info.py` & `lidarr-py-0.3.1/lidarr/models/parsed_track_info.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/ping_resource.py` & `lidarr-py-0.3.1/lidarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/primary_album_type.py` & `lidarr-py-0.3.1/lidarr/models/primary_album_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_format_item.py` & `lidarr-py-0.3.1/lidarr/models/profile_format_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_format_item_resource.py` & `lidarr-py-0.3.1/lidarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item.py` & `lidarr-py-0.3.1/lidarr/models/profile_primary_album_type_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_primary_album_type_item_resource.py` & `lidarr-py-0.3.1/lidarr/models/profile_primary_album_type_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_release_status_item.py` & `lidarr-py-0.3.1/lidarr/models/profile_release_status_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_release_status_item_resource.py` & `lidarr-py-0.3.1/lidarr/models/profile_release_status_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item.py` & `lidarr-py-0.3.1/lidarr/models/profile_secondary_album_type_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/profile_secondary_album_type_item_resource.py` & `lidarr-py-0.3.1/lidarr/models/profile_secondary_album_type_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/proper_download_types.py` & `lidarr-py-0.3.1/lidarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/provider_message.py` & `lidarr-py-0.3.1/lidarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/provider_message_type.py` & `lidarr-py-0.3.1/lidarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/proxy_type.py` & `lidarr-py-0.3.1/lidarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality.py` & `lidarr-py-0.3.1/lidarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_definition_resource.py` & `lidarr-py-0.3.1/lidarr/models/quality_definition_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_model.py` & `lidarr-py-0.3.1/lidarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_profile.py` & `lidarr-py-0.3.1/lidarr/models/quality_profile.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_profile_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/quality_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item.py` & `lidarr-py-0.3.1/lidarr/models/quality_profile_quality_item.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_profile_quality_item_resource.py` & `lidarr-py-0.3.1/lidarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/quality_profile_resource.py` & `lidarr-py-0.3.1/lidarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/queue_bulk_resource.py` & `lidarr-py-0.3.1/lidarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/queue_resource.py` & `lidarr-py-0.3.1/lidarr/models/queue_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     id: Optional[int]
     artist_id: Optional[int]
     album_id: Optional[int]
     artist: Optional[ArtistResource]
     album: Optional[AlbumResource]
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
@@ -53,15 +54,15 @@
     error_message: Optional[str]
     download_id: Optional[str]
     protocol: Optional[DownloadProtocol]
     download_client: Optional[str]
     indexer: Optional[str]
     output_path: Optional[str]
     download_forced: Optional[bool]
-    __properties = ["id", "artistId", "albumId", "artist", "album", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "downloadForced"]
+    __properties = ["id", "artistId", "albumId", "artist", "album", "quality", "customFormats", "customFormatScore", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "downloadForced"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -172,14 +173,15 @@
             "id": obj.get("id"),
             "artist_id": obj.get("artistId"),
             "album_id": obj.get("albumId"),
             "artist": ArtistResource.from_dict(obj.get("artist")) if obj.get("artist") is not None else None,
             "album": AlbumResource.from_dict(obj.get("album")) if obj.get("album") is not None else None,
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

### Comparing `lidarr-py-0.3.0/lidarr/models/queue_resource_paging_resource.py` & `lidarr-py-0.3.1/lidarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/queue_status_resource.py` & `lidarr-py-0.3.1/lidarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/ratings.py` & `lidarr-py-0.3.1/lidarr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/rejection.py` & `lidarr-py-0.3.1/lidarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/rejection_type.py` & `lidarr-py-0.3.1/lidarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/release_profile_resource.py` & `lidarr-py-0.3.1/lidarr/models/release_profile_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/release_resource.py` & `lidarr-py-0.3.1/lidarr/models/release_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/release_status.py` & `lidarr-py-0.3.1/lidarr/models/release_status.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/remote_path_mapping_resource.py` & `lidarr-py-0.3.1/lidarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/rename_track_resource.py` & `lidarr-py-0.3.1/lidarr/models/rename_track_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/rescan_after_refresh_type.py` & `lidarr-py-0.3.1/lidarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/retag_track_resource.py` & `lidarr-py-0.3.1/lidarr/models/retag_track_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/revision.py` & `lidarr-py-0.3.1/lidarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/root_folder_resource.py` & `lidarr-py-0.3.1/lidarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/runtime_mode.py` & `lidarr-py-0.3.1/lidarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/secondary_album_type.py` & `lidarr-py-0.3.1/lidarr/models/secondary_album_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/select_option.py` & `lidarr-py-0.3.1/lidarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/sort_direction.py` & `lidarr-py-0.3.1/lidarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/system_resource.py` & `lidarr-py-0.3.1/lidarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/tag_details_resource.py` & `lidarr-py-0.3.1/lidarr/models/tag_details_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     """
     id: Optional[int]
     label: Optional[str]
     delay_profile_ids: Optional[List]
     import_list_ids: Optional[List]
     notification_ids: Optional[List]
     restriction_ids: Optional[List]
-    indexer_ids: Optional[List]
     artist_ids: Optional[List]
-    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "indexerIds", "artistIds"]
+    indexer_ids: Optional[List]
+    download_client_ids: Optional[List]
+    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "artistIds", "indexerIds", "downloadClientIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -79,21 +80,25 @@
         if self.notification_ids is None:
             _dict['notificationIds'] = None
 
         # set to None if restriction_ids (nullable) is None
         if self.restriction_ids is None:
             _dict['restrictionIds'] = None
 
+        # set to None if artist_ids (nullable) is None
+        if self.artist_ids is None:
+            _dict['artistIds'] = None
+
         # set to None if indexer_ids (nullable) is None
         if self.indexer_ids is None:
             _dict['indexerIds'] = None
 
-        # set to None if artist_ids (nullable) is None
-        if self.artist_ids is None:
-            _dict['artistIds'] = None
+        # set to None if download_client_ids (nullable) is None
+        if self.download_client_ids is None:
+            _dict['downloadClientIds'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> TagDetailsResource:
         """Create an instance of TagDetailsResource from a dict"""
         if obj is None:
@@ -105,12 +110,13 @@
         _obj = TagDetailsResource.parse_obj({
             "id": obj.get("id"),
             "label": obj.get("label"),
             "delay_profile_ids": obj.get("delayProfileIds"),
             "import_list_ids": obj.get("importListIds"),
             "notification_ids": obj.get("notificationIds"),
             "restriction_ids": obj.get("restrictionIds"),
+            "artist_ids": obj.get("artistIds"),
             "indexer_ids": obj.get("indexerIds"),
-            "artist_ids": obj.get("artistIds")
+            "download_client_ids": obj.get("downloadClientIds")
         })
         return _obj
```

### Comparing `lidarr-py-0.3.0/lidarr/models/tag_difference.py` & `lidarr-py-0.3.1/lidarr/models/tag_difference.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/tag_resource.py` & `lidarr-py-0.3.1/lidarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/task_resource.py` & `lidarr-py-0.3.1/lidarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/track.py` & `lidarr-py-0.3.1/lidarr/models/track.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/track_file.py` & `lidarr-py-0.3.1/lidarr/models/track_file.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/track_file_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/track_file_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/track_file_list_resource.py` & `lidarr-py-0.3.1/lidarr/models/track_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/track_file_resource.py` & `lidarr-py-0.3.1/lidarr/models/track_file_resource.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
-from typing import Optional
+from typing import List, Optional
 from pydantic import BaseModel
+from lidarr.models.custom_format_resource import CustomFormatResource
 from lidarr.models.media_info_resource import MediaInfoResource
 from lidarr.models.parsed_track_info import ParsedTrackInfo
 from lidarr.models.quality_model import QualityModel
 
 class TrackFileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -35,18 +36,20 @@
     path: Optional[str]
     size: Optional[int]
     date_added: Optional[datetime]
     scene_name: Optional[str]
     release_group: Optional[str]
     quality: Optional[QualityModel]
     quality_weight: Optional[int]
+    custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     media_info: Optional[MediaInfoResource]
     quality_cutoff_not_met: Optional[bool]
     audio_tags: Optional[ParsedTrackInfo]
-    __properties = ["id", "artistId", "albumId", "path", "size", "dateAdded", "sceneName", "releaseGroup", "quality", "qualityWeight", "mediaInfo", "qualityCutoffNotMet", "audioTags"]
+    __properties = ["id", "artistId", "albumId", "path", "size", "dateAdded", "sceneName", "releaseGroup", "quality", "qualityWeight", "customFormats", "customFormatScore", "mediaInfo", "qualityCutoffNotMet", "audioTags"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -70,14 +73,21 @@
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         # override the default output from pydantic by calling `to_dict()` of quality
         if self.quality:
             _dict['quality'] = self.quality.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in custom_formats (list)
+        _items = []
+        if self.custom_formats:
+            for _item in self.custom_formats:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['customFormats'] = _items
         # override the default output from pydantic by calling `to_dict()` of media_info
         if self.media_info:
             _dict['mediaInfo'] = self.media_info.to_dict()
         # override the default output from pydantic by calling `to_dict()` of audio_tags
         if self.audio_tags:
             _dict['audioTags'] = self.audio_tags.to_dict()
         # set to None if path (nullable) is None
@@ -88,14 +98,18 @@
         if self.scene_name is None:
             _dict['sceneName'] = None
 
         # set to None if release_group (nullable) is None
         if self.release_group is None:
             _dict['releaseGroup'] = None
 
+        # set to None if custom_formats (nullable) is None
+        if self.custom_formats is None:
+            _dict['customFormats'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> TrackFileResource:
         """Create an instance of TrackFileResource from a dict"""
         if obj is None:
             return None
@@ -110,13 +124,15 @@
             "path": obj.get("path"),
             "size": obj.get("size"),
             "date_added": obj.get("dateAdded"),
             "scene_name": obj.get("sceneName"),
             "release_group": obj.get("releaseGroup"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "quality_weight": obj.get("qualityWeight"),
+            "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "media_info": MediaInfoResource.from_dict(obj.get("mediaInfo")) if obj.get("mediaInfo") is not None else None,
             "quality_cutoff_not_met": obj.get("qualityCutoffNotMet"),
             "audio_tags": ParsedTrackInfo.from_dict(obj.get("audioTags")) if obj.get("audioTags") is not None else None
         })
         return _obj
```

### Comparing `lidarr-py-0.3.0/lidarr/models/track_list_lazy_loaded.py` & `lidarr-py-0.3.1/lidarr/models/track_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/track_resource.py` & `lidarr-py-0.3.1/lidarr/models/track_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/tracked_download_state.py` & `lidarr-py-0.3.1/lidarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/tracked_download_status.py` & `lidarr-py-0.3.1/lidarr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/tracked_download_status_message.py` & `lidarr-py-0.3.1/lidarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/ui_config_resource.py` & `lidarr-py-0.3.1/lidarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/update_changes.py` & `lidarr-py-0.3.1/lidarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/update_mechanism.py` & `lidarr-py-0.3.1/lidarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/update_resource.py` & `lidarr-py-0.3.1/lidarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/models/write_audio_tags_type.py` & `lidarr-py-0.3.1/lidarr/models/write_audio_tags_type.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr/rest.py` & `lidarr-py-0.3.1/lidarr/rest.py`

 * *Files identical despite different names*

### Comparing `lidarr-py-0.3.0/lidarr_py.egg-info/PKG-INFO` & `lidarr-py-0.3.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: lidarr-py
-Version: 0.3.0
-Summary: Lidarr API wrapper
-Project-URL: Homepage, https://github.com/devopsarr/lidarr-py
-Project-URL: Bug Tracker, https://github.com/devopsarr/lidarr-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # lidarr-py
 Lidarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.3.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -166,55 +153,60 @@
 *DelayProfileApi* | [**list_delay_profile**](docs/DelayProfileApi.md#list_delay_profile) | **GET** /api/v1/delayprofile | 
 *DelayProfileApi* | [**update_delay_profile**](docs/DelayProfileApi.md#update_delay_profile) | **PUT** /api/v1/delayprofile/{id} | 
 *DelayProfileApi* | [**update_delay_profile_reorder**](docs/DelayProfileApi.md#update_delay_profile_reorder) | **PUT** /api/v1/delayprofile/reorder/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v1/diskspace | 
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
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_artist**](docs/HistoryApi.md#list_history_artist) | **GET** /api/v1/history/artist | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v1/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v1/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v1/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v1/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v1/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v1/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v1/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v1/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v1/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v1/importlist/{id} | 
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v1/importlistexclusion/{id} | 
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
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v1/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v1/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v1/config/indexer/{id} | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
@@ -275,31 +267,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v1/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v1/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v1/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v1/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v1/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v1/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v1/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v1/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v1/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v1/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v1/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v1/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v1/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v1/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v1/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v1/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v1/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v1/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v1/remotepathmapping/{id} | 
 *RenameTrackApi* | [**list_rename**](docs/RenameTrackApi.md#list_rename) | **GET** /api/v1/rename | 
 *RetagTrackApi* | [**list_retag**](docs/RetagTrackApi.md#list_retag) | **GET** /api/v1/retag | 
@@ -388,35 +375,39 @@
  - [CustomFilterResource](docs/CustomFilterResource.md)
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [EntityHistoryEventType](docs/EntityHistoryEventType.md)
  - [Field](docs/Field.md)
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
+ - [LocalizationResource](docs/LocalizationResource.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
  - [LogResourcePagingResource](docs/LogResourcePagingResource.md)
  - [ManualImportResource](docs/ManualImportResource.md)
  - [ManualImportUpdateResource](docs/ManualImportUpdateResource.md)
  - [MediaCover](docs/MediaCover.md)
  - [MediaCoverTypes](docs/MediaCoverTypes.md)
```

### Comparing `lidarr-py-0.3.0/lidarr_py.egg-info/SOURCES.txt` & `lidarr-py-0.3.1/lidarr_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -123,35 +123,39 @@
 lidarr/models/custom_filter_resource.py
 lidarr/models/custom_format.py
 lidarr/models/custom_format_resource.py
 lidarr/models/custom_format_specification_schema.py
 lidarr/models/database_type.py
 lidarr/models/delay_profile_resource.py
 lidarr/models/disk_space_resource.py
+lidarr/models/download_client_bulk_resource.py
 lidarr/models/download_client_config_resource.py
 lidarr/models/download_client_resource.py
 lidarr/models/download_protocol.py
 lidarr/models/entity_history_event_type.py
 lidarr/models/field.py
 lidarr/models/file_date_type.py
 lidarr/models/health_check_result.py
 lidarr/models/health_resource.py
 lidarr/models/history_resource.py
 lidarr/models/history_resource_paging_resource.py
 lidarr/models/host_config_resource.py
 lidarr/models/i_custom_format_specification.py
+lidarr/models/import_list_bulk_resource.py
 lidarr/models/import_list_exclusion_resource.py
 lidarr/models/import_list_monitor_type.py
 lidarr/models/import_list_resource.py
 lidarr/models/import_list_type.py
+lidarr/models/indexer_bulk_resource.py
 lidarr/models/indexer_config_resource.py
 lidarr/models/indexer_resource.py
 lidarr/models/iso_country.py
 lidarr/models/language_resource.py
 lidarr/models/links.py
+lidarr/models/localization_resource.py
 lidarr/models/log_file_resource.py
 lidarr/models/log_resource.py
 lidarr/models/log_resource_paging_resource.py
 lidarr/models/manual_import_resource.py
 lidarr/models/manual_import_update_resource.py
 lidarr/models/media_cover.py
 lidarr/models/media_cover_types.py
```

### Comparing `lidarr-py-0.3.0/pyproject.toml` & `lidarr-py-0.3.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 [project]
 name = "lidarr-py"
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
 description = "Lidarr API wrapper"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

