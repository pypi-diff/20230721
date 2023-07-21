# Comparing `tmp/lusid-scheduler-sdk-preview-0.0.801.tar.gz` & `tmp/lusid-scheduler-sdk-preview-0.0.804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-scheduler-sdk-preview-0.0.801.tar", last modified: Wed Jul 12 14:15:58 2023, max compression
+gzip compressed data, was "dist/lusid-scheduler-sdk-preview-0.0.804.tar", last modified: Fri Jul 21 09:11:01 2023, max compression
```

## Comparing `lusid-scheduler-sdk-preview-0.0.801.tar` & `lusid-scheduler-sdk-preview-0.0.804.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8886 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/
--rw-r--r--   0 root         (0) root         (0)     4369 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/
--rw-r--r--   0 root         (0) root         (0)      328 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    52333 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/images_api.py
--rw-r--r--   0 root         (0) root         (0)    74271 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    55693 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/schedules_api.py
--rw-r--r--   0 root         (0) root         (0)    27412 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16623 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5095 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/
--rw-r--r--   0 root         (0) root         (0)     3216 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7220 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     8983 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7224 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    11992 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/argument_definition.py
--rw-r--r--   0 root         (0) root         (0)    24696 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/create_job_request.py
--rw-r--r--   0 root         (0) root         (0)    18889 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/create_schedule_request.py
--rw-r--r--   0 root         (0) root         (0)     8005 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9494 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     8718 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/image.py
--rw-r--r--   0 root         (0) root         (0)    10613 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/image_summary.py
--rw-r--r--   0 root         (0) root         (0)    18900 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/job_definition.py
--rw-r--r--   0 root         (0) root         (0)    18845 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/job_history.py
--rw-r--r--   0 root         (0) root         (0)    20106 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/job_run_result.py
--rw-r--r--   0 root         (0) root         (0)     6418 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/link.py
--rw-r--r--   0 root         (0) root         (0)     9532 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10697 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     5844 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/notification.py
--rw-r--r--   0 root         (0) root         (0)    10271 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/repository.py
--rw-r--r--   0 root         (0) root         (0)     6408 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/required_resources.py
--rw-r--r--   0 root         (0) root         (0)     6592 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7743 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_image_summary.py
--rw-r--r--   0 root         (0) root         (0)     7435 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_job_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_job_history.py
--rw-r--r--   0 root         (0) root         (0)     7351 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_repository.py
--rw-r--r--   0 root         (0) root         (0)     7575 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     9669 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/scan_report.py
--rw-r--r--   0 root         (0) root         (0)     9993 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/scan_summary.py
--rw-r--r--   0 root         (0) root         (0)    13684 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     6751 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/start_job_request.py
--rw-r--r--   0 root         (0) root         (0)     6547 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/start_job_response.py
--rw-r--r--   0 root         (0) root         (0)     7564 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/start_schedule_response.py
--rw-r--r--   0 root         (0) root         (0)     7315 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     6024 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/time_trigger.py
--rw-r--r--   0 root         (0) root         (0)     4068 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/trigger.py
--rw-r--r--   0 root         (0) root         (0)    22675 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/update_job_request.py
--rw-r--r--   0 root         (0) root         (0)    17929 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/update_schedule_request.py
--rw-r--r--   0 root         (0) root         (0)    14153 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/upload_image_instructions.py
--rw-r--r--   0 root         (0) root         (0)     5321 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/upload_image_request.py
--rw-r--r--   0 root         (0) root         (0)     9287 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/vulnerability.py
--rw-r--r--   0 root         (0) root         (0)    13553 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/utilities/
--rw-r--r--   0 root         (0) root         (0)       62 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      367 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2624 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-12 14:15:58.000000 lusid-scheduler-sdk-preview-0.0.801/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2275 2023-07-12 14:15:37.000000 lusid-scheduler-sdk-preview-0.0.801/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8886 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/
+-rw-r--r--   0 root         (0) root         (0)     4369 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    52333 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/images_api.py
+-rw-r--r--   0 root         (0) root         (0)    74271 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    55693 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/schedules_api.py
+-rw-r--r--   0 root         (0) root         (0)    27412 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16623 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5095 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7220 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     8983 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7224 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    11992 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/argument_definition.py
+-rw-r--r--   0 root         (0) root         (0)    24696 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/create_job_request.py
+-rw-r--r--   0 root         (0) root         (0)    18889 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/create_schedule_request.py
+-rw-r--r--   0 root         (0) root         (0)     8005 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9494 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/image.py
+-rw-r--r--   0 root         (0) root         (0)    10613 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/image_summary.py
+-rw-r--r--   0 root         (0) root         (0)    18900 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    18845 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/job_history.py
+-rw-r--r--   0 root         (0) root         (0)    20106 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/job_run_result.py
+-rw-r--r--   0 root         (0) root         (0)     6418 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     9532 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10697 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     5844 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/notification.py
+-rw-r--r--   0 root         (0) root         (0)    10271 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/repository.py
+-rw-r--r--   0 root         (0) root         (0)     6408 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/required_resources.py
+-rw-r--r--   0 root         (0) root         (0)     6592 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7743 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_image_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7435 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_job_history.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_repository.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9669 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/scan_report.py
+-rw-r--r--   0 root         (0) root         (0)     9993 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/scan_summary.py
+-rw-r--r--   0 root         (0) root         (0)    13684 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/start_job_request.py
+-rw-r--r--   0 root         (0) root         (0)     6547 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/start_job_response.py
+-rw-r--r--   0 root         (0) root         (0)     7564 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/start_schedule_response.py
+-rw-r--r--   0 root         (0) root         (0)     7315 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/time_trigger.py
+-rw-r--r--   0 root         (0) root         (0)     4068 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/trigger.py
+-rw-r--r--   0 root         (0) root         (0)    22675 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/update_job_request.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/update_schedule_request.py
+-rw-r--r--   0 root         (0) root         (0)    14153 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/upload_image_instructions.py
+-rw-r--r--   0 root         (0) root         (0)     5321 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/upload_image_request.py
+-rw-r--r--   0 root         (0) root         (0)     9287 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/vulnerability.py
+-rw-r--r--   0 root         (0) root         (0)    13553 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/utilities/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      367 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 09:11:01.000000 lusid-scheduler-sdk-preview-0.0.804/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-07-21 09:09:59.000000 lusid-scheduler-sdk-preview-0.0.804/setup.py
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/README.md` & `lusid-scheduler-sdk-preview-0.0.804/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-scheduler-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.801
-- Package version: 0.0.801
+- API version: 0.0.804
+- Package version: 0.0.804
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/__init__.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.0.801"
+__version__ = "0.0.804"
 
 # import apis into sdk package
 from lusid_scheduler.api.application_metadata_api import ApplicationMetadataApi
 from lusid_scheduler.api.images_api import ImagesApi
 from lusid_scheduler.api.jobs_api import JobsApi
 from lusid_scheduler.api.schedules_api import SchedulesApi
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/application_metadata_api.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/application_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/images_api.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/images_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -163,15 +163,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "str",
             400: "LusidValidationProblemDetails",
@@ -306,15 +306,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "file",
             400: "LusidValidationProblemDetails",
@@ -456,15 +456,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Image",
             400: "LusidValidationProblemDetails",
@@ -656,15 +656,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfImageSummary",
             400: "LusidValidationProblemDetails",
@@ -845,15 +845,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfRepository",
             400: "LusidValidationProblemDetails",
@@ -992,15 +992,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "UploadImageInstructions",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/jobs_api.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -162,15 +162,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "JobDefinition",
             400: "LusidValidationProblemDetails",
@@ -315,15 +315,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -502,15 +502,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfJobHistory",
             400: "LusidValidationProblemDetails",
@@ -652,15 +652,15 @@
             ['text/plain', 'application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "str",
             400: "LusidValidationProblemDetails",
@@ -802,15 +802,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "JobRunResult",
             400: "LusidValidationProblemDetails",
@@ -955,15 +955,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -1144,15 +1144,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfJobDefinition",
             400: "LusidValidationProblemDetails",
@@ -1311,15 +1311,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             202: "StartJobResponse",
             400: "LusidValidationProblemDetails",
@@ -1478,15 +1478,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "JobDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api/schedules_api.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api/schedules_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -158,15 +158,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -311,15 +311,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {}
 
         return self.api_client.call_api(
@@ -472,15 +472,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -625,15 +625,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -814,15 +814,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfScheduleDefinition",
             400: "LusidValidationProblemDetails",
@@ -967,15 +967,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             202: "StartScheduleResponse",
             400: "LusidValidationProblemDetails",
@@ -1134,15 +1134,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.0.801'
+        header_params['X-LUSID-SDK-Version'] = '0.0.804'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ScheduleDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/api_client.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.0.801/python'
+        self.user_agent = 'OpenAPI-Generator/0.0.804/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/configuration.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.801\n"\
-               "SDK Package Version: 0.0.801".\
+               "Version of the API: 0.0.804\n"\
+               "SDK Package Version: 0.0.804".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/exceptions.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/__init__.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/access_controlled_action.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/access_controlled_resource.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/access_controlled_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/action_id.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/argument_definition.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/argument_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/create_job_request.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/create_job_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/create_schedule_request.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/create_schedule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/id_selector_definition.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/id_selector_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/identifier_part_schema.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/image.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/image_summary.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/image_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/job_definition.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/job_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/job_history.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/job_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/job_run_result.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/job_run_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/link.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/lusid_problem_details.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/lusid_validation_problem_details.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/notification.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/repository.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/required_resources.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/required_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_id.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_access_controlled_resource.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_image_summary.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_image_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_job_definition.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_job_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_job_history.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_job_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_repository.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/resource_list_of_schedule_definition.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/resource_list_of_schedule_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/scan_report.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/scan_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/scan_summary.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/scan_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/schedule_definition.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/schedule_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/start_job_request.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/start_job_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/start_job_response.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/start_job_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/start_schedule_response.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/start_schedule_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/tag.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/time_trigger.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/time_trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/trigger.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/update_job_request.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/update_job_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/update_schedule_request.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/update_schedule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/upload_image_instructions.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/upload_image_instructions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/upload_image_request.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/upload_image_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/models/vulnerability.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/models/vulnerability.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/rest.py` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Scheduler API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.0.801
+    The version of the OpenAPI document: 0.0.804
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler/utilities/config_keys.json` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-scheduler-sdk-preview-0.0.801/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt` & `lusid-scheduler-sdk-preview-0.0.804/lusid_scheduler_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-scheduler-sdk-preview-0.0.801/setup.py` & `lusid-scheduler-sdk-preview-0.0.804/setup.py`

 * *Files identical despite different names*

