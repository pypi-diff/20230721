# Comparing `tmp/readarr-py-0.4.0.tar.gz` & `tmp/readarr-py-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readarr-py-0.4.0.tar", last modified: Mon Jul 17 13:06:13 2023, max compression
+gzip compressed data, was "readarr-py-0.4.1.tar", last modified: Fri Jul 21 11:35:17 2023, max compression
```

## Comparing `readarr-py-0.4.0.tar` & `readarr-py-0.4.1.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.640531 readarr-py-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 13:05:58.000000 readarr-py-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40875 2023-07-17 13:06:13.640531 readarr-py-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40399 2023-07-17 13:05:58.000000 readarr-py-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-17 13:05:58.000000 readarr-py-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.588531 readarr-py-0.4.0/readarr/
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.604531 readarr-py-0.4.0/readarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31205 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/author_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/author_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/author_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    43863 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37656 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/bookshelf_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30424 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35492 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36232 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/development_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    67048 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/edition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    66152 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    65318 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53261 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_provider_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29962 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53933 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25206 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30616 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30616 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30969 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/rename_book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/retag_book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30232 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29647 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.636531 readarr-py-0.4.0/readarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/add_author_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/add_book_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/allow_fingerprinting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_metadata_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_add_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/books_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/bookshelf_author_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/bookshelf_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/development_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_client_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/entity_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/i_custom_format_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/indexer_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/iso_country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/manual_import_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_provider_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/new_item_monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/parsed_book_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/parsed_track_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/profile_format_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_quality_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rename_book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/retag_book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_book_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_book_link_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_book_link_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tag_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/write_audio_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/write_book_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.640531 readarr-py-0.4.0/readarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40875 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:06:13.640531 readarr-py-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 13:05:58.000000 readarr-py-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:17.277190 readarr-py-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-21 11:34:58.000000 readarr-py-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40875 2023-07-21 11:35:17.277190 readarr-py-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40399 2023-07-21 11:34:58.000000 readarr-py-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:34:58.000000 readarr-py-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:17.209190 readarr-py-0.4.1/readarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:17.229189 readarr-py-0.4.1/readarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31205 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/author_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/author_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/author_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43863 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/book_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37656 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/book_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/book_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/bookshelf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30424 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35492 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36232 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/development_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67048 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/edition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66152 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65318 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53261 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/metadata_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/metadata_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/metadata_provider_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29962 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53933 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25206 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30616 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30616 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30969 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/rename_book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/retag_book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30232 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29647 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:17.273189 readarr-py-0.4.1/readarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/add_author_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/add_book_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/allow_fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_metadata_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/author_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_add_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_file_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/book_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/books_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/bookshelf_author_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/bookshelf_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/development_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/edition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/edition_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/edition_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/edition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/entity_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/i_custom_format_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/import_list_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/import_list_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/iso_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/manual_import_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/media_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/metadata_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/metadata_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/metadata_provider_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/new_item_monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/parsed_book_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/parsed_track_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/profile_format_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_profile_quality_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/rename_book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/retag_book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series_book_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series_book_link_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series_book_link_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/tag_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/write_audio_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/models/write_book_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-21 11:34:58.000000 readarr-py-0.4.1/readarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:35:17.273189 readarr-py-0.4.1/readarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40875 2023-07-21 11:35:17.000000 readarr-py-0.4.1/readarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-21 11:35:17.000000 readarr-py-0.4.1/readarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:35:17.000000 readarr-py-0.4.1/readarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-21 11:35:17.000000 readarr-py-0.4.1/readarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 11:35:17.000000 readarr-py-0.4.1/readarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:35:17.277190 readarr-py-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-21 11:34:58.000000 readarr-py-0.4.1/setup.py
```

### Comparing `readarr-py-0.4.0/LICENSE` & `readarr-py-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/PKG-INFO` & `readarr-py-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readarr-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Readarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/readarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.4.0
+- Package version: 0.4.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
```

### Comparing `readarr-py-0.4.0/README.md` & `readarr-py-0.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.4.0
+- Package version: 0.4.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
```

### Comparing `readarr-py-0.4.0/pyproject.toml` & `readarr-py-0.4.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # coding: utf-8
 
 [project]
 name = "readarr-py"
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
 description = "Readarr API wrapper"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `readarr-py-0.4.0/readarr/__init__.py` & `readarr-py-0.4.1/readarr/__init__.py`

 * *Files 0% similar despite different names*

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
 from readarr.api.api_info_api import ApiInfoApi
 from readarr.api.authentication_api import AuthenticationApi
 from readarr.api.author_api import AuthorApi
 from readarr.api.author_editor_api import AuthorEditorApi
```

### Comparing `readarr-py-0.4.0/readarr/api/__init__.py` & `readarr-py-0.4.1/readarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/api_info_api.py` & `readarr-py-0.4.1/readarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/authentication_api.py` & `readarr-py-0.4.1/readarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/author_api.py` & `readarr-py-0.4.1/readarr/api/author_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/author_editor_api.py` & `readarr-py-0.4.1/readarr/api/author_editor_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/author_lookup_api.py` & `readarr-py-0.4.1/readarr/api/author_lookup_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/backup_api.py` & `readarr-py-0.4.1/readarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/blocklist_api.py` & `readarr-py-0.4.1/readarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/book_api.py` & `readarr-py-0.4.1/readarr/api/book_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/book_editor_api.py` & `readarr-py-0.4.1/readarr/api/book_editor_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/book_file_api.py` & `readarr-py-0.4.1/readarr/api/book_file_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/book_lookup_api.py` & `readarr-py-0.4.1/readarr/api/book_lookup_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/bookshelf_api.py` & `readarr-py-0.4.1/readarr/api/bookshelf_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/calendar_api.py` & `readarr-py-0.4.1/readarr/api/calendar_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/calendar_feed_api.py` & `readarr-py-0.4.1/readarr/api/calendar_feed_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/command_api.py` & `readarr-py-0.4.1/readarr/api/command_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/custom_filter_api.py` & `readarr-py-0.4.1/readarr/api/custom_filter_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/custom_format_api.py` & `readarr-py-0.4.1/readarr/api/custom_format_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/cutoff_api.py` & `readarr-py-0.4.1/readarr/api/cutoff_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/delay_profile_api.py` & `readarr-py-0.4.1/readarr/api/delay_profile_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/development_config_api.py` & `readarr-py-0.4.1/readarr/api/development_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/disk_space_api.py` & `readarr-py-0.4.1/readarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/download_client_api.py` & `readarr-py-0.4.1/readarr/api/download_client_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/download_client_config_api.py` & `readarr-py-0.4.1/readarr/api/download_client_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/edition_api.py` & `readarr-py-0.4.1/readarr/api/edition_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/file_system_api.py` & `readarr-py-0.4.1/readarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/health_api.py` & `readarr-py-0.4.1/readarr/api/health_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/history_api.py` & `readarr-py-0.4.1/readarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/host_config_api.py` & `readarr-py-0.4.1/readarr/api/host_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/import_list_api.py` & `readarr-py-0.4.1/readarr/api/import_list_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/import_list_exclusion_api.py` & `readarr-py-0.4.1/readarr/api/import_list_exclusion_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/indexer_api.py` & `readarr-py-0.4.1/readarr/api/indexer_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/indexer_config_api.py` & `readarr-py-0.4.1/readarr/api/indexer_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/initialize_js_api.py` & `readarr-py-0.4.1/readarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/language_api.py` & `readarr-py-0.4.1/readarr/api/language_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/localization_api.py` & `readarr-py-0.4.1/readarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/log_api.py` & `readarr-py-0.4.1/readarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/log_file_api.py` & `readarr-py-0.4.1/readarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/manual_import_api.py` & `readarr-py-0.4.1/readarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/media_cover_api.py` & `readarr-py-0.4.1/readarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/media_management_config_api.py` & `readarr-py-0.4.1/readarr/api/media_management_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/metadata_api.py` & `readarr-py-0.4.1/readarr/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/metadata_profile_api.py` & `readarr-py-0.4.1/readarr/api/metadata_profile_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/metadata_profile_schema_api.py` & `readarr-py-0.4.1/readarr/api/metadata_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/metadata_provider_config_api.py` & `readarr-py-0.4.1/readarr/api/metadata_provider_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/missing_api.py` & `readarr-py-0.4.1/readarr/api/missing_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/naming_config_api.py` & `readarr-py-0.4.1/readarr/api/naming_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/notification_api.py` & `readarr-py-0.4.1/readarr/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/parse_api.py` & `readarr-py-0.4.1/readarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/ping_api.py` & `readarr-py-0.4.1/readarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/quality_definition_api.py` & `readarr-py-0.4.1/readarr/api/quality_definition_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/quality_profile_api.py` & `readarr-py-0.4.1/readarr/api/quality_profile_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/quality_profile_schema_api.py` & `readarr-py-0.4.1/readarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/queue_action_api.py` & `readarr-py-0.4.1/readarr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/queue_api.py` & `readarr-py-0.4.1/readarr/api/queue_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/queue_details_api.py` & `readarr-py-0.4.1/readarr/api/queue_details_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/queue_status_api.py` & `readarr-py-0.4.1/readarr/api/queue_status_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/release_api.py` & `readarr-py-0.4.1/readarr/api/release_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/release_profile_api.py` & `readarr-py-0.4.1/readarr/api/release_profile_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/release_push_api.py` & `readarr-py-0.4.1/readarr/api/release_push_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/remote_path_mapping_api.py` & `readarr-py-0.4.1/readarr/api/remote_path_mapping_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/rename_book_api.py` & `readarr-py-0.4.1/readarr/api/rename_book_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/retag_book_api.py` & `readarr-py-0.4.1/readarr/api/retag_book_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/root_folder_api.py` & `readarr-py-0.4.1/readarr/api/root_folder_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/search_api.py` & `readarr-py-0.4.1/readarr/api/search_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/series_api.py` & `readarr-py-0.4.1/readarr/api/series_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/static_resource_api.py` & `readarr-py-0.4.1/readarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/system_api.py` & `readarr-py-0.4.1/readarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/tag_api.py` & `readarr-py-0.4.1/readarr/api/tag_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/tag_details_api.py` & `readarr-py-0.4.1/readarr/api/tag_details_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/task_api.py` & `readarr-py-0.4.1/readarr/api/task_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/ui_config_api.py` & `readarr-py-0.4.1/readarr/api/ui_config_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/update_api.py` & `readarr-py-0.4.1/readarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api/update_log_file_api.py` & `readarr-py-0.4.1/readarr/api/update_log_file_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/api_client.py` & `readarr-py-0.4.1/readarr/api_client.py`

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
-        self.user_agent = 'readarr-py/v0.4.0'
+        self.user_agent = 'readarr-py/v0.4.1'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `readarr-py-0.4.0/readarr/api_response.py` & `readarr-py-0.4.1/readarr/api_response.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/configuration.py` & `readarr-py-0.4.1/readarr/configuration.py`

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

### Comparing `readarr-py-0.4.0/readarr/exceptions.py` & `readarr-py-0.4.1/readarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/__init__.py` & `readarr-py-0.4.1/readarr/models/__init__.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/add_author_options.py` & `readarr-py-0.4.1/readarr/models/add_author_options.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/add_book_options.py` & `readarr-py-0.4.1/readarr/models/add_book_options.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/allow_fingerprinting.py` & `readarr-py-0.4.1/readarr/models/allow_fingerprinting.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/api_info_resource.py` & `readarr-py-0.4.1/readarr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/apply_tags.py` & `readarr-py-0.4.1/readarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/authentication_type.py` & `readarr-py-0.4.1/readarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author.py` & `readarr-py-0.4.1/readarr/models/author.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_editor_resource.py` & `readarr-py-0.4.1/readarr/models/author_editor_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/author_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_metadata.py` & `readarr-py-0.4.1/readarr/models/author_metadata.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_metadata_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/author_metadata_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_resource.py` & `readarr-py-0.4.1/readarr/models/author_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_statistics_resource.py` & `readarr-py-0.4.1/readarr/models/author_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_status_type.py` & `readarr-py-0.4.1/readarr/models/author_status_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/author_title_info.py` & `readarr-py-0.4.1/readarr/models/author_title_info.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/backup_resource.py` & `readarr-py-0.4.1/readarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/backup_type.py` & `readarr-py-0.4.1/readarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/blocklist_bulk_resource.py` & `readarr-py-0.4.1/readarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/blocklist_resource.py` & `readarr-py-0.4.1/readarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/blocklist_resource_paging_resource.py` & `readarr-py-0.4.1/readarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book.py` & `readarr-py-0.4.1/readarr/models/book.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_add_type.py` & `readarr-py-0.4.1/readarr/models/book_add_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_editor_resource.py` & `readarr-py-0.4.1/readarr/models/book_editor_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_file.py` & `readarr-py-0.4.1/readarr/models/book_file.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_file_list_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/book_file_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_file_list_resource.py` & `readarr-py-0.4.1/readarr/models/book_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_file_resource.py` & `readarr-py-0.4.1/readarr/models/book_file_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/book_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_list_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/book_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_resource.py` & `readarr-py-0.4.1/readarr/models/book_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_resource_paging_resource.py` & `readarr-py-0.4.1/readarr/models/book_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/book_statistics_resource.py` & `readarr-py-0.4.1/readarr/models/book_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/books_monitored_resource.py` & `readarr-py-0.4.1/readarr/models/books_monitored_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/bookshelf_author_resource.py` & `readarr-py-0.4.1/readarr/models/bookshelf_author_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/bookshelf_resource.py` & `readarr-py-0.4.1/readarr/models/bookshelf_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/certificate_validation_type.py` & `readarr-py-0.4.1/readarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/command.py` & `readarr-py-0.4.1/readarr/models/command.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/command_priority.py` & `readarr-py-0.4.1/readarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/command_resource.py` & `readarr-py-0.4.1/readarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/command_status.py` & `readarr-py-0.4.1/readarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/command_trigger.py` & `readarr-py-0.4.1/readarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/custom_filter_resource.py` & `readarr-py-0.4.1/readarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/custom_format.py` & `readarr-py-0.4.1/readarr/models/custom_format.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/custom_format_resource.py` & `readarr-py-0.4.1/readarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/custom_format_specification_schema.py` & `readarr-py-0.4.1/readarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/database_type.py` & `readarr-py-0.4.1/readarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/delay_profile_resource.py` & `readarr-py-0.4.1/readarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/development_config_resource.py` & `readarr-py-0.4.1/readarr/models/development_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/disk_space_resource.py` & `readarr-py-0.4.1/readarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/download_client_bulk_resource.py` & `readarr-py-0.4.1/readarr/models/download_client_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/download_client_config_resource.py` & `readarr-py-0.4.1/readarr/models/download_client_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/download_client_resource.py` & `readarr-py-0.4.1/readarr/models/download_client_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/download_protocol.py` & `readarr-py-0.4.1/readarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/edition.py` & `readarr-py-0.4.1/readarr/models/edition.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/edition_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/edition_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/edition_list_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/edition_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/edition_resource.py` & `readarr-py-0.4.1/readarr/models/edition_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/entity_history_event_type.py` & `readarr-py-0.4.1/readarr/models/entity_history_event_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/field.py` & `readarr-py-0.4.1/readarr/models/field.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/file_date_type.py` & `readarr-py-0.4.1/readarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/health_check_result.py` & `readarr-py-0.4.1/readarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/health_resource.py` & `readarr-py-0.4.1/readarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/history_resource.py` & `readarr-py-0.4.1/readarr/models/history_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/history_resource_paging_resource.py` & `readarr-py-0.4.1/readarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/host_config_resource.py` & `readarr-py-0.4.1/readarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/i_custom_format_specification.py` & `readarr-py-0.4.1/readarr/models/i_custom_format_specification.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/import_list_bulk_resource.py` & `readarr-py-0.4.1/readarr/models/import_list_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/import_list_exclusion_resource.py` & `readarr-py-0.4.1/readarr/models/import_list_exclusion_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/import_list_monitor_type.py` & `readarr-py-0.4.1/readarr/models/import_list_monitor_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/import_list_resource.py` & `readarr-py-0.4.1/readarr/models/import_list_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/import_list_type.py` & `readarr-py-0.4.1/readarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/indexer_bulk_resource.py` & `readarr-py-0.4.1/readarr/models/indexer_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/indexer_config_resource.py` & `readarr-py-0.4.1/readarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/indexer_resource.py` & `readarr-py-0.4.1/readarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/iso_country.py` & `readarr-py-0.4.1/readarr/models/iso_country.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/language_resource.py` & `readarr-py-0.4.1/readarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/links.py` & `readarr-py-0.4.1/readarr/models/links.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/log_file_resource.py` & `readarr-py-0.4.1/readarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/log_resource.py` & `readarr-py-0.4.1/readarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/log_resource_paging_resource.py` & `readarr-py-0.4.1/readarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/manual_import_resource.py` & `readarr-py-0.4.1/readarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/manual_import_update_resource.py` & `readarr-py-0.4.1/readarr/models/manual_import_update_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/media_cover.py` & `readarr-py-0.4.1/readarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/media_cover_types.py` & `readarr-py-0.4.1/readarr/models/media_cover_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/media_info_model.py` & `readarr-py-0.4.1/readarr/models/media_info_model.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/media_info_resource.py` & `readarr-py-0.4.1/readarr/models/media_info_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/media_management_config_resource.py` & `readarr-py-0.4.1/readarr/models/media_management_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/metadata_profile.py` & `readarr-py-0.4.1/readarr/models/metadata_profile.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/metadata_profile_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/metadata_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/metadata_profile_resource.py` & `readarr-py-0.4.1/readarr/models/metadata_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/metadata_provider_config_resource.py` & `readarr-py-0.4.1/readarr/models/metadata_provider_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/metadata_resource.py` & `readarr-py-0.4.1/readarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/monitor_types.py` & `readarr-py-0.4.1/readarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/monitoring_options.py` & `readarr-py-0.4.1/readarr/models/monitoring_options.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/naming_config_resource.py` & `readarr-py-0.4.1/readarr/models/naming_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/new_item_monitor_types.py` & `readarr-py-0.4.1/readarr/models/new_item_monitor_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/notification_resource.py` & `readarr-py-0.4.1/readarr/models/notification_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/paging_resource_filter.py` & `readarr-py-0.4.1/readarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/parse_resource.py` & `readarr-py-0.4.1/readarr/models/parse_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/parsed_book_info.py` & `readarr-py-0.4.1/readarr/models/parsed_book_info.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/parsed_track_info.py` & `readarr-py-0.4.1/readarr/models/parsed_track_info.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/ping_resource.py` & `readarr-py-0.4.1/readarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/profile_format_item.py` & `readarr-py-0.4.1/readarr/models/profile_format_item.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/profile_format_item_resource.py` & `readarr-py-0.4.1/readarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/proper_download_types.py` & `readarr-py-0.4.1/readarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/provider_message.py` & `readarr-py-0.4.1/readarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/provider_message_type.py` & `readarr-py-0.4.1/readarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/proxy_type.py` & `readarr-py-0.4.1/readarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality.py` & `readarr-py-0.4.1/readarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_definition_resource.py` & `readarr-py-0.4.1/readarr/models/quality_definition_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_model.py` & `readarr-py-0.4.1/readarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_profile.py` & `readarr-py-0.4.1/readarr/models/quality_profile.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_profile_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/quality_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_profile_quality_item.py` & `readarr-py-0.4.1/readarr/models/quality_profile_quality_item.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_profile_quality_item_resource.py` & `readarr-py-0.4.1/readarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/quality_profile_resource.py` & `readarr-py-0.4.1/readarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/queue_bulk_resource.py` & `readarr-py-0.4.1/readarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/queue_resource.py` & `readarr-py-0.4.1/readarr/models/queue_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/queue_resource_paging_resource.py` & `readarr-py-0.4.1/readarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/queue_status_resource.py` & `readarr-py-0.4.1/readarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/ratings.py` & `readarr-py-0.4.1/readarr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/rejection.py` & `readarr-py-0.4.1/readarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/rejection_type.py` & `readarr-py-0.4.1/readarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/release_profile_resource.py` & `readarr-py-0.4.1/readarr/models/release_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/release_resource.py` & `readarr-py-0.4.1/readarr/models/release_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/remote_path_mapping_resource.py` & `readarr-py-0.4.1/readarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/rename_book_resource.py` & `readarr-py-0.4.1/readarr/models/rename_book_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/rescan_after_refresh_type.py` & `readarr-py-0.4.1/readarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/retag_book_resource.py` & `readarr-py-0.4.1/readarr/models/retag_book_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/revision.py` & `readarr-py-0.4.1/readarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/root_folder_resource.py` & `readarr-py-0.4.1/readarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/runtime_mode.py` & `readarr-py-0.4.1/readarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/select_option.py` & `readarr-py-0.4.1/readarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series.py` & `readarr-py-0.4.1/readarr/models/series.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series_book_link.py` & `readarr-py-0.4.1/readarr/models/series_book_link.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series_book_link_list_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/series_book_link_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series_book_link_resource.py` & `readarr-py-0.4.1/readarr/models/series_book_link_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/series_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series_list_lazy_loaded.py` & `readarr-py-0.4.1/readarr/models/series_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/series_resource.py` & `readarr-py-0.4.1/readarr/models/series_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/sort_direction.py` & `readarr-py-0.4.1/readarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/system_resource.py` & `readarr-py-0.4.1/readarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/tag_details_resource.py` & `readarr-py-0.4.1/readarr/models/tag_details_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/tag_difference.py` & `readarr-py-0.4.1/readarr/models/tag_difference.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/tag_resource.py` & `readarr-py-0.4.1/readarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/task_resource.py` & `readarr-py-0.4.1/readarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/tracked_download_state.py` & `readarr-py-0.4.1/readarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/tracked_download_status.py` & `readarr-py-0.4.1/readarr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/tracked_download_status_message.py` & `readarr-py-0.4.1/readarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/ui_config_resource.py` & `readarr-py-0.4.1/readarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/update_changes.py` & `readarr-py-0.4.1/readarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/update_mechanism.py` & `readarr-py-0.4.1/readarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/update_resource.py` & `readarr-py-0.4.1/readarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/write_audio_tags_type.py` & `readarr-py-0.4.1/readarr/models/write_audio_tags_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/models/write_book_tags_type.py` & `readarr-py-0.4.1/readarr/models/write_book_tags_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr/rest.py` & `readarr-py-0.4.1/readarr/rest.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.4.0/readarr_py.egg-info/PKG-INFO` & `readarr-py-0.4.1/readarr_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readarr-py
-Version: 0.4.0
+Version: 0.4.1
 Summary: Readarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/readarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.4.0
+- Package version: 0.4.1
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
```

### Comparing `readarr-py-0.4.0/readarr_py.egg-info/SOURCES.txt` & `readarr-py-0.4.1/readarr_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

