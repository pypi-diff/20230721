# Comparing `tmp/pycti-5.9.5.tar.gz` & `tmp/pycti-5.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.9.5.tar", last modified: Fri Jul 21 00:02:40 2023, max compression
+gzip compressed data, was "pycti-5.9.6.tar", last modified: Fri Jul 21 09:15:44 2023, max compression
```

## Comparing `pycti-5.9.5.tar` & `pycti-5.9.6.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.567153 pycti-5.9.5/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-21 00:02:25.000000 pycti-5.9.5/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-21 00:02:40.567153 pycti-5.9.5/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-21 00:02:25.000000 pycti-5.9.5/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.555153 pycti-5.9.5/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.559153 pycti-5.9.5/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.559153 pycti-5.9.5/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.563153 pycti-5.9.5/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18920 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14380 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26464 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24764 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24745 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15528 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15569 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15159 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25500 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23092 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15146 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23103 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16472 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16308 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17571 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22793 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23119 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21424 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23961 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24599 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18630 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18892 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14713 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18186 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.567153 pycti-5.9.5/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7763 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106275 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.555153 pycti-5.9.5/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-21 00:02:25.000000 pycti-5.9.5/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-21 00:02:40.567153 pycti-5.9.5/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.106283 pycti-5.9.6/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-21 09:15:31.000000 pycti-5.9.6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-21 09:15:44.106283 pycti-5.9.6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-21 09:15:31.000000 pycti-5.9.6/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.094283 pycti-5.9.6/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.098283 pycti-5.9.6/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.098283 pycti-5.9.6/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.102283 pycti-5.9.6/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18920 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14380 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26464 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24764 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24745 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15528 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15569 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15159 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25500 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23092 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15146 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23103 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16472 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16308 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17571 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22793 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23119 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21424 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23961 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24599 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10192 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18630 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18892 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14713 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18186 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.106283 pycti-5.9.6/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7763 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106275 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-21 09:15:31.000000 pycti-5.9.6/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 09:15:44.098283 pycti-5.9.6/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-21 09:15:44.000000 pycti-5.9.6/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-21 09:15:44.000000 pycti-5.9.6/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 09:15:44.000000 pycti-5.9.6/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-21 09:15:44.000000 pycti-5.9.6/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-21 09:15:44.000000 pycti-5.9.6/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-21 09:15:31.000000 pycti-5.9.6/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-21 09:15:44.106283 pycti-5.9.6/setup.cfg
```

### Comparing `pycti-5.9.5/LICENSE` & `pycti-5.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/PKG-INFO` & `pycti-5.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.5
+Version: 5.9.6
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.9.5 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.6 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.5/README.md` & `pycti-5.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/__init__.py` & `pycti-5.9.6/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.9.5"
+__version__ = "5.9.6"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.9.5/pycti/api/opencti_api_client.py` & `pycti-5.9.6/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/api/opencti_api_connector.py` & `pycti-5.9.6/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/api/opencti_api_work.py` & `pycti-5.9.6/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/connector/opencti_connector.py` & `pycti-5.9.6/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/connector/opencti_connector_helper.py` & `pycti-5.9.6/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_attack_pattern.py` & `pycti-5.9.6/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_campaign.py` & `pycti-5.9.6/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_case_incident.py` & `pycti-5.9.6/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_case_rfi.py` & `pycti-5.9.6/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_case_rft.py` & `pycti-5.9.6/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_channel.py` & `pycti-5.9.6/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_course_of_action.py` & `pycti-5.9.6/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_data_component.py` & `pycti-5.9.6/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_data_source.py` & `pycti-5.9.6/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_event.py` & `pycti-5.9.6/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_external_reference.py` & `pycti-5.9.6/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_feedback.py` & `pycti-5.9.6/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_grouping.py` & `pycti-5.9.6/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_identity.py` & `pycti-5.9.6/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_incident.py` & `pycti-5.9.6/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_indicator.py` & `pycti-5.9.6/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_infrastructure.py` & `pycti-5.9.6/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_intrusion_set.py` & `pycti-5.9.6/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.9.6/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_label.py` & `pycti-5.9.6/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_language.py` & `pycti-5.9.6/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_location.py` & `pycti-5.9.6/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_malware.py` & `pycti-5.9.6/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_malware_analysis.py` & `pycti-5.9.6/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_marking_definition.py` & `pycti-5.9.6/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_narrative.py` & `pycti-5.9.6/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_note.py` & `pycti-5.9.6/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_observed_data.py` & `pycti-5.9.6/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_opinion.py` & `pycti-5.9.6/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_report.py` & `pycti-5.9.6/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix.py` & `pycti-5.9.6/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_core_object.py` & `pycti-5.9.6/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.9.6/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.9.6/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.9.6/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.9.6/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.9.6/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.9.6/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_task.py` & `pycti-5.9.6/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_threat_actor.py` & `pycti-5.9.6/pycti/entities/opencti_threat_actor.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,16 +283,19 @@
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         if "x_opencti_type" in stix_object:
             type = stix_object["x_opencti_type"].lower()
         elif self.opencti.get_attribute_in_extension("type", stix_object) is not None:
             type = self.opencti.get_attribute_in_extension("type", stix_object).lower()
-        elif "individual" in stix_object["resource_level"].lower():
+        elif (
+            "resource_level" in stix_object
+            and stix_object["resource_level"].lower() == "individual"
+        ):
             type = "threat-actor-individual"
         else:
             type = "threat-actor-group"
 
-        if "threat-actor-group" in type:
-            return self.threat_actor_group.import_from_stix2(**kwargs)
-        if "threat-actor-individual" in type:
+        if type == "threat-actor-individual":
             return self.threat_actor_individual.import_from_stix2(**kwargs)
+        else:
+            return self.threat_actor_group.import_from_stix2(**kwargs)
```

### Comparing `pycti-5.9.5/pycti/entities/opencti_threat_actor_group.py` & `pycti-5.9.6/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_threat_actor_individual.py` & `pycti-5.9.6/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_tool.py` & `pycti-5.9.6/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_vocabulary.py` & `pycti-5.9.6/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/entities/opencti_vulnerability.py` & `pycti-5.9.6/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/utils/constants.py` & `pycti-5.9.6/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/utils/opencti_stix2.py` & `pycti-5.9.6/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.9.6/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/utils/opencti_stix2_update.py` & `pycti-5.9.6/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti/utils/opencti_stix2_utils.py` & `pycti-5.9.6/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti.egg-info/PKG-INFO` & `pycti-5.9.6/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.5
+Version: 5.9.6
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.9.5 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.6 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.5/pycti.egg-info/SOURCES.txt` & `pycti-5.9.6/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pycti.egg-info/requires.txt` & `pycti-5.9.6/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/pyproject.toml` & `pycti-5.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.9.5/setup.cfg` & `pycti-5.9.6/setup.cfg`

 * *Files identical despite different names*

