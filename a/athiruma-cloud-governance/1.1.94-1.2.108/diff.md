# Comparing `tmp/athiruma-cloud-governance-1.1.94.tar.gz` & `tmp/athiruma-cloud-governance-1.2.108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athiruma-cloud-governance-1.1.94.tar", last modified: Tue May 16 15:00:04 2023, max compression
+gzip compressed data, was "athiruma-cloud-governance-1.2.108.tar", last modified: Mon Jun  5 18:05:24 2023, max compression
```

## Comparing `athiruma-cloud-governance-1.1.94.tar` & `athiruma-cloud-governance-1.2.108.tar`

### file list

```diff
@@ -1,216 +1,228 @@
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.843766 athiruma-cloud-governance-1.1.94/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/LICENSE
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      100 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/MANIFEST.in
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-05-16 15:00:04.843766 athiruma-cloud-governance-1.1.94/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/README.md
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.811766 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14832 2023-05-16 15:00:04.000000 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/PKG-INFO
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9295 2023-05-16 15:00:04.000000 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/SOURCES.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-05-16 15:00:04.000000 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/dependency_links.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-05-16 15:00:04.000000 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/not-zip-safe
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-05-16 15:00:04.000000 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/requires.txt
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-05-16 15:00:04.000000 athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/top_level.txt
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.811766 athiruma-cloud-governance-1.1.94/cloud_governance/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.811766 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.811766 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.812766 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12256 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11138 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11021 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5355 2023-05-16 14:59:43.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7250 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.812766 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1439 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.812766 athiruma-cloud-governance-1.1.94/cloud_governance/common/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.812766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.812766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.813766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13290 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.813766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-04-28 14:53:44.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.813766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4803 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.813766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.814766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19858 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.814766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1797 2023-05-04 18:16:50.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/iam_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.815766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/price.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/resources_pricing.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.816766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11967 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/s3_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.816766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/sts/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/sts/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/sts/sts_oprations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.816766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3210 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/utils.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.817766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.817766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.818766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.818766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/google_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.819766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.819766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/ibm_account.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.820766 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/classic_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.821766 athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2523 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elastic_upload.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11551 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elasticsearch_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.822766 athiruma-cloud-governance-1.1.94/cloud_governance/common/google_drive/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/google_drive/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/google_drive/google_drive_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/google_drive/upload_to_gsheet.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.823766 athiruma-cloud-governance-1.1.94/cloud_governance/common/jira/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/jira/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/jira/jira.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/jira/jira_operations.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.823766 athiruma-cloud-governance-1.1.94/cloud_governance/common/ldap/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/ldap/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/ldap/ldap_search.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.824766 athiruma-cloud-governance-1.1.94/cloud_governance/common/logger/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/logger/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      466 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/logger/init_logger.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1578 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/logger/logger_time_stamp.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.825766 athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/gmail.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15240 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/mail_message.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6306 2023-05-16 14:12:25.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/postfix.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.825766 athiruma-cloud-governance-1.1.94/cloud_governance/common/tool/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/tool/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/common/tool/tool.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.826766 athiruma-cloud-governance-1.1.94/cloud_governance/main/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/main/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18288 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/main/environment_variables.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/main/environment_variables_exceptions.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/main/es_uploader.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16298 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/main/main.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/main/run_cloud_resource_orchestration.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.826766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.830766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7428 2023-05-01 19:09:57.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6305 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15631 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer_payer_billings.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5350 2023-03-03 18:04:44.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_in_use.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4452 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9741 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_idle.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_run.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8141 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_stop.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2538 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/empty_roles.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3027 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ip_unattached.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6776 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/monthly_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2906 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/nat_gateway_unused.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2839 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/s3_inactive.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5680 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/skipped_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51727 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_cluster_resource.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3505 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_snapshots.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.830766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/azure/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.831766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/gcp/cost_billing_reports.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.833766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-05-08 04:46:20.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/cost_billing_reports.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_over_usage.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5384 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_report.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_baremetal.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4583 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_vm.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.833766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.833766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.833766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.834766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.835766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25600 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3811 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41752 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.836766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8869 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11803 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6139 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.837766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.839766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9166 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14370 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.839766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17153 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1712 2023-05-16 14:05:39.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.840766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.840766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.841766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3795 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.841766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/__init__.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.841766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
-drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-05-16 15:00:04.842766 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-05-16 15:00:04.843766 athiruma-cloud-governance-1.1.94/setup.cfg
--rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2928 2023-05-16 15:00:02.000000 athiruma-cloud-governance-1.1.94/setup.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11357 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/LICENSE
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      181 2023-06-05 17:39:13.000000 athiruma-cloud-governance-1.2.108/MANIFEST.in
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14833 2023-06-05 18:05:24.343894 athiruma-cloud-governance-1.2.108/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14122 2023-05-17 09:33:23.000000 athiruma-cloud-governance-1.2.108/README.md
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.331894 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14833 2023-06-05 18:05:24.000000 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/PKG-INFO
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9785 2023-06-05 18:05:24.000000 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/SOURCES.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-06-05 18:05:24.000000 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/dependency_links.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        1 2023-06-05 18:05:24.000000 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/not-zip-safe
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      608 2023-06-05 18:05:24.000000 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/requires.txt
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       17 2023-06-05 18:05:24.000000 athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/top_level.txt
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.331894 athiruma-cloud-governance-1.2.108/cloud_governance/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.331894 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.331894 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    15932 2023-06-05 16:07:17.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13037 2023-06-05 16:07:17.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3473 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11247 2023-06-01 02:43:42.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5359 2023-06-01 03:19:52.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7250 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/monitor/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/monitor/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1539 2023-05-31 11:17:10.000000 athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/common/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudtrail/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudtrail/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    13416 2023-05-17 09:33:23.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.332893 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudwatch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudwatch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2312 2023-04-28 14:53:44.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.333894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cost_explorer/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cost_explorer/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8012 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cost_explorer/cost_explorer_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.333894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/dynamodb/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/dynamodb/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4916 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.333894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/ec2/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/ec2/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    21038 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/ec2/ec2_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.333894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/iam/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/iam/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2159 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/iam/iam_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.333894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/price/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/price/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5501 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/price/price.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1599 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/price/resources_pricing.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.333894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/s3/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/s3/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12090 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/s3/s3_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/savingsplan/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/savingsplan/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3927 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/savingsplan/savings_plans_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/sts/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/sts/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      376 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/sts/sts_oprations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/utils/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/utils/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3279 2023-05-17 09:33:23.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/utils/utils.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/cost_management/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/cost_management/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3647 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/subscriptions/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/subscriptions/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2143 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1746 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/gcp/google_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.334894 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/account/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/account/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8637 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/account/ibm_account.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.335893 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/classic/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/classic/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3531 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/classic/classic_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.335893 athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2576 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/elastic_upload.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      484 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/elasticsearch_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    11743 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/elasticsearch_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.335893 athiruma-cloud-governance-1.2.108/cloud_governance/common/google_drive/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/google_drive/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8244 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/google_drive/google_drive_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10366 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/google_drive/upload_to_gsheet.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.335893 athiruma-cloud-governance-1.2.108/cloud_governance/common/jira/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/jira/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9020 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/jira/jira.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9134 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/jira/jira_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.335893 athiruma-cloud-governance-1.2.108/cloud_governance/common/ldap/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/ldap/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2500 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/ldap/ldap_search.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.336894 athiruma-cloud-governance-1.2.108/cloud_governance/common/logger/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/logger/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      456 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/logger/init_logger.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1637 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/logger/logger_time_stamp.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.336894 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1858 2023-04-16 06:07:13.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/gmail.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19703 2023-06-05 17:43:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/mail_message.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6410 2023-06-05 17:45:02.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/postfix.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.336894 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/templates/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1018 2023-06-01 02:43:42.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/templates/cro_request_for_manager_approval.j2
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.336894 athiruma-cloud-governance-1.2.108/cloud_governance/common/tool/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/tool/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      248 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/common/tool/tool.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.337894 athiruma-cloud-governance-1.2.108/cloud_governance/main/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    19841 2023-06-01 03:19:28.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/environment_variables.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      437 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/environment_variables_exceptions.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10656 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/es_uploader.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    16465 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/main.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      366 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/main_common_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      776 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/main/run_cloud_resource_orchestration.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.337894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.338894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7429 2023-06-01 02:21:54.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7322 2023-05-17 09:33:23.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_explorer.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    18530 2023-06-01 02:43:42.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_explorer_payer_billings.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5351 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      616 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ebs_in_use.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4559 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ebs_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9743 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ec2_idle.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1592 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ec2_run.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8185 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ec2_stop.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2774 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/empty_roles.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3233 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ip_unattached.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6778 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/monthly_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2914 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/s3_inactive.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5684 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/skipped_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4948 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/unused_nat_gateway.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    51750 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/zombie_cluster_resource.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3588 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/zombie_snapshots.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.338894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10216 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/azure/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.338894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/common_policies/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/common_policies/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     7140 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/common_policies/send_aggregated_alerts.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.339894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14218 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/gcp/cost_billing_reports.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.339894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-01-13 08:45:30.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4118 2023-05-08 04:46:20.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/cost_billing_reports.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3595 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/ibm_cost_over_usage.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5385 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/ibm_cost_report.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4997 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/tag_baremetal.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     4584 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/tag_vm.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.339894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.339894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.339894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/cost_expenditure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/cost_expenditure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1060 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.339894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1900 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2534 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.340894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    25603 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     5115 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3811 2023-05-31 05:52:32.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    41961 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.340894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9497 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     8362 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2613 2023-04-20 10:33:28.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    12945 2023-05-17 09:33:23.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     6140 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.341894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3389 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1968 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2912 2023-03-22 05:22:40.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    10510 2023-04-18 07:27:25.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.341894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    27642 2023-03-23 05:18:00.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3470 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1373 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     9167 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1164 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    14304 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.341894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)    17154 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1775 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/azure/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/azure/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1129 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gcp/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gcp/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1116 2023-03-17 06:23:24.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gitleaks/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gitleaks/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     3796 2023-05-19 17:31:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/__init__.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/ibm_operations/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)      625 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1123 2023-05-15 10:36:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/tagging/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2357 2023-03-09 05:50:15.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+drwxrwxr-x   0 athiruma (4206838) athiruma (4206838)        0 2023-06-05 18:05:24.342894 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_runners/
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)        0 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_runners/__init__.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     1174 2023-05-19 08:12:08.000000 athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_runners/common_policy_runner.py
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)       79 2023-06-05 18:05:24.352894 athiruma-cloud-governance-1.2.108/setup.cfg
+-rw-rw-r--   0 athiruma (4206838) athiruma (4206838)     2929 2023-06-05 18:04:02.000000 athiruma-cloud-governance-1.2.108/setup.py
```

### Comparing `athiruma-cloud-governance-1.1.94/LICENSE` & `athiruma-cloud-governance-1.2.108/LICENSE`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/PKG-INFO` & `athiruma-cloud-governance-1.2.108/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiruma-cloud-governance
-Version: 1.1.94
+Version: 1.2.108
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -50,15 +50,15 @@
 * [tag_non_cluster](cloud_governance/policy/policy_operations/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
 * [tag_iam_user](cloud_governance/policy/policy_operations/aws/tag_user): update the user tags from the csv file
 * [cost_explorer](cloud_governance/policy/aws/cost_explorer.py): Get data from cost explorer and upload to ElasticSearch
 * [ip_unattached](cloud_governance/policy/aws/ip_unattached.py): Get the unattached IP and delete it after 7 days.
 * [s3_inactive](cloud_governance/policy/aws/s3_inactive.py): Get the inactive/empty buckets and delete them after 7 days.
 * [empty_roles](cloud_governance/policy/aws/empty_roles.py): Get empty roles and delete it after 7 days.
 * [zombie_snapshots](cloud_governance/policy/aws/zombie_snapshots.py): Get the zombie snapshots and delete it after 7 days.
-* [nat_gateway_unused](cloud_governance/policy/aws/nat_gateway_unused.py): Get the unused nat gateways and deletes it after 7 days.
+* [nat_gateway_unused](cloud_governance/policy/aws/unused_nat_gateway.py): Get the unused nat gateways and deletes it after 7 days.
 * gitleaks: scan Github repository git leak (security scan)  
 * [cost_over_usage](cloud_governance/policy/aws/cost_over_usage.py): send mail to aws user if over usage cost
 
 [IBM policies](cloud_governance/policy/ibm)
 
 * [tag_baremetal](cloud_governance/policy/ibm/tag_baremetal.py): Tag IBM baremetal machines
 * [tag_vm](cloud_governance/policy/ibm/tag_vm.py): Tga IBM Virtual Machines machines
```

### Comparing `athiruma-cloud-governance-1.1.94/README.md` & `athiruma-cloud-governance-1.2.108/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 * [tag_non_cluster](cloud_governance/policy/policy_operations/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
 * [tag_iam_user](cloud_governance/policy/policy_operations/aws/tag_user): update the user tags from the csv file
 * [cost_explorer](cloud_governance/policy/aws/cost_explorer.py): Get data from cost explorer and upload to ElasticSearch
 * [ip_unattached](cloud_governance/policy/aws/ip_unattached.py): Get the unattached IP and delete it after 7 days.
 * [s3_inactive](cloud_governance/policy/aws/s3_inactive.py): Get the inactive/empty buckets and delete them after 7 days.
 * [empty_roles](cloud_governance/policy/aws/empty_roles.py): Get empty roles and delete it after 7 days.
 * [zombie_snapshots](cloud_governance/policy/aws/zombie_snapshots.py): Get the zombie snapshots and delete it after 7 days.
-* [nat_gateway_unused](cloud_governance/policy/aws/nat_gateway_unused.py): Get the unused nat gateways and deletes it after 7 days.
+* [nat_gateway_unused](cloud_governance/policy/aws/unused_nat_gateway.py): Get the unused nat gateways and deletes it after 7 days.
 * gitleaks: scan Github repository git leak (security scan)  
 * [cost_over_usage](cloud_governance/policy/aws/cost_over_usage.py): send mail to aws user if over usage cost
 
 [IBM policies](cloud_governance/policy/ibm)
 
 * [tag_baremetal](cloud_governance/policy/ibm/tag_baremetal.py): Tag IBM baremetal machines
 * [tag_vm](cloud_governance/policy/ibm/tag_vm.py): Tga IBM Virtual Machines machines
```

### Comparing `athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/PKG-INFO` & `athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athiruma-cloud-governance
-Version: 1.1.94
+Version: 1.2.108
 Summary: Cloud Governance Tool
 Home-page: https://github.com/redhat-performance/cloud-governance
 Author: Red Hat
 Author-email: ebattat@redhat.com, athiruma@redhat.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
@@ -50,15 +50,15 @@
 * [tag_non_cluster](cloud_governance/policy/policy_operations/aws/tag_non_cluster): tag ec2 resources (instance, volume, ami, snapshot) by instance name
 * [tag_iam_user](cloud_governance/policy/policy_operations/aws/tag_user): update the user tags from the csv file
 * [cost_explorer](cloud_governance/policy/aws/cost_explorer.py): Get data from cost explorer and upload to ElasticSearch
 * [ip_unattached](cloud_governance/policy/aws/ip_unattached.py): Get the unattached IP and delete it after 7 days.
 * [s3_inactive](cloud_governance/policy/aws/s3_inactive.py): Get the inactive/empty buckets and delete them after 7 days.
 * [empty_roles](cloud_governance/policy/aws/empty_roles.py): Get empty roles and delete it after 7 days.
 * [zombie_snapshots](cloud_governance/policy/aws/zombie_snapshots.py): Get the zombie snapshots and delete it after 7 days.
-* [nat_gateway_unused](cloud_governance/policy/aws/nat_gateway_unused.py): Get the unused nat gateways and deletes it after 7 days.
+* [nat_gateway_unused](cloud_governance/policy/aws/unused_nat_gateway.py): Get the unused nat gateways and deletes it after 7 days.
 * gitleaks: scan Github repository git leak (security scan)  
 * [cost_over_usage](cloud_governance/policy/aws/cost_over_usage.py): send mail to aws user if over usage cost
 
 [IBM policies](cloud_governance/policy/ibm)
 
 * [tag_baremetal](cloud_governance/policy/ibm/tag_baremetal.py): Tag IBM baremetal machines
 * [tag_vm](cloud_governance/policy/ibm/tag_vm.py): Tga IBM Virtual Machines machines
```

### Comparing `athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/SOURCES.txt` & `athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 cloud_governance/common/clouds/aws/iam/__init__.py
 cloud_governance/common/clouds/aws/iam/iam_operations.py
 cloud_governance/common/clouds/aws/price/__init__.py
 cloud_governance/common/clouds/aws/price/price.py
 cloud_governance/common/clouds/aws/price/resources_pricing.py
 cloud_governance/common/clouds/aws/s3/__init__.py
 cloud_governance/common/clouds/aws/s3/s3_operations.py
+cloud_governance/common/clouds/aws/savingsplan/__init__.py
+cloud_governance/common/clouds/aws/savingsplan/savings_plans_operations.py
 cloud_governance/common/clouds/aws/sts/__init__.py
 cloud_governance/common/clouds/aws/sts/sts_oprations.py
 cloud_governance/common/clouds/aws/utils/__init__.py
 cloud_governance/common/clouds/aws/utils/utils.py
 cloud_governance/common/clouds/azure/__init__.py
 cloud_governance/common/clouds/azure/cost_management/__init__.py
 cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py
@@ -72,21 +74,23 @@
 cloud_governance/common/logger/__init__.py
 cloud_governance/common/logger/init_logger.py
 cloud_governance/common/logger/logger_time_stamp.py
 cloud_governance/common/mails/__init__.py
 cloud_governance/common/mails/gmail.py
 cloud_governance/common/mails/mail_message.py
 cloud_governance/common/mails/postfix.py
+cloud_governance/common/mails/templates/cro_request_for_manager_approval.j2
 cloud_governance/common/tool/__init__.py
 cloud_governance/common/tool/tool.py
 cloud_governance/main/__init__.py
 cloud_governance/main/environment_variables.py
 cloud_governance/main/environment_variables_exceptions.py
 cloud_governance/main/es_uploader.py
 cloud_governance/main/main.py
+cloud_governance/main/main_common_operations.py
 cloud_governance/main/run_cloud_resource_orchestration.py
 cloud_governance/policy/__init__.py
 cloud_governance/policy/aws/__init__.py
 cloud_governance/policy/aws/cost_billing_reports.py
 cloud_governance/policy/aws/cost_explorer.py
 cloud_governance/policy/aws/cost_explorer_payer_billings.py
 cloud_governance/policy/aws/cost_over_usage.py
@@ -94,21 +98,23 @@
 cloud_governance/policy/aws/ebs_unattached.py
 cloud_governance/policy/aws/ec2_idle.py
 cloud_governance/policy/aws/ec2_run.py
 cloud_governance/policy/aws/ec2_stop.py
 cloud_governance/policy/aws/empty_roles.py
 cloud_governance/policy/aws/ip_unattached.py
 cloud_governance/policy/aws/monthly_report.py
-cloud_governance/policy/aws/nat_gateway_unused.py
 cloud_governance/policy/aws/s3_inactive.py
 cloud_governance/policy/aws/skipped_resources.py
+cloud_governance/policy/aws/unused_nat_gateway.py
 cloud_governance/policy/aws/zombie_cluster_resource.py
 cloud_governance/policy/aws/zombie_snapshots.py
 cloud_governance/policy/azure/__init__.py
 cloud_governance/policy/azure/cost_billing_reports.py
+cloud_governance/policy/common_policies/__init__.py
+cloud_governance/policy/common_policies/send_aggregated_alerts.py
 cloud_governance/policy/gcp/__init__.py
 cloud_governance/policy/gcp/cost_billing_reports.py
 cloud_governance/policy/ibm/__init__.py
 cloud_governance/policy/ibm/cost_billing_reports.py
 cloud_governance/policy/ibm/ibm_cost_over_usage.py
 cloud_governance/policy/ibm/ibm_cost_report.py
 cloud_governance/policy/ibm/tag_baremetal.py
@@ -153,8 +159,10 @@
 cloud_governance/policy/policy_operations/gitleaks/__init__.py
 cloud_governance/policy/policy_operations/gitleaks/gitleaks.py
 cloud_governance/policy/policy_operations/ibm/__init__.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/__init__.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py
 cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py
 cloud_governance/policy/policy_operations/ibm/tagging/__init__.py
-cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py
+cloud_governance/policy/policy_runners/__init__.py
+cloud_governance/policy/policy_runners/common_policy_runner.py
```

### Comparing `athiruma-cloud-governance-1.1.94/athiruma_cloud_governance.egg-info/requires.txt` & `athiruma-cloud-governance-1.2.108/athiruma_cloud_governance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/collect_cro_reports.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,104 @@
+import logging
 from datetime import datetime, timedelta
 
 import typeguard
 
 from cloud_governance.cloud_resource_orchestration.aws.ec2.cost_over_usage import CostOverUsage
 from cloud_governance.cloud_resource_orchestration.aws.ec2.monitor_tickets import MonitorTickets
+from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
 from cloud_governance.common.jira.jira_operations import JiraOperations
+from cloud_governance.common.logger.init_logger import handler
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class CollectCROReports:
     """
     This method collects the user/instance-id data from the cost-explorer
     """
 
     DEFAULT_ROUND_DIGITS = 3
     ZERO = 0
+    TICKET_ID_KEY = 'ticket_id'
+    COST_EXPLORER_TAGS = {TICKET_ID_KEY: 'TicketId'}
+    AND = 'And'
+    ALLOCATED_BUDGET = 'AllocatedBudget'
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__account_name = self.__environment_variables_dict.get('account', '').replace('OPENSHIFT-', '').strip()
         self.__cost_over_usage = CostOverUsage()
         self.jira_operations = JiraOperations()
         self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME', '')
         self.__es_index_cro = self.__environment_variables_dict.get('CRO_ES_INDEX', '')
+        self.__account_id = IAMOperations().get_aws_account_id_name()
+        self.__ce_payer_index = self.__environment_variables_dict.get('CE_PAYER_INDEX')
+
+    def get_account_budget_from_payer_ce_report(self):
+        """
+        This method returns the account budget from the payer ce reports
+        Check policy cost_explorer_payer_billings
+        :return:
+        """
+        query = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"term": {"CloudName.keyword": self.__public_cloud_name}},
+                        {"term": {"AccountId.keyword": self.__account_id}},
+                        {"term": {"Month": str(datetime.utcnow().year)}},
+                    ]
+                }
+            },
+            "size": 1
+        }
+        response = self.__cost_over_usage.es_operations.fetch_data_by_es_query(query=query, es_index=self.__ce_payer_index, search_size=1, limit_to_size=True)
+        if response:
+            return response[0].get('_source').get(self.ALLOCATED_BUDGET)
+        return 0
+
+    def get_total_account_usage_cost(self):
+        """
+        This method returns the total account budget till date for this year
+        :return:
+        """
+        current_date = datetime.utcnow().date()
+        start_date = datetime(current_date.year, 1, 1).date()
+        cost_explorer_operations = self.__cost_over_usage.get_cost_explorer_operations()
+        response = cost_explorer_operations.get_cost_and_usage_from_aws(start_date=str(start_date), end_date=str(current_date+timedelta(days=1)), granularity='MONTHLY')
+        total_cost = cost_explorer_operations.get_filter_data(ce_data=response['ResultsByTime'], group_by=False)
+        return total_cost
 
     @typeguard.typechecked
     @logger_time_stamp
-    def get_user_cost_data(self, user: str, requested_date: datetime, user_project: str = '', forecast: bool = False, duration: int = 0):
+    def get_user_cost_data(self, group_by_tag_name: str, group_by_tag_value: str, requested_date: datetime = '', forecast: bool = False, duration: int = 0, extra_filter_key_values: dict = None):
         """
         This method fetch data from the es_reports
+        :param extra_filter_key_values:
+        :param group_by_tag_value:
+        :param group_by_tag_name:
         :param duration:
         :param forecast:
-        :param user_project:
-        :param user:
         :param requested_date:
         :return:
         """
+        extra_filter_matches = [{'Tags': {'Key': group_by_tag_name, 'Values': [group_by_tag_value]}}]
+        if extra_filter_key_values:
+            extra_filter_matches.extend([{'Tags': {'Key': filter_key, 'Values': [filter_value]}} for filter_key, filter_value in extra_filter_key_values.items()])
+        start_date = requested_date.replace(minute=self.ZERO, hour=self.ZERO, second=self.ZERO, microsecond=self.ZERO)
         if forecast:
-            current_date = requested_date.replace(minute=self.ZERO, hour=self.ZERO, second=self.ZERO, microsecond=self.ZERO)
-            end_date = current_date + timedelta(days=duration)
-            response = self.__cost_over_usage.get_forecast_cost_data(start_date=current_date, end_date=end_date,
-                                                                     extra_matches=[{'Tags': {'Key': 'User', 'Values': [user]}},
-                                                                                    {'Tags': {'Key': 'Project', 'Values': [user_project]}}], extra_operation='And', tag_name='User')
+            end_date = start_date + timedelta(days=duration)
+            response = self.__cost_over_usage.get_forecast_cost_data(start_date=start_date, end_date=end_date,
+                                                                     extra_matches=extra_filter_matches, extra_operation=self.AND, tag_name=group_by_tag_name)
             return_key = 'Forecast'
         else:
-            jira_created_date = requested_date.replace(minute=self.ZERO, hour=self.ZERO, second=self.ZERO, microsecond=self.ZERO)
-            response = self.__cost_over_usage.get_monthly_user_es_cost_data(start_date=jira_created_date,
+            response = self.__cost_over_usage.get_monthly_user_es_cost_data(start_date=start_date,
                                                                             end_date=datetime.utcnow().replace(microsecond=self.ZERO) + timedelta(days=1),
-                                                                            extra_matches=[{'Tags': {'Key': 'User', 'Values': [user]}}, {'Tags': {'Key': 'Project', 'Values': [user_project]}}], extra_operation='And', tag_name='User')
+                                                                            extra_matches=extra_filter_matches, extra_operation=self.AND, tag_name=group_by_tag_name)
             return_key = 'Cost'
         if response:
             return round(response[self.ZERO].get(return_key), self.DEFAULT_ROUND_DIGITS)
         return self.ZERO
 
     @typeguard.typechecked
     @logger_time_stamp
@@ -84,18 +130,20 @@
             'duration': int(instance_data[self.ZERO].get('duration')),
             'approved_manager': instance_data[self.ZERO].get('approved_manager'),
             'user_manager': instance_data[self.ZERO].get('manager'),
             'project': instance_data[self.ZERO].get('project'),
             'owner': instance_data[self.ZERO].get('owner'),
             'total_spots': len([instance for instance in instance_data if instance.get('instance_plan').lower() == 'spot']),
             'total_ondemand': len([instance for instance in instance_data if instance.get('instance_plan').lower() == 'ondemand']),
+            self.ALLOCATED_BUDGET: self.get_account_budget_from_payer_ce_report(),
             'instances': [f"{instance.get('instance_name')}, {instance.get('instance_id')}, "
                           f"{instance.get('instance_plan')}, "
                           f"{instance.get('instance_type')}, "
-                          f"{instance.get('instance_state')}, {instance.get('instance_running_days')}" for instance in instance_data]
+                          f"{instance.get('instance_state')}, {instance.get('instance_running_days')}" for instance in instance_data],
+            'instance_types': [instance.get('instance_type') for instance in instance_data]
         }
 
     @typeguard.typechecked
     @logger_time_stamp
     def __prepare_update_es_data(self, source: dict, instance_data: list, user_cost: float, cost_estimation: float):
         """
         This method update the values of jira id data
@@ -112,14 +160,18 @@
                 source['instances'][index[self.ZERO]] = f"{instance.get('instance_name')}, {instance.get('instance_id')}, " \
                                                 f"{instance.get('instance_plan')}, {instance.get('instance_type')}, " \
                                                 f"{instance.get('instance_state')}, {running_days}"
             else:
                 source['instances'].append(f"{instance.get('instance_name')}, {instance.get('instance_id')}, "
                                            f"{instance.get('instance_plan')}, {instance.get('instance_type')}, "
                                            f"{instance.get('instance_state')}, {running_days}")
+                if source.get('instance_types'):
+                    source['instance_types'].append(instance.get('instance_type'))
+                else:
+                    source['instance_types'] = [instance.get('instance_type')]
                 if instance.get('instance_plan').lower() == 'spot':
                     source['total_spots'] = source.get('total_spots') + 1
                 else:
                     if instance.get('instance_plan').lower() == 'ondemand':
                         source['total_ondemand'] = source.get('total_ondemand') + 1
         MonitorTickets().verify_es_instances_state(es_data=source)
         if datetime.strptime(source.get('timestamp'), "%Y-%m-%dT%H:%M:%S.%f").date() != datetime.now().date():
@@ -145,17 +197,20 @@
         """
         upload_data = {}
         for ticket_id, instance_data in monitor_data.items():
             user = instance_data[self.ZERO].get('user')
             user_project = instance_data[self.ZERO].get('project')
             issue_description = self.jira_operations.get_issue_description(ticket_id=ticket_id, state='ANY')
             ticket_opened_date = issue_description.get('TicketOpenedDate')
-            user_cost = self.get_user_cost_data(user, requested_date=ticket_opened_date, user_project=user_project)
+            group_by_tag_name = self.COST_EXPLORER_TAGS[self.TICKET_ID_KEY]
+            user_cost = self.get_user_cost_data(group_by_tag_name=group_by_tag_name, group_by_tag_value=ticket_id,
+                                                requested_date=ticket_opened_date,
+                                                extra_filter_key_values={'Project': user_project})
             duration = int(instance_data[self.ZERO].get('duration', 0))
-            user_forecast = self.get_user_cost_data(user, requested_date=datetime.utcnow(), user_project=user_project, forecast=True, duration=duration)
+            user_forecast = self.get_user_cost_data(group_by_tag_name=group_by_tag_name, group_by_tag_value=ticket_id, requested_date=datetime.utcnow(), extra_filter_key_values={'Project': user_project}, forecast=True, duration=duration)
             cost_estimation = float(instance_data[self.ZERO].get('estimated_cost', self.ZERO))
             if self.__cost_over_usage.es_operations.verify_elastic_index_doc_id(index=self.__cost_over_usage.es_index_cro, doc_id=ticket_id):
                 es_data = self.__cost_over_usage.es_operations.get_es_data_by_id(id=ticket_id, index=self.__cost_over_usage.es_index_cro)
                 es_data['_source']['ticket_opened_date'] = ticket_opened_date.date()
                 es_data['_source']['forecast'] = user_forecast
                 es_data['_source']['user'] = user
                 source = self.__prepare_update_es_data(source=es_data.get('_source'), instance_data=instance_data, cost_estimation=cost_estimation, user_cost=user_cost)
@@ -163,43 +218,55 @@
                 upload_data[ticket_id] = source
             else:
                 if ticket_id not in upload_data:
                     source = self.prepare_instance_data(instance_data=instance_data, ticket_id=ticket_id, cost_estimation=cost_estimation, user=user,  user_cost=user_cost, ticket_opened_date=ticket_opened_date)
                     source['ticket_opened_date'] = ticket_opened_date.date()
                     source['forecast'] = user_forecast
                     source['user'] = user
+                    if not source.get(self.ALLOCATED_BUDGET):
+                        source[self.ALLOCATED_BUDGET] = self.get_account_budget_from_payer_ce_report()
                     self.__cost_over_usage.es_operations.upload_to_elasticsearch(index=self.__es_index_cro, data=source, id=ticket_id)
                     upload_data[ticket_id] = source
         return upload_data
 
     @logger_time_stamp
     def update_in_progress_ticket_cost(self):
         """
         This method updates the in-progress tickets costs
         :return:
         """
-        query = {"query": {"match_phrase": {"ticket_id_state.keyword": "in-progress"}}}
+        query = {"query": {"bool": {"must": [
+                        {"term": {"cloud_name.keyword": self.__public_cloud_name}},
+                        {"term": {"account_name.keyword": self.__account_name.upper()}},
+                        {"term": {"ticket_id_state.keyword": "in-progress"}}
+                    ]
+                }}}
         in_progress_es_tickets = self.__cost_over_usage.es_operations.fetch_data_by_es_query(query=query, es_index=self.__es_index_cro)
+        total_account_cost = self.get_total_account_usage_cost()
         for in_progress_ticket in in_progress_es_tickets:
             source_data = in_progress_ticket.get('_source')
-            ticket_id = source_data.get('ticket_id')
+            ticket_id = source_data.get(self.TICKET_ID_KEY)
             if source_data.get('account_name').lower() in self.__account_name.lower():
-                user = source_data.get('user', '')
-                if not user:
-                    user = source_data.get('user_cro')
                 ticket_opened_date = datetime.strptime(source_data.get('ticket_opened_date'), "%Y-%m-%d")
                 duration = int(source_data.get('duration', 0))
                 user_project = source_data.get('project')
-                user_cost = self.get_user_cost_data(user, requested_date=ticket_opened_date, user_project=user_project)
-                user_forecast = self.get_user_cost_data(user, requested_date=datetime.utcnow(), user_project=user_project, forecast=True, duration=duration)
-                update_data = {'actual_cost': user_cost, 'forecast': user_forecast, 'timestamp': datetime.utcnow()}
+                group_by_tag_name = self.COST_EXPLORER_TAGS[self.TICKET_ID_KEY]
+                user_cost = self.get_user_cost_data(group_by_tag_name=group_by_tag_name, group_by_tag_value=ticket_id, requested_date=ticket_opened_date)
+                user_forecast = self.get_user_cost_data(group_by_tag_name=group_by_tag_name, group_by_tag_value=ticket_id, requested_date=datetime.utcnow(), forecast=True, duration=duration)
+                update_data = {'actual_cost': user_cost, 'forecast': user_forecast, 'timestamp': datetime.utcnow(), f'TotalCurrentUsage-{datetime.utcnow().year}': total_account_cost}
+                if not source_data.get(self.ALLOCATED_BUDGET):
+                    update_data[self.ALLOCATED_BUDGET] = self.get_account_budget_from_payer_ce_report()
                 self.__cost_over_usage.es_operations.update_elasticsearch_index(index=self.__es_index_cro, metadata=update_data, id=ticket_id)
 
     @typeguard.typechecked
     @logger_time_stamp
     def run(self, monitor_data: dict):
         """
-        This method run data collection methods
+        This method runs data collection methods
         :param monitor_data:
         :return:
         """
-        return self.__upload_cro_report_to_es(monitor_data=monitor_data)
+        handler.setLevel(logging.WARN)
+        result = self.__upload_cro_report_to_es(monitor_data=monitor_data)
+        handler.setLevel(logging.WARN)
+        return result
+
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/cost_over_usage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,35 @@
+import logging
 from datetime import datetime, timedelta
 
-import boto3
 import typeguard
 
 from cloud_governance.common.clouds.aws.cost_explorer.cost_explorer_operations import CostExplorerOperations
 from cloud_governance.common.elasticsearch.elasticsearch_operations import ElasticSearchOperations
 from cloud_governance.common.ldap.ldap_search import LdapSearch
+from cloud_governance.common.logger.init_logger import logger, handler
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.common.mails.mail_message import MailMessage
 from cloud_governance.common.mails.postfix import Postfix
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class CostOverUsage:
     """
-    This class will monitor the cost explorer reports and send alert to the user if they exceed specified amount
+    This class will monitors the cost explorer reports and sends alert to the user if they exceed specified amount
     """
 
     DEFAULT_ROUND_DIGITS = 3
+    SEND_ALERT_DAY = 3
     FORECAST_GRANULARITY = 'MONTHLY'
     FORECAST_COST_METRIC = 'UNBLENDED_COST'
     OVER_USAGE_THRESHOLD = 0.05
+    CLOUD_GOVERNANCE_ES_MAIL_INDEX = 'cloud-governance-mail-messages'
+    CRO_OVER_USAGE_ALERT = 'cro-over-usage-alert'
+    TIMESTAMP_DATE_FORMAT = "%Y-%m-%dT%H:%M:%S.%f"
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__aws_account = self.__environment_variables_dict.get('account', '').replace('OPENSHIFT-', '').strip()
         self.__postfix_mail = Postfix()
         self.__mail_message = MailMessage()
         self.__es_host = self.__environment_variables_dict.get('es_host', '')
@@ -38,182 +43,233 @@
         self.current_end_date = datetime.utcnow()
         self.current_start_date = self.current_end_date - timedelta(days=self.__cro_duration_days)
         self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME')
         self.__ce_operations = CostExplorerOperations()
         self.es_operations = ElasticSearchOperations(es_host=self.__es_host, es_port=self.__es_port)
         self.__over_usage_threshold = self.OVER_USAGE_THRESHOLD * self.__over_usage_amount
 
+    def get_cost_explorer_operations(self):
+        return self.__ce_operations
+
     @typeguard.typechecked
     @logger_time_stamp
     def get_cost_based_on_tag(self, start_date: str, end_date: str, tag_name: str, extra_filters: any = None, extra_operation: str = 'And', granularity: str = None, forecast: bool = False):
         """
         This method gives the cost based on the tag_name
         :param forecast:
         :param granularity:
         :param extra_operation: default, And
         :param extra_filters:
         :param tag_name:
         :param start_date:
         :param end_date:
         :return:
         """
-        remove_savings_cost = {  # removed the savings plan usage from the user costs
-            'Not': {
-                'Dimensions': {
-                    'Key': 'RECORD_TYPE',
-                    'Values': ['SavingsPlanRecurringFee', 'SavingsPlanNegation', 'SavingsPlanCoveredUsage']
-                }
-            }
-        }
-        Filters = remove_savings_cost
+        # remove_savings_cost = {  # removed the savings plan usage from the user costs
+        #     'Not': {
+        #         'Dimensions': {
+        #             'Key': 'RECORD_TYPE',
+        #             'Values': ['SavingsPlanRecurringFee', 'SavingsPlanNegation', 'SavingsPlanCoveredUsage']
+        #         }
+        #     }
+        # }
+        Filters = {} #remove_savings_cost
         if extra_filters:
             if type(extra_filters) == list:
-                Filters = {
-                    extra_operation: [
-                        *extra_filters,
-                        remove_savings_cost
-                    ]
-                }
+                if len(extra_filters) == 1:
+                    Filters = extra_filters[0]
+                else:
+                    Filters = {
+                        extra_operation: [
+                            *extra_filters,
+                            # remove_savings_cost
+                        ]
+                    }
             else:
                 Filters = {
-                    extra_operation: [
-                        extra_filters,
-                        remove_savings_cost
-                    ]
+                    # extra_operation: [
+                        extra_filters
+                        # remove_savings_cost
+                    # ]
                 }
         if forecast:
             results_by_time = self.__ce_operations.get_cost_forecast(start_date=start_date, end_date=end_date, granularity=self.FORECAST_GRANULARITY, cost_metric=self.FORECAST_COST_METRIC, Filter=Filters)['Total']
             response = [{'Forecast': round(float(results_by_time.get('Amount')), self.DEFAULT_ROUND_DIGITS)}]
         else:
             results_by_time = self.__ce_operations.get_cost_by_tags(start_date=start_date, end_date=end_date, tag=tag_name, Filter=Filters, granularity=granularity)['ResultsByTime']
             response = self.__ce_operations.get_filter_data(ce_data=results_by_time, tag_name=tag_name)
         return response
 
     @typeguard.typechecked
     @logger_time_stamp
     def __get_start_end_dates(self, start_date: datetime = None, end_date: datetime = None):
         """
-        This method return the start_date and end_date
+        This method returns the start_date and end_date
         :param start_date:
         :param end_date:
         :return:
         """
         if not start_date and not end_date:
             end_date = self.current_end_date.date()
             start_date = self.current_start_date.replace(day=1).date()
         elif not start_date:
             start_date = self.current_start_date.date()
             end_date = end_date.date()
         else:
             if not end_date:
                 end_date = self.current_end_date.date()
-                start_date = start_date.date()
+            else:
+                end_date = end_date.date()
             start_date = start_date.date()
-            end_date = end_date.date()
         return start_date, end_date
 
     @typeguard.typechecked
     @logger_time_stamp
     def get_monthly_user_es_cost_data(self, tag_name: str = 'User', start_date: datetime = None, end_date: datetime = None, extra_matches: any = None, granularity: str = 'MONTHLY', extra_operation: str = 'And'):
         """
-        This method get the user cost from the es-data
+        This method gets the user cost from the es-data
         :param tag_name: by default User
         :param start_date:
         :param end_date:
         :param extra_matches:
         :param granularity: by default MONTHLY
         :param extra_operation:
         :return:
         """
         start_date, end_date = self.__get_start_end_dates(start_date=start_date, end_date=end_date)
         return self.get_cost_based_on_tag(start_date=str(start_date), end_date=str(end_date), tag_name=tag_name, granularity=granularity, extra_filters=extra_matches, extra_operation=extra_operation)
 
     def get_forecast_cost_data(self, tag_name: str = 'User', start_date: datetime = None, end_date: datetime = None, extra_matches: any = None, granularity: str = 'MONTHLY', extra_operation: str = 'And'):
         """
-        This method return the forecast based on inputs
+        This method returns the forecast based on inputs
         :param tag_name: by default User
         :param start_date:
         :param end_date:
         :param extra_matches:
         :param granularity: by default MONTHLY
         :param extra_operation:
         :return:
         """
         start_date, end_date = self.__get_start_end_dates(start_date=start_date, end_date=end_date)
         return self.get_cost_based_on_tag(start_date=str(start_date), end_date=str(end_date), tag_name=tag_name, granularity=granularity, extra_filters=extra_matches, extra_operation=extra_operation, forecast=True)
 
+    def verify_user_should_open_ticket_or_not(self, user_name: str, user_cost: float):
+        """
+        This method returns a boolean indicating whether the user should open the ticket or not
+        :param user_cost:
+        :param user_name:
+        :return:
+        """
+        query = {  # check user opened the ticket in elastic_search
+            "query": {
+                "bool": {
+                    "must": [{"term": {"user": user_name}},
+                             {"term": {"ticket_id_state.keyword": 'in-progress'}},
+                             {"term": {"account_name.keyword": self.__aws_account.upper()}}
+                             ],
+                    "filter": {
+                        "range": {
+                            "timestamp": {
+                                "format": "yyyy-MM-dd",
+                                "lte": str(self.current_end_date.date()),
+                                "gte": str(self.current_start_date.date()),
+                            }
+                        }
+                    }
+                }
+            }
+        }
+        user_in_progress_tickets = self.es_operations.fetch_data_by_es_query(es_index=self.es_index_cro, query=query)
+        if not user_in_progress_tickets:
+            return True
+        else:
+            total_in_progress_tickets_cost = 0
+            for cro_data in user_in_progress_tickets:
+                opened_ticket_cost = float(cro_data.get('_source').get('estimated_cost'))
+                total_in_progress_tickets_cost += opened_ticket_cost
+            if user_cost - total_in_progress_tickets_cost > self.__over_usage_amount:
+                return True
+        return False
+
     @logger_time_stamp
     def get_cost_over_usage_users(self):
         """
         This method returns the cost over usage users which are not opened ticket
         :return:
         """
         over_usage_users = []
         current_month_users = self.get_monthly_user_es_cost_data()
         for user in current_month_users:
-            user_name = user.get('User')
-            cost = round(user.get('Cost'), self.DEFAULT_ROUND_DIGITS)
-            if cost >= (self.__over_usage_amount - self.__over_usage_threshold):
-                query = {  # check user opened the ticket in elastic_search
-                    "query": {
-                        "bool": {
-                            "must": {
-                                "term": {"user": user_name}
-                            },
-                            "filter": {
-                                "range": {
-                                    "timestamp": {
-                                        "format": "yyyy-MM-dd",
-                                        "lte": str(self.current_end_date.date()),
-                                        "gte": str(self.current_start_date.date()),
-                                    }
-                                }
-                            }
-                        }
-                    }
-                }
-                response = self.es_operations.fetch_data_by_es_query(es_index=self.es_index_cro, query=query)
-                if not response:
+            user_name = str(user.get('User'))
+            user_cost = round(user.get('Cost'), self.DEFAULT_ROUND_DIGITS)
+            if user_cost >= (self.__over_usage_amount - self.__over_usage_threshold):
+                if self.verify_user_should_open_ticket_or_not(user_name=user_name, user_cost=user_cost):
                     over_usage_users.append(user)
-                for cro_data in response:
-                    project = cro_data.get('_source').get('project')
-                    ticket_id_state = cro_data.get('_source').get('ticket_id_state')
-                    if 'close' in ticket_id_state.lower():
-                        ticket_closed_time = datetime.strptime(cro_data.get('_source').get('timestamp'), "%Y-%m-%dT%H:%M:%S.%f")
-                        month_start_date = ticket_closed_time if self.current_start_date < ticket_closed_time else self.current_start_date
-                        user_response = self.get_monthly_user_es_cost_data(start_date=month_start_date, extra_matches={'Tags': {'Key': 'User', 'Values': [user_name]}}, extra_operation='And', tag_name='Project')
-                        if user_response:
-                            if project in [res.get('Project') for res in user_response]:
-                                user_cost = round(user_response[0].get('Cost'), self.DEFAULT_ROUND_DIGITS)
-                                user['Cost'] = user_cost
-                                user['Project'] = project
-                                if user_cost >= self.__over_usage_amount:
-                                    over_usage_users.append(user)
         return over_usage_users
 
     @logger_time_stamp
     def send_alerts_to_over_usage_users(self):
         """
         This method send alerts to cost over usage users
+        Send alert to users every 3rd day, if not open ticket
         :return:
         """
         users_list = self.get_cost_over_usage_users()
+        alerted_users = []
         for row in users_list:
             user, cost, project = row.get('User'), row.get('Cost'), row.get('Project', '')
+            # send_alert, alert_number = self.get_last_mail_alert_status(user=str(user))
+            # if send_alert:
+            alerted_users.append(user)
             cc = [*self.__cro_admins]
             user_details = self.__ldap_search.get_user_details(user_name=user)
             if user_details:
                 name = f'{user_details.get("FullName")}'
                 cc.append(user_details.get('managerId'))
                 subject, body = self.__mail_message.cro_cost_over_usage(CloudName=self.__public_cloud_name,
                                                                         OverUsageCost=self.__over_usage_amount,
                                                                         FullName=name, Cost=cost, Project=project, to=user)
-                self.__postfix_mail.send_email_postfix(to=user, cc=cc, content=body, subject=subject, mime_type='html')
-        return [row.get('User') for row in users_list]
+                es_data = {'Alert': 1}
+                handler.setLevel(logging.WARN)
+                self.__postfix_mail.send_email_postfix(to=user, cc=[], content=body, subject=subject, mime_type='html', es_data=es_data, message_type=self.CRO_OVER_USAGE_ALERT)
+                handler.setLevel(logging.INFO)
+        return alerted_users
+
+    def get_last_mail_alert_status(self, user: str):
+        """
+        This method return the last mail alert.
+        :param user:
+        :return:
+        """
+        query = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"term": {"To.keyword": user}},
+                        {"term": {"MessageType.keyword": self.CRO_OVER_USAGE_ALERT}},
+                    ]
+                }
+            },
+            "size": 1,
+            "sort": {"timestamp": "desc"}
+        }
+        response = self.es_operations.fetch_data_by_es_query(query=query, es_index=self.CLOUD_GOVERNANCE_ES_MAIL_INDEX, search_size=1, limit_to_size=True)
+        if response:
+            last_alert = response[0]
+            last_send_date = last_alert.get('_source').get('timestamp')
+            alert_number = last_alert.get('_source').get('Alert', 0)
+            current_date = datetime.utcnow().date()
+            last_send_date = datetime.strptime(last_send_date, self.TIMESTAMP_DATE_FORMAT).date()
+            days = (current_date - last_send_date).days
+            if days % self.SEND_ALERT_DAY == 0 and last_send_date != current_date:
+                return True, alert_number
+            logger.warning(f"Already sent mail on {last_send_date} to {user}")
+            return False, alert_number
+        return True, 0
 
     @logger_time_stamp
     def run(self):
         """
-        This method run the cost over usage methods
+        This method runs the cost over usage methods
         :return:
         """
         return self.send_alerts_to_over_usage_users()
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_cro_instances.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/monitor_tickets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import logging
 from datetime import datetime
 
 import boto3
 import typeguard
 
 from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.common.elasticsearch.elasticsearch_operations import ElasticSearchOperations
 from cloud_governance.common.jira.jira_operations import JiraOperations
+from cloud_governance.common.logger.init_logger import handler
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 from cloud_governance.common.mails.mail_message import MailMessage
 from cloud_governance.common.mails.postfix import Postfix
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class MonitorTickets:
@@ -64,15 +66,15 @@
             for ticket_id, description in tickets.items():
                 if description.get('TicketOpenedDate').date() != datetime.now().date():
                     user = description.get('EmailAddress').split('@')[0]
                     manager = description.get('ManagerApprovalAddress').split('@')[0]
                     cc = self.__default_admins
                     if ticket_status == self.NEW:  # alert manager if didn't take any action
                         to = manager
-                        subject, body = self.__mail_message.cro_request_for_manager_approval(manager=to, user=user, cloud_name=self.__cloud_name)
+                        subject, body = self.__mail_message.cro_request_for_manager_approval(manager=to, request_user=user, cloud_name=self.__cloud_name, ticket_id=ticket_id, description=description)
                         cc.append(description.get('EmailAddress'))
                     else:  # alert user if doesn't add tag name
                         to = user
                         cc.append(description.get('ManagerApprovalAddress'))
                         subject, body = self.__mail_message.cro_send_user_alert_to_add_tags(user=user, ticket_id=ticket_id)
                     if ticket_status in (self.NEW, self.REFINEMENT):
                         self.__postfix.send_email_postfix(to=to, cc=cc, subject=subject, content=body, mime_type='html')
@@ -91,18 +93,20 @@
             es_id_data = self.__es_operations.get_es_data_by_id(id=ticket_id, index=self.es_cro_index).get('_source')
             if es_id_data:
                 ticket_opened_date = description.get('TicketOpenedDate').date()
                 self.__region_name = description.get('Region')
                 ticket_monitoring_days = (current_date - ticket_opened_date).days
                 duration = int(es_id_data.get('duration'))
                 remaining_duration = duration - ticket_monitoring_days
+                handler.setLevel(logging.WARN)
                 es_data_change = self.verify_es_instances_state(es_data=es_id_data)
                 if es_data_change:
                     self.__es_operations.update_elasticsearch_index(index=self.es_cro_index, id=ticket_id, metadata=es_id_data)
                 self.__alert_in_progress_ticket_users(ticket_id=ticket_id, es_id_data=es_id_data, remaining_duration=remaining_duration)
+                handler.setLevel(logging.INFO)
 
     @typeguard.typechecked
     @logger_time_stamp
     def __tag_extend_instances(self, sub_tasks: list, ticket_id: str, duration: int, sub_task_count: int, estimated_cost: float):
         """
         This method extend the duration if the user opened expand ticket
         :param sub_tasks:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/run_cro.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
                 if last_updated_time == datetime.utcnow().date():
                     first_run = False
         self.__environment_variables_dict.update({'CRO_FIRST_RUN': first_run})
         if first_run:
             cost_over_usage_users = self.cro_cost_over_usage.run()
             logger.info(f'Cost Over Usage Users list: {", ".join(cost_over_usage_users)}')
             self.monitor_tickets.run()
+            self.cro_reports.update_in_progress_ticket_cost()
 
     @logger_time_stamp
     def save_current_timestamp(self):
         """
         This method saves the current timestamp
         Storing timestamp for not sending multiple alerts in a day, if we run any number of times
         :return:
@@ -92,15 +93,14 @@
         2. Tag the new instances
         3. monitor and upload the new instances' data
         4. Monitor the Jira ticket progressing
         :return:
         """
         self.send_cro_alerts()
         self.run_cloud_resources()
-        self.cro_reports.update_in_progress_ticket_cost()
         self.save_current_timestamp()
 
     @logger_time_stamp
     def run(self):
         """
         This method start the aws CRO operations
         :return:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/aws/ec2/tag_cro_instances.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/cloud_resource_orchestration/monitor/cloud_monitor.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     IBM = "IBM"
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', '')
         self.__cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME')
         self.__monitor = self.__environment_variables_dict.get('MONITOR')
+        self.__account = self.__environment_variables_dict.get('account')
         self.__run_cro = RunCRO()
 
     @logger_time_stamp
     def aws_cloud_monitor(self):
         """
         This method ture if the cloud name is
         """
@@ -32,15 +33,15 @@
     @logger_time_stamp
     def run_cloud_monitor(self):
         """
         This method run the public cloud monitor
         """
 
         if self.__cloud_name.upper() == self.AWS:
-            logger.info(f'CLOUD_RESOURCE_ORCHESTRATION = True, PublicCloudName=  {self.__cloud_name}')
+            logger.info(f'CLOUD_RESOURCE_ORCHESTRATION = True, PublicCloudName=  {self.__cloud_name}, Account {self.__account}')
             self.aws_cloud_monitor()
 
     def run(self):
         """
         This method monitoring the cloud resources
         """
         self.run_cloud_monitor()
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudtrail/cloudtrail_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,33 +190,36 @@
         @param start_time:
         @return:
         """
         current_time = datetime.now(start_time.tzinfo).replace(tzinfo=None)
         diff = (current_time - start_time.replace(tzinfo=None))
         return (diff.days * 24 * 60 * 60) + diff.seconds
 
-    def get_username_by_instance_id_and_time(self, resource_id: str, resource_type: str, start_time: datetime = '', event_type: str = 'ResourceType'):
+    def get_username_by_instance_id_and_time(self, resource_id: str, resource_type: str, start_time: datetime = '', event_type: str = 'ResourceType', end_time: datetime = None):
         """
         This method find Username in cloud trail events according to start_time and resource_id
         @param event_type:
         @param start_time:
         @param resource_id:
         @param resource_type:
+        @param end_time:
         @return: if user not found it return empty string
+
         """
-        if start_time:
+        if start_time and not end_time:
             delay_seconds = int(os.environ.get('SLEEP_SECONDS', self.SLEEP_SECONDS))
             if self.__get_time_difference(start_time=start_time) <= delay_seconds:
                 time.sleep(delay_seconds)
             search_time = timedelta(seconds=self.SEARCH_SECONDS)
             end_time = start_time + search_time
             start_time = start_time - search_time
         else:
-            start_time = datetime.now() - timedelta(days=self.LOOKBACK_DAYS)
-            end_time = datetime.now()
+            if not start_time and not end_time:
+                start_time = datetime.now() - timedelta(days=self.LOOKBACK_DAYS)
+                end_time = datetime.now()
         username, event = self.__get_user_by_resource_id(start_time, end_time, resource_id, resource_type, event_type)
         return self.__check_filter_username(username, event)
 
     def get_stop_time(self, resource_id: str, event_name: str):
         """
         This method return the time of when instance is stopped
         @param resource_id:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/cloudwatch/cloudwatch_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/dynamodb/dynamodb_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/ec2/ec2_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/ec2/ec2_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,99 +354,112 @@
         return self.ec2_client.describe_snapshots(OwnerIds=['self'])['Snapshots']
 
     def get_security_groups(self):
         """
         This method returns security groups in the region
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_security_groups, input_tag='SecurityGroups', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_security_groups,
+                                                    input_tag='SecurityGroups', check_tag='NextToken')
 
     def get_elastic_ips(self):
         """
         This method returns elastic_ips in the region
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_addresses, input_tag='Addresses', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_addresses, input_tag='Addresses',
+                                                    check_tag='NextToken')
 
     def get_network_interface(self):
         """
         This method returns network_interface in the region
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_network_interfaces, input_tag='NetworkInterfaces', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_network_interfaces,
+                                                    input_tag='NetworkInterfaces', check_tag='NextToken')
 
     def get_load_balancers(self):
         """
         This method returns load balancers in the region
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.elb1_client.describe_load_balancers, input_tag='LoadBalancerDescriptions', check_tag='Marker')
+        return self.utils.get_details_resource_list(func_name=self.elb1_client.describe_load_balancers,
+                                                    input_tag='LoadBalancerDescriptions', check_tag='Marker')
 
     def get_load_balancers_v2(self):
         """
         This method returns load balancers v2 in the region
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.elbv2_client.describe_load_balancers, input_tag='LoadBalancers', check_tag='Marker')
+        return self.utils.get_details_resource_list(func_name=self.elbv2_client.describe_load_balancers,
+                                                    input_tag='LoadBalancers', check_tag='Marker')
 
     def get_vpcs(self):
         """
         This method returns all vpcs
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_vpcs, input_tag='Vpcs', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_vpcs, input_tag='Vpcs',
+                                                    check_tag='NextToken')
 
     def get_subnets(self):
         """
         This method returns all subnets
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_subnets, input_tag='Subnets', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_subnets, input_tag='Subnets',
+                                                    check_tag='NextToken')
 
     def get_route_tables(self):
         """
         This method returns all route tables
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_route_tables, input_tag='RouteTables', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_route_tables,
+                                                    input_tag='RouteTables', check_tag='NextToken')
 
     def get_internet_gateways(self):
         """
         This method returns all internet gateways
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_internet_gateways, input_tag='InternetGateways', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_internet_gateways,
+                                                    input_tag='InternetGateways', check_tag='NextToken')
 
     def get_dhcp_options(self):
         """
         This method returns all dhcp options
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_dhcp_options, input_tag='DhcpOptions', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_dhcp_options,
+                                                    input_tag='DhcpOptions', check_tag='NextToken')
 
     def get_vpce(self):
         """
         This method returns all vpc endpoints
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_vpc_endpoints, input_tag='VpcEndpoints', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_vpc_endpoints,
+                                                    input_tag='VpcEndpoints', check_tag='NextToken')
 
     def get_nat_gateways(self):
         """
         This method returns all nat gateways
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_nat_gateways, input_tag='NatGateways', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_nat_gateways,
+                                                    input_tag='NatGateways', check_tag='NextToken')
 
     def get_nacls(self):
         """
         This method returns all network acls
         @return:
         """
-        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_network_acls, input_tag='NetworkAcls', check_tag='NextToken')
+        return self.utils.get_details_resource_list(func_name=self.ec2_client.describe_network_acls,
+                                                    input_tag='NetworkAcls', check_tag='NextToken')
 
     def is_cluster_resource(self, resource_id: str):
         """
         This method checks tags have cluster key, if cluster return True else False
         @param resource_id:
         @return:
         """
@@ -504,29 +517,43 @@
                 user = self.get_tag(name='User', tags=instance.get('Tags'))
                 if user in users_list:
                     users_list[user].append(user_data)
                 else:
                     users_list[user] = [user_data]
         return users_list
 
-    def get_tag_value_from_tags(self, tags: list, tag_name: str, cast_type: str = 'str') -> any:
+    def get_tag_value_from_tags(self, tags: list, tag_name: str, cast_type: str = 'str',
+                                default_value: any = '') -> any:
         """
         This method return the tag value inputted by tag_name
         """
         if tags:
             for tag in tags:
                 key = tag.get('Key').lower().replace("_", '').replace("-", '').strip()
                 if key == tag_name.lower():
                     if cast_type:
                         if cast_type == 'int':
                             return int(tag.get('Value').strip())
                         elif cast_type == 'float':
                             return float(tag.get('Value').strip())
-                        return str(tag.get('Value').strip())
-        return ''
+                        else:
+                            return str(tag.get('Value').strip())
+                    return tag.get('Value').strip()
+        return default_value
+
+    def get_active_regions(self):
+        """
+        This method return active regions in aws account
+        :return:
+        """
+        responses = self.ec2_client.describe_regions()['Regions']
+        active_regions = []
+        for region in responses:
+            active_regions.append(region.get('RegionName'))
+        return active_regions
 
     def get_ec2_instance_list(self, **kwargs):
         """
         This method returns the list of instances
         :param kwargs:
         :return:
         """
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/iam/iam_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/iam/iam_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 import boto3
 
 from cloud_governance.common.clouds.aws.utils.utils import Utils
 
 
 class IAMOperations:
 
-    def __init__(self):
-        self.iam_client = boto3.client('iam')
+    def __init__(self, iam_client=None):
+        self.iam_client = iam_client if iam_client else boto3.client('iam')
         self.utils = Utils()
+        self.__sts_client = sts_client = boto3.client('sts')
 
     def get_user_tags(self, username: str):
         """
         This method return tags from the iam resources
         @param username:
         @return:
         """
@@ -58,7 +59,16 @@
         :return:
         """
         iam_users = []
         users = self.get_users()
         for user in users:
             iam_users.append(user.get('UserName'))
         return iam_users
+
+    def get_aws_account_id_name(self):
+        """
+        This method returns the aws account_id
+        :return:
+        """
+        response = self.__sts_client.get_caller_identity()
+        account_id = response['Account']
+        return account_id
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/price.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/price/price.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/price/resources_pricing.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/price/resources_pricing.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/s3/s3_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/s3/s3_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,28 +222,30 @@
         except ClientError as err:
             raise
         except Exception:
             raise
 
     @logger_time_stamp
     @typeguard.typechecked
-    def get_last_objects(self, bucket: str, logs_bucket_key: str, policy: str):
+    def get_last_objects(self, bucket: str, logs_bucket_key: str = '', policy: str = '', key_prefix: str = ''):
         """
         This method return last object per policy, only path without file name
         @param logs_bucket_key:
         @param bucket:
         @param policy:
+        @param key_prefix:
         @return:
         """
         try:
-            if '_' in policy:
-                policy = policy.replace('_', '-')
-            date_key = (datetime.datetime.now() - datetime.timedelta(days=1)).strftime("%Y/%m/%d")
-            objs = self.__s3_client.list_objects_v2(Bucket=bucket,
-                                                    Prefix=f'{logs_bucket_key}/{policy}/{date_key}')['Contents']
+            if not key_prefix:
+                if '_' in policy:
+                    policy = policy.replace('_', '-')
+                date_key = (datetime.datetime.now() - datetime.timedelta(days=1)).strftime("%Y/%m/%d")
+                key_prefix = f'{logs_bucket_key}/{policy}/{date_key}'
+            objs = self.__s3_client.list_objects_v2(Bucket=bucket, Prefix=key_prefix)['Contents']
         except:
             return None
         get_last_modified_key = lambda obj: int(obj['LastModified'].strftime('%s'))
         full_path = [obj['Key'] for obj in sorted(objs, key=get_last_modified_key)][-1]
         return os.path.dirname(full_path)
 
     @staticmethod
@@ -298,24 +300,25 @@
         @param policy:
         @return:
         """
         return self.get_last_objects(bucket=self.__bucket,
                                      logs_bucket_key=f'{self.__logs_bucket_key}/{self.__region}',
                                      policy=policy)
 
-    def get_last_s3_policy_content(self, policy: str, file_name: str):
+    def get_last_s3_policy_content(self, policy: str = '', file_name: str = '', s3_file_path: str = None):
         """
         This method return last policy content
         @return:
         """
         with tempfile.TemporaryDirectory() as temp_local_directory:
             local_file = temp_local_directory + '/' + file_name + '.gz'
-            if self.__get_s3_latest_policy_file(policy=policy):
-                latest_policy_path = self.__get_s3_latest_policy_file(policy=policy)
-                self.download_file(bucket=self.__bucket,
-                                   key=str(latest_policy_path),
-                                   download_file=file_name + '.gz',
-                                   file_name_path=local_file)
-                # gzip
-                os.system(f"gzip -d {local_file}")
-                with open(os.path.join(temp_local_directory, file_name)) as f:
-                    return f.read()
+            if not s3_file_path:
+                if self.__get_s3_latest_policy_file(policy=policy):
+                    s3_file_path = self.__get_s3_latest_policy_file(policy=policy)
+            self.download_file(bucket=self.__bucket,
+                               key=str(s3_file_path),
+                               download_file=file_name + '.gz',
+                               file_name_path=local_file)
+            # gzip
+            os.system(f"gzip -d {local_file}")
+            with open(os.path.join(temp_local_directory, file_name)) as f:
+                return f.read()
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/aws/utils/utils.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/aws/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,21 +68,22 @@
         """
         This method tag the aws resources with batch wise of 20
         :param client_method:
         :param tags:
         :param resource_ids:
         :return:
         """
-        proc = []
-        bulk_resource_ids_list = self.__split_run_bulks(iterable=resource_ids, limit=self.__update_tag_bulks)  # split the aws resource_ids into batches
-        co = 0
-        cpu_based_resource_ids_list = self.__split_run_bulks(iterable=bulk_resource_ids_list, limit=self.__update_tag_bulks)
-        for cpu_based_resource_ids_list in cpu_based_resource_ids_list:
-            for resource_ids_list in cpu_based_resource_ids_list:
-                p = Process(target=self.__tag_resources, args=(client_method, resource_ids_list, tags, ))
-                co += 1
-                p.start()
-                proc.append(p)
-            for p in proc:
-                p.join()
-        return co
+        if tags:
+            proc = []
+            bulk_resource_ids_list = self.__split_run_bulks(iterable=resource_ids, limit=self.__update_tag_bulks)  # split the aws resource_ids into batches
+            co = 0
+            cpu_based_resource_ids_list = self.__split_run_bulks(iterable=bulk_resource_ids_list, limit=self.__update_tag_bulks)
+            for cpu_based_resource_ids_list in cpu_based_resource_ids_list:
+                for resource_ids_list in cpu_based_resource_ids_list:
+                    p = Process(target=self.__tag_resources, args=(client_method, resource_ids_list, tags, ))
+                    co += 1
+                    p.start()
+                    proc.append(p)
+                for p in proc:
+                    p.join()
+            return co
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/cost_management/cost_management_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/azure/subscriptions/azure_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/gcp/google_account.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/gcp/google_account.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/account/ibm_account.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/account/ibm_account.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/clouds/ibm/classic/classic_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/clouds/ibm/classic/classic_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elastic_upload.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/elastic_upload.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,24 +29,24 @@
         """
         try:
             if not es_index:
                 es_index = self.es_index
             count = 0
             for item in items:
                 if not item.get('Account'):
-                    item['Account'] = self.account
+                    item['Account'] = kwargs.get('Account') if kwargs.get('Account') else self.account
                 if kwargs.get('set_index'):
                     self.elastic_search_operations.upload_to_elasticsearch(index=es_index, data=item, id=item[kwargs.get('set_index')])
                 else:
                     self.elastic_search_operations.upload_to_elasticsearch(index=es_index, data=item)
                 count += 1
             if count > 0 and len(items) > 0:
-                logger.info(f'Data Uploaded to {es_index} successfully, Total data: {count}')
+                logger.warn(f'Data Uploaded to {es_index} successfully, Total data: {count}')
         except Exception as err:
-            logger.info(f'Error raised {err}')
+            logger.error(f'Error raised {err}')
 
     def literal_eval(self, data: any):
         """
         This method convert string object into its original datatype
         ex: "{'Project': 'Cloud-Governance'}" --> {'Project': 'Cloud-Governance'}
         @param data:
         @return:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/elasticsearch/elasticsearch_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/elasticsearch/elasticsearch_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,16 @@
 
     def __init__(self, es_host: str, es_port: str, region: str = '', bucket: str = '', logs_bucket_key: str = '',
                  timeout: int = 2000):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.__es_host = es_host
         self.__es_port = es_port
         self.__region = region
-        self.__timeout = int(
-            self.__environment_variables_dict.get('ES_TIMEOUT')) if self.__environment_variables_dict.get(
-            'ES_TIMEOUT') else timeout
-        self.__es = Elasticsearch([{'host': self.__es_host, 'port': self.__es_port}], timeout=self.__timeout,
-                                  max_retries=2)
+        self.__timeout = int(self.__environment_variables_dict.get('ES_TIMEOUT')) if self.__environment_variables_dict.get('ES_TIMEOUT') else timeout
+        self.__es = Elasticsearch([{'host': self.__es_host, 'port': self.__es_port}], timeout=self.__timeout, max_retries=2)
 
     def __elasticsearch_get_index_hits(self, index: str, uuid: str = '', workload: str = '', fast_check: bool = False,
                                        id: bool = False):
         """
         This method search for data per index in last 2 minutes and return the number of docs or zero
         :param index:
         :param workload: need only if there is different timestamp parameter in Elasticsearch
@@ -130,28 +127,27 @@
         if es_add_items:
             for key, value in es_add_items.items():
                 data[key] = value
 
         # utcnow - solve timestamp issue
         if not data.get('timestamp'):
             data['timestamp'] = datetime.utcnow()  # datetime.now()
-
+        data['policy'] = self.__environment_variables_dict.get('policy')
         # Upload data to elastic search server
         try:
             if isinstance(data, dict):  # JSON Object
                 self.__es.index(index=index, doc_type=doc_type, body=data, **kwargs)
             else:  # JSON Array
                 for record in data:
                     self.__es.index(index=index, doc_type=doc_type, body=record, **kwargs)
             return True
         except Exception as err:
             raise err
 
     @typechecked()
-    @logger_time_stamp
     def update_elasticsearch_index(self, index: str, id: str, metadata: dict = ''):
         """
         This method update existing index
         :param index: index name
         :param id: The specific index id
         :param metadata: The metadata for enrich that existing index according to id
         :return:
@@ -209,44 +205,47 @@
         query['query']['bool']['filter']['range']['timestamp']['lte'] = str(end_datetime.replace(microsecond=0))
         query['query']['bool']['filter']['range']['timestamp']['gte'] = str(start_datetime.replace(microsecond=0))
         return query
 
     @typechecked()
     @logger_time_stamp
     def fetch_data_by_es_query(self, es_index: str, query: dict = None, start_datetime: datetime = None,
-                               end_datetime: datetime = None, result_agg: bool = False, group_by: str = ''):
+                               end_datetime: datetime = None, result_agg: bool = False, group_by: str = '', search_size: int = 100, limit_to_size: bool = False):
         """
         This method fetches the data in between range, if you need aggregation results pass you own query with aggegation
         @param es_index:
         @param start_datetime:
         @param end_datetime:
         @param query:
         @param result_agg:
         @param group_by:
+        @param search_size:
+        @param limit_to_size: limit to size
         @return:
         """
         es_data = []
         if self.__es.indices.exists(index=es_index):
             if not query:
                 if start_datetime and end_datetime:
                     query = self.get_query_data_between_range(start_datetime=start_datetime, end_datetime=end_datetime)
             if query:
-                response = self.__es.search(index=es_index, body=query, doc_type='_doc', size=100, scroll='1h')
+                response = self.__es.search(index=es_index, body=query, doc_type='_doc', size=search_size, scroll='1h')
                 if result_agg:
                     es_data.extend(response.get('aggregations').get(group_by).get('buckets'))
                 else:
-                    scroll_id = response.get('_scroll_id')
                     if response.get('hits').get('hits'):
                         es_data.extend(response.get('hits').get('hits'))
-                    while scroll_id:
-                        response = self.__es.scroll(scroll_id=scroll_id, scroll="1h")
-                        if len(response.get('hits').get('hits')) > 0:
-                            es_data.extend(response.get('hits').get('hits'))
-                        else:
-                            break
+                    if not limit_to_size:
+                        scroll_id = response.get('_scroll_id')
+                        while scroll_id:
+                            response = self.__es.scroll(scroll_id=scroll_id, scroll="1h")
+                            if len(response.get('hits').get('hits')) > 0:
+                                es_data.extend(response.get('hits').get('hits'))
+                            else:
+                                break
         return es_data
 
     @typechecked()
     @logger_time_stamp
     def delete_data_in_between_in_es(self, es_index: str, start_datetime: datetime, end_datetime: datetime):
         """
         This method deletes the data in between two ranges
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/google_drive/google_drive_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/google_drive/google_drive_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/google_drive/upload_to_gsheet.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/google_drive/upload_to_gsheet.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/jira/jira.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/jira/jira.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/jira/jira_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/jira/jira_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/ldap/ldap_search.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/ldap/ldap_search.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/logger/logger_time_stamp.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/logger/logger_time_stamp.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,22 @@
         @param args:
         @param kwargs:
         @return: prefix + input method + suffix
         """
         time_start = time.time()
         date_time_start = datetime.datetime.now().strftime(datetime_format)
         try:
-            logger.info(f'Method name: {method.__name__} {kwargs} , Start time: {date_time_start} ')
+            logger.warn(f'Method name: {method.__name__} , Start time: {date_time_start} ')
+            logger.info(f'Method name: {method.__name__} {kwargs}')
             result = method(*args, **kwargs)
             time_end = time.time()
             date_time_end = datetime.datetime.now().strftime(datetime_format)
             total_time = time_end - time_start
             total_time_str = f'Total time: {round(total_time, 2)} sec'
-            logger.info(f'Method name: {method.__name__} , End time: {date_time_end} , {total_time_str}')
+            logger.warn(f'Method name: {method.__name__} , End time: {date_time_end} , {total_time_str}')
         except Exception as err:
             time_end = time.time()
             total_time = time_end - time_start
             date_time_end = datetime.datetime.now().strftime(datetime_format)
             logger.error(f'Method name: {method.__name__} , End time with errors: {date_time_end} , Total time: {round(total_time, 2)} sec')
             raise err  # Exception(method.__name__, err)
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/gmail.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/gmail.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/common/mails/mail_message.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/common/mails/mail_message.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,46 @@
+import os.path
+
+from jinja2 import Environment, FileSystemLoader
+
 from cloud_governance.common.ldap.ldap_search import LdapSearch
 from cloud_governance.main.environment_variables import environment_variables
 
 
 class MailMessage:
 
-    RESTRICTION = 'Do not reply this email. If you need more clarification, please reach out to us in the CoreOS slack channel - #perf-dept-public-clouds.'
+    RESTRICTION = 'Do not reply this email. If you need more information, please reach out to us in the slack channel - #perf-dept-public-clouds.'
     FOOTER = '<div style="color:gray">---<br />Thanks, <br />Cloud GovernanceTeam</div>'
 
     def __init__(self):
         self.__environment_variables_dict = environment_variables.environment_variables_dict
-        self.account = self.__environment_variables_dict.get('account', '')
+        self.account = self.__environment_variables_dict.get('account', '').upper()
         self.policy = self.__environment_variables_dict.get('policy', '')
         self.region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', '')
+        self.__LDAP_HOST_NAME = self.__environment_variables_dict.get('LDAP_HOST_NAME')
+        self.__ldap_search = LdapSearch(ldap_host_name=self.__LDAP_HOST_NAME)
+        self.__public_cloud_name = self.__environment_variables_dict.get('PUBLIC_CLOUD_NAME')
         self.__portal = self.__environment_variables_dict.get('CRO_PORTAL', '')
         self.__cro_duration_days = self.__environment_variables_dict.get('CRO_DURATION_DAYS')
         self.__LDAP_HOST_NAME = self.__environment_variables_dict.get('LDAP_HOST_NAME')
         self.__ldap_search = LdapSearch(ldap_host_name=self.__LDAP_HOST_NAME)
+        self.__templates_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'templates')
+        self.env_loader = Environment(loader=FileSystemLoader(self.__templates_path))
 
     def get_user_ldap_details(self, user_name: str):
         """
         This method return user details from ldap
         :param user_name:
         :return:
         """
         user_details = self.__ldap_search.get_user_details(user_name=user_name)
-        return user_details.get('displayName')
+        if user_details:
+            return user_details.get('displayName')
+        else:
+            return None
 
     def ec2_stop(self, name: str, days: int, image_id: str, delete_instance_days: int, instance_name: str,
                  resource_id: str, stopped_time: str, ec2_type: str, **kwargs):
         extra_purse = ''
         if kwargs.get("extra_purse"):
             extra_purse = f', Cost {round(kwargs.get("extra_purse"), 3)} $ '
         subject = f'cloud-governance alert: ec2-stop'
@@ -247,22 +259,22 @@
         This method return the CRO Alert Message
         :param days:
         :param user:
         :param ticket_id:
         :return:
         """
         ticket_id = ticket_id.split('-')[-1]
-        subject = f'CRO Alert: Expiring in {days} days'
+        subject = f'[Action required] Cloud Resources Ticket Expiring in {days} days'
         user_display_name = self.get_user_ldap_details(user_name=user)
         body = f"""
                 <div>
-                <p>Hi {user_display_name},</p>
+                    <p>Hi {user_display_name},</p>
                 </div>
                 <div>
-                    <p>You project budget request (TicketId: {ticket_id}) will be expired in {days} days</p>
+                    <p>You project budget request ( TicketId: {ticket_id} ) will be expired in {days} days.</p>
                     <p>You can extend the project duration in the following url {self.__portal} or terminate the instances</p>
                     <p>Visit the <a href="{self.__portal}">wiki page</a> to get more information</p>
                 </div>
                 {self.FOOTER}
 """.strip()
         return subject, body
 
@@ -274,62 +286,68 @@
         """
         cloud_name = kwargs.get('CloudName', 'NA').upper()
         over_usage_cost = kwargs.get('OverUsageCost', 'NA')
         full_name = kwargs.get('FullName', '')
         if not full_name:
             full_name = kwargs.get('to')
         user_cost = round(kwargs.get('Cost', 0), 3)
-        subject = f'{cloud_name} Cost Over Usage alert: > {over_usage_cost} $'
+        subject = f'[Action required]: Cloud Resources Open Ticket Request'
+        if user_cost > over_usage_cost:
+            message = f"it's over {over_usage_cost} $."
+        else:
+            message = f"it may over {over_usage_cost} $ in next few days."
         body = f"""
         <div>
         Hi {full_name},
         </div><br/>
         <div>
-            Your {cloud_name} cost usage in the last {self.__cro_duration_days} days is {user_cost}$ and it's over {over_usage_cost} $.<br/>
+            Your {cloud_name} cost usage in the last {self.__cro_duration_days} days is {user_cost}$ and {message}<br/>
             You must open the project ticket in the following <a href="{self.__portal}">Link</a>.<br />
-            After submitting a ticket, you must add Tag (TicketID:#) to every active resource that is related to the project ticket.<br/>
+            After submitting a ticket, you must add Tag (TicketId:#) to every active resource that is related to the project ticket.<br/>
             
             If you have any questions, please let us know in slack channel #perf-dept-public-clouds
         <div><br/><br/>
         {self.FOOTER}
 """
         return subject, body
 
-    def cro_request_for_manager_approval(self, manager: str, user: str, cloud_name: str):
+    def cro_request_for_manager_approval(self, manager: str, request_user: str, cloud_name: str, ticket_id: str, description: dict):
         """
         This method returns the message for manager, regarding user approval
+        :param description:
+        :param ticket_id:
         :param manager:
-        :param user:
+        :param request_user:
         :param cloud_name:
         :return:
         """
-        subject = 'CRO Alert: Required budget approval'
+        subject = '[Action required]: Cloud Resources Budget Request Approval'
         manager_full_name = self.get_user_ldap_details(user_name=manager)
-        user_full_name = self.get_user_ldap_details(user_name=user)
-        body = f"""
-            <div>Hi {manager_full_name},</div><br />
-            <div>{user_full_name} is waiting for your project cloud budget approval<br />
-            Please approve the request in the following url< a href="{self.__portal}">{self.__portal}</a></div><br />
-            {self.FOOTER}
-        """
+        user_full_name = self.get_user_ldap_details(user_name=request_user)
+        ticket_id = ticket_id.split('-')[-1]
+        context = {'manager': manager, 'manager_full_name': manager_full_name, 'user_full_name': user_full_name,
+                   'ticket_id': ticket_id, 'portal': self.__portal, 'request_user': request_user, 'description': description,
+                   'footer': self.FOOTER}
+        template_loader = self.env_loader.get_template('cro_request_for_manager_approval.j2')
+        body = template_loader.render(context)
         return subject, body
 
     def cro_send_user_alert_to_add_tags(self, user: str, ticket_id: str):
         """
         This method return the subject, body for adding tags
         :param user:
         :param ticket_id:
         :return:
         """
-        subject = 'CRO Alert: Required addition of TicketId tag'
+        subject = '[Action required]: Required addition of TicketId tag'
         ticket_id = ticket_id.split('-')[-1]
         user_display_name = self.get_user_ldap_details(user_name=user)
         body = f"""
         <div>Hi {user_display_name},</div><br />
-        <p>Your project budget request ( TicketId: # ) was approved by your manager.</p><br />
+        <p>Your project budget request ( TicketId: {ticket_id} ) was approved by your manager.</p><br />
         <p>Please tag your instances with tag TicketId: {ticket_id}</p>
         </div><br />
         {self.FOOTER}
         """
         return subject, body
 
     def cro_send_closed_alert(self, user: str, es_data: dict, ticket_id: str):
@@ -342,13 +360,80 @@
         """
         subject = 'CRO Alert: Closing ticket'
         ticket_id = ticket_id.split('-')[-1]
         user_full_name = self.get_user_ldap_details(user_name=user)
         body = f"""
         <div>Hi {user_full_name},</div><br />
             <div>
-            Your cloud project request ( TicketId:{ticket_id} ) duration expired and the ticket auto closed.<br />
-            You can find the summary in <a href="{self.__portal}/wikipage">Portal</a>.<br />
+            Your cloud project request ( TicketId: {ticket_id} ) duration expired and the ticket auto closed.<br />
+            You can find the summary in <a href="{self.__portal}/wiki/clouds">Portal</a>.<br />
             </div><br /><br/>
         {self.FOOTER}
         """
         return subject, body
+
+    def filter_resources_on_days(self, resources: dict):
+        """
+        This method return the resources based on the days
+        :param resources:
+        :param days:
+        :return:
+        """
+        resources_by_days = {}
+        for policy_name, resource_data in resources.items():
+            for region_name, policy_region_data in resource_data.items():
+                for data_item in policy_region_data:
+                    resources_by_days.setdefault(data_item.get('Days'), []).append(data_item)
+        return resources_by_days
+
+    def get_data_in_html_table_format(self, resources: dict):
+        """
+        This method return user policy alerts in HTML table format
+        :param resources:
+        :return:
+        """
+        html_table_format = '<table width="auto" border="2" style="border-collapse: collapse;padding: 10px;border: 2px solid black;">'
+        html_style_value = "border-collapse: collapse;padding: 10px;border: 2px solid black;"
+        html_style = f'style="{html_style_value}"'
+        html_style_color = f'style="color:red;{html_style_value}"'
+        td_left, td_right = f'<td align="left" {html_style}>', '</td>'
+        td_left_color = f'<td align="left" {html_style_color}>'
+        th_left, th_right = f'<th align="left" {html_style}>', '</th>'
+        tr_left, tr_right = f'<tr {html_style}>', '</tr>'
+        thead_values = ['Policy', 'Region', 'ResourceId', 'Name', 'Action', 'DeletedDay']
+        html_table_format += '<thead>' + tr_left + ''.join([f'{th_left}{value}{th_right}' for value in thead_values]) + f'{tr_right}</thead><tbody>'
+        for days, resource_data in resources.items():
+            resource_data = sorted(resource_data, key=lambda item: (item.get('Policy'), item.get('Region')))
+            for resource in resource_data:
+                td_data = [resource.get(th_value) for th_value in thead_values]
+                if 'Deleted' == resource.get('Action'):
+                    html_table_format += f"""{tr_left }{''.join([f'{td_left_color}{value}{td_right}' for value in td_data])}{tr_right}"""
+                else:
+                    html_table_format += f"""{tr_left}{''.join([f'{td_left}{value}{td_right}' for value in td_data])}{tr_right}"""
+        html_table_format += '</tbody></table>'
+        return html_table_format
+
+    def get_agg_policies_mail_message(self, user: str, user_resources: dict):
+        """
+        This method return the message for the aggregated alert of all policies
+        :param user:
+        :param user_resources:
+        :return:
+        """
+        display_name = self.get_user_ldap_details(user_name=user)
+        resources_by_days = self.filter_resources_on_days(resources=user_resources)
+        table_data = self.get_data_in_html_table_format(resources=resources_by_days)
+        display_name = display_name if display_name else user
+        subject = f'Cloud Governance: Policy Alerts'
+        body = f"""
+        <div>
+            <p>Hi {display_name},</p>
+        </div>
+        <div>
+            <p>You can find below your unused resources in the {self.__public_cloud_name} account ({self.account}).</p>
+            <p>If you want to keep them, please add "Policy=Not_Delete" or "Policy=skip" tag for each resource</p>
+            {table_data}
+        </div>
+        <p>{self.RESTRICTION}</p>
+        {self.FOOTER}
+"""
+        return subject, body
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/main/environment_variables.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/main/environment_variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+
 import tempfile
 from ast import literal_eval
 
 import boto3
 
 from cloud_governance.main.environment_variables_exceptions import ParseFailed
 
@@ -34,23 +35,27 @@
                 pass  # ignore
 
         ##################################################################################################
         # dynamic parameters - configure for local run
         # parameters for running policies
         self._environment_variables_dict['account'] = EnvironmentVariables.get_env('account', '').upper().strip()
         self._environment_variables_dict['AWS_DEFAULT_REGION'] = EnvironmentVariables.get_env('AWS_DEFAULT_REGION', '')
+        self._environment_variables_dict['log_level'] = EnvironmentVariables.get_env('log_level', 'INFO')
+        self._environment_variables_dict['PRINT_LOGS'] = EnvironmentVariables.get_boolean_from_environment('PRINT_LOGS', True)
+        if not self._environment_variables_dict['AWS_DEFAULT_REGION']:
+            self._environment_variables_dict['AWS_DEFAULT_REGION'] = 'us-east-2'
         self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = EnvironmentVariables.get_env('PUBLIC_CLOUD_NAME', 'AWS')
         if EnvironmentVariables.get_env('AWS_ACCESS_KEY_ID', '') and EnvironmentVariables.get_env('AWS_SECRET_ACCESS_KEY', ''):
             self._environment_variables_dict['account'] = self.get_aws_account_alias_name().upper()
         self._environment_variables_dict['policy'] = EnvironmentVariables.get_env('policy', '')
 
         self._environment_variables_dict['aws_non_cluster_policies'] = ['ec2_idle', 'ec2_stop', 'ec2_run', 'ebs_in_use',
                                                                         'ebs_unattached', 's3_inactive',
                                                                         'empty_roles', 'ip_unattached',
-                                                                        'nat_gateway_unused',
+                                                                        'unused_nat_gateway',
                                                                         'zombie_snapshots', 'skipped_resources',
                                                                         'monthly_report']
         self._environment_variables_dict['cost_policies'] = ['cost_explorer', 'cost_over_usage', 'cost_billing_reports', 'cost_explorer_payer_billings']
         self._environment_variables_dict['ibm_policies'] = ['tag_baremetal', 'tag_vm', 'ibm_cost_report',
                                                             'ibm_cost_over_usage']
 
         # AWS env vars
@@ -164,24 +169,35 @@
         if self._environment_variables_dict.get('GCP_DATABASE_TABLE_NAME'):
             self._environment_variables_dict['PUBLIC_CLOUD_NAME'] = 'GCP'
 
         self._environment_variables_dict['EMAIL_ALERT'] = EnvironmentVariables.get_boolean_from_environment('EMAIL_ALERT', True)
         self._environment_variables_dict['MANAGER_EMAIL_ALERT'] = EnvironmentVariables.get_boolean_from_environment('MANAGER_EMAIL_ALERT', True)
         self._environment_variables_dict['UPDATE_TAG_BULKS'] = int(EnvironmentVariables.get_env('UPDATE_TAG_BULKS', '20'))
 
+        # policies aggregate alert
+        self._environment_variables_dict['BUCKET_NAME'] = EnvironmentVariables.get_env('BUCKET_NAME')
+        self._environment_variables_dict['BUCKET_KEY'] = EnvironmentVariables.get_env('BUCKET_KEY')
+        self._environment_variables_dict['MAIL_ALERT_DAYS'] = literal_eval(EnvironmentVariables.get_env('MAIL_ALERT_DAYS', '[]'))
+        self._environment_variables_dict['POLICY_ACTIONS_DAYS'] = literal_eval(EnvironmentVariables.get_env('POLICY_ACTIONS_DAYS', '[]'))
+        self._environment_variables_dict['DEFAULT_ADMINS'] = literal_eval(EnvironmentVariables.get_env('DEFAULT_ADMINS', '[]'))
+        self._environment_variables_dict['KERBEROS_USERS'] = literal_eval(EnvironmentVariables.get_env('KERBEROS_USERS', '[]'))
+        self._environment_variables_dict['POLICIES_TO_ALERT'] = literal_eval(EnvironmentVariables.get_env('POLICIES_TO_ALERT', '[]'))
+        if self._environment_variables_dict.get('policy') in ['send_aggregated_alerts']:
+            self._environment_variables_dict['COMMON_POLICIES'] = True
         # CRO -- Cloud Resource Orch
         self._environment_variables_dict['CLOUD_RESOURCE_ORCHESTRATION'] = EnvironmentVariables.get_boolean_from_environment('CLOUD_RESOURCE_ORCHESTRATION', False)
         self._environment_variables_dict['USER_COST_INDEX'] = EnvironmentVariables.get_env('USER_COST_INDEX', '')
         self._environment_variables_dict['CRO_ES_INDEX'] = EnvironmentVariables.get_env('CRO_ES_INDEX', 'cloud-governance-resource-orchestration')
         self._environment_variables_dict['CRO_COST_OVER_USAGE'] = int(EnvironmentVariables.get_env('CRO_COST_OVER_USAGE', '500'))
         self._environment_variables_dict['CRO_DEFAULT_ADMINS'] = literal_eval(EnvironmentVariables.get_env('CRO_DEFAULT_ADMINS', "[]"))
         self._environment_variables_dict['CRO_DURATION_DAYS'] = int(EnvironmentVariables.get_env('CRO_DURATION_DAYS', '30'))
         self._environment_variables_dict['RUN_ACTIVE_REGIONS'] = EnvironmentVariables.get_boolean_from_environment('RUN_ACTIVE_REGIONS', False)
         self._environment_variables_dict['CRO_RESOURCE_TAG_NAME'] = EnvironmentVariables.get_env('CRO_RESOURCE_TAG_NAME', 'TicketId')
         self._environment_variables_dict['CRO_REPLACED_USERNAMES'] = literal_eval(EnvironmentVariables.get_env('CRO_REPLACED_USERNAMES', "['osdCcsAdmin']"))
+        self._environment_variables_dict['CE_PAYER_INDEX'] = EnvironmentVariables.get_env('CE_PAYER_INDEX', '')
 
 
     @staticmethod
     def to_bool(arg, def_val: bool = None):
         if isinstance(arg, bool):
             return arg
         if isinstance(arg, (int, float)):
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/main/es_uploader.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/main/es_uploader.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/main/main.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/main/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import typeguard
 from ast import literal_eval  # str to dict
 import boto3  # regions
 
 from cloud_governance.cloud_resource_orchestration.monitor.cloud_monitor import CloudMonitor
+from cloud_governance.main.main_common_operations import run_common_policies
 from cloud_governance.main.run_cloud_resource_orchestration import run_cloud_resource_orchestration
 from cloud_governance.policy.policy_operations.aws.cost_expenditure.cost_report_policies import CostReportPolicies
 from cloud_governance.policy.policy_operations.azure.azure_policy_runner import AzurePolicyRunner
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp, logger
 from cloud_governance.policy.policy_operations.aws.tag_cluster.run_tag_cluster_resouces import tag_cluster_resource, \
     remove_cluster_resources_tags
 from cloud_governance.policy.policy_operations.aws.tag_non_cluster.run_tag_non_cluster_resources import tag_non_cluster_resource, \
@@ -186,15 +187,17 @@
     upload_data_es = environment_variables_dict.get('upload_data_es', '')
     es_host = environment_variables_dict.get('es_host', '')
     es_port = environment_variables_dict.get('es_port', '')
     es_index = environment_variables_dict.get('es_index', '')
     es_doc_type = environment_variables_dict.get('es_doc_type', '')
     bucket = environment_variables_dict.get('bucket', '')
 
-    if environment_variables_dict.get('CLOUD_RESOURCE_ORCHESTRATION'):
+    if environment_variables_dict.get('COMMON_POLICIES'):
+        run_common_policies()
+    elif environment_variables_dict.get('CLOUD_RESOURCE_ORCHESTRATION'):
         run_cloud_resource_orchestration()
     else:
         non_cluster_polices_runner = None
         is_non_cluster_polices_runner = policy in environment_variables_dict.get('aws_non_cluster_policies')
         if is_non_cluster_polices_runner:
             non_cluster_polices_runner = ZombieNonClusterPolicies()
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/main/run_cloud_resource_orchestration.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/main/run_cloud_resource_orchestration.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_billing_reports.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_billing_reports.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             self.update_to_gsheet = UploadToGsheet()
             self.cost_center, self.__account_budget, self.__years, self.__owner = self.update_to_gsheet.get_cost_center_budget_details(account_id=self.__account_id)
         except:
             pass
 
     def __get_start_date(self, end_date: datetime, days: int, operation: operator) -> datetime:
         """
-        This method return start_date
+        This method returns start_date
         @param operation:
         @param end_date:
         @param days:
         @return:
         """
         return operation(end_date, datetime.timedelta(days=days))
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_explorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from ast import literal_eval
 
 from cloud_governance.common.clouds.aws.ec2.ec2_operations import EC2Operations
 from cloud_governance.common.elasticsearch.elastic_upload import ElasticUpload
 from cloud_governance.common.clouds.aws.cost_explorer.cost_explorer_operations import CostExplorerOperations
 from cloud_governance.common.logger.init_logger import logger
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
@@ -12,14 +11,26 @@
 class CostExplorer:
     """
     This class fetches the cost_explorer report from the AWS based on two days ago data and upload to ElasticSearch.
     fetching AWS cost explorer of two days ago because day ago cost calculation is not closed.
     """
 
     BULK_UPLOAD_THREADS = 8
+    SAVINGS_PLAN_FILTER = {  # savings plan usage for ce filter
+                            'Dimensions': {
+                                        'Key': 'RECORD_TYPE',
+                                        'Values': ['SavingsPlanRecurringFee', 'SavingsPlanNegation', 'SavingsPlanCoveredUsage']
+                                }
+                    }
+    EXCLUDE = 'exclude'
+    INCLUDE = 'include'
+    CE_KEY_RESULTS_BY_TIME = 'ResultsByTime'
+    INDEX_ID = 'index_id'
+    APPEND = 'a'
+    CE_OPERATION = 'Not'
 
     def __init__(self):
         super().__init__()
         self.__environment_variables_dict = environment_variables.environment_variables_dict
         self.start_date = self.__environment_variables_dict.get('start_date', '')  # yyyy-mm-dd
         self.end_date = self.__environment_variables_dict.get('end_date', '')  # yyyy-mm-dd
         self.granularity = self.__environment_variables_dict.get('granularity', 'DAILY')
@@ -28,19 +39,20 @@
         self.file_name = self.__environment_variables_dict.get('file_name', '')
         self.__cost_explorer = CostExplorerOperations()
         self.region = self.__environment_variables_dict.get('AWS_DEFAULT_REGION', 'us-east-1')
         self._ec2_operations = EC2Operations(region=self.region)
         self._elastic_upload = ElasticUpload()
         self.__account = self.__environment_variables_dict.get('account').upper().replace('OPENSHIFT-', "").strip()
 
-    def filter_data_by_tag(self, groups: dict, tag: str):
+    def filter_data_by_tag(self, groups: dict, tag: str, savings_plan: str):
         """
         This method extract data by tag
         @param tag:
         @param groups: Data from the cloud explorer
+        @param savings_plan:
         @return: converted into dict format
         """
         data = {}
         start_time = groups.get('TimePeriod').get('Start')
         account = self.__account
         for group in groups.get('Groups'):
             name = ''
@@ -54,59 +66,64 @@
                 amount = group.get('Metrics').get(self.cost_metric).get('Amount')
             if name and amount:
                 if 'aws-go-sdk' in name:
                     name = 'aws-go-sdk'
                 else:
                     if 'vm_import_image' in name:
                         name = 'vm_import_image'
-                index_id = f'{start_time.lower()}-{account.lower()}-{tag.lower()}-{name.lower()}'
+                index_id = f'{start_time}-{account}-{tag}-savings-{savings_plan}-{name}'.lower()
                 if index_id not in data:
-                    upload_data = {tag: name if tag.upper() in ('ChargeType'.upper(), 'PurchaseType'.upper()) else name.upper(),
-                                   'Cost': round(float(amount), 3), 'index_id': index_id, 'timestamp': start_time}
+                    upload_data = {tag: name if tag.upper() in list(self.__cost_explorer.CE_COST_TYPES) else name.upper(),
+                                   'Cost': round(float(amount), 3), self.INDEX_ID: index_id, 'timestamp': start_time, 'savings_plan': savings_plan}
                     if 'global' in self._elastic_upload.es_index:
                         if 'Budget' not in upload_data:
                             upload_data['Budget'] = self._elastic_upload.account
+                    upload_data['tag'] = tag.lower()
                     data[index_id] = upload_data
                 else:
                     data[index_id]['Cost'] += round(float(amount), 3)
         return list(data.values())
 
     def __get_daily_cost_by_tags(self):
         """
         This method extracts the costs by tags and upload to elastic search
         @return:
         """
         data_house = {}
         for tag in self.cost_tags:
-            if self.start_date and self.end_date:
-                response = self.__cost_explorer.get_cost_by_tags(tag=tag, start_date=self.start_date, end_date=self.end_date, granularity=self.granularity, cost_metric=self.cost_metric)
-            else:
-                response = self.__cost_explorer.get_cost_by_tags(tag=tag, granularity=self.granularity, cost_metric=self.cost_metric)
-            results_by_time = response.get('ResultsByTime')
-            if results_by_time:
-                data_house[tag] = []
-                for result in results_by_time:
-                    data_house[tag].extend(self.filter_data_by_tag(result, tag))
+            for savings_plan in [self.EXCLUDE, self.INCLUDE]:
+                filters = {}
+                if savings_plan == self.EXCLUDE:
+                    filters = {self.CE_OPERATION: self.SAVINGS_PLAN_FILTER}
+                if self.start_date and self.end_date:
+                    response = self.__cost_explorer.get_cost_by_tags(tag=tag, start_date=self.start_date, end_date=self.end_date, granularity=self.granularity, cost_metric=self.cost_metric, Filter=filters)
+                else:
+                    response = self.__cost_explorer.get_cost_by_tags(tag=tag, granularity=self.granularity, cost_metric=self.cost_metric, Filter=filters)
+                results_by_time = response.get(self.CE_KEY_RESULTS_BY_TIME)
+                if results_by_time:
+                    data_house[f'{tag}-{savings_plan}'] = []
+                    for result in results_by_time:
+                        data_house[f'{tag}-{savings_plan}'].extend(self.filter_data_by_tag(result, tag, savings_plan))
         return data_house
 
     @logger_time_stamp
     def __upload_data(self, data: list, index: str):
         """
         This method upload to elastic search
         @param data:
         @param index:
         @return:
         """
         if self.file_name:
-            with open(f'/tmp/{self.file_name}', 'a') as file:
+            with open(f'/tmp/{self.file_name}', self.APPEND) as file:
                 for value in data:
                     file.write(f'{value}\n')
         else:
             for value in data:
-                self.upload_item_to_es(index=index, item=value, index_id=value['index_id'])
+                self.upload_item_to_es(index=index, item=value, index_id=value[self.INDEX_ID])
             logger.info(f'Data uploaded to {index}, Total Data: {len(data)}')
 
     def upload_item_to_es(self, item: dict, index: str, index_id: str = ''):
         """
         This method upload one item to es
         @param item:
         @param index:
@@ -122,16 +139,16 @@
         """
         This method upload daily tag cost into ElasticSearch
         @return:
         """
         logger.info(f'Get {self.granularity} Cost usage by metric: {self.cost_metric}')
         cost_data = self.__get_daily_cost_by_tags()
         for key, values in cost_data.items():
-            index = f'{self._elastic_upload.es_index}-{key.lower()}'
-            self.__upload_data(values, index)
+            logger.info(f"Uploading the data of {key} tag")
+            self.__upload_data(values, self._elastic_upload.es_index)
 
     def run(self):
         """
         This method run the operations
         @return:
         """
         self.upload_tags_cost_to_elastic_search()
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_explorer_payer_billings.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_explorer_payer_billings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import copy
 import datetime
+import logging
 from ast import literal_eval
 
 import boto3
-from dateutil.relativedelta import relativedelta
 
+from cloud_governance.common.clouds.aws.iam.iam_operations import IAMOperations
+from cloud_governance.common.clouds.aws.savingsplan.savings_plans_operations import SavingsPlansOperations
 from cloud_governance.common.logger.logger_time_stamp import logger_time_stamp
 
-from cloud_governance.common.logger.init_logger import logger
+from cloud_governance.common.logger.init_logger import logger, handler
 from cloud_governance.common.clouds.aws.cost_explorer.cost_explorer_operations import CostExplorerOperations
 from cloud_governance.policy.aws.cost_billing_reports import CostBillingReports
 
 
 class CostExplorerPayerBillings(CostBillingReports):
     """
     This class is responsible for generation cost billing report for Budget, Actual, Forecast from the Org level
     Monthly savings Plan Amortization: (linked_account_total_cost/payer_account_total_cost) * monthly_savings_plan_cost
     Monthly_support_fee: (monthly_support_fee - (monthly_support_fee * discount ) ) * (linked_account_total_cost/payer_account_total_cost)
     """
 
+    DEFAULT_ROUND_DIGITS = 3
+
     def __init__(self):
         super().__init__()
         self.__aws_role = self._environment_variables_dict.get("AWS_ACCOUNT_ROLE")
         self.__access_key, self.__secret_key, self.__session = self.__get_sts_credentials()
         self.__ce_client = boto3.client('ce', aws_access_key_id=self.__access_key, aws_secret_access_key=self.__secret_key, aws_session_token=self.__session)
+        self.__savings_plan_client = boto3.client('savingsplans', aws_access_key_id=self.__access_key, aws_secret_access_key=self.__secret_key, aws_session_token=self.__session)
+        self.__iam_client = boto3.client('iam', aws_access_key_id=self.__access_key, aws_secret_access_key=self.__secret_key, aws_session_token=self.__session)
+        self.__assumed_role_account_name = IAMOperations(iam_client=self.__iam_client).get_account_alias_cloud_name()
         self.__cost_explorer_operations = CostExplorerOperations(ce_client=self.__ce_client)
+        self.__savings_plan_operations = SavingsPlansOperations(savings_plan_client=self.__savings_plan_client)
         self.__replacement_account = literal_eval(self._environment_variables_dict.get('REPLACE_ACCOUNT_NAME'))
         self.__savings_discounts = float(self._environment_variables_dict.get('PAYER_SUPPORT_FEE_CREDIT', 0))
         self.__monthly_cost_for_spa_calc = {}
         self.__monthly_cost_for_support_fee = {}
         self.__temporary_dir = self._environment_variables_dict.get('TEMPORARY_DIR', '')
 
     def __get_sts_credentials(self):
@@ -62,28 +70,28 @@
                                 acc_cost_center, account_budget, years, owner = self.update_to_gsheet.get_cost_center_budget_details(account_id=name, dir_path=self.__temporary_dir)
                                 timestamp = datetime.datetime.strptime(start_time, '%Y-%m-%d')
                                 month = datetime.datetime.strftime(timestamp, "%Y %b")
                                 month_full_name = datetime.datetime.strftime(timestamp, "%B")
                                 payer_monthly_savings_plan = self.update_to_gsheet.get_monthly_spa(month_name=month_full_name, dir_path=self.__temporary_dir)
                                 budget = account_budget if start_time.split('-')[0] in years else 0
                                 index_id = f'{start_time}-{name}'
-                                upload_data = {tag: name, 'Actual': round(float(amount), 3), 'start_date': start_time,
+                                upload_data = {tag: name, 'Actual': round(float(amount), self.DEFAULT_ROUND_DIGITS), 'start_date': start_time,
                                                'timestamp': timestamp, 'CloudName': 'AWS', 'Month': month,
                                                'Forecast': 0,
                                                'filter_date': f'{start_time}-{month.split()[-1]}',
-                                               'Budget': round(budget / self.MONTHS, 3), 'CostCenter': cost_center,
+                                               'Budget': round(budget / self.MONTHS, self.DEFAULT_ROUND_DIGITS), 'CostCenter': cost_center,
                                                'AllocatedBudget': budget,
                                                "Owner": owner,
                                                'SavingsPlanCost': (float(amount) / float(self.__monthly_cost_for_spa_calc.get(start_time))) * payer_monthly_savings_plan,
                                                'TotalPercentage': (float(amount) / float(self.__monthly_cost_for_spa_calc.get(start_time)))
                                                }
                                 upload_data['PremiumSupportFee'] = (float(self.__monthly_cost_for_support_fee.get(start_time)) - (float(self.__monthly_cost_for_support_fee.get(start_time)) * self.__savings_discounts)) * upload_data['TotalPercentage'],
                             else:
                                 index_id = f'{start_time}-{name}'
-                                upload_data = {tag: name, 'Actual': round(float(amount), 3)}
+                                upload_data = {tag: name, 'Actual': round(float(amount), self.DEFAULT_ROUND_DIGITS)}
                             if index_id:
                                 data[index_id] = upload_data
         if cost_data.get('DimensionValueAttributes'):
             for dimension_values in cost_data.get('DimensionValueAttributes'):
                 account_id = dimension_values.get("Value")
                 account = dimension_values.get('Attributes').get('description')
                 if self.__replacement_account.get(account):
@@ -95,15 +103,15 @@
         return data
 
     def filter_forecast_data(self, cost_forecast_data: list, cost_usage_data: dict, account_id: str, cost_center: int, account: str):
         acc_cost_center, account_budget, years, owner = self.update_to_gsheet.get_cost_center_budget_details(account_id=account_id, dir_path=self.__temporary_dir)
         for cost_forecast in cost_forecast_data:
             start_date = str((cost_forecast.get('TimePeriod').get('Start')))
             start_year = start_date.split('-')[0]
-            cost = round(float(cost_forecast.get('MeanValue')), 3)
+            cost = round(float(cost_forecast.get('MeanValue')), self.DEFAULT_ROUND_DIGITS)
             index = f'{start_date}-{account_id}'
             month_full_name = datetime.datetime.strftime(datetime.datetime.strptime(start_date, '%Y-%m-%d'), "%B")
             total_percentage = (cost / float(self.__monthly_cost_for_spa_calc.get(start_date)))
             payer_monthly_savings_plan = self.update_to_gsheet.get_monthly_spa(month_name=month_full_name, dir_path=self.__temporary_dir)
             if index in cost_usage_data[account]:
                 cost_usage_data[account][index]['Forecast'] = cost
                 cost_usage_data[account][index]['TotalPercentage'] = total_percentage
@@ -120,25 +128,24 @@
                 data['Account'] = account
                 data['start_date'] = str((cost_forecast.get('TimePeriod').get('Start')))
                 data['index_id'] = f"""{data['start_date']}-{data['Account'].lower()}"""
                 data['timestamp'] = datetime.datetime.strptime(data['start_date'], '%Y-%m-%d')
                 data['Month'] = datetime.datetime.strftime(data['timestamp'], '%Y %b')
                 data['Owner'] = owner
                 if start_year in years:
-                    data['Budget'] = round(account_budget / self.MONTHS, 3)
+                    data['Budget'] = round(account_budget / self.MONTHS, self.DEFAULT_ROUND_DIGITS)
                     data['AllocatedBudget'] = account_budget
                 else:
                     data['Budget'] = 0
                     data['AllocatedBudget'] = 0
                 data['CostCenter'] = cost_center
                 data['CloudName'] = "AWS"
                 data['filter_date'] = f'{data["start_date"]}-{data["Month"].split()[-1]}'
                 cost_usage_data[account][index] = data
 
-    @logger_time_stamp
     def get_linked_accounts_forecast(self, linked_account_usage: dict):
         """
         This method append the forecast to the linked accounts
         """
         start_date, end_date = self.get_date_ranges(days=self.FORECAST_DAYS)
         for account, account_cost_usage in copy.deepcopy(linked_account_usage).items():
             list_usage = list(account_cost_usage.values())[0]
@@ -168,17 +175,46 @@
         for cost_center in cost_centers:
             cost_data = self.__cost_explorer_operations.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity="MONTHLY", GroupBy=[{'Type': 'DIMENSION', 'Key': 'LINKED_ACCOUNT'}], Filter={'CostCategories': {'Key': 'CostCenter', 'Values': [cost_center.get('CostCenter')]}})
             cost_center_usage_accounts = self.filter_data_by_tag(cost_data, tag='AccountId', cost_center=int(cost_center.get('CostCenter')))
             for idx, usage in cost_center_usage_accounts.items():
                 account = usage['Account']
                 cost_usage_data.setdefault(account, {}).update({idx: usage})
         self.get_linked_accounts_forecast(linked_account_usage=cost_usage_data)
+        self.__get_ce_cost_usage_by_filter_tag(tag_name='spot', cost_centers=cost_centers, cost_usage_data=cost_usage_data)
+        handler.setLevel(logging.WARN)
+        #  To prevent printing the **kwargs of the function when using the logger_time_stamp decorator.
         self.upload_data_elastic_search(linked_account_usage=cost_usage_data)
+        handler.setLevel(logging.INFO)
         return cost_usage_data
 
+    def __get_ce_cost_usage_by_filter_tag(self, cost_centers: list, tag_name: str, cost_usage_data: dict):
+        """
+        This method returns the cost by filter tag_name
+        :param cost_centers:
+        :param tag_name:
+        :return:
+        """
+        start_date, end_date = self.get_date_ranges()
+        for cost_center in cost_centers:
+            cost_center_number = cost_center.get('CostCenter')
+            filter_cost_center = {'CostCategories': {'Key': 'CostCenter', 'Values': [cost_center_number]}}
+            values = self.__cost_explorer_operations.CE_COST_FILTERS[tag_name.upper()]['Values']
+            filter_tag_value = {'Dimensions': {'Key': 'PURCHASE_TYPE', 'Values': values}}
+            group_by = {'Type': 'DIMENSION', 'Key': 'LINKED_ACCOUNT'}
+            cost_data = self.__cost_explorer_operations.get_cost_and_usage_from_aws(start_date=start_date, end_date=end_date, granularity="MONTHLY",
+                                                                                    GroupBy=[group_by], Filter={'And': [filter_cost_center, filter_tag_value]})
+            filtered_data = self.__cost_explorer_operations.get_ce_report_filter_data(ce_response=cost_data, tag_name=tag_name)
+            if filtered_data:
+                for index_id, row in filtered_data.items():
+                    account = row.get('Account')
+                    if account in self.__replacement_account:
+                        account = self.__replacement_account[account]
+                    if account in cost_usage_data:
+                        cost_usage_data[account][index_id][f'{tag_name.title()}Usage'] = round(float(row.get(tag_name)), self.DEFAULT_ROUND_DIGITS)
+
     @logger_time_stamp
     def upload_data_elastic_search(self, linked_account_usage: dict):
         """This method uploads the data to elastic search"""
         for account, monthly_cost in linked_account_usage.items():
             monthly_account_cost = []
             for month, cost in monthly_cost.items():
                 monthly_account_cost.append(cost)
@@ -186,17 +222,17 @@
 
     def filter_cost_details_for_sp(self, total_cost: list):
         """"This method filter the account total cost"""
         results = {}
         for row in total_cost:
             start_time = row.get('TimePeriod').get('Start')
             if row.get('MeanValue'):
-                cost = round(float(row.get('MeanValue')), 3)
+                cost = round(float(row.get('MeanValue')), self.DEFAULT_ROUND_DIGITS)
             else:
-                cost = round(float(row.get('Total').get('UnblendedCost').get('Amount')), 3)
+                cost = round(float(row.get('Total').get('UnblendedCost').get('Amount')), self.DEFAULT_ROUND_DIGITS)
             results[start_time] = cost
         return results
 
     def get_monthly_cost_details(self, start_date: datetime = None, end_date: datetime = None):
         """This method list the savings plan details"""
         current_date = datetime.datetime.utcnow()
         if not start_date and not end_date:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/cost_over_usage.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/cost_over_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.__ignore_mails = self.__environment_variables_dict.get('IGNORE_MAILS', '')
         self.__ldap_host_name = self.__environment_variables_dict.get('LDAP_HOST_NAME', '')
         self.__ldap = LdapSearch(ldap_host_name=self.__ldap_host_name)
         self._elastic_upload = ElasticUpload()
 
     def get_user_used_instances(self, user_used_list: list):
         """
-        This method return user used instances group by region
+        This method returns user used instances group by region
         @return:
         """
         region_resources = {}
         if isinstance(user_used_list, list):
             for instance in user_used_list:
                 if instance:
                     if instance['Region'] in region_resources:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_in_use.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ebs_in_use.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ebs_unattached.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ebs_unattached.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,13 +48,14 @@
                                                                              resource_id='VolumeId',
                                                                              resource_type='CreateVolume',
                                                                              resource=volume,
                                                                              empty_days=last_detached_days,
                                                                              days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
                                                                              extra_purse=ebs_cost, delta_cost=delta_cost)
                         if unattached_volumes:
-                            unattached_volumes_data.append([volume.get('VolumeId'),
-                                                            self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Name'),
-                                                            self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='User'),
-                                                            str(last_detached_days),
-                                                            self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Policy')])
+                            unattached_volumes_data.append({'ResourceId': volume.get('VolumeId'),
+                                                            'Name': self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Name'),
+                                                            'User': self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='User'),
+                                                            'Days': str(last_detached_days),
+                                                            'Skip': self._get_tag_name_from_tags(tags=volume.get('Tags'), tag_name='Policy')
+                                                            })
         return unattached_volumes_data
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_idle.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ec2_idle.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,24 +112,24 @@
                                                    resource_type='InstanceId', namespace='AWS/EC2',
                                                    metric_names={'CPUUtilization': 'Percent', 'NetworkIn': 'Bytes', 'NetworkOut': 'Bytes'},
                                                    statistic='Average')
         return metrics['MetricDataResults']
 
     def __get_proposed_metrics(self, metrics: list, metric_period: int):
         """
-        This method return the metrics
+        This method returns the metrics
         @param metrics:
         @param metric_period:
         @return:
         """
         return self.__get_metrics_average(metric_list=metrics, metric_period=metric_period)
 
     def __get_time_difference(self, launch_time: datetime):
         """
-        This method return the difference of datetime
+        This method returns the difference of datetime
         @param launch_time:
         @return:
         """
         end_time = datetime.now()
         return (end_time - launch_time.replace(tzinfo=None)).days
 
     def __trigger_mail(self, tags: list, resource_id: str, days: int, ec2_type: str = '', instance_id: str = '', **kwargs):
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_run.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ec2_run.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ec2_stop.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ec2_stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,20 @@
                                             days=days, ec2_type=resource.get("InstanceType"), instance_id=instance_id, admins=self._admins,
                                             message_type='notify-admin', stop_cost=stop_cost, delta_charge=delta_charge)
                     if sign(days, instance_days):
                         if days >= delete_instance_days:
                             stopped_instance_tags[instance_id] = resource.get('Tags')
                             ec2_types[instance_id] = resource.get('InstanceType')
                             block_device_mappings[instance_id] = resource.get('BlockDeviceMappings')
-                        stopped_instances.append([resource.get('InstanceId'), self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Name'),
-                                                  self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User'), str(resource.get('LaunchTime')),
-                                                  self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Policy')
-                                                  ])
+                        stopped_instances.append({
+                            'ResourceId': resource.get('InstanceId'),
+                            'Name': self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Name'),
+                            'User': self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='User'),
+                            'LaunchTime': str(resource.get('LaunchTime')),
+                            'Policy': self._get_tag_name_from_tags(tags=resource.get('Tags'), tag_name='Policy')})
         if self._dry_run == "no":
             for instance_id, tags in stopped_instance_tags.items():
                 if self._get_policy_value(tags=tags) not in ('NOTDELETE', 'SKIP'):
                     tags.append({'Key': 'Policy', 'Value': 'backup'})
                     tag_specifications = [{'ResourceType': 'image', 'Tags': tags}]
                     if sign == ge:
                         tag_specifications.append({'ResourceType': 'snapshot', 'Tags': tags})
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/empty_roles.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/empty_roles.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """
 
     def __init__(self):
         super().__init__()
 
     def run(self):
         """
-        This method return all empty roles, delete if dry_run no
+        This method returns all empty roles, delete if dry_run no
         @return:
         """
         return self.__delete_empty_roles()
 
     def __delete_empty_roles(self):
         """
         This method deletes the role after 7 days of empty
@@ -36,14 +36,19 @@
                     if not role_inline_policies.get('PolicyNames') and not role_attached_policies.get('AttachedPolicies'):
                         role_empty = True
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='Name'):
                             tags.append({'Key': 'Name', 'Value': role_name})
                         empty_days = self._get_resource_last_used_days(tags=tags)
                         empty_role = self._check_resource_and_delete(resource_name='IAM Role', resource_id='RoleName', resource_type='CreateRole', resource=get_role, empty_days=empty_days, days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags)
                         if empty_role:
-                            zombie_roles.append([empty_role.get('RoleName'), self._get_tag_name_from_tags(tags=tags, tag_name='User'), self._get_policy_value(tags=tags), empty_days])
+                            zombie_roles.append({
+                                'ResourceId': empty_role.get('RoleName'),
+                                'Name': empty_role.get('RoleName'),
+                                'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                'Skip': self._get_policy_value(tags=tags),
+                                'Days': empty_days})
                     else:
                         empty_days = 0
                     self._update_resource_tags(resource_id=role_name, tags=tags, left_out_days=empty_days, resource_left_out=role_empty)
             except Exception as err:
                 logger.info(f'Error occur:{role_name}, {err}')
         return zombie_roles
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/ip_unattached.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/ip_unattached.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
 
     def __init__(self):
         super().__init__()
 
     def run(self):
         """
-        This method return zombie elastic_ip's and delete if dry_run no
+        This method returns zombie elastic_ip's and delete if dry_run no
         @return:
         """
         addresses = self._ec2_operations.get_elastic_ips()
         zombie_addresses = []
         for address in addresses:
             ip_no_used = False
             tags = address.get('Tags', [])
@@ -36,14 +36,17 @@
                                                                  resource_id='AllocationId',
                                                                  resource_type='AllocateAddress',
                                                                  resource=address,
                                                                  empty_days=unused_days,
                                                                  days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags,
                                                                  extra_purse=eip_cost, delta_cost=delta_cost)
                     if zombie_eip:
-                        zombie_addresses.append([address.get('AllocationId'), self._get_tag_name_from_tags(tags=tags),
-                                                 self._get_tag_name_from_tags(tags=tags, tag_name='User'), address.get('PublicIp'),
-                                                 self._get_policy_value(tags=tags), unused_days])
+                        zombie_addresses.append({'ResourceId': address.get('AllocationId'),
+                                                 'Name': self._get_tag_name_from_tags(tags=tags),
+                                                 'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                                 'PublicIp': address.get('PublicIp'),
+                                                 'Skip': self._get_policy_value(tags=tags),
+                                                 'Days': unused_days})
                 else:
                     unused_days = 0
                 self._update_resource_tags(resource_id=address.get('AllocationId'), tags=tags, left_out_days=unused_days, resource_left_out=ip_no_used)
         return zombie_addresses
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/monthly_report.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/monthly_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,24 +22,24 @@
         if self._es_host:
             self._elastic_operations = ElasticSearchOperations(es_host=self._es_host, es_port=self._es_port)
         self._postfix_mail = Postfix()
         self._mail_message = MailMessage()
 
     def policy_description(self, policy_name: str):
         """
-        This method return the policy description
+        This method returns the policy description
         @param policy_name:
         @return:
         """
         policy_descriptions = {
             'ec2_stop': 'Delete the stopped instances that are stopped for more than 30 days ',
             'ec2_idle': 'stops the idle instances in the last 7 days.  ( CPU < 5%, Network < 5k )',
             'ebs_unattached': 'Delete  unattached EBS volumes, where the unused days are calculated by the last DeattachedTime',
             'ip_unattached': 'Delete all the elastic_ips that are unused',
-            'nat_gateway_unused': ' Delete all unused nat gateways',
+            'unused_nat_gateway': ' Delete all unused nat gateways',
             'zombie_snapshots': 'Delete all the snapshots which the AMI does not use',
             's3_inactive': 'Delete the empty buckets which don’t have any content.',
             'empty_roles': 'Delete the empty role which does\'t have any policies',
             'zombie_cluster_resource': 'Delete up the cluster resources which are not deleted while cleaning the cluster'
         }
         return policy_descriptions.get(policy_name)
 
@@ -78,15 +78,15 @@
             subject, body = self._mail_message.monthly_html_mail_message(data=content)
             self._postfix_mail.send_email_postfix(subject=subject, content=body, to=self._to_mail, cc=self._to_cc, mime_type='html', message_type='monthly_report')
             return 'Successfully Send the Monthly report'
         return 'No Data to send to the Monthly report'
 
     def row_span(self, cols: int):
         """
-        This method return the table data with colspan
+        This method returns the table data with colspan
         @param cols:
         @return:
         """
         return f'<td rowspan="{cols}" align="center" style="border: 1px solid black;font-weight: bold;color:blue">'
 
     def prepare_html_table_message(self, data: dict):
         """
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/s3_inactive.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/s3_inactive.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
 
     def __init__(self):
         super().__init__()
 
     def run(self):
         """
-        This method return all Empty buckets and delete if dry_run no
+        This method returns all Empty buckets and delete if dry_run no
         @return:
         """
         return self.__delete_s3_inactive()
 
     def __delete_s3_inactive(self):
         """
         This method delete the empty bucket more than 7 days
@@ -45,14 +45,14 @@
                         empty_days = self._get_resource_last_used_days(tags=tags)
                         bucket_empty = True
                         if not self._get_tag_name_from_tags(tags=tags, tag_name='User'):
                             region = self._s3_client.get_bucket_location(Bucket=bucket_name)['LocationConstraint']
                             self._cloudtrail.set_cloudtrail(region_name=region)
                         empty_bucket = self._check_resource_and_delete(resource_name='S3 Bucket', resource_id='Name', resource_type='CreateBucket', resource=bucket, empty_days=empty_days, days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE, tags=tags)
                         if empty_bucket:
-                            empty_buckets.append([bucket.get('Name'), self._get_tag_name_from_tags(tags=tags, tag_name='User'), str(bucket.get('CreationDate')), str(empty_days), self._get_policy_value(tags=tags)])
+                            empty_buckets.append({'ResourceId': bucket.get('Name'), 'Name': bucket.get('Name'), 'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'), 'Date': str(bucket.get('CreationDate')), 'Days': str(empty_days), 'Skip': self._get_policy_value(tags=tags)})
                 else:
                     empty_days = 0
                 self._update_resource_tags(resource_id=bucket_name, tags=tags, left_out_days=empty_days, resource_left_out=bucket_empty)
             except Exception as err:
                 logger.info(f'{err}, {bucket.get("Name")}')
         return empty_buckets
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/skipped_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/skipped_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         volume_types_cost = {}
         for volume_type in volume_types:
             volume_types_cost[volume_type] = self._aws_price.get_ebs_cost(volume_type=volume_type, region=self._region)
         return volume_types_cost
 
     def get_resources(self, resource_name: str):
         """
-        This method return resource data based on resource name
+        This method returns resource data based on resource name
         @param resource_name:
         @return:
         """
         if resource_name == 'Instance':
             reservations = self._ec2_operations.get_instances()
             return [resource for instances in reservations for resource in instances['Instances']]
         elif resource_name == 'Volume':
@@ -41,27 +41,27 @@
             return self._ec2_operations.get_elastic_ips()
         else:
             if resource_name == 'NatGateway':
                 return self._ec2_operations.get_nat_gateways()
 
     def get_ebs_cost(self, volume_id: str):
         """
-        This method return the size of the ebs_volume
+        This method returns the size of the ebs_volume
         @param volume_id:
         @return:
         """
         volume_types = {'standard': 'standard', 'io1': 'io', 'io2': 'io', 'gp2': 'gp', 'gp3': 'gp', 'sc1': 'sc1',
                         'st1': 'st1'}
         volume = self._ec2_client.describe_volumes(VolumeIds=[volume_id])['Volumes'][0]
         volume_type = volume.get('VolumeType')
         return volume.get('Size') * float(self._ebs_prices[volume_types[volume_type]])
 
     def get_instance_volume_size(self, resource: dict):
         """
-        This method return size of the attached volumes of the instance
+        This method returns size of the attached volumes of the instance
         @param resource:
         @return:
         """
         stopped_time = self._cloudtrail.get_stop_time(resource_id=resource.get('InstanceId'), event_name='StopInstances')
         if stopped_time:
             calculate_days = self._calculate_days(create_date=stopped_time)
         else:
@@ -102,15 +102,15 @@
                         resource_data['ResourceName'] = resource_type
                         not_delete_resources.append(resource_data)
 
         return not_delete_resources
 
     def run(self):
         """
-        This method return all tag "Not_Delete" or "skip" resources
+        This method returns all tag "Not_Delete" or "skip" resources
         @return:
         """
         resources_data = self.get_not_delete_resources()
         if self._es_upload.es_host:
             end_datetime = datetime.datetime.now().replace(hour=0, minute=0, second=0, microsecond=0)
             start_datetime = end_datetime - datetime.timedelta(1)
             # deleting past data to show fresh report
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_cluster_resource.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/zombie_cluster_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.delete_iam_resource = DeleteIAMResources(iam_client=self.iam_client)
         self.delete_s3_resource = DeleteS3Resources(s3_client=self.s3_client, s3_resource=self.s3_resource)
         self.ec2_operations = EC2Operations(region=region)
         self.__get_details_resource_list = Utils().get_details_resource_list
 
     def all_cluster_instance(self):
         """
-        This method return list of cluster's instance tag name that contains openshift tag prefix from all regions
+        This method returns list of cluster's instance tag name that contains openshift tag prefix from all regions
         :return: list of cluster's instance tag name
         """
         instances_list = []
         result_instance = {}
         regions_data = self.ec2_client.describe_regions()
         for region in regions_data['Regions']:
             __ec2 = boto3.client('ec2', region_name=region['RegionName'])
@@ -59,15 +59,15 @@
                         for tag in item['Tags']:
                             if tag['Key'].startswith(self.cluster_prefix):
                                 result_instance[instance_id] = tag['Key']
         return result_instance
 
     def _cluster_instance(self):
         """
-        This method return list of cluster's instance tag name that contains openshift tag prefix
+        This method returns list of cluster's instance tag name that contains openshift tag prefix
         :return: list of cluster's instance tag name
         """
         instances_list = []
         result_instance = {}
         ec2s_data = self.ec2_operations.get_instances()
         for items in ec2s_data:
             if items.get('Instances'):
@@ -81,15 +81,15 @@
                         if tag['Key'].startswith(self.cluster_prefix):
                             result_instance[instance_id] = tag['Key']
 
         return result_instance
 
     def __get_cluster_resources(self, resources_list: list, input_resource_id: str, tags: str = 'Tags'):
         """
-        This method return all cluster resources keys that start with cluster prefix
+        This method returns all cluster resources keys that start with cluster prefix
         :param resources_list:
         :param tags:
         :return: dictionary of the resources key and id
         """
         result_resources_key_id = {}
         for resource in resources_list:
             if resource.get(input_resource_id):
@@ -177,15 +177,15 @@
             for key, value in exist_resources.items():
                 if zombie_value == value:
                     zombie_resources[key] = value
         return zombie_resources
 
     def zombie_cluster_volume(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's volume according to cluster tag name and cluster name data
+        This method returns list of cluster's volume according to cluster tag name and cluster name data
         delete only available resource that related to cluster
         """
         available_volumes = []
         volumes_data = self.ec2_operations.get_volumes()
         # filter in-use resource
         for volume in volumes_data:
             if volume['State'] == 'available':
@@ -203,15 +203,15 @@
                     if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource_id=zombie, resource='ec2_volume')
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_ami(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's ami according to cluster tag name and cluster name data
+        This method returns list of cluster's ami according to cluster tag name and cluster name data
         """
         images_data = self.ec2_operations.get_images()
         exist_ami = self.__get_cluster_resources(resources_list=images_data, input_resource_id='ImageId')
         zombies = self.__get_zombie_resources(exist_ami)
         resources = self._get_tags_of_zombie_resources(resources=images_data, resource_id_name='ImageId',
                                                        zombies=zombies, aws_service='ec2')
         cluster_left_out_days = {}
@@ -230,15 +230,15 @@
                             logger.info(f'deregister_image: {zombie}')
                 except Exception as err:
                     logger.exception(f'Cannot deregister_image: {zombie}, {err}')
         return zombies, cluster_left_out_days
 
     def zombie_cluster_snapshot(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's snapshot according to cluster tag name and cluster name data
+        This method returns list of cluster's snapshot according to cluster tag name and cluster name data
         """
         snapshots_data = self.ec2_operations.get_snapshots()
         exist_snapshot = self.__get_cluster_resources(resources_list=snapshots_data, input_resource_id='SnapshotId')
         zombies = self.__get_zombie_resources(exist_snapshot)
         resources = self._get_tags_of_zombie_resources(resources=snapshots_data, resource_id_name='SnapshotId', zombies=zombies, aws_service='ec2')
         cluster_left_out_days = {}
         if zombies:
@@ -314,15 +314,15 @@
                     tag = self.__get_vpc_tags(vpc_id=vpc_id, cluster_tag=cluster_tag)
                     if tag:
                         ids[resource.get(output_tag)] = tag
         return ids
 
     def zombie_cluster_security_group(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of zombie cluster's security groups compare to existing instances and cluster name data
+        This method returns list of zombie cluster's security groups compare to existing instances and cluster name data
         :return: list of zombie cluster's security groups
         """
         security_groups = self.ec2_operations.get_security_groups()
         exist_security_group = self.__get_cluster_resources(resources_list=security_groups, input_resource_id='GroupId')
         zombies = self.__get_zombie_resources(exist_security_group)
         if vpc_id and not zombies:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=security_groups, output_tag='GroupId', cluster_tag=cluster_tag_vpc)
@@ -342,15 +342,15 @@
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource('security_group', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_elastic_ip(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of zombie cluster's elastic ip according to existing instances and cluster name data
+        This method returns list of zombie cluster's elastic ip according to existing instances and cluster name data
         """
         exist_elastic_ip_association = []
         exist_elastic_ip_allocation = []
         elastic_ips_data = self.ec2_operations.get_elastic_ips()
         for elastic_ip in elastic_ips_data:
             if elastic_ip.get('AssociationId'):
                 exist_elastic_ip_association.append(elastic_ip)
@@ -380,15 +380,15 @@
                     if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='elastic_ip', resource_id=zombie, cluster_tag=cluster_tag)
         zombies = {**zombies_all}
         return zombies, cluster_left_out_days
 
     def zombie_cluster_network_interface(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of zombie cluster's network interface according to existing instances and cluster name data
+        This method returns list of zombie cluster's network interface according to existing instances and cluster name data
         """
         network_interfaces_data = self.ec2_operations.get_network_interface()
         exist_network_interface = self.__get_cluster_resources(resources_list=network_interfaces_data, input_resource_id='NetworkInterfaceId', tags='TagSet')
         zombies = self.__get_zombie_resources(exist_network_interface)
         if not zombies and vpc_id:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=network_interfaces_data, output_tag='NetworkInterfaceId', tags='TagSet', cluster_tag=cluster_tag_vpc)
         resources = self._get_tags_of_zombie_resources(resources=network_interfaces_data, resource_id_name='NetworkInterfaceId', zombies=zombies, aws_service='ec2', aws_tag='TagSet')
@@ -409,15 +409,15 @@
                     if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='network_interface', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_load_balancer(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's load balancer according to cluster vpc and cluster name data
+        This method returns list of cluster's load balancer according to cluster vpc and cluster name data
         """
 
         exist_load_balancer = {}
         load_balancers_data = self.ec2_operations.get_load_balancers()
         for resource in load_balancers_data:
             resource_id = resource['LoadBalancerName']
             tags = self.elb_client.describe_tags(LoadBalancerNames=[resource_id])
@@ -443,15 +443,15 @@
                 else:
                     if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer', resource_id=zombie, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_load_balancer_v2(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's load balancer according to cluster vpc and cluster name data
+        This method returns list of cluster's load balancer according to cluster vpc and cluster name data
         """
         exist_load_balancer = {}
         load_balancers_data = self.ec2_operations.get_load_balancers_v2()
         for resource in load_balancers_data:
             resource_id = resource['LoadBalancerArn']
             tags = self.elbv2_client.describe_tags(ResourceArns=[resource_id])
             for item in tags['TagDescriptions']:
@@ -476,26 +476,26 @@
                 else:
                     if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='load_balancer_v2', resource_id=zombie, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def __get_all_exist_vpcs(self):
         """
-        This method return all exist vpc ids (for supporting Network ACL - missing OpenShift tags)
+        This method returns all exist vpc ids (for supporting Network ACL - missing OpenShift tags)
         :return:
         """
         vpcs_data = self.ec2_operations.get_vpcs()
         vpcs_list = []
         for resource in vpcs_data:
             vpcs_list.append(resource['VpcId'])
         return vpcs_list
 
     def zombie_cluster_vpc(self):
         """
-        This method return list of cluster's vpc according to cluster tag name and cluster name data
+        This method returns list of cluster's vpc according to cluster tag name and cluster name data
         """
         vpcs_data = self.ec2_operations.get_vpcs()
         exist_vpc = self.__get_cluster_resources(resources_list=vpcs_data, input_resource_id='VpcId')
         zombies = self.__get_zombie_resources(exist_vpc)
         delete_dict = {"ELB": self.zombie_cluster_load_balancer, "ELBV2": self.zombie_cluster_load_balancer_v2,
                        "VPCE": self.zombie_cluster_vpc_endpoint, "DHCP": self.zombie_cluster_dhcp_option,
                        "RT": self.zombie_cluster_route_table, "SG": self.zombie_cluster_security_group,
@@ -513,15 +513,15 @@
                     if self._force_delete and self.delete:
                         self.delete_ec2_resource.delete_zombie_resource(resource='vpc', resource_id=zombie, pending_resources=delete_dict, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_subnet(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's subnet according to cluster tag name and cluster name data
+        This method returns list of cluster's subnet according to cluster tag name and cluster name data
         """
         subnets_data = self.ec2_operations.get_subnets()
         exist_subnet = self.__get_cluster_resources(resources_list=subnets_data, input_resource_id='SubnetId')
         zombies = self.__get_zombie_resources(exist_subnet)
         if not zombies and vpc_id:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=subnets_data, output_tag='SubnetId',
                                                    cluster_tag=cluster_tag_vpc)
@@ -540,15 +540,15 @@
                     if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='subnet', resource_id=zombie_id,  cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_route_table(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's route table according to cluster tag name and cluster name data
+        This method returns list of cluster's route table according to cluster tag name and cluster name data
         """
         route_tables_data = self.ec2_operations.get_route_tables()
         exist_route_table = self.__get_cluster_resources(resources_list=route_tables_data, input_resource_id='RouteTableId')
         zombies = self.__get_zombie_resources(exist_route_table)
         if not zombies and vpc_id:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=route_tables_data, output_tag='RouteTableId', cluster_tag=cluster_tag_vpc)
         resources = self._get_tags_of_zombie_resources(resources=route_tables_data, resource_id_name='RouteTableId', zombies=zombies, aws_service='ec2')
@@ -567,15 +567,15 @@
                     if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='route_table', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_internet_gateway(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's route table internet gateway according to cluster tag name and cluster name data
+        This method returns list of cluster's route table internet gateway according to cluster tag name and cluster name data
         """
         internet_gateways_data = self.ec2_operations.get_internet_gateways()
         exist_internet_gateway = self.__get_cluster_resources(resources_list=internet_gateways_data, input_resource_id='InternetGatewayId')
         zombies = self.__get_zombie_resources(exist_internet_gateway)
         if not zombies and vpc_id:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=internet_gateways_data, output_tag='InternetGatewayId', input_tag='Attachments', cluster_tag=cluster_tag_vpc)
         resources = self._get_tags_of_zombie_resources(resources=internet_gateways_data, resource_id_name='InternetGatewayId', zombies=zombies, aws_service='ec2')
@@ -597,15 +597,15 @@
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='internet_gateway', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_dhcp_option(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's dhcp option according to cluster tag name and cluster name data
+        This method returns list of cluster's dhcp option according to cluster tag name and cluster name data
         """
         dhcp_options_data = self.ec2_operations.get_dhcp_options()
         exist_dhcp_option = self.__get_cluster_resources(resources_list=dhcp_options_data, input_resource_id='DhcpOptionsId')
         zombies = self.__get_zombie_resources(exist_dhcp_option)
         resources = self._get_tags_of_zombie_resources(resources=dhcp_options_data, resource_id_name='DhcpOptionsId', zombies=zombies, aws_service='ec2')
         cluster_left_out_days = {}
         vpcs = self.ec2_client.describe_vpcs()['Vpcs']
@@ -624,15 +624,15 @@
                             self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie, vpc_id=vpc_id)
                         else:
                             self.delete_ec2_resource.delete_zombie_resource(resource='dhcp_options', resource_id=zombie)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_vpc_endpoint(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of cluster's vpc endpoint according to cluster tag name and cluster name data
+        This method returns list of cluster's vpc endpoint according to cluster tag name and cluster name data
         """
         vpc_endpoints_data = self.ec2_operations.get_vpce()
         exist_vpc_endpoint = self.__get_cluster_resources(resources_list=vpc_endpoints_data, input_resource_id='VpcEndpointId')
         zombies = self.__get_zombie_resources(exist_vpc_endpoint)
         if not zombies and vpc_id:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=vpc_endpoints_data, output_tag='VpcEndpointId', cluster_tag=cluster_tag_vpc)
         resources = self._get_tags_of_zombie_resources(resources=vpc_endpoints_data, resource_id_name='VpcEndpointId', zombies=zombies, aws_service='ec2')
@@ -653,15 +653,15 @@
                     if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='vpc_endpoints', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_nat_gateway(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of zombie cluster's nat gateway according to cluster tag name and cluster name data
+        This method returns list of zombie cluster's nat gateway according to cluster tag name and cluster name data
         """
         nat_gateways_data = self.ec2_operations.get_nat_gateways()
         exist_nat_gateway = self.__get_cluster_resources(resources_list=nat_gateways_data, input_resource_id='NatGatewayId')
         zombies = self.__get_zombie_resources(exist_nat_gateway)
         if not zombies and vpc_id:
             zombies = self.__get_zombies_by_vpc_id(vpc_id=vpc_id, resources=nat_gateways_data, output_tag='NatGatewayId', cluster_tag=cluster_tag_vpc)
         resources = self._get_tags_of_zombie_resources(resources=nat_gateways_data, resource_id_name='NatGatewayId', zombies=zombies, aws_service='ec2')
@@ -679,15 +679,15 @@
                     if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='nat_gateways', resource_id=zombie_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_network_acl(self, vpc_id: str = '', cluster_tag_vpc: str = ''):
         """
-        This method return list of zombie cluster's network acl according to existing vpc id and cluster name data
+        This method returns list of zombie cluster's network acl according to existing vpc id and cluster name data
         """
         exist_network_acl = {}
         network_acls_data = self.ec2_operations.get_nacls()
         for resource in network_acls_data:
             exist_network_acl[resource['NetworkAclId']] = resource['VpcId']
         zombie_resources = {}
         all_exist_vpcs = self.__get_all_exist_vpcs()
@@ -716,15 +716,15 @@
                     if self._force_delete and self.delete:
                         for zombie_id in zombie_ids:
                             self.delete_ec2_resource.delete_zombie_resource(resource='network_acl', resource_id=zombie_id, vpc_id=vpc_id, cluster_tag=cluster_tag)
         return zombies, cluster_left_out_days
 
     def zombie_cluster_role(self):
         """
-        This method return list of cluster's role in all regions according to cluster name and cluster name data
+        This method returns list of cluster's role in all regions according to cluster name and cluster name data
         * Role is a global resource, need to scan for live cluster in all regions
         """
         exist_role_name_tag = {}
         roles_data = self.__get_details_resource_list(func_name=self.iam_client.list_roles, input_tag='Roles', check_tag='Marker')
         for role in roles_data:
             role_name = role['RoleName']
             if 'worker-role' in role_name or 'master-role' in role_name:
@@ -753,15 +753,15 @@
                     else:
                         if self._force_delete and self.delete:
                             self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_role')
         return zombies, cluster_left_out_days
 
     def zombie_cluster_user(self):
         """
-        This method return list of cluster's user according to cluster name and cluster name data
+        This method returns list of cluster's user according to cluster name and cluster name data
         * User is a global resource, need to scan for live cluster in all regions
         """
         exist_user_name_tag = {}
         users_data = self.__get_details_resource_list(func_name=self.iam_client.list_users, input_tag='Users', check_tag='Marker')
         for user in users_data:
             user_name = user['UserName']
             user_data = self.iam_client.get_user(UserName=user_name)
@@ -788,15 +788,15 @@
                     if self._force_delete and self.delete:
                         self.delete_iam_resource.delete_iam_zombie_resource(resource_id=zombie, resource_type='iam_user')
 
         return zombies, cluster_left_out_days
 
     def zombie_cluster_s3_bucket(self, cluster_stamp: str = 'image-registry'):
         """
-        This method return list of cluster's s3 bucket according to cluster name and cluster name data
+        This method returns list of cluster's s3 bucket according to cluster name and cluster name data
         * S3 is a global resource, need to scan for live cluster in all regions
         """
         exist_bucket_name_tag = {}
         response = self.s3_client.list_buckets()
 
         # Fetch all bucket with stamp
         for bucket in response['Buckets']:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/aws/zombie_snapshots.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/aws/zombie_snapshots.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         images_array = snapshot_description.split('ami-')[1:]
         for image in images_array:
             image_ids.append(f'ami-{image.split(" ")[0]}')
         return image_ids
 
     def run(self):
         """
-        This method return all the zombie snapshots, delete if dry_run no
+        This method returns all the zombie snapshots, delete if dry_run no
         @return:
         """
         snapshots = self._ec2_operations.get_snapshots()
         zombie_snapshots = []
         image_ids = self._get_ami_ids()
         for snapshot in snapshots:
             if not self._check_cluster_tag(tags=snapshot.get('Tags')):
@@ -47,18 +47,19 @@
                                                                           resource_id='SnapshotId',
                                                                           resource_type='CreateSnapshot',
                                                                           resource=snapshot,
                                                                           empty_days=unused_days,
                                                                           days_to_delete_resource=self.DAYS_TO_DELETE_RESOURCE,
                                                                           tags=tags)
                         if zombie_snapshot:
-                            zombie_snapshots.append([snapshot.get('SnapshotId'),
-                                                     self._get_tag_name_from_tags(tags=tags),
-                                                     self._get_tag_name_from_tags(tags=tags, tag_name='User'),
-                                                     f'{str(snapshot.get("VolumeSize"))}Gb',
-                                                     self._get_policy_value(tags=snapshot.get('Tags')), str(unused_days)
-                                                     ])
+                            zombie_snapshots.append({'ResourceId': snapshot.get('SnapshotId'),
+                                                     'Name': self._get_tag_name_from_tags(tags=tags),
+                                                     'User': self._get_tag_name_from_tags(tags=tags, tag_name='User'),
+                                                     'Size': f'{str(snapshot.get("VolumeSize"))}Gb',
+                                                     'Skip': self._get_policy_value(tags=snapshot.get('Tags')),
+                                                     'Days': str(unused_days)
+                            })
                     else:
                         unused_days = 0
                     self._update_resource_tags(resource_id=snapshot_id, tags=tags, left_out_days=unused_days,
                                                resource_left_out=not found)
         return zombie_snapshots
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/azure/cost_billing_reports.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/azure/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/gcp/cost_billing_reports.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/gcp/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/cost_billing_reports.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/cost_billing_reports.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_over_usage.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/ibm_cost_over_usage.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/ibm_cost_report.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/ibm_cost_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self.year = self.__environment_variables_dict.get('year', '')
         self.owned_tags = ['owner', 'budget', 'environment', 'manager', 'user', 'project', 'fqdn']
         self._elastic_upload = ElasticUpload()
 
     @typechecked
     def collect_tags_from_machines(self, tags: list):
         """
-        This method return tags from list of string tags
+        This method returns tags from list of string tags
         @param tags:
         @return:
         """
         hardware_tags = {}
         if tags:
             for tag in tags:
                 if ':' in tag:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_baremetal.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/tag_baremetal.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/ibm/tag_vm.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/ibm/tag_vm.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
 
     def __init__(self):
         super().__init__()
 
     def get_virtual_machine_username(self, vm_id: str):
         """
-        This method return the virtual machine username from the billing order lists
+        This method returns the virtual machine username from the billing order lists
         @param vm_id:
         @return:
         """
         vm_data = self._classic_operations.get_virtual_machine_data(vm_id=str(vm_id))
         return vm_data.get('billingItem').get('orderItem').get('order').get('userRecord').get('username'), f'{vm_data.get("hostname")}.{vm_data.get("domain")}'
 
     def tag_update_virtual_machine(self, user_tags: list, vm_tags: list, vm_id: str, vm_name: str):
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/cost_expenditure/cost_report_policies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/cloudtrail_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/dynamodb_upload_data/upload_data_to_dynamodb.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/remove_cluster_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             added_tags.extend(self._input_tags_list_builder())
             self.ec2_client.delete_tags(Resources=instance_list, Tags=added_tags)
             logger.info(f'InstanceId :: {instance_list} {added_tags}')
         return added_tags
 
     def get_cluster(self, clusters: list):
         """
-        This method return cluster, and it tags
+        This method returns cluster, and it tags
         @param clusters:
         @return:
         """
         cluster_dict = {}
         cluster_tags = {}
         for instance in clusters:
             for item in instance:
@@ -201,15 +201,15 @@
             cluster_process = Process(target=self.remove_tags_of_resources, args=(cluster_images, instance_tags, 'ImageId',))
             cluster_process.start()
             cluster_process.join()
         return len(cluster_images)
 
     def cluster_snapshot(self, instance_tags: dict):
         """
-        This method return list of cluster's snapshot according to cluster tag name
+        This method returns list of cluster's snapshot according to cluster tag name
         @return:
         """
         snapshots_data = self.ec2_operations.get_snapshots()
         cluster_snapshot, non_cluster_snapshot = self.ec2_operations.scan_cluster_non_cluster_resources(
             snapshots_data)
         if not self.cluster_only:
             cluster_process = Process(target=self.remove_tags_of_resources, args=(cluster_snapshot, instance_tags, 'SnapshotId', ))
@@ -454,15 +454,15 @@
                     tags = list(instance_tags.get(full_name))
             logger.info(f'Role Name :: {role_name_list} {tags}')
             cluster_ids.extend(role_name_list)
         return cluster_ids
 
     def cluster_user(self, instance_tags: dict):
         """
-        This method return list of cluster's user according to cluster name
+        This method returns list of cluster's user according to cluster name
         @param instance_tags:
         @return:
         """
         # tag_user
         cluster_names = [name.split('/')[-1] for name in instance_tags.keys()]
         user_ids = []
         for cluster_name in cluster_names:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/run_tag_cluster_resouces.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_cluster/tag_cluster_resouces.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             if not tag.get('Key').startswith('aws'):
                 filter_tags.append(tag)
         return filter_tags
 
     def __generate_cluster_resources_list_by_tag(self, resources_list: list, input_resource_id: str,
                                                  tags: str = 'Tags'):
         """
-        This method return resource list that related to input resource id according to cluster's tag name and update the tags
+        This method returns resource list that related to input resource id according to cluster's tag name and update the tags
         @param resources_list:
         @param input_resource_id:
         @param ids:
         @param tags:
         @return:
         """
         cluster_ids = {}
@@ -147,15 +147,15 @@
                 except Exception as err:
                     logger.info(err)
             result_resources_list.extend(cluster_id)
         return sorted(result_resources_list)
 
     def __generate_cluster_resources_list_by_vpc(self, resources_list: list, input_resource_id: str):
         """
-        This method return resource list that related to input resource id according to cluster's vpc id
+        This method returns resource list that related to input resource id according to cluster's vpc id
         @param resources_list:
         @param input_resource_id:
         @return:
         """
         result_resources_list = []
         vpc_data = self.get_cluster_vpc()
         for resource in resources_list:
@@ -224,21 +224,21 @@
     def __validate_existing_tag(self, tags: list):
         """
         This method validates that permanent tag exists in tags list
         @param tags:
         @return:
         """
         check_tags = ['User', 'Project', 'Manager', 'Owner', 'Email']
+        tag_count = 0
         for tag in tags:
             if tag.get('Key') in check_tags:
+                tag_count += 1
                 if tag.get('Value') == 'NA':
                     return False
-            else:
-                return False
-        return True
+        return tag_count == len(check_tags)
 
     def update_cluster_tags(self, resources: list):
         """
         This method update the Cluster instance tags and returns the updated tags list ids.
         @param resources:
         @param queue:
         @return:
@@ -253,15 +253,16 @@
                 if tags:
                     # search that not exist permanent tags in the resource
                     if not self.__validate_existing_tag(tags):
                         for tag in tags:
                             if self.cluster_prefix in tag.get('Key'):
                                 add_tags = self.__append_input_tags()
                                 cluster_name = tag.get('Key').split('/')[-1]
-                                if cluster_name in cluster_instances:
+                                user = self.ec2_operations.get_tag_value_from_tags(tags=tags, tag_name='User')
+                                if cluster_name in cluster_instances and user and user != 'NA':
                                     add_tags = self.__filter_resource_tags_by_add_tags(tags=tags, search_tags=cluster_tags[cluster_name])
                                     if add_tags:
                                         cluster_instances[cluster_name].append(instance_id)
                                     break
                                 else:
                                     username = self.get_username(start_time=item.get('LaunchTime'), resource_id=instance_id, resource_type='AWS::EC2::Instance', tags=tags)
                                     if username:
@@ -288,15 +289,15 @@
                                         add_tags.extend(self._fill_na_tags())
                                     add_tags.append({'Key': 'LaunchTime',
                                                      'Value': self.get_date_from_date_time(item.get('LaunchTime'))})
                                     add_tags = self.remove_creation_date(add_tags)
                                     add_tags = self.__filter_resource_tags_by_add_tags(tags=item.get('Tags'),
                                                                                        search_tags=add_tags)
                                     if add_tags:
-                                        cluster_instances[cluster_name] = [instance_id]
+                                        cluster_instances.setdefault(cluster_name, []).append(instance_id)
                                         cluster_tags[cluster_name] = add_tags
                                     break
         for cluster_instance_name, instance_ids in cluster_instances.items():
             if self.dry_run == 'no':
                 try:
                     self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=instance_ids, tags=cluster_tags.get(cluster_instance_name))
                     logger.info(f'Cluster :: {cluster_instance_name} count: {len(instance_ids)} :: InstanceId :: {instance_ids} :: {cluster_tags.get(cluster_instance_name)}')
@@ -308,15 +309,15 @@
             self.cluster_role(list(cluster_instances.keys()))
             self.cluster_user(list(cluster_instances.keys()))
             self.cluster_s3_bucket(list(cluster_instances.keys()))
         return sorted(result_instance_list)
 
     def cluster_instance(self):
         """
-        This method return list of cluster's instance according to cluster tag name,
+        This method returns list of cluster's instance according to cluster tag name,
         The instances list is different from other resources
         it will search for full cluster name (including random suffix string) in case of user input cluster name was given
         @return:
         """
         self.cluster_key = self.__init_cluster_name()
         instances_list = self._get_instances_data()
         if instances_list:
@@ -329,98 +330,98 @@
                 ids = self.update_cluster_tags(cluster)
                 return ids
         else:
             return []
 
     def cluster_volume(self):
         """
-        This method return list of cluster's volume according to cluster tag name
+        This method returns list of cluster's volume according to cluster tag name
         @return:
         """
         volumes_data = self.ec2_operations.get_volumes()
         cluster, non_cluster = self.ec2_operations.scan_cluster_non_cluster_resources(volumes_data)
         if not self.cluster_only:
             ids = self.__generate_cluster_resources_list_by_tag(cluster, 'VolumeId')
             self.non_cluster_update.update_volumes(non_cluster)
         else:
             ids = self.__generate_cluster_resources_list_by_tag(cluster, 'VolumeId')
         return ids
 
     def cluster_ami(self):
         """
-        This method return list of cluster's ami according to cluster tag name
+        This method returns list of cluster's ami according to cluster tag name
         @return:
         """
         images_data = self.ec2_operations.get_images()
         cluster, non_cluster = self.ec2_operations.scan_cluster_non_cluster_resources(images_data)
         if not self.cluster_only:
             ids = self.__generate_cluster_resources_list_by_tag(cluster, 'ImageId')
             self.non_cluster_update.update_ami(non_cluster)
         else:
             ids = self.__generate_cluster_resources_list_by_tag(cluster, 'ImageId')
         return ids
 
     def cluster_snapshot(self):
         """
-        This method return list of cluster's snapshot according to cluster tag name
+        This method returns list of cluster's snapshot according to cluster tag name
         @return:
         """
         snapshots_data = self.ec2_operations.get_snapshots()
         cluster, non_cluster = self.ec2_operations.scan_cluster_non_cluster_resources(snapshots_data)
         if not self.cluster_only:
             ids = self.__generate_cluster_resources_list_by_tag(cluster, 'SnapshotId')
             self.non_cluster_update.update_snapshots(non_cluster)
         else:
             ids = self.__generate_cluster_resources_list_by_tag(cluster, 'SnapshotId')
         return ids
 
     def __get_security_group_data(self):
         """
-        This method return security group data
+        This method returns security group data
         @return:
         """
         return self.ec2_operations.get_security_groups()
 
     def cluster_security_group(self):
         """
-        This method return list of cluster's security group according to cluster tag name
+        This method returns list of cluster's security group according to cluster tag name
         @return:
         """
         security_group_ids = self.__generate_cluster_resources_list_by_tag(
             resources_list=self.__get_security_group_data(),
             input_resource_id='GroupId')
         logger.info(f'cluster_security_group count: {len(sorted(security_group_ids))} {sorted(security_group_ids)}')
 
     def cluster_elastic_ip(self):
         """
-        This method return list of cluster's elastic ip according to cluster tag name
+        This method returns list of cluster's elastic ip according to cluster tag name
         @return:
         """
         elastic_ips_data = self.ec2_operations.get_elastic_ips()
         elastic_ips = self.__generate_cluster_resources_list_by_tag(resources_list=elastic_ips_data,
                                                                     input_resource_id='AllocationId')
         logger.info(f'cluster_elastic_ip count: {len(sorted(elastic_ips))} {sorted(elastic_ips)}')
         return sorted(elastic_ips)
 
     def cluster_network_interface(self):
         """
-        This method return list of cluster's network interface according to cluster tag name
+        This method returns list of cluster's network interface according to cluster tag name
         @return:
         """
         network_interfaces_data = self.ec2_operations.get_network_interface()
         network_interface_ids = self.__generate_cluster_resources_list_by_tag(resources_list=network_interfaces_data,
                                                                               input_resource_id='NetworkInterfaceId',
                                                                               tags='TagSet')
         logger.info(
             f'cluster_network_interface count: {len(sorted(network_interface_ids))} {sorted(network_interface_ids)}')
         return sorted(network_interface_ids)
 
     def cluster_load_balancer(self):
         """
-        This method return list of cluster's load balancer according to cluster vpc
+        This method returns list of cluster's load balancer according to cluster vpc
         @return:
         """
         result_resources_list = []
         load_balancers_data = self.ec2_operations.get_load_balancers()
         for resource in load_balancers_data:
             resource_id = resource['LoadBalancerName']
             tags = self.elb_client.describe_tags(LoadBalancerNames=[resource_id])
@@ -460,15 +461,15 @@
                                 break
         logger.info(
             f'cluster_load_balancer count: {len(sorted(result_resources_list))} {sorted(result_resources_list)}')
         return sorted(result_resources_list)
 
     def cluster_load_balancer_v2(self):
         """
-        This method return list of cluster's load balancer according to cluster vpc
+        This method returns list of cluster's load balancer according to cluster vpc
         @return:
         """
         result_resources_list = []
         load_balancers_data = self.ec2_operations.get_load_balancers_v2()
         for resource in load_balancers_data:
             resource_id = resource['LoadBalancerArn']
             tags = self.elbv2_client.describe_tags(ResourceArns=[resource_id])
@@ -508,15 +509,15 @@
                                 break
         logger.info(
             f'cluster_load_balancer_v2 count: {len(sorted(result_resources_list))} {sorted(result_resources_list)}')
         return sorted(result_resources_list)
 
     def cluster_vpc(self):
         """
-        This method return list of cluster's vpc according to cluster tag name
+        This method returns list of cluster's vpc according to cluster tag name
         @return:
         """
         vpcs_data = self.ec2_operations.get_vpcs()
         vpc_ids = self.__generate_cluster_resources_list_by_tag(resources_list=vpcs_data, input_resource_id='VpcId')
         logger.info(f'cluster_vpc count: {len(sorted(vpc_ids))} {sorted(vpc_ids)}')
         self.cluster_network_acl()
         return sorted(vpc_ids)
@@ -535,94 +536,94 @@
                     if self.cluster_prefix in tag.get('Key'):
                         vpc_ids[vpc.get('VpcId')] = [tag for tag in vpc.get('Tags') if tag.get('Key') != 'Name']
                         break
         return vpc_ids
 
     def cluster_subnet(self):
         """
-        This method return list of cluster's subnet according to cluster tag name
+        This method returns list of cluster's subnet according to cluster tag name
         @return:
         """
         subnets_data = self.ec2_operations.get_subnets()
         subnet_ids = self.__generate_cluster_resources_list_by_tag(resources_list=subnets_data,
                                                                    input_resource_id='SubnetId')
         logger.info(f'cluster_subnet count: {len(sorted(subnet_ids))} {sorted(subnet_ids)}')
         return sorted(subnet_ids)
 
     def cluster_route_table(self):
         """
-        This method return list of cluster's route table according to cluster tag name
+        This method returns list of cluster's route table according to cluster tag name
         @return:
         """
         route_tables_data = self.ec2_operations.get_route_tables()
         route_table_ids = self.__generate_cluster_resources_list_by_tag(resources_list=route_tables_data,
                                                                         input_resource_id='RouteTableId')
         logger.info(f'cluster_route_table count: {len(sorted(route_table_ids))} {sorted(route_table_ids)}')
         return sorted(route_table_ids)
 
     def cluster_internet_gateway(self):
         """
-        This method return list of cluster's route table internet gateway according to cluster tag name
+        This method returns list of cluster's route table internet gateway according to cluster tag name
         @return:
         """
         internet_gateways_data = self.ec2_operations.get_internet_gateways()
         internet_gateway_ids = self.__generate_cluster_resources_list_by_tag(resources_list=internet_gateways_data,
                                                                              input_resource_id='InternetGatewayId')
         logger.info(
             f'cluster_internet_gateway count: {len(sorted(internet_gateway_ids))} {sorted(internet_gateway_ids)}')
         return sorted(internet_gateway_ids)
 
     def cluster_dhcp_option(self):
         """
-        This method return list of cluster's dhcp option according to cluster tag name
+        This method returns list of cluster's dhcp option according to cluster tag name
         @return:
         """
         dhcp_options_data = self.ec2_operations.get_dhcp_options()
         dhcp_ids = self.__generate_cluster_resources_list_by_tag(resources_list=dhcp_options_data,
                                                                  input_resource_id='DhcpOptionsId')
         logger.info(f'cluster_dhcp_option count: {len(sorted(dhcp_ids))} {sorted(dhcp_ids)}')
         return sorted(dhcp_ids)
 
     def cluster_vpc_endpoint(self):
         """
-        This method return list of cluster's vpc endpoint according to cluster tag name
+        This method returns list of cluster's vpc endpoint according to cluster tag name
         @return:
         """
         vpc_endpoints_data = self.ec2_operations.get_vpce()
         vpc_endpoint_ids = self.__generate_cluster_resources_list_by_tag(resources_list=vpc_endpoints_data,
                                                                          input_resource_id='VpcEndpointId')
         logger.info(f'cluster_vpc_endpoint count: {len(sorted(vpc_endpoint_ids))} {sorted(vpc_endpoint_ids)}')
         return sorted(vpc_endpoint_ids)
 
     def cluster_nat_gateway(self):
         """
-        This method return list of cluster's nat gateway according to cluster tag name
+        This method returns list of cluster's nat gateway according to cluster tag name
         @return:
         """
         nat_gateways_data = self.ec2_operations.get_nat_gateways()
         nat_gateway_id = self.__generate_cluster_resources_list_by_tag(resources_list=nat_gateways_data,
                                                                        input_resource_id='NatGatewayId')
         logger.info(f'cluster_nat_gateway count: {len(sorted(nat_gateway_id))} {sorted(nat_gateway_id)}')
         return sorted(nat_gateway_id)
 
     def cluster_network_acl(self):
         """
-        This method return list of cluster's network acl according to cluster vpc id
+        This method returns list of cluster's network acl according to cluster vpc id
         Missing OpenShift Tags for it based on VPCs
         @return:
         """
         network_acls_data = self.ec2_operations.get_nacls()
         network_acl_ids = self.__generate_cluster_resources_list_by_vpc(resources_list=network_acls_data,
                                                                         input_resource_id='NetworkAclId')
         logger.info(f'cluster_network_acl count: {len(network_acl_ids)}, {network_acl_ids}')
         return sorted(network_acl_ids)
 
     def cluster_role(self, cluster_names: list = []):
         """
-        This method return list of cluster's role according to cluster name
+        This method returns list of cluster's role according to cluster name
         @param cluster_names:
         @return:
         """
         # tag_role
         result_role_list = []
         # if cluster_key exit
         if self.cluster_name:
@@ -664,15 +665,15 @@
                     else:
                         logger.info(f'Missing role for cluster {cluster_name}')
         logger.info(f'cluster_role count: {len(sorted(result_role_list))} {sorted(result_role_list)}')
         return sorted(result_role_list)
 
     def cluster_user(self, cluster_names: list = []):
         """
-        This method return list of cluster's user according to cluster name
+        This method returns list of cluster's user according to cluster name
         @param cluster_names:
         @return:
         """
         # tag_user
         result_user_list = []
         if self.cluster_name:
             cluster_names.append(self.cluster_name)
@@ -747,15 +748,15 @@
         @param tags:
         @return:
         """
         return [tag for tag in tags if tag.get('Key') != 'LaunchTime']
 
     def cluster_s3_bucket(self, cluster_names: list = []):
         """
-        This method return list of cluster's s3 bucket according to cluster name
+        This method returns list of cluster's s3 bucket according to cluster name
         @param cluster_names:
         @return:
         """
         bucket_result_list = []
         response = self.s3_client.list_buckets()
         # if cluster_key exit
         if self.cluster_name:
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/non_cluster_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,23 +96,23 @@
                 tags.append({'Key': key, 'Value': user})
             elif user and key == 'Email':
                 tags.append({'Key': key, 'Value': f'{user}@redhat.com'})
             else:
                 tags.append({'Key': key, 'Value': value})
         return tags
 
-    def _get_username_from_cloudtrail(self, start_time: datetime, resource_id: str, resource_type: str):
+    def _get_username_from_cloudtrail(self, start_time: datetime, resource_id: str, resource_type: str, end_time: datetime = None):
         """
-        This method return username fom cloudtrail
+        This method returns username fom cloudtrail
         @param start_time:
         @param resource_id:
         @param resource_type:
         @return:
         """
-        return self.cloudtrail.get_username_by_instance_id_and_time(start_time=start_time, resource_id=resource_id, resource_type=resource_type)
+        return self.cloudtrail.get_username_by_instance_id_and_time(start_time=start_time, resource_id=resource_id, resource_type=resource_type, end_time=end_time)
 
     def _get_resource_data(self, resource_method: callable):
         """
         This method returns the resource_data
         @return:
         """
         resource_data = resource_method()
@@ -128,15 +128,15 @@
         @param date_time:
         @return:
         """
         return date_time.strftime('%Y/%m/%d %H:%M:%S')
 
     def _build_tag(self, key: str, value: any):
         """
-        This method return Key value pair
+        This method returns Key value pair
         @param key:
         @param value:
         @return:
         """
         if isinstance(value, datetime):
             value = self._convert_datetime_format(date_time=value)
         return {'Key': key, 'Value': value}
@@ -159,15 +159,15 @@
                                                           resource_type='AWS::EC2::Instance')
             launch_time = instance_item.get('LaunchTime')
             tags.append(self._build_tag(key='LaunchTime', value=launch_time))
         return tags, username
 
     def _get_tags_fom_attachments(self, attachments: list):
         """
-        This method return tags from attachments
+        This method returns tags from attachments
         @param attachments:
         @return:
         """
         tags = []
         username = ''
         if attachments:
             for attachment in attachments:
@@ -203,18 +203,34 @@
         """
         name_tag = self.ec2_operations.get_tag_value_from_tags(tags=tags, tag_name='Name') if tags else resource_name
         for user in self.iam_users:
             if user in name_tag:
                 return user
         return None
 
-    def get_username(self, start_time: datetime, resource_id: str, resource_type: str, tags: list, resource_name: str = ''):
+    def get_username(self, start_time: datetime, resource_id: str, resource_type: str, tags: list, resource_name: str = '', end_time: datetime = None):
         """
         This method returns the username
         :return:
         """
         iam_username = self.get_user_name_from_name_tag(tags=tags, resource_name=resource_name)
         if not iam_username:
             iam_username = self.get_user_name_from_name_tag(resource_name=resource_name)
             if not iam_username:
-                return self._get_username_from_cloudtrail(start_time=start_time, resource_id=resource_id, resource_type=resource_type)
+                return self._get_username_from_cloudtrail(start_time=start_time, resource_id=resource_id, resource_type=resource_type, end_time=end_time)
         return iam_username
+
+    def validate_existing_tag(self, tags: list):
+        """
+        This method validates that permanent tag exists in tags list
+        @param tags:
+        @return:
+        """
+        check_tags = ['User', 'Project', 'Manager', 'Owner', 'Email']
+        tag_count = 0
+        if tags:
+            for tag in tags:
+                if tag.get('Key') in check_tags:
+                    tag_count += 1
+                    if tag.get('Value') == 'NA':
+                        return False
+        return tag_count == len(check_tags)
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/remove_non_cluster_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/run_tag_non_cluster_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/tag_non_cluster_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 
 from cloud_governance.common.logger.init_logger import logger
 from cloud_governance.policy.policy_operations.aws.tag_non_cluster.non_cluster_operations import NonClusterOperations
 
 
 class TagNonClusterResources(NonClusterOperations):
     """
@@ -63,23 +63,25 @@
         if not instances_list:
             instances_list = self._get_resource_data(resource_method=self._get_instances_data)
         instances_ids = []
         for instance in instances_list:
             for item in instance:
                 instance_id = item.get('InstanceId')
                 launch_time = item.get('LaunchTime')
-                add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=item.get('Tags'))
-                if add_tags:
-                    if self.dry_run == 'no':
-                        try:
-                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[instance_id], tags=add_tags)
-                            logger.info(f'Added tags to instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
-                        except Exception as err:
-                            logger.info(err)
-                    instances_ids.append(instance_id)
+                tags = item.get('Tags')
+                if not self.validate_existing_tag(tags=tags):
+                    add_tags = self.__get_instance_tags(launch_time=launch_time, instance_id=instance_id, tags=tags)
+                    if add_tags:
+                        if self.dry_run == 'no':
+                            try:
+                                self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[instance_id], tags=add_tags)
+                                logger.info(f'Added tags to instance: {instance_id} total: {len(add_tags)} tags: {add_tags}')
+                            except Exception as err:
+                                logger.info(err)
+                        instances_ids.append(instance_id)
         logger.info(f'non_cluster_ec2 count: {len(sorted(instances_ids))} {sorted(instances_ids)}')
         return sorted(instances_ids)
 
     def update_volumes(self, volumes_data: list = None):
         """
         This method updates the tags of non-cluster volumes
         @param volumes_data:
@@ -87,45 +89,46 @@
         """
         if not volumes_data:
             volumes_data = self._get_resource_data(resource_method=self.ec2_operations.get_volumes)
         volume_ids = []
         for volume in volumes_data:
             volume_id = volume.get('VolumeId')
             tags = volume.get('Tags')
-            username = self.get_username(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume', tags=tags)
-            search_tags = []
-            if not username:
-                get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
-                search_tags.extend(get_tags)
-            else:
-                search_tags.extend(self._append_input_tags())
-            if username:
-                user_tags = self.iam_client.get_user_tags(username=username)
-                if not user_tags:
-                    search_tags.extend(self._fill_na_tags(user=username))
+            if not self.validate_existing_tag(tags=tags):
+                username = self.get_username(start_time=volume.get('CreateTime'), resource_id=volume_id, resource_type='AWS::EC2::Volume', tags=tags)
+                search_tags = []
+                if not username:
+                    get_tags, username = self._get_tags_fom_attachments(attachments=volume.get('Attachments'))
+                    search_tags.extend(get_tags)
                 else:
-                    search_tags.extend(user_tags)
-                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
-                search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
-            else:
-                search_tags.extend(self._fill_na_tags())
-                search_tags.extend(self._append_input_tags())
-                search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
-            if not self.__check_name_in_tags(volume.get('Tags')):
-                tag_name = f'{username}-{volume_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{volume_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{volume_id[-self.SHORT_RESOURCE_ID:]}'
-                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
-            volume_tags = self._get_tags_of_resources(tags=volume.get('Tags'), search_tags=search_tags)
-            if volume_tags:
-                if self.dry_run == 'no':
-                    try:
-                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[volume_id], tags=volume_tags)
-                        logger.info(f'added tags to volume_id: {volume_id} total: {len(volume_tags)}  tags: {volume_tags}')
-                    except Exception as err:
-                        logger.info(err)
-                volume_ids.append(volume_id)
+                    search_tags.extend(self._append_input_tags())
+                if username:
+                    user_tags = self.iam_client.get_user_tags(username=username)
+                    if not user_tags:
+                        search_tags.extend(self._fill_na_tags(user=username))
+                    else:
+                        search_tags.extend(user_tags)
+                        search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                    search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
+                else:
+                    search_tags.extend(self._fill_na_tags())
+                    search_tags.extend(self._append_input_tags())
+                    search_tags.append(self._build_tag(key='LaunchTime', value=volume.get('CreateTime')))
+                if not self.__check_name_in_tags(volume.get('Tags')):
+                    tag_name = f'{username}-{volume_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{volume_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{volume_id[-self.SHORT_RESOURCE_ID:]}'
+                    search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+                volume_tags = self._get_tags_of_resources(tags=volume.get('Tags'), search_tags=search_tags)
+                if volume_tags:
+                    if self.dry_run == 'no':
+                        try:
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[volume_id], tags=volume_tags)
+                            logger.info(f'added tags to volume_id: {volume_id} total: {len(volume_tags)}  tags: {volume_tags}')
+                        except Exception as err:
+                            logger.info(err)
+                    volume_ids.append(volume_id)
         logger.info(f'non_cluster_volumes count: {len(sorted(volume_ids))} {sorted(volume_ids)}')
         return sorted(volume_ids)
 
     def update_snapshots(self, snapshots: list = None):
         """
         This method updates the tags of  non-cluster snapshots
         @param snapshots:
@@ -133,51 +136,58 @@
         """
         if not snapshots:
             snapshots = self._get_resource_data(resource_method=self.ec2_operations.get_snapshots)
         snapshot_ids = []
         for snapshot in snapshots:
             snapshot_id = snapshot.get('SnapshotId')
             tags = snapshot.get('Tags')
-            username = self.get_username(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags)
-            search_tags = []
-            if not username:
-                if snapshot.get('Description') and 'Created' in snapshot.get('Description'):
-                    image_tags, username = self._get_tags_from_snapshot_description_images(description=snapshot.get('Description'))
-                    if not username:
-                        instance_id = snapshot.get('Description').split(" ")[2].split("(")[1][:-1]
-                        instances = self._get_instances_data(instance_id)
-                        if instances:
-                            for item in instances:
-                                if item.get('InstanceId') == instance_id:
-                                    item_tags, username = self._get_tags_from_instance_item(instance_item=item)
-            else:
-                search_tags.extend(self._append_input_tags())
-            if username:
-                user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
-                if not user_tags:
-                    search_tags.extend(self._fill_na_tags(user=username))
+            if not self.validate_existing_tag(tags=tags):
+                username = self.get_username(start_time=snapshot.get('StartTime'), resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags)
+                if 'vm_import_image' in username:
+                    start_time = snapshot.get('StartTime') + timedelta(seconds=5)
+                    end_time = start_time + timedelta(minutes=30)
+                    assume_username = self.get_username(start_time=start_time, resource_id=snapshot_id, resource_type='AWS::EC2::Snapshot', tags=tags, end_time=end_time)
+                    if assume_username:
+                        username = assume_username
+                search_tags = []
+                if not username:
+                    if snapshot.get('Description') and 'Created' in snapshot.get('Description'):
+                        image_tags, username = self._get_tags_from_snapshot_description_images(description=snapshot.get('Description'))
+                        if not username:
+                            instance_id = snapshot.get('Description').split(" ")[2].split("(")[1][:-1]
+                            instances = self._get_instances_data(instance_id)
+                            if instances:
+                                for item in instances:
+                                    if item.get('InstanceId') == instance_id:
+                                        item_tags, username = self._get_tags_from_instance_item(instance_item=item)
                 else:
-                    search_tags.extend(user_tags)
-            else:
-                search_tags.extend(self._fill_na_tags())
-                search_tags.extend(self._append_input_tags())
-            if not self.__check_name_in_tags(snapshot.get('Tags')):
-                tag_name = f'{username}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{snapshot_id[:self.SHOT_SNAPSHOT_ID]}-{self.region}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}'
-                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
-            search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
-            snapshot_tags = self._get_tags_of_resources(tags=snapshot.get('Tags'), search_tags=search_tags)
-            if snapshot_tags:
-                if self.dry_run == 'no':
-                    try:
-                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[snapshot_id], tags=snapshot_tags)
-                        logger.info(f'added tags to snapshots: {snapshot_id} total: {len(snapshot_tags)} tags: {snapshot_tags}')
-                    except Exception as err:
-                        logger.info(err)
-                snapshot_ids.append(snapshot_id)
+                    search_tags.extend(self._append_input_tags())
+                if username:
+                    user_tags = self.iam_client.get_user_tags(username=username)
+                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                    if not user_tags:
+                        search_tags.extend(self._fill_na_tags(user=username))
+                    else:
+                        search_tags.extend(user_tags)
+                else:
+                    search_tags.extend(self._fill_na_tags())
+                    search_tags.extend(self._append_input_tags())
+                if not self.__check_name_in_tags(snapshot.get('Tags')):
+                    tag_name = f'{username}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{snapshot_id[:self.SHOT_SNAPSHOT_ID]}-{self.region}-{snapshot_id[-self.SHORT_RESOURCE_ID:]}'
+                    search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+                search_tags.append(self._build_tag(key='LaunchTime', value=snapshot.get('StartTime')))
+                snapshot_tags = self._get_tags_of_resources(tags=snapshot.get('Tags'), search_tags=search_tags)
+                if snapshot_tags:
+                    if self.dry_run == 'no':
+                        try:
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[snapshot_id], tags=snapshot_tags)
+                            logger.info(f'added tags to snapshots: {snapshot_id} total: {len(snapshot_tags)} tags: {snapshot_tags}')
+                        except Exception as err:
+                            logger.info(err)
+                    snapshot_ids.append(snapshot_id)
         logger.info(f'non_cluster_snapshot count: {len(sorted(snapshot_ids))} {sorted(snapshot_ids)}')
         return sorted(snapshot_ids)
 
     def update_ami(self, images: list = None):
         """
         This method update the tags of non-cluster Amazon Machine Images
         @param images:
@@ -188,34 +198,35 @@
             _, images = self.ec2_operations.scan_cluster_non_cluster_resources(images)
         image_ids = []
         for image in images:
             image_id = image.get('ImageId')
             tags = image.get('Tags')
             image_name = image.get('Name')
             start_time = datetime.fromisoformat(image.get('CreationDate')[:-1] + '+00:00')
-            username = self.get_username(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami', tags=tags, resource_name=image_name)
-            search_tags = []
-            search_tags.extend(self._append_input_tags())
-            if username:
-                user_tags = self.iam_client.get_user_tags(username=username)
-                search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
-                if not user_tags:
-                    search_tags.extend(self._fill_na_tags(user=username))
+            if not self.validate_existing_tag(tags=tags):
+                username = self.get_username(start_time=start_time, resource_id=image_id, resource_type='AWS::EC2::Ami', tags=tags, resource_name=image_name)
+                search_tags = []
+                search_tags.extend(self._append_input_tags())
+                if username:
+                    user_tags = self.iam_client.get_user_tags(username=username)
+                    search_tags.append({'Key': 'Email', 'Value': f'{username}@redhat.com'})
+                    if not user_tags:
+                        search_tags.extend(self._fill_na_tags(user=username))
+                    else:
+                        search_tags.extend(user_tags)
                 else:
-                    search_tags.extend(user_tags)
-            else:
-                search_tags.extend(self._fill_na_tags())
-            if not self.__check_name_in_tags(image.get('Tags')):
-                tag_name = f'{username}-{image_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{image_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{image_id[-self.SHORT_RESOURCE_ID:]}'
-                search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
-            search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
-            image_tags = self._get_tags_of_resources(tags=image.get('Tags'), search_tags=search_tags)
-            if image_tags:
-                if self.dry_run == 'no':
-                    try:
-                        self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[image_id], tags=image_tags)
-                        logger.info(f'added tags to image: {image_id} total: {len(image_tags)} tags: {image_tags}')
-                    except Exception as err:
-                        logger.info(err)
-                image_ids.append(image_id)
+                    search_tags.extend(self._fill_na_tags())
+                if not self.__check_name_in_tags(image.get('Tags')):
+                    tag_name = f'{username}-{image_id[-self.SHORT_RESOURCE_ID:]}' if username else f'{image_id[:self.SHORT_RESOURCE_NAME]}-{self.region}-{image_id[-self.SHORT_RESOURCE_ID:]}'
+                    search_tags.append({'Key': 'cg-Name', 'Value': tag_name})
+                search_tags.append(self._build_tag(key='LaunchTime', value=start_time))
+                image_tags = self._get_tags_of_resources(tags=image.get('Tags'), search_tags=search_tags)
+                if image_tags:
+                    if self.dry_run == 'no':
+                        try:
+                            self.utils.tag_aws_resources(client_method=self.ec2_client.create_tags, resource_ids=[image_id], tags=image_tags)
+                            logger.info(f'added tags to image: {image_id} total: {len(image_tags)} tags: {image_tags}')
+                        except Exception as err:
+                            logger.info(err)
+                    image_ids.append(image_id)
         logger.info(f'non_cluster_amis count: {len(sorted(image_ids))} {sorted(image_ids)}')
         return sorted(image_ids)
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_non_cluster/update_na_tag_resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         resource_ids = []
         for resource in resources:
             resource_ids.append(resource.get(resource_id))
         return resource_ids
 
     def __get_key_value(self, key, value):
         """
-        This method return key-value pairs
+        This method returns key-value pairs
         :param key:
         :param value:
         :return:
         """
         return {'Key': key, 'Value': value}
 
     def __convert_key_value(self, keys, values):
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/iam_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/remove_user_tags.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/run_tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/tag_user/tag_iam_user.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_ec2_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_iam_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/delete_s3_resources.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/run_zombie_cluster_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
 
 @typeguard.typechecked
 @logger_time_stamp
 def zombie_cluster_resource(delete: bool = False, region: str = 'us-east-2', resource: str = '', cluster_tag: str = '',
                             resource_name: str = '', service_type: str = ''):
     """
-    This method return zombie cluster resources,
+    This method returns zombie cluster resources,
     How its works? if not exist an instance cluster, the resource is zombie
     if delete true it will delete the zombie resource
     :return: list of zombie resources
     """
     zombie_result = {}
     all_cluster_data = []
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/validate_zombies.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_cluster/zombie_cluster_common_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         tags = {}
         if data:
             tags = literal_eval(data)
         return tags
 
     def get_tag_name_from_tags(self, tags: list, tag_name: str):
         """
-        This method return tag_name from resource_tags
+        This method returns tag_name from resource_tags
         @param tags:
         @param tag_name:
         @return:
         """
         if tags:
             for tag in tags:
                 if tag.get('Key') == tag_name:
@@ -72,15 +72,15 @@
                 zombie_cluster_user_tag[zombies[zombie_id]] = self.get_tag_name_from_tags(tags=resource.get(tag),
                                                                                           tag_name='User')
         return zombie_cluster_user_tag
 
     def _get_tags_of_zombie_resources(self, resources: list, resource_id_name: str, zombies: dict, aws_service: str,
                                       aws_tag: str = 'Tags'):
         """
-        This method return tags of the resource i.e {resource_id: tags}
+        This method returns tags of the resource i.e {resource_id: tags}
         @param resources:
         @param tags:
         @return:
         """
         resources_tags = {}
         for resource in resources:
             aws_tags = []
@@ -174,26 +174,25 @@
             if not found:
                 tags.append({'Key': tag_name, 'Value': str(tag_value)})
             return tags
         return [{'Key': tag_name, 'Value': str(tag_value)}]
 
     def get_cluster_delete_days(self, tags: list) -> int:
         """
-        This method return the ClusterDeleteDays tag
+        This method returns the ClusterDeleteDays tag
         @param tags:
         @return:
         """
         cluster_delete_days = self.get_tag_name_from_tags(tags=tags, tag_name='ClusterDeleteDays')
         if not cluster_delete_days:
             cluster_delete_days = 1
         else:
             cluster_delete_days = int(cluster_delete_days) + 1
         return cluster_delete_days
 
-    @logger_time_stamp
     def trigger_mail(self, tags: list, resource_id: str, days: int, resources: list, message_type: str):
         """
         This method send triggering mail
         @param message_type:
         @param resources:
         @param days:
         @param tags:
@@ -251,15 +250,14 @@
             if cluster_tag in cluster_left_out_days:
                 if cluster_tag in notify_tag_data:
                     notify_data.setdefault(cluster_tag, []).append({func_name: notify_tag_data[cluster_tag]})
                 if cluster_tag in delete_tag_data:
                     delete_data.setdefault(cluster_tag, []).append({func_name: delete_tag_data[cluster_tag]})
         return notify_data, delete_data, cluster_data
 
-    @logger_time_stamp
     def send_mails_to_cluster_user(self, notify_data: dict, delete_data: dict, cluster_data: dict):
         """
         This method send mail to the user to notify cluster status
         @param cluster_data:
         @param notify_data:
         @param delete_data:
         @return:
@@ -271,15 +269,14 @@
                                   days=self.DAYS_TO_TRIGGER_RESOURCE_MAIL,
                                   resources=resource_ids, message_type='notification')
             for cluster_tag, resource_ids in delete_data.items():
                 self.update_resource_tags(tags=cluster_data[cluster_tag], tag_name='Name', tag_value=cluster_tag)
                 self.trigger_mail(tags=cluster_data[cluster_tag], resource_id=cluster_tag,
                                   days=self.DAYS_TO_DELETE_RESOURCE, resources=resource_ids, message_type='delete')
 
-    @logger_time_stamp
     def _check_zombie_cluster_deleted_days(self, resources: dict, cluster_left_out_days: dict, zombie: str, cluster_tag: str):
         """
         This method check the cluster delete days and return the clusters
         @param resources:
         @param cluster_left_out_days:
         @return:
         """
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/run_zombie_non_cluster_policies.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                 if tag.get('Key').strip().lower() == tag_name.lower():
                     return tag.get('Value').strip()
             return ''
         return ''
 
     def _calculate_days(self, create_date: datetime):
         """
-        This method return the days
+        This method returns the days
         @return:
         """
         today = datetime.date.today()
         days = today - create_date.date()
         return days.days
 
     def _get_ami_ids(self):
@@ -231,15 +231,15 @@
                 self._s3_client.delete_bucket(Bucket=resource_id)
             elif self._policy == 'empty_roles':
                 self._iam_client.delete_role(RoleName=resource_id)
             elif self._policy == 'ebs_unattached':
                 self._ec2_client.delete_volume(VolumeId=resource_id)
             elif self._policy == 'ip_unattached':
                 self._ec2_client.release_address(AllocationId=resource_id)
-            elif self._policy == 'nat_gateway_unused':
+            elif self._policy == 'unused_nat_gateway':
                 self._ec2_client.delete_nat_gateway(NatGatewayId=resource_id)
             elif self._policy == 'zombie_snapshots':
                 self._ec2_client.delete_snapshot(SnapshotId=resource_id)
             logger.info(f'{self._policy} deleted: {resource_id}')
         except Exception as err:
             logger.info(f'Exception raised: {err}: {resource_id}')
 
@@ -287,15 +287,15 @@
             if self._get_tag_name_from_tags(tags=tags, tag_name='LastUsedDay') or resource_left_out:
                 tags = self._update_tag_value(tags=tags, tag_name='LastUsedDay', tag_value=str(left_out_days))
                 try:
                     if self._policy == 's3_inactive':
                         self._s3_client.put_bucket_tagging(Bucket=resource_id, Tagging={'TagSet': tags})
                     elif self._policy == 'empty_roles':
                         self._iam_client.tag_role(RoleName=resource_id, Tags=tags)
-                    elif self._policy in ('ip_unattached', 'nat_gateway_unused', 'zombie_snapshots'):
+                    elif self._policy in ('ip_unattached', 'unused_nat_gateway', 'zombie_snapshots'):
                         self._ec2_client.create_tags(Resources=[resource_id], Tags=tags)
                 except Exception as err:
                     logger.info(f'Exception raised: {err}: {resource_id}')
 
     def _organise_instance_data(self, resources: list):
         """
         This method convert all datetime into string
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/aws/zombie_non_cluster/zombie_non_cluster_polices.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,12 +23,12 @@
                 response = cls[1]().run()
                 if isinstance(response, str):
                     logger.info(f'key: {cls[0]}, Response: {response}')
                 else:
                     logger.info(f'key: {cls[0]}, count: {len(response)}, {response}')
                     policy_result = response
                     if self._policy_output:
-                        if self._policy not in ('ec2_idle', 'ebs_in_use', 'ec2_run'):
-                            beautify_data = self._beautify_upload_data(upload_resource_data=response)
-                            policy_result = {'count': len(beautify_data), self._policy: beautify_data}
+                        # if self._policy not in ('ec2_idle', 'ebs_in_use', 'ec2_run', 's3_inactive', 'zombie_snapshots', 'nat_gateway_unused'):
+                        #     beautify_data = self._beautify_upload_data(upload_resource_data=response)
+                        #     policy_result = {'count': len(beautify_data), self._policy: beautify_data}
                         logger.info(policy_result)
                         self._s3operations.save_results_to_s3(policy=self._policy.replace('_', '-'), policy_output=self._policy_output, policy_result=policy_result)
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/azure/azure_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gcp/gcp_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/gitleaks/gitleaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     #     """
     #     resource_file = self.__resources_file_full_path
     #     if os.path.isfile(resource_file):
     #         os.remove(resource_file)
 
     def __get_gitleaks_report(self):
         """
-        This method return dict report content
+        This method returns dict report content
         """
         report_file = self.__report_file_full_path
         if os.path.isfile(report_file):
             json_file = open(report_file)
             json_str = json_file.read()
             json_data = json.loads(json_str)
             return json_data
```

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/ibm_operations/ibm_policy_runner.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py` & `athiruma-cloud-governance-1.2.108/cloud_governance/policy/policy_operations/ibm/tagging/tagging_operations.py`

 * *Files identical despite different names*

### Comparing `athiruma-cloud-governance-1.1.94/setup.py` & `athiruma-cloud-governance-1.2.108/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 from os import path
 from setuptools import setup, find_packages
 
 
-__version__ = '1.1.94'
+__version__ = '1.2.108'
 
 
 here = path.abspath(path.dirname(__file__))
 
 
 if path.isfile(path.join(here, 'README.md')):
     with open(path.join(here, 'README.md'), encoding='utf-8') as f:
```

