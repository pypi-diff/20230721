# Comparing `tmp/data_ecosystem_services-202307.0.4.tar.gz` & `tmp/data_ecosystem_services-202307.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_ecosystem_services-202307.0.4.tar", max compression
+gzip compressed data, was "data_ecosystem_services-202307.0.5.tar", max compression
```

## Comparing `data_ecosystem_services-202307.0.4.tar` & `data_ecosystem_services-202307.0.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0      918 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/__main__.py
--rw-r--r--   0        0        0     1264 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/__init__.py
--rw-r--r--   0        0        0     5030 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/column.py
--rw-r--r--   0        0        0    23557 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/customfieldsendpoint.py
--rw-r--r--   0        0        0    13817 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/datasource.py
--rw-r--r--   0        0        0     2037 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/endpoint.py
--rw-r--r--   0        0        0    12009 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/excelmetadata.py
--rw-r--r--   0        0        0      566 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/execution_session.py
--rw-r--r--   0        0        0     4530 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/idfinderendpoint.py
--rw-r--r--   0        0        0    16621 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/manifest.py
--rw-r--r--   0        0        0     5003 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/query.py
--rw-r--r--   0        0        0    51147 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/schema.py
--rw-r--r--   0        0        0     7345 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/table.py
--rw-r--r--   0        0        0     1486 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/tagsendpoint.py
--rw-r--r--   0        0        0    25982 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/tokenendpoint.py
--rw-r--r--   0        0        0     1044 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_client_service/__init__.py
--rw-r--r--   0        0        0       41 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_client_service/az_client.py
--rw-r--r--   0        0        0     4570 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_client_service/azd_client.py
--rw-r--r--   0        0        0     1050 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_key_vault_service/__init__.py
--rw-r--r--   0        0        0     8966 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_key_vault_service/az_key_vault.py
--rw-r--r--   0        0        0     1073 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_storage_service/__init__.py
--rw-r--r--   0        0        0     2665 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/az_storage_service/az_storage_queue.py
--rw-r--r--   0        0        0     1024 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_admin_service/__init__.py
--rw-r--r--   0        0        0    15940 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_admin_service/environment_logging.py
--rw-r--r--   0        0        0     8398 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_admin_service/environment_tracing.py
--rw-r--r--   0        0        0     1013 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_security_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_security_service/security_base64.py
--rw-r--r--   0        0        0    21410 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_security_service/security_core.py
--rw-r--r--   0        0        0     1175 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/__init__.py
--rw-r--r--   0        0        0    42751 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/dataset_metadata.py
--rw-r--r--   0        0        0    40188 2023-07-18 10:51:23.910975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/environment_metadata.py
--rw-r--r--   0        0        0    36068 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/job_metadata.py
--rw-r--r--   0        0        0     2254 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/logging_metadata.py
--rw-r--r--   0        0        0    22352 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
--rw-r--r--   0        0        0     1727 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/__init__.py
--rw-r--r--   0        0        0    33787 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
--rw-r--r--   0        0        0     8962 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
--rw-r--r--   0        0        0    25880 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
--rw-r--r--   0        0        0     3825 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
--rw-r--r--   0        0        0     3949 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
--rw-r--r--   0        0        0    48198 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
--rw-r--r--   0        0        0     5323 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
--rw-r--r--   0        0        0     4903 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
--rw-r--r--   0        0        0     4648 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/job_core.py
--rw-r--r--   0        0        0    17832 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
--rw-r--r--   0        0        0     8956 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/directory_paths.txt
--rw-r--r--   0        0        0      827 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/github_service/__init__.py
--rw-r--r--   0        0        0     7250 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/github_service/github_secret.py
--rw-r--r--   0        0        0     1707 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/jira_service/__init__.py
--rw-r--r--   0        0        0     6295 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/jira_service/jira_client.py
--rw-r--r--   0        0        0       44 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/output.txt
--rw-r--r--   0        0        0      869 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/posit_service/__init__.py
--rw-r--r--   0        0        0    20785 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/posit_service/posit_connect.py
--rw-r--r--   0        0        0      825 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/python_service/__init__.py
--rw-r--r--   0        0        0       24 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/python_service/python_client.py
--rw-r--r--   0        0        0    15021 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/requirements.txt
--rw-r--r--   0        0        0      832 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/windows_service/__init__.py
--rw-r--r--   0        0        0     2499 2023-07-18 10:51:23.914975 data_ecosystem_services-202307.0.4/data_ecosystem_services/windows_service/windows_credential.py
--rw-r--r--   0        0        0    11357 2023-07-18 10:51:23.950976 data_ecosystem_services-202307.0.4/license.md
--rw-r--r--   0        0        0     3914 2023-07-18 10:54:37.490507 data_ecosystem_services-202307.0.4/pyproject.toml
--rw-r--r--   0        0        0    52292 2023-07-18 10:51:23.950976 data_ecosystem_services-202307.0.4/readme.md
--rw-r--r--   0        0        0      130 2023-07-18 10:51:23.950976 data_ecosystem_services-202307.0.4/setup.cfg
--rw-r--r--   0        0        0      127 2023-07-18 10:51:23.950976 data_ecosystem_services-202307.0.4/setup.py
--rw-r--r--   0        0        0    55802 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.4/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/__main__.py
+-rw-r--r--   0        0        0     1264 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/__init__.py
+-rw-r--r--   0        0        0     5030 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/column.py
+-rw-r--r--   0        0        0    24777 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/customfieldsendpoint.py
+-rw-r--r--   0        0        0    13817 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/datasource.py
+-rw-r--r--   0        0        0     2037 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/endpoint.py
+-rw-r--r--   0        0        0    12009 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/excelmetadata.py
+-rw-r--r--   0        0        0      566 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/execution_session.py
+-rw-r--r--   0        0        0     4530 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/idfinderendpoint.py
+-rw-r--r--   0        0        0    16621 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/manifest.py
+-rw-r--r--   0        0        0     5003 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/query.py
+-rw-r--r--   0        0        0    51042 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/schema.py
+-rw-r--r--   0        0        0     7345 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/table.py
+-rw-r--r--   0        0        0     1486 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tagsendpoint.py
+-rw-r--r--   0        0        0    25982 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tokenendpoint.py
+-rw-r--r--   0        0        0     1044 2023-07-21 03:11:49.056186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/__init__.py
+-rw-r--r--   0        0        0       41 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/az_client.py
+-rw-r--r--   0        0        0     4570 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/azd_client.py
+-rw-r--r--   0        0        0     1050 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/__init__.py
+-rw-r--r--   0        0        0     8967 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/az_key_vault.py
+-rw-r--r--   0        0        0     1073 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/__init__.py
+-rw-r--r--   0        0        0     2665 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/az_storage_queue.py
+-rw-r--r--   0        0        0     1024 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/__init__.py
+-rw-r--r--   0        0        0    15940 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_logging.py
+-rw-r--r--   0        0        0     8398 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_tracing.py
+-rw-r--r--   0        0        0     1013 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/security_base64.py
+-rw-r--r--   0        0        0    21410 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/security_core.py
+-rw-r--r--   0        0        0     1175 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/__init__.py
+-rw-r--r--   0        0        0    42751 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/dataset_metadata.py
+-rw-r--r--   0        0        0    40188 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/environment_metadata.py
+-rw-r--r--   0        0        0    36068 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/job_metadata.py
+-rw-r--r--   0        0        0     2254 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/logging_metadata.py
+-rw-r--r--   0        0        0    22352 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/pipeline_metadata.py
+-rw-r--r--   0        0        0     1727 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/__init__.py
+-rw-r--r--   0        0        0    33787 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py
+-rw-r--r--   0        0        0     8962 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py
+-rw-r--r--   0        0        0    25880 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py
+-rw-r--r--   0        0        0     3825 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py
+-rw-r--r--   0        0        0     3949 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_core.py
+-rw-r--r--   0        0        0    48455 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_file.py
+-rw-r--r--   0        0        0     5323 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_http.py
+-rw-r--r--   0        0        0     4903 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py
+-rw-r--r--   0        0        0     4648 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/job_core.py
+-rw-r--r--   0        0        0    17832 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/repo_core.py
+-rw-r--r--   0        0        0     8956 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/directory_paths.txt
+-rw-r--r--   0        0        0      827 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/__init__.py
+-rw-r--r--   0        0        0     7250 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/github_secret.py
+-rw-r--r--   0        0        0     1707 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/__init__.py
+-rw-r--r--   0        0        0     6295 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/jira_client.py
+-rw-r--r--   0        0        0       44 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/output.txt
+-rw-r--r--   0        0        0      869 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/__init__.py
+-rw-r--r--   0        0        0    21086 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/posit_connect.py
+-rw-r--r--   0        0        0      825 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/python_service/__init__.py
+-rw-r--r--   0        0        0       24 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/python_service/python_client.py
+-rw-r--r--   0        0        0    15021 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/requirements.txt
+-rw-r--r--   0        0        0      832 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/__init__.py
+-rw-r--r--   0        0        0     2499 2023-07-21 03:11:49.060186 data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/windows_credential.py
+-rw-r--r--   0        0        0    11357 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/license.md
+-rw-r--r--   0        0        0     3914 2023-07-21 03:15:32.962769 data_ecosystem_services-202307.0.5/pyproject.toml
+-rw-r--r--   0        0        0    52292 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/readme.md
+-rw-r--r--   0        0        0      130 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/setup.cfg
+-rw-r--r--   0        0        0      127 2023-07-21 03:11:49.068187 data_ecosystem_services-202307.0.5/setup.py
+-rw-r--r--   0        0        0    55802 1970-01-01 00:00:00.000000 data_ecosystem_services-202307.0.5/PKG-INFO
```

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/__main__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/__main__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/column.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/column.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/customfieldsendpoint.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/customfieldsendpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,17 +317,19 @@
                 api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
                 response_custom = requests.post(
                     api_url, headers=headers, timeout=REQUEST_TIMEOUT, json=data)
 
                 response_custom.raise_for_status()
                 custom_result = response_custom.json()
                 number_received = custom_result.get('number_received')
-                logger.info(f"number_received:{number_received}")
+                logger.info(f"number_received: {number_received}")
                 updated_objects = custom_result.get('updated_objects')
+                logger.info(f"updated_objects: {updated_objects}")
                 new_objects = custom_result.get('new_objects')
+                logger.info(f"new_objects: {new_objects}")
                 error_objects = custom_result.get('error_objects')
                 if error_objects and len(error_objects) > 0:
                     error_message = ', '.join(str(e)
                                               for e in error_objects)
                     raise EdcAlationError(
                         f"Errors occurred: {error_message}: api_url {api_url}")
                 error = custom_result.get('error')
@@ -339,14 +341,40 @@
 
             except Exception as ex:
                 error_msg = f"Error: {str(ex)} : {str(key)}: {str(object_type)}"
                 exc_info = sys.exc_info()
                 logger_singleton.error_with_exception(error_msg, exc_info)
                 raise
 
+    def wrap_with_quotes(self, key):
+        """
+        Wraps a string key with double quotes if it is not already wrapped.
+
+        Args:
+            key (str): The string key to be wrapped.
+
+        Returns:
+            str: The key wrapped with double quotes, if it was not already wrapped.
+
+        Example:
+            >>> key1 = 'example'
+            >>> key2 = '"example"'
+            >>> wrapped_key1 = wrap_with_quotes(key1)
+            >>> wrapped_key2 = wrap_with_quotes(key2)
+            >>> print(wrapped_key1)
+            "example"
+            >>> print(wrapped_key2)
+            "example"
+        """
+
+        if key.startswith("\"") and key.endswith("\""):
+            return key  # Key is already wrapped
+
+        return f"\"{key}\""  # Wrap the key with double quotes
+
     def get_data(self, u):
         """Get data from an object or its 'get_alation_data' method.
 
         Args:
             u: The object from which to retrieve the data.
 
         Returns:
@@ -452,28 +480,38 @@
                 else:
                     raise EdcAlationError(
                         f"Errors occurred and cannot process object because it is missing get_alation_data: {str(fields)}")
 
                 # Remove the data source ID from the key if it exists to avoid duplicate data source ID
                 key = key.replace(str(alation_datasource_id) + ".", "")
 
+                if object_type == 'schema':
+                    key = self.wrap_with_quotes(key)
+                    # key = key.replace('.', '%2E')
+
                 # Add the data source ID to the key
                 full_key = f"{alation_datasource_id}.{key}"
 
                 # Check if the key contains special characters
                 if self.has_special_chars(full_key):
                     logger.warning(
                         f"The following submitted key contains special characters: {str(full_key)}")
 
                 # Remove the key from the fields if it exists to avoid duplicate key
                 if 'key' in processed_fields:
                     processed_fields.pop('key')
 
+                params = {
+                    "create_new": "false",
+                    "replace_values": "true"
+                }
+
                 # Add the key to the fields
-                single_update = {"key": full_key, **processed_fields}
+                single_update = {
+                    "key": full_key, **processed_fields}
                 self.updates.append(single_update)
 
                 # Submit the updates if the batch size is reached or if force_submit is True
                 if len(self.updates) >= batch_size or force_submit:
                     # Create the request body with array if needed
                     array_of_json = [json.dumps(u) for u in self.updates]
                     if len(array_of_json) > 1:
@@ -493,24 +531,24 @@
                         logger.error(error_msg)
                         raise EdcAlationError(error_msg)
 
                     # submit the batch
                     logger.info(
                         f"Submitting {object_type} batch")
                     metadata_endpoint = '/api/v1/bulk_metadata/custom_fields/default'
-                    api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}?create_new=false"
+                    api_url = f"{edc_alation_base_url}{metadata_endpoint}/{object_type}"
 
                     # Create headers
-                    headers = {'Token': edc_alation_api_token,
-                               'Content-Type': 'application/json',
-                               'Accept': 'application/json'}
+                    headers = {"TOKEN": edc_alation_api_token,
+                               "Token": edc_alation_api_token,
+                               "content-type": 'application/json'}
 
                     # Submit the updates using the constructed URL and request_body
                     response = requests.post(
-                        api_url, headers=headers, json=data, verify=True, timeout=REQUEST_TIMEOUT)
+                        api_url, headers=headers, json=data, params=params, verify=True, timeout=REQUEST_TIMEOUT)
                     response_json = response.json()
 
                     # Clear updates after submission
                     self.updates = []
                     logger.info(
                         f"Response Status {object_type} batch of {request_body}")
                     response.raise_for_status()
```

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/datasource.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/datasource.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/endpoint.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/endpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/excelmetadata.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/excelmetadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/execution_session.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/execution_session.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/idfinderendpoint.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/idfinderendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/manifest.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/manifest.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/query.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/query.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/schema.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,17 +853,15 @@
                 logger.info('Updating table {}'.format(table.name))
 
                 if schema_name == 'object_name_is_missing' or schema_name == 'object name is missing':
                     raise ValueError('Invalid schema_name value.')
 
                 # Update the table
                 if ENCODE_PERIOD:
-                    encoded_schema_name = quote(schema_name)
-                    encoded_schema_name = encoded_schema_name.replace(
-                        ".", "%2E")
+                    encoded_schema_name = f"\"{schema_name}\""
                 else:
                     encoded_schema_name = schema_name
 
                 table_name = table.name
                 if ENCODE_PERIOD:
                     encoded_table_name = quote(table_name)
                     encoded_table_name = encoded_table_name.replace(
```

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/table.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/table.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/tagsendpoint.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tagsendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/alation_service/tokenendpoint.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/alation_service/tokenendpoint.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/az_client_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/az_client_service/azd_client.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_client_service/azd_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/az_key_vault_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/az_key_vault_service/az_key_vault.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_key_vault_service/az_key_vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,10 +190,10 @@
                     self.credential_device = self.get_credential_device()
                     self.client_device = self.get_secret_client(
                         self.credential_device)
                     secret_value = self.retrieve_secret(
                         self.client_device, secret_name)
 
                 logger.info(
-                    "Retrieve3d secret for key: {secret_name} with length: {len(secret_value)}")
+                    f"Retrieve3d secret for key: {secret_name} with length: {len(secret_value)}")
 
             return secret_value
```

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/az_storage_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/az_storage_service/az_storage_queue.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/az_storage_service/az_storage_queue.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_admin_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_admin_service/environment_logging.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_logging.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_admin_service/environment_tracing.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_admin_service/environment_tracing.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_security_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_security_service/security_core.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_security_service/security_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/dataset_metadata.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/dataset_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/environment_metadata.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/environment_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/job_metadata.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/job_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/logging_metadata.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/logging_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_self_service/pipeline_metadata.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_self_service/pipeline_metadata.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_convert.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_crud.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/dataset_extract.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_core.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_file.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1115,31 +1115,35 @@
                 file_data, overwrite=True, max_concurrency=5)
         except Exception as ex:
             print(ex)
             result = "upload failed"
         return result
 
     @staticmethod
-    def get_latest_file(path, file_type=None):
+    def get_latest_file(path, file_type=None, prefix=None):
         """
         Gets the most recently modified file in a given directory.
 
         Args:
             path (str): The path to the directory to search.
+            file_type (str): File extension to filter by.
+            prefix (str): Prefix to filter files by.
 
         Returns:
             str: The full path of the most recently modified file. If the directory is empty or does not exist, 
             returns an empty string.
         """
         files = glob.glob(os.path.join(path, "*"))
-        if "." not in file_type:
-            file_type = "." + file_type
-
         if file_type:
+            if "." not in file_type:
+                file_type = "." + file_type
             files = [file for file in files if file.endswith(f"{file_type}")]
+        if prefix:
+            files = [file for file in files if os.path.basename(
+                file).startswith(prefix)]
         if not files:  # If no files found, return None
             return None
         latest_file = max(files, key=os.path.getctime)
         return latest_file
 
     @staticmethod
     def create_tar_gz_for_folder(folder_name, output_file_name_no_extension):
```

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_http.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_http.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/environment_spark.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/job_core.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/job_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/cdc_tech_environment_service/repo_core.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/cdc_tech_environment_service/repo_core.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/directory_paths.txt` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/directory_paths.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/github_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/github_service/github_secret.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/github_service/github_secret.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/jira_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/jira_service/jira_client.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/jira_service/jira_client.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/posit_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/posit_service/posit_connect.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/posit_service/posit_connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import os
-from azure.storage.queue import QueueServiceClient
-from azure.identity import ClientSecretCredential
 import requests
 from typing import List
 import json
 
 from data_ecosystem_services.cdc_admin_service import (
     environment_tracing as pade_env_tracing,
     environment_logging as pade_env_logging
@@ -180,45 +178,52 @@
             swagger_file (str): The path to the Swagger specification file. This file describes the structure of the API that the application will provide.
             requirements_file (str): The path to the requirements.txt file. This file lists the Python packages that the application requires to run.
 
         Returns:
             str: The path to the generated manifest.json file. This file includes a summary of the application's structure and dependencies.
         """
 
+        pade_env_tracing.TracerSingleton.log_to_console = False
         logger_singleton = pade_env_logging.LoggerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         logger = logger_singleton.get_logger()
-        pade_env_tracing.TracerSingleton.log_to_console = False
         tracer_singleton = pade_env_tracing.TracerSingleton.instance(
             NAMESPACE_NAME, SERVICE_NAME)
         tracer = tracer_singleton.get_tracer()
 
         with tracer.start_as_current_span("generate_manifest"):
 
             # Load the Swagger JSON file
-            with open(swagger_file, "rb", encoding="utf-8") as f:
-                swagger = json.load(f)
+            with open(swagger_file, "rb", encoding="utf-8") as swagger_file_handle:
+                swagger = json.load(swagger_file_handle)
+
+            logger.info(f"swagger_length: {len(swagger)}")
 
             # Load the requirements file
-            with open(requirements_file, "r", encoding="utf-8") as f:
-                requirements = [r.strip() for r in f.readlines()]
+            with open(requirements_file, "r", encoding="utf-8") as requirements_file_handle:
+                requirements = [requirements_file_line.strip(
+                ) for requirements_file_line in requirements_file_handle.readlines()]
+
+            logger.info(f"requirements_length: {len(requirements)}")
 
             # Extract version information from the Swagger data
             swagger_version = swagger['info']['version']
+            logger.info(f"swagger_version: {swagger_version}")
 
             # Extract basePath from the Swagger data
-            swagger_basePath = swagger.get('basePath', '')
+            swagger_base_path = swagger.get('basePath', '')
+            logger.info(f"swagger_basePath: {swagger_base_path}")
 
             endpoints = []
             for path, methods in swagger['paths'].items():
                 for method, info in methods.items():
                     # Check if the method is a HTTP verb
                     if method in ['get', 'post', 'put', 'delete', 'patch']:
                         endpoints.append({
-                            "path": swagger_basePath + path,  # Include basePath in the path
+                            "path": swagger_base_path + path,  # Include basePath in the path
                             "method": method.upper(),  # Convert to uppercase
                             # Use 'summary' for description
                             "description": info.get('summary', '')
                         })
 
             manifest = {
                 "name": swagger['info']['title'],
```

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/python_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/python_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/requirements.txt` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/requirements.txt`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/windows_service/__init__.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/__init__.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/data_ecosystem_services/windows_service/windows_credential.py` & `data_ecosystem_services-202307.0.5/data_ecosystem_services/windows_service/windows_credential.py`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/license.md` & `data_ecosystem_services-202307.0.5/license.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/pyproject.toml` & `data_ecosystem_services-202307.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [project.urls]
 "Homepage" = "https://test.pypi.org/project/data-ecosystem-services"
 "Documentation" = "https://gift.readthedocs.io"
 "Repository" = "https://github.com/cdcent/data-ecosystem-services"
 
 [tool.poetry]
 name="data_ecosystem_services"
-version="202307.0.4"
+version="202307.0.5"
 description="Program Agnostic Data Ecosystem (PADE) - Python Services"
 authors=["John Bowyer <zfi4@cdc.gov>"]
 readme = "readme.md"
 license="Apache"
 homepage="https://test.pypi.org/project/data-ecosystem-services"
 repository="https://github.com/cdcent/data-ecosystem-services"
 classifiers=[
```

### Comparing `data_ecosystem_services-202307.0.4/readme.md` & `data_ecosystem_services-202307.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `data_ecosystem_services-202307.0.4/PKG-INFO` & `data_ecosystem_services-202307.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-ecosystem-services
-Version: 202307.0.4
+Version: 202307.0.5
 Summary: Program Agnostic Data Ecosystem (PADE) - Python Services
 Home-page: https://test.pypi.org/project/data-ecosystem-services
 License: Apache
 Author: John Bowyer
 Author-email: zfi4@cdc.gov
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

