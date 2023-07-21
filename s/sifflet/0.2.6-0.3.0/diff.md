# Comparing `tmp/sifflet-0.2.6.tar.gz` & `tmp/sifflet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sifflet-0.2.6.tar", last modified: Thu Dec 29 16:59:52 2022, max compression
+gzip compressed data, was "sifflet-0.3.0.tar", last modified: Fri Jul 21 12:59:46 2023, max compression
```

## Comparing `sifflet-0.2.6.tar` & `sifflet-0.3.0.tar`

### file list

```diff
@@ -1,269 +1,39 @@
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.532263 sifflet-0.2.6/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 sifflet-0.2.6/LICENSE
--rw-r--r--   0 baptiste   (501) staff       (20)       24 2022-08-11 16:27:52.000000 sifflet-0.2.6/MANIFEST.in
--rw-r--r--   0 baptiste   (501) staff       (20)     3464 2022-12-29 16:59:52.532112 sifflet-0.2.6/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)     3073 2022-08-11 16:27:52.000000 sifflet-0.2.6/README.md
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.498071 sifflet-0.2.6/client/
--rw-r--r--   0 baptiste   (501) staff       (20)      881 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/__init__.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.503360 sifflet-0.2.6/client/api/
--rw-r--r--   0 baptiste   (501) staff       (20)      214 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/api/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)    21243 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/access_token_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    68125 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/asset_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    20877 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/automation_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5576 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/aws_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5931 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/chart_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5961 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/collection_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    25681 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/config_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11226 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/dags_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11200 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/dashboard_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    22004 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/datapoint_qualification_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     7356 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/dataset_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    71331 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/dataset_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6374 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/dataset_field_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    64588 2022-12-19 08:51:56.000000 sifflet-0.2.6/client/api/datasource_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16878 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/datasource_connection_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     7494 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/dbt_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5818 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/feature_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    31877 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/idp_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    45636 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/incident_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    21273 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/lineage_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    10951 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/mail_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6211 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/notification_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    70342 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/rule_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    29957 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/rule_run_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15914 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/rule_template_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    24821 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/secret_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6355 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/sifflet_rule_run_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    25140 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/slack_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    19985 2022-12-19 08:51:56.000000 sifflet-0.2.6/client/api/statistics_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    27039 2022-12-19 08:51:56.000000 sifflet-0.2.6/client/api/tag_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6060 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/time_zone_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     6084 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/usage_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    65478 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/api/user_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5610 2022-12-15 10:09:23.000000 sifflet-0.2.6/client/api/versions_controller_api.py
--rw-r--r--   0 baptiste   (501) staff       (20)    39276 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/api_client.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17321 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/configuration.py
--rw-r--r--   0 baptiste   (501) staff       (20)     5277 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/exceptions.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.528764 sifflet-0.2.6/client/model/
--rw-r--r--   0 baptiste   (501) staff       (20)      340 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/model/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11985 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/a_rule_graphs_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12136 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/access_token_creation_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12934 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/access_token_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12649 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/action_condition_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14504 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/airflow_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11783 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/airflow_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12114 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/apply_automation_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16696 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12872 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13424 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/asset_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11891 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/asset_statistics_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14158 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/asset_usage_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12569 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/assets_catalog_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14512 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/assign_owners_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11924 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/assign_owners_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15175 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/athena_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12659 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/athena_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11889 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/automation_suggested_rules_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14571 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/big_query_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11844 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/big_query_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12375 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/catalog_filter_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14440 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/chart_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12276 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/checked_rule_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14664 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/collection_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13084 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11813 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/connection_test_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11623 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/create_access_token_request.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11806 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/create_comment_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14234 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/create_comment_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11641 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/create_comment_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11605 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/csv_content_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16468 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dag_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12750 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dag_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17472 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/model/dag_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12859 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dag_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16350 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dashboard_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12602 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dashboard_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16641 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dashboard_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15778 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/databricks_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13192 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/databricks_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14379 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datapoint_qualification_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17562 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_asset_overview.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13888 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_asset_overview_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12605 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_brief_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17485 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16224 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_dto_dataset_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12893 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13272 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dataset_params_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11834 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasets_tags_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17058 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_batch_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15581 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16706 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14147 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_ingestion_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11649 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_overview_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14843 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12675 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11906 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/datasource_statistics_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14762 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dbt_cloud_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12085 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dbt_cloud_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14521 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dbt_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11820 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/dbt_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12346 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/entity_urn.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13466 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/event_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16176 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/event_dto_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12550 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/event_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11854 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/export_as_csv_request_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16105 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/external_table_properties.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12120 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/external_table_properties_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11809 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/feature_consumption_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    17509 2022-12-19 08:51:56.000000 sifflet-0.2.6/client/model/field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16073 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/field_level_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13699 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/model/field_search_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12002 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/filter_element_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14670 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/firebolt_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11994 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/firebolt_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    24081 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/get_all_datasource_params_type200_response_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    19309 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/get_asset_overview_by_urn200_response.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16347 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/get_sifflet_rule_graph_by_run_and_group200_response_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12476 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/git_connection.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11822 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/git_connection_test_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12041 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11403 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/graph_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15887 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/histogram_graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11888 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/histogram_graph_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14479 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/histogram_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12233 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/histogram_point_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12474 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/idp_json_schema_params_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12260 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/import_report_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14988 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_detail_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13456 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12547 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_scope.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12583 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11910 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_statistics_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14932 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_status_update_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12303 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/incident_status_update_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11624 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/ingestion_run_summary.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12014 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/model/input_cardinality_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14350 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/issue_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12257 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/issue_overview_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12184 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/last_ingestion_status_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12192 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/last_run_status_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15404 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/lineage_entity_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14741 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/looker_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12039 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/looker_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12139 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/message_report_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12567 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/monitoring_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14774 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/mssql_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12163 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/mssql_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15686 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/multi_metrics_graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11671 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/multi_metrics_graph_dto_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14113 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/multi_metrics_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11851 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/multi_metrics_point_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14962 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/mysql_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12351 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/mysql_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11999 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/node_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14789 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/postgresql_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14720 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/power_bi_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12048 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/power_bi_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12347 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/preview_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12943 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/problem.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14734 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/quick_sight_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12047 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/quick_sight_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14783 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/redshift_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11594 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/resource_ids_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16195 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13650 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_details_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12514 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_dry_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12434 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_dry_run_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14715 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13149 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_graph_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    16476 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_graph_dto_graph_points_inner.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15663 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_info_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11631 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_overview_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12693 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_run_details_by_group.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13487 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_run_details_by_group_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    15612 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11898 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_statistics_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12774 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/model/rule_template_brief.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13225 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_template_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11905 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_template_index_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11836 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_template_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13169 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/rule_test_result_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11779 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/saml2_auth_n_config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13003 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/saml2_config_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11931 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/save_mail_addresses_summary.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12228 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/schema_version_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12081 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_access_token_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12091 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_dataset_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12192 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_datasource_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12192 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_datasource_ingestion_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12132 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_field_level_search_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12101 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_incident_light_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12132 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_rule_catalog_asset_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12184 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_rule_run_details_by_group_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12041 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_rule_run_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12000 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_tag_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12051 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/search_collection_time_zone_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11974 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/secret_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11764 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/slack_channel_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14900 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/snowflake_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12269 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/snowflake_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11837 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/status_type.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14447 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/status_update_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11859 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/status_update_payload_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11595 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/string_payload.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14504 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/tableau_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11783 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/tableau_params_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13052 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/tag_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14902 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/time_series_point.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12950 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/time_series_point_all_of.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13254 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/time_window.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11925 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/time_zone_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14117 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/unknown_datasource_params.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11703 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/upstream_of_field_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11977 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/usage_per_datasource_user_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    12748 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/user_asset_bookmark_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14794 2022-12-29 16:54:24.000000 sifflet-0.2.6/client/model/user_detail_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    11923 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/user_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    13041 2022-12-14 16:40:15.000000 sifflet-0.2.6/client/model/versions_dto.py
--rw-r--r--   0 baptiste   (501) staff       (20)    82788 2022-12-19 08:51:56.000000 sifflet-0.2.6/client/model_utils.py
--rw-r--r--   0 baptiste   (501) staff       (20)    14473 2022-12-14 16:40:16.000000 sifflet-0.2.6/client/rest.py
--rw-r--r--   0 baptiste   (501) staff       (20)      666 2022-08-11 16:27:52.000000 sifflet-0.2.6/pyproject.toml
--rw-r--r--   0 baptiste   (501) staff       (20)      142 2022-10-11 14:49:57.000000 sifflet-0.2.6/requirements.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       38 2022-12-29 16:59:52.532313 sifflet-0.2.6/setup.cfg
--rw-r--r--   0 baptiste   (501) staff       (20)      962 2022-08-11 16:27:52.000000 sifflet-0.2.6/setup.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.529444 sifflet-0.2.6/sifflet/
--rw-r--r--   0 baptiste   (501) staff       (20)       27 2022-12-29 16:59:44.000000 sifflet-0.2.6/sifflet/__init__.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.530355 sifflet-0.2.6/sifflet/apis/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/apis/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)      602 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/apis/base.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1034 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/cli.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.530661 sifflet-0.2.6/sifflet/configure/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/configure/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1435 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/configure/commands.py
--rw-r--r--   0 baptiste   (501) staff       (20)     2534 2022-11-09 15:06:09.000000 sifflet-0.2.6/sifflet/configure/service.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1201 2022-10-11 14:49:57.000000 sifflet-0.2.6/sifflet/constants.py
--rw-r--r--   0 baptiste   (501) staff       (20)     3611 2022-10-11 14:49:57.000000 sifflet-0.2.6/sifflet/errors.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.531090 sifflet-0.2.6/sifflet/ingest/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/ingest/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1198 2022-12-14 16:43:30.000000 sifflet-0.2.6/sifflet/ingest/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     1074 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/ingest/commands.py
--rw-r--r--   0 baptiste   (501) staff       (20)      522 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/ingest/service.py
--rw-r--r--   0 baptiste   (501) staff       (20)      454 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/logger.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.531509 sifflet-0.2.6/sifflet/rules/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/rules/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)     3018 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/rules/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)     2928 2022-11-16 12:15:08.000000 sifflet-0.2.6/sifflet/rules/commands.py
--rw-r--r--   0 baptiste   (501) staff       (20)     9593 2022-12-15 17:04:34.000000 sifflet-0.2.6/sifflet/rules/service.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.531925 sifflet-0.2.6/sifflet/status/
--rw-r--r--   0 baptiste   (501) staff       (20)        0 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/status/__init__.py
--rw-r--r--   0 baptiste   (501) staff       (20)      953 2022-11-15 17:48:16.000000 sifflet-0.2.6/sifflet/status/api.py
--rw-r--r--   0 baptiste   (501) staff       (20)      554 2022-08-11 16:27:52.000000 sifflet-0.2.6/sifflet/status/commands.py
--rw-r--r--   0 baptiste   (501) staff       (20)     2277 2022-11-09 15:10:45.000000 sifflet-0.2.6/sifflet/status/service.py
--rw-r--r--   0 baptiste   (501) staff       (20)      779 2022-11-09 15:05:47.000000 sifflet-0.2.6/sifflet/utils.py
-drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2022-12-29 16:59:52.530154 sifflet-0.2.6/sifflet.egg-info/
--rw-r--r--   0 baptiste   (501) staff       (20)     3464 2022-12-29 16:59:52.000000 sifflet-0.2.6/sifflet.egg-info/PKG-INFO
--rw-r--r--   0 baptiste   (501) staff       (20)     8735 2022-12-29 16:59:52.000000 sifflet-0.2.6/sifflet.egg-info/SOURCES.txt
--rw-r--r--   0 baptiste   (501) staff       (20)        1 2022-12-29 16:59:52.000000 sifflet-0.2.6/sifflet.egg-info/dependency_links.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       45 2022-12-29 16:59:52.000000 sifflet-0.2.6/sifflet.egg-info/entry_points.txt
--rw-r--r--   0 baptiste   (501) staff       (20)      143 2022-12-29 16:59:52.000000 sifflet-0.2.6/sifflet.egg-info/requires.txt
--rw-r--r--   0 baptiste   (501) staff       (20)       15 2022-12-29 16:59:52.000000 sifflet-0.2.6/sifflet.egg-info/top_level.txt
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.080716 sifflet-0.3.0/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/LICENSE
+-rw-r--r--   0 baptiste   (501) staff       (20)       25 2023-07-20 17:15:19.000000 sifflet-0.3.0/MANIFEST.in
+-rw-r--r--   0 baptiste   (501) staff       (20)     4042 2023-07-21 12:59:46.080533 sifflet-0.3.0/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)     3652 2023-07-20 17:15:19.000000 sifflet-0.3.0/README.md
+-rw-r--r--   0 baptiste   (501) staff       (20)      724 2023-07-20 17:22:51.000000 sifflet-0.3.0/pyproject.toml
+-rw-r--r--   0 baptiste   (501) staff       (20)      123 2023-07-21 09:10:18.000000 sifflet-0.3.0/requirements.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       38 2023-07-21 12:59:46.080766 sifflet-0.3.0/setup.cfg
+-rw-r--r--   0 baptiste   (501) staff       (20)      964 2023-07-20 17:15:19.000000 sifflet-0.3.0/setup.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.078077 sifflet-0.3.0/sifflet.egg-info/
+-rw-r--r--   0 baptiste   (501) staff       (20)     4042 2023-07-21 12:59:46.000000 sifflet-0.3.0/sifflet.egg-info/PKG-INFO
+-rw-r--r--   0 baptiste   (501) staff       (20)      745 2023-07-21 12:59:46.000000 sifflet-0.3.0/sifflet.egg-info/SOURCES.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)        1 2023-07-21 12:59:46.000000 sifflet-0.3.0/sifflet.egg-info/dependency_links.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       49 2023-07-21 12:59:46.000000 sifflet-0.3.0/sifflet.egg-info/entry_points.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       92 2023-07-21 12:59:46.000000 sifflet-0.3.0/sifflet.egg-info/requires.txt
+-rw-r--r--   0 baptiste   (501) staff       (20)       12 2023-07-21 12:59:46.000000 sifflet-0.3.0/sifflet.egg-info/top_level.txt
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.078478 sifflet-0.3.0/sifflet_cli/
+-rw-r--r--   0 baptiste   (501) staff       (20)       27 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1051 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/cli.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.078711 sifflet-0.3.0/sifflet_cli/code/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/code/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      175 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/code/commands.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.078946 sifflet-0.3.0/sifflet_cli/code/workspace/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/code/workspace/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     2553 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/code/workspace/commands.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.079185 sifflet-0.3.0/sifflet_cli/configure/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/configure/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1938 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/configure/commands.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.079497 sifflet-0.3.0/sifflet_cli/ingest/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/ingest/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     1086 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/ingest/commands.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      454 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/logger.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.080084 sifflet-0.3.0/sifflet_cli/rules/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/rules/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     3362 2023-07-20 17:45:51.000000 sifflet-0.3.0/sifflet_cli/rules/commands.py
+-rw-r--r--   0 baptiste   (501) staff       (20)     6046 2023-07-21 09:04:47.000000 sifflet-0.3.0/sifflet_cli/rules/displayrules.py
+drwxr-xr-x   0 baptiste   (501) staff       (20)        0 2023-07-21 12:59:46.080334 sifflet-0.3.0/sifflet_cli/status/
+-rw-r--r--   0 baptiste   (501) staff       (20)        0 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/status/__init__.py
+-rw-r--r--   0 baptiste   (501) staff       (20)      750 2023-07-20 17:15:19.000000 sifflet-0.3.0/sifflet_cli/status/commands.py
```

### Comparing `sifflet-0.2.6/PKG-INFO` & `sifflet-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sifflet
-Version: 0.2.6
-Summary: Sifflet sdk
-Home-page: https://www.siffletdata.com/
-Author: Sifflet
-Author-email: support@siffletdata.com
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Sifflet CLI
 ==========
 
 This package provides a command line interface (CLI) to [Sifflet](https://www.siffletdata.com/)  application.
 
 # Getting Started
 ## Installation
@@ -26,40 +12,54 @@
 pip install sifflet
 
 sifflet --version
 ```
 
 ## Configuration
 
-Before using the Sifflet CLI, you need to set your tenant and credentials. 
+Before using the Sifflet CLI, you need to set your tenant and credentials.
 You can do it in several ways:
 - Sifflet command line `sifflet configure` (which will persists configuration in a file)
-- Or with environment variables  
+- Or with environment variables
 
-You will need in both cases the following information:  
-`<your_tenant_name>`: if you access to Sifflet with "https://abcdef.siffletdata.com", then your tenant would be `abcdef`  
-`<your_sifflet_access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
+You will need in both cases the following information:
+- `<access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
+- For SaaS version: `<tenant_name>`: Name of your tenant. Sifflet UI URL is `https://<tenant_name>.siffletdata.com`. Sifflet Backend URL is `https://<tenant_name>api.siffletdata.com`. For instance, if you access to Sifflet UI with `https://mycompany.siffletdata.com`, then your tenant would be `mycompany`.
+- For self-hosted deployment: `<backend_url>`: Full URL to the Sifflet backend on your deployment including for instance: `https://sifflet-backend.mycompany.com`
 
 
 #### Sifflet configure
-You can input the tenant and credentials directly with the `sifflet configure` command
+You can input the tenant and credentials directly with the `sifflet configure` command.
+
+For SaaS version:
+```shell
+> sifflet configure --tenant <tenant_name>
+Your API access token [None]: <access_token>
+```
+or, for self-hosted deployment:
 ```shell
-> sifflet configure
-Your tenant name [None]: <your_tenant_name>
-Your API access token [None]: <your_sifflet_access_token>
+> sifflet configure --backend-url <backend_url>
+Your API access token [None]: <access_token>
 ```
-The use of `sifflet configure` will persist the configuration in a file located at `~/.sifflet/config.ini` 
+
+The use of `sifflet configure` will persist the configuration in a file located at `~/.sifflet/config.ini`
 (or in `%UserProfile%\.sifflet/config.ini` on Windows).
 
 #### Environment variables
 To use environment variables, you can do the following:
 
+For SaaS version:
+```shell
+> export SIFFLET_TENANT=<tenant_name>
+> export SIFFLET_TOKEN=<access_token>
+```
+or, for self-hosted deployment:
 ```shell
-> export SIFFLET_TENANT=<your_tenant_name>
-> export SIFFLET_TOKEN=<your_sifflet_access_token> 
+> export SIFFLET_BACKEND_URL=<backend_url>
+> export SIFFLET_TOKEN=<access_token>
 ```
 
 
 You can check that setup is done correctly with `sifflet status`.
 
 ```shell
 > sifflet status
@@ -78,15 +78,15 @@
 The documentation with the available commands can be found [here](https://docs.siffletdata.com/docs/cli-command-line-interface).
 
 ## Help
 The `--help` option is available for any command, for instance `sifflet --help` or `sifflet rules list --help`.
 
 ## Examples
 
-### Trigger a specific rule 
+### Trigger a specific rule
 - First, find your rule id with `sifflet rules list`. You can filter with `--name` to narrow your search.
 
 ```shell
 # Display rules
 sifflet rules list
 sifflet rules list --name <search_criteria>
 ```
```

### Comparing `sifflet-0.2.6/pyproject.toml` & `sifflet-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 legacy_tox_ini = """
 [tox]
 envlist =
     py3{11,10,9,8,7}
 skip_missing_interpreters = true
 
 [testenv]
-deps = -r requirements-dev.txt
-commands = pytest tests --junitxml=report.xml
-
+commands_pre =
+    pip install ../sifflet-sdk
+    pip install -r requirements-dev.txt
+commands =
+    pytest tests --junitxml=report.xml
 [testenv:black]
 deps=
     black
 commands=
     black --check sifflet
 """
```

### Comparing `sifflet-0.2.6/setup.py` & `sifflet-0.3.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import setuptools
 
-import sifflet
+import sifflet_cli
 
 long_description = open("README.md", "r", encoding="utf-8").read()
 requirements = [i.strip() for i in open("requirements.txt").readlines()]
 
 setuptools.setup(
     name="sifflet",
-    version=sifflet.__version__,
+    version=sifflet_cli.__version__,
     author="Sifflet",
     author_email="support@siffletdata.com",
     url="https://www.siffletdata.com/",
-    description="Sifflet sdk",
-    py_modules=["sifflet"],
+    description="Sifflet CLI",
+    py_modules=["sifflet_cli"],
     entry_points={
         "console_scripts": [
-            "sifflet = sifflet.cli:main",
+            "sifflet = sifflet_cli.cli:main",
         ],
     },
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     include_package_data=True,
-    packages=setuptools.find_packages(include=["sifflet", "sifflet.*", "client", "client.*"]),
+    packages=setuptools.find_packages(include=["sifflet_cli", "sifflet_cli.*"]),
     python_requires=">=3.7",
     install_requires=requirements,
 )
```

### Comparing `sifflet-0.2.6/sifflet/cli.py` & `sifflet-0.3.0/sifflet_cli/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import sys
 
 import click
-
-from sifflet import __version__
-from sifflet.configure.commands import configure
-from sifflet.configure.service import ConfigureService
-from sifflet.constants import SIFFLET_CONFIG_CTX
-from sifflet.errors import exception_handler
-from sifflet.ingest.commands import ingest
-from sifflet.rules.commands import rules
-from sifflet.status.commands import status
+from sifflet_sdk.configure.service import ConfigureService
+from sifflet_sdk.constants import SIFFLET_CONFIG_CTX
+from sifflet_sdk.errors import exception_handler
+
+from sifflet_cli import __version__
+from sifflet_cli.code.commands import code
+from sifflet_cli.configure.commands import configure
+from sifflet_cli.ingest.commands import ingest
+from sifflet_cli.rules.commands import rules
+from sifflet_cli.status.commands import status
 
 
 @exception_handler
 def main():
     """Entrypoint"""
     sys.exit(sifflet_cli())  # pylint: disable=E1120
 
 
 @click.group()
 @click.version_option(__version__)
 @click.option("--debug", is_flag=True, hidden=True)
-@click.option("--dev", "dev_mode", is_flag=True, hidden=True)
 @click.pass_context
-def sifflet_cli(ctx, debug: bool, dev_mode: bool):
+def sifflet_cli(ctx, debug: bool):
     """Sifflet CLI"""
-    sifflet_config = ConfigureService().load_configuration(debug, dev_mode)
+    sifflet_config = ConfigureService().load_configuration(debug)
     ctx.ensure_object(dict)
     ctx.obj[SIFFLET_CONFIG_CTX] = sifflet_config
 
 
 sifflet_cli.add_command(status)
 sifflet_cli.add_command(configure)
 sifflet_cli.add_command(rules)
 sifflet_cli.add_command(ingest)
+sifflet_cli.add_command(code)
```

### Comparing `sifflet-0.2.6/sifflet/ingest/commands.py` & `sifflet-0.3.0/sifflet_cli/ingest/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import click
+from sifflet_sdk.constants import SIFFLET_CONFIG_CTX
+from sifflet_sdk.ingest.service import IngestionService
 
-from sifflet.constants import SIFFLET_CONFIG_CTX
-from sifflet.ingest.service import IngestionService
-from sifflet.logger import logger
+from sifflet_cli.logger import logger
 
 
 @click.group()
 def ingest():
     """Control ingestion of tools into Sifflet."""
```

### Comparing `sifflet-0.2.6/sifflet/rules/commands.py` & `sifflet-0.3.0/sifflet_cli/rules/commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 from typing import List
 
 import click
 from click_aliases import ClickAliasedGroup
+from sifflet_sdk.constants import (
+    DEFAULT_PAGE_NUM,
+    DEFAULT_PAGE_SIZE,
+    OutputType,
+    SIFFLET_CONFIG_CTX,
+)
+from sifflet_sdk.rules.service import RulesService
 
-from sifflet.constants import SIFFLET_CONFIG_CTX, OutputType, DEFAULT_PAGE_SIZE, DEFAULT_PAGE_NUM
-from sifflet.rules.service import RulesService
+from sifflet_cli.rules.displayrules import DisplayRules
 
 
 @click.group(cls=ClickAliasedGroup)
 def rules():
     """List and control rules"""
 
 
@@ -39,20 +45,26 @@
     required=False,
     help="Page number of the server side pagination",
     default=DEFAULT_PAGE_NUM,
     show_default=True,
 )
 @click.pass_context
 def list_rules(
-    ctx, name: str, output: str = "table", page_size: int = DEFAULT_PAGE_SIZE, page_num: int = DEFAULT_PAGE_NUM
+    ctx,
+    name: str,
+    output: str = "table",
+    page_size: int = DEFAULT_PAGE_SIZE,
+    page_num: int = DEFAULT_PAGE_NUM,
 ):
     """Display all rules created"""
     sifflet_config = ctx.obj[SIFFLET_CONFIG_CTX]
-    service = RulesService(sifflet_config, output_type=output, page_size=page_size, page_num=page_num)
-    service.show_rules(name)
+    service = RulesService(sifflet_config, page_size=page_size, page_num=page_num)
+    response_rules, response_total_count = service.fetch_rules(filter_name=name)
+    utils = DisplayRules(output_type=output, page_num=page_num)
+    utils.show_rules(rules=response_rules, total_count=response_total_count, filter_name=name)
 
 
 @rules.command()
 @click.option("--id", "ids", multiple=True, required=True, help="The rule id to trigger")
 @click.pass_context
 def run(ctx, ids: List[str]):
     """Run one or several rules - requires rule id(s)"""
@@ -88,13 +100,19 @@
     required=False,
     help="Page number of the server side pagination",
     default=DEFAULT_PAGE_NUM,
     show_default=True,
 )
 @click.pass_context
 def run_history(
-    ctx, rule_id: str, output: str = "table", page_size: int = DEFAULT_PAGE_SIZE, page_num: int = DEFAULT_PAGE_NUM
+    ctx,
+    rule_id: str,
+    output: str = "table",
+    page_size: int = DEFAULT_PAGE_SIZE,
+    page_num: int = DEFAULT_PAGE_NUM,
 ):
     """Display all rule runs for a given rule id"""
     sifflet_config = ctx.obj[SIFFLET_CONFIG_CTX]
-    service = RulesService(sifflet_config, output_type=output, page_size=page_size, page_num=page_num)
-    service.show_run_history(rule_id=rule_id)
+    service = RulesService(sifflet_config, page_size=page_size, page_num=page_num)
+    rule_info, rule_runs, total_count = service.fetch_run_history(rule_id=rule_id)
+    utils = DisplayRules(output_type=output)
+    utils.show_run_history(rule_info, rule_runs, total_count)
```

### Comparing `sifflet-0.2.6/sifflet.egg-info/PKG-INFO` & `sifflet-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sifflet
-Version: 0.2.6
-Summary: Sifflet sdk
+Version: 0.3.0
+Summary: Sifflet CLI
 Home-page: https://www.siffletdata.com/
 Author: Sifflet
 Author-email: support@siffletdata.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -26,40 +26,54 @@
 pip install sifflet
 
 sifflet --version
 ```
 
 ## Configuration
 
-Before using the Sifflet CLI, you need to set your tenant and credentials. 
+Before using the Sifflet CLI, you need to set your tenant and credentials.
 You can do it in several ways:
 - Sifflet command line `sifflet configure` (which will persists configuration in a file)
-- Or with environment variables  
+- Or with environment variables
 
-You will need in both cases the following information:  
-`<your_tenant_name>`: if you access to Sifflet with "https://abcdef.siffletdata.com", then your tenant would be `abcdef`  
-`<your_sifflet_access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
+You will need in both cases the following information:
+- `<access_token>`: you can find more information on how to generate it [here](https://docs.siffletdata.com/docs/generate-an-api-token)
+- For SaaS version: `<tenant_name>`: Name of your tenant. Sifflet UI URL is `https://<tenant_name>.siffletdata.com`. Sifflet Backend URL is `https://<tenant_name>api.siffletdata.com`. For instance, if you access to Sifflet UI with `https://mycompany.siffletdata.com`, then your tenant would be `mycompany`.
+- For self-hosted deployment: `<backend_url>`: Full URL to the Sifflet backend on your deployment including for instance: `https://sifflet-backend.mycompany.com`
 
 
 #### Sifflet configure
-You can input the tenant and credentials directly with the `sifflet configure` command
+You can input the tenant and credentials directly with the `sifflet configure` command.
+
+For SaaS version:
+```shell
+> sifflet configure --tenant <tenant_name>
+Your API access token [None]: <access_token>
+```
+or, for self-hosted deployment:
 ```shell
-> sifflet configure
-Your tenant name [None]: <your_tenant_name>
-Your API access token [None]: <your_sifflet_access_token>
+> sifflet configure --backend-url <backend_url>
+Your API access token [None]: <access_token>
 ```
-The use of `sifflet configure` will persist the configuration in a file located at `~/.sifflet/config.ini` 
+
+The use of `sifflet configure` will persist the configuration in a file located at `~/.sifflet/config.ini`
 (or in `%UserProfile%\.sifflet/config.ini` on Windows).
 
 #### Environment variables
 To use environment variables, you can do the following:
 
+For SaaS version:
+```shell
+> export SIFFLET_TENANT=<tenant_name>
+> export SIFFLET_TOKEN=<access_token>
+```
+or, for self-hosted deployment:
 ```shell
-> export SIFFLET_TENANT=<your_tenant_name>
-> export SIFFLET_TOKEN=<your_sifflet_access_token> 
+> export SIFFLET_BACKEND_URL=<backend_url>
+> export SIFFLET_TOKEN=<access_token>
 ```
 
 
 You can check that setup is done correctly with `sifflet status`.
 
 ```shell
 > sifflet status
@@ -78,15 +92,15 @@
 The documentation with the available commands can be found [here](https://docs.siffletdata.com/docs/cli-command-line-interface).
 
 ## Help
 The `--help` option is available for any command, for instance `sifflet --help` or `sifflet rules list --help`.
 
 ## Examples
 
-### Trigger a specific rule 
+### Trigger a specific rule
 - First, find your rule id with `sifflet rules list`. You can filter with `--name` to narrow your search.
 
 ```shell
 # Display rules
 sifflet rules list
 sifflet rules list --name <search_criteria>
 ```
```

