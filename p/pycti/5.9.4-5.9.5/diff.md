# Comparing `tmp/pycti-5.9.4.tar.gz` & `tmp/pycti-5.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.9.4.tar", last modified: Wed Jul 19 02:58:30 2023, max compression
+gzip compressed data, was "pycti-5.9.5.tar", last modified: Fri Jul 21 00:02:40 2023, max compression
```

## Comparing `pycti-5.9.4.tar` & `pycti-5.9.5.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.072955 pycti-5.9.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-19 02:58:17.000000 pycti-5.9.4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-19 02:58:30.072955 pycti-5.9.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-19 02:58:17.000000 pycti-5.9.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.060955 pycti-5.9.4/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.064955 pycti-5.9.4/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.064955 pycti-5.9.4/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.072955 pycti-5.9.4/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14340 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25926 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24724 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24705 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15508 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15549 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15139 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23072 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15126 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23083 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15950 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22773 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23099 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21404 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23941 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18610 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18872 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.072955 pycti-5.9.4/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6827 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106275 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-19 02:58:17.000000 pycti-5.9.4/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-19 02:58:30.064955 pycti-5.9.4/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-19 02:58:30.000000 pycti-5.9.4/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-19 02:58:17.000000 pycti-5.9.4/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-19 02:58:30.076955 pycti-5.9.4/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.567153 pycti-5.9.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-07-21 00:02:25.000000 pycti-5.9.5/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-21 00:02:40.567153 pycti-5.9.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-07-21 00:02:25.000000 pycti-5.9.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.555153 pycti-5.9.5/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4457 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.559153 pycti-5.9.5/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28771 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.559153 pycti-5.9.5/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45760 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.563153 pycti-5.9.5/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18920 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14380 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26464 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24764 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24745 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15528 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15569 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15159 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11897 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25500 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23092 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18533 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15146 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23103 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16472 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16308 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17571 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22793 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23119 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21424 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23961 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24599 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10147 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18630 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18892 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14713 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18186 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.567153 pycti-5.9.5/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7763 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106275 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-07-21 00:02:25.000000 pycti-5.9.5/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-21 00:02:40.555153 pycti-5.9.5/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2419 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-07-21 00:02:40.000000 pycti-5.9.5/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-07-21 00:02:25.000000 pycti-5.9.5/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-07-21 00:02:40.567153 pycti-5.9.5/setup.cfg
```

### Comparing `pycti-5.9.4/LICENSE` & `pycti-5.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/PKG-INFO` & `pycti-5.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.4
+Version: 5.9.5
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
-Metadata-Version: 2.1 Name: pycti Version: 5.9.4 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.5 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.4/README.md` & `pycti-5.9.5/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/__init__.py` & `pycti-5.9.5/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.9.4"
+__version__ = "5.9.5"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.9.4/pycti/api/opencti_api_client.py` & `pycti-5.9.5/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/api/opencti_api_connector.py` & `pycti-5.9.5/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/api/opencti_api_work.py` & `pycti-5.9.5/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/connector/opencti_connector.py` & `pycti-5.9.5/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/connector/opencti_connector_helper.py` & `pycti-5.9.5/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_attack_pattern.py` & `pycti-5.9.5/pycti/entities/opencti_attack_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,18 +423,18 @@
                 ] = self.opencti.get_attribute_in_mitre_extension(
                     "detection", stix_object
                 )
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-            if "granted_refs" not in stix_object:
-                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
-                    "granted_refs", stix_object
-                )
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -474,16 +474,16 @@
                 x_mitre_id=x_mitre_id,
                 killChainPhases=extras["kill_chain_phases_ids"]
                 if "kill_chain_phases_ids" in extras
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_attack_pattern] Missing parameters: stixObject")
 
     def delete(self, **kwargs):
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_campaign.py` & `pycti-5.9.5/pycti/entities/opencti_campaign.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,18 +346,18 @@
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-            if "granted_refs" not in stix_object:
-                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
-                    "granted_refs", stix_object
-                )
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -391,14 +391,14 @@
                 else None,
                 last_seen=stix_object["last_seen"]
                 if "last_seen" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_campaign] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_case_incident.py` & `pycti-5.9.5/pycti/entities/opencti_case_incident.py`

 * *Files 2% similar despite different names*

```diff
@@ -464,14 +464,15 @@
         created = kwargs.get("created", None)
         modified = kwargs.get("modified", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
         severity = kwargs.get("severity", None)
         priority = kwargs.get("priority", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
+        object_assignee = kwargs.get("objectAssignee", None)
         granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
         response_types = kwargs.get("response_types", None)
         x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
 
         if name is not None:
             self.opencti.log("info", "Creating Case Incident {" + name + "}.")
@@ -490,14 +491,15 @@
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
                         "objectLabel": object_label,
                         "objectOrganization": granted_refs,
+                        "objectAssignee": object_assignee,
                         "objects": objects,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
@@ -630,24 +632,28 @@
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-            if "granted_refs" not in stix_object:
-                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
-                    "granted_refs", stix_object
-                )
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
             if "x_opencti_workflow_id" not in stix_object:
                 stix_object[
                     "x_opencti_workflow_id"
                 ] = self.opencti.get_attribute_in_extension(
                     "x_opencti_workflow_id", stix_object
                 )
+            if "x_opencti_assignee_ids" not in stix_object:
+                stix_object[
+                    "x_opencti_assignee_ids"
+                ] = self.opencti.get_attribute_in_extension("assignee_ids", stix_object)
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -677,16 +683,19 @@
                 priority=stix_object["priority"] if "priority" in stix_object else None,
                 response_types=stix_object["response_types"]
                 if "response_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
+                else None,
+                objectAssignee=stix_object["x_opencti_assignee_ids"]
+                if "x_opencti_assignee_ids" in stix_object
                 else None,
                 x_opencti_workflow_id=stix_object["x_opencti_workflow_id"]
                 if "x_opencti_workflow_id" in stix_object
                 else None,
                 update=update,
             )
         else:
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_case_rfi.py` & `pycti-5.9.5/pycti/entities/opencti_case_rfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,18 +622,18 @@
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-            if "granted_refs" not in stix_object:
-                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
-                    "granted_refs", stix_object
-                )
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -658,16 +658,16 @@
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
                 information_types=stix_object["information_types"]
                 if "information_types" in stix_object
                 else None,
             )
         else:
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_case_rft.py` & `pycti-5.9.5/pycti/entities/opencti_case_rft.py`

 * *Files 1% similar despite different names*

```diff
@@ -618,18 +618,18 @@
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-            if "granted_refs" not in stix_object:
-                stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
-                    "granted_refs", stix_object
-                )
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -657,16 +657,16 @@
                 else None,
                 takedown_types=stix_object["takedown_types"]
                 if "takedown_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_caseRft] Missing parameters: stixObject"
             )
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_channel.py` & `pycti-5.9.5/pycti/entities/opencti_channel.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,14 +379,14 @@
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 channel_types=stix_object["channel_types"]
                 if "channel_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_channel] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_course_of_action.py` & `pycti-5.9.5/pycti/entities/opencti_course_of_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,14 @@
                 if "description" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
                 x_mitre_id=x_mitre_id,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_course_of_action] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_data_component.py` & `pycti-5.9.5/pycti/entities/opencti_data_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -417,16 +417,16 @@
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 dataSource=stix_object["dataSource"]
                 if "dataSource" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_data_source] Missing parameters: stixObject"
             )
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_data_source.py` & `pycti-5.9.5/pycti/entities/opencti_data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,16 +409,16 @@
                 else None,
                 collection_layers=stix_object["collection_layers"]
                 if "collection_layers" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_data_source] Missing parameters: stixObject"
             )
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_event.py` & `pycti-5.9.5/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_external_reference.py` & `pycti-5.9.5/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_feedback.py` & `pycti-5.9.5/pycti/entities/opencti_feedback.py`

 * *Files 0% similar despite different names*

```diff
@@ -681,16 +681,16 @@
                 )
                 if "description" in stix_object
                 else None,
                 rating=stix_object["rating"] if "rating" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             self.opencti.log(
                 "error", "[opencti_feedback] Missing parameters: stixObject"
             )
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_grouping.py` & `pycti-5.9.5/pycti/entities/opencti_grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -623,15 +623,15 @@
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 x_opencti_aliases=self.opencti.stix2.pick_aliases(stix_object),
                 update=update,
             )
         else:
             LOGGER.error("[opencti_grouping] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_identity.py` & `pycti-5.9.5/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_incident.py` & `pycti-5.9.5/pycti/entities/opencti_incident.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,14 +408,14 @@
                 if "incident_type" in stix_object
                 else None,
                 severity=stix_object["severity"] if "severity" in stix_object else None,
                 source=stix_object["source"] if "source" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_incident] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_indicator.py` & `pycti-5.9.5/pycti/entities/opencti_indicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,14 +592,14 @@
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 x_opencti_create_observables=stix_object["x_opencti_create_observables"]
                 if "x_opencti_create_observables" in stix_object
                 else False,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_indicator] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_infrastructure.py` & `pycti-5.9.5/pycti/entities/opencti_infrastructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,15 @@
         description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         infrastructure_types = kwargs.get("infrastructure_types", None)
         first_seen = kwargs.get("first_seen", None)
         last_seen = kwargs.get("last_seen", None)
         kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
+        granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             LOGGER.info("Creating Infrastructure {%s}.", name)
             query = """
                 mutation InfrastructureAdd($input: InfrastructureAddInput!) {
                     infrastructureAdd(input: $input) {
@@ -339,14 +340,15 @@
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
                         "objectLabel": object_label,
+                        "objectOrganization": granted_refs,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
@@ -377,22 +379,24 @@
         :return Infrastructure object
     """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
-
-        # Search in extensions
-        if "x_opencti_stix_ids" not in stix_object:
-            stix_object["x_opencti_stix_ids"] = self.opencti.get_attribute_in_extension(
-                "stix_ids", stix_object
-            )
-
         if stix_object is not None:
+            # Search in extensions
+            if "x_opencti_stix_ids" not in stix_object:
+                stix_object[
+                    "x_opencti_stix_ids"
+                ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
@@ -428,11 +432,14 @@
                 else None,
                 killChainPhases=extras["kill_chain_phases_ids"]
                 if "kill_chain_phases_ids" in extras
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
+                else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_infrastructure] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_intrusion_set.py` & `pycti-5.9.5/pycti/entities/opencti_intrusion_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,14 +389,14 @@
                 else None,
                 secondary_motivations=stix_object["secondary_motivations"]
                 if "secondary_motivations" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_intrusion_set] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.9.5/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_label.py` & `pycti-5.9.5/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_language.py` & `pycti-5.9.5/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_location.py` & `pycti-5.9.5/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_malware.py` & `pycti-5.9.5/pycti/entities/opencti_malware.py`

 * *Files 0% similar despite different names*

```diff
@@ -435,14 +435,14 @@
                 else None,
                 killChainPhases=extras["kill_chain_phases_ids"]
                 if "kill_chain_phases_ids" in extras
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_malware] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_malware_analysis.py` & `pycti-5.9.5/pycti/entities/opencti_malware_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,14 +447,14 @@
                 sample=stix_object["sample_ref"]
                 if "sample_ref" in stix_object
                 else None,
                 modules=stix_object["modules"] if "modules" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_malware_analysis] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_marking_definition.py` & `pycti-5.9.5/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_narrative.py` & `pycti-5.9.5/pycti/entities/opencti_narrative.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,14 @@
                 aliases=self.opencti.stix2.pick_aliases(stix_object),
                 narrative_types=stix_object["narrative_types"]
                 if "narrative_types" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_narrative] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_note.py` & `pycti-5.9.5/pycti/entities/opencti_note.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,14 @@
                 authors=stix_object["authors"] if "authors" in stix_object else None,
                 note_types=stix_object["note_types"]
                 if "note_types" in stix_object
                 else None,
                 likelihood=stix_object["likelihood"]
                 if "likelihood" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_note] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_observed_data.py` & `pycti-5.9.5/pycti/entities/opencti_observed_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,16 +623,16 @@
                 else None,
                 number_observed=stix_object["number_observed"]
                 if "number_observed" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
 
             return observed_data_result
         else:
             LOGGER.error("[opencti_observed_data] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_opinion.py` & `pycti-5.9.5/pycti/entities/opencti_opinion.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,14 +586,14 @@
                 if "explanation" in stix_object
                 else None,
                 authors=stix_object["authors"] if "authors" in stix_object else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
                 opinion=stix_object["opinion"] if "opinion" in stix_object else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_opinion] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_report.py` & `pycti-5.9.5/pycti/entities/opencti_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,14 +654,14 @@
                 else None,
                 published=stix_object["published"]
                 if "published" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_report] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix.py` & `pycti-5.9.5/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_core_object.py` & `pycti-5.9.5/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.9.5/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.9.5/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.9.5/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.9.5/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.9.5/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.9.5/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_task.py` & `pycti-5.9.5/pycti/entities/opencti_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -450,15 +450,17 @@
         created = kwargs.get("created", None)
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
         due_date = kwargs.get("due_date", None)
         created_by = kwargs.get("createdBy", None)
         object_marking = kwargs.get("objectMarking", None)
         object_label = kwargs.get("objectLabel", None)
+        object_assignee = kwargs.get("objectAssignee", None)
         granted_refs = kwargs.get("objectOrganization", None)
+        x_opencti_workflow_id = kwargs.get("x_opencti_workflow_id", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             self.opencti.log("info", "Creating Task {" + name + "}.")
             query = """
                 mutation TaskAdd($input: TaskAddInput!) {
                     taskAdd(input: $input) {
@@ -478,14 +480,16 @@
                         "description": description,
                         "due_date": due_date,
                         "objects": objects,
                         "createdBy": created_by,
                         "objectLabel": object_label,
                         "objectMarking": object_marking,
                         "objectOrganization": granted_refs,
+                        "objectAssignee": object_assignee,
+                        "x_opencti_workflow_id": x_opencti_workflow_id,
                         "update": update,
                     }
                 },
             )
             return self.opencti.process_multiple_fields(result["data"]["taskAdd"])
         else:
             self.opencti.log(
@@ -626,14 +630,24 @@
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
             if "granted_refs" not in stix_object:
                 stix_object["granted_refs"] = self.opencti.get_attribute_in_extension(
                     "granted_refs", stix_object
                 )
+            if "x_opencti_workflow_id" not in stix_object:
+                stix_object[
+                    "x_opencti_workflow_id"
+                ] = self.opencti.get_attribute_in_extension(
+                    "x_opencti_workflow_id", stix_object
+                )
+            if "x_opencti_assignee_ids" not in stix_object:
+                stix_object[
+                    "x_opencti_assignee_ids"
+                ] = self.opencti.get_attribute_in_extension("assignee_ids", stix_object)
 
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
@@ -647,16 +661,22 @@
                 name=stix_object["name"],
                 description=self.opencti.stix2.convert_markdown(
                     stix_object["description"]
                 )
                 if "description" in stix_object
                 else None,
                 due_date=stix_object["due_date"] if "due_date" in stix_object else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
+                else None,
+                objectAssignee=stix_object["x_opencti_assignee_ids"]
+                if "x_opencti_assignee_ids" in stix_object
+                else None,
+                x_opencti_workflow_id=stix_object["x_opencti_workflow_id"]
+                if "x_opencti_workflow_id" in stix_object
                 else None,
                 update=update,
             )
         else:
             self.opencti.log("error", "[opencti_task] Missing parameters: stixObject")
 
     def delete(self, **kwargs):
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_threat_actor.py` & `pycti-5.9.5/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_threat_actor_group.py` & `pycti-5.9.5/pycti/entities/opencti_threat_actor_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,14 @@
                 else None,
                 personal_motivations=stix_object["personal_motivations"]
                 if "personal_motivations" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_threat_actor_group] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_threat_actor_individual.py` & `pycti-5.9.5/pycti/entities/opencti_threat_actor_individual.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,16 +461,16 @@
                 else None,
                 personal_motivations=stix_object["personal_motivations"]
                 if "personal_motivations" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
-                objectOrganization=stix_object["granted_refs"]
-                if "granted_refs" in stix_object
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
                 else None,
                 update=update,
             )
         else:
             LOGGER.error(
                 "[opencti_threat_actor_individual] Missing parameters: stixObject"
             )
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_tool.py` & `pycti-5.9.5/pycti/entities/opencti_tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -297,14 +297,15 @@
         name = kwargs.get("name", None)
         description = kwargs.get("description", None)
         aliases = kwargs.get("aliases", None)
         tool_types = kwargs.get("tool_types", None)
         tool_version = kwargs.get("tool_version", None)
         kill_chain_phases = kwargs.get("killChainPhases", None)
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
+        granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             LOGGER.info("Creating Tool {%s}.", name)
             query = """
                 mutation ToolAdd($input: ToolAddInput!) {
                     toolAdd(input: $input) {
@@ -319,14 +320,15 @@
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
                         "objectLabel": object_label,
+                        "objectOrganization": granted_refs,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
@@ -357,15 +359,18 @@
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
             return self.opencti.tool.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
@@ -398,11 +403,14 @@
                 else None,
                 killChainPhases=extras["kill_chain_phases_ids"]
                 if "kill_chain_phases_ids" in extras
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
+                else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_tool] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/entities/opencti_vocabulary.py` & `pycti-5.9.5/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/entities/opencti_vulnerability.py` & `pycti-5.9.5/pycti/entities/opencti_vulnerability.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,14 +295,15 @@
         x_opencti_availability_impact = kwargs.get(
             "x_opencti_availability_impact", None
         )
         x_opencti_confidentiality_impact = kwargs.get(
             "x_opencti_confidentiality_impact", None
         )
         x_opencti_stix_ids = kwargs.get("x_opencti_stix_ids", None)
+        granted_refs = kwargs.get("objectOrganization", None)
         update = kwargs.get("update", False)
 
         if name is not None:
             LOGGER.info("Creating Vulnerability {%s}.", name)
             query = """
                 mutation VulnerabilityAdd($input: VulnerabilityAddInput!) {
                     vulnerabilityAdd(input: $input) {
@@ -317,14 +318,15 @@
                 query,
                 {
                     "input": {
                         "stix_id": stix_id,
                         "createdBy": created_by,
                         "objectMarking": object_marking,
                         "objectLabel": object_label,
+                        "objectOrganization": granted_refs,
                         "externalReferences": external_references,
                         "revoked": revoked,
                         "confidence": confidence,
                         "lang": lang,
                         "created": created,
                         "modified": modified,
                         "name": name,
@@ -400,15 +402,18 @@
                 ] = self.opencti.get_attribute_in_extension(
                     "confidentiality_impact", stix_object
                 )
             if "x_opencti_stix_ids" not in stix_object:
                 stix_object[
                     "x_opencti_stix_ids"
                 ] = self.opencti.get_attribute_in_extension("stix_ids", stix_object)
-
+            if "x_opencti_granted_refs" not in stix_object:
+                stix_object[
+                    "x_opencti_granted_refs"
+                ] = self.opencti.get_attribute_in_extension("granted_refs", stix_object)
             return self.create(
                 stix_id=stix_object["id"],
                 createdBy=extras["created_by_id"]
                 if "created_by_id" in extras
                 else None,
                 objectMarking=extras["object_marking_ids"]
                 if "object_marking_ids" in extras
@@ -456,11 +461,14 @@
                     "x_opencti_confidentiality_impact"
                 ]
                 if "x_opencti_confidentiality_impact" in stix_object
                 else None,
                 x_opencti_stix_ids=stix_object["x_opencti_stix_ids"]
                 if "x_opencti_stix_ids" in stix_object
                 else None,
+                objectOrganization=stix_object["x_opencti_granted_refs"]
+                if "x_opencti_granted_refs" in stix_object
+                else None,
                 update=update,
             )
         else:
             LOGGER.error("[opencti_vulnerability] Missing parameters: stixObject")
```

### Comparing `pycti-5.9.4/pycti/utils/constants.py` & `pycti-5.9.5/pycti/utils/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -144,14 +144,16 @@
     [
         ("name", StringProperty(required=True)),
         ("spec_version", StringProperty(fixed="2.1")),
         ("description", StringProperty()),
         ("severity", StringProperty()),
         ("priority", StringProperty()),
         ("response_types", ListProperty(StringProperty)),
+        ("x_opencti_workflow_id", StringProperty()),
+        ("x_opencti_assignee_ids", ListProperty(StringProperty)),
         (
             "object_refs",
             ListProperty(
                 ReferenceProperty(valid_types=["SCO", "SDO", "SRO"], spec_version="2.1")
             ),
         ),
     ],
@@ -159,25 +161,52 @@
 class CustomObjectCaseIncident:
     """Case-Incident object."""
 
     pass
 
 
 @CustomObject(
+    "case-rfi",
+    [
+        ("name", StringProperty(required=True)),
+        ("spec_version", StringProperty(fixed="2.1")),
+        ("description", StringProperty()),
+        ("severity", StringProperty()),
+        ("priority", StringProperty()),
+        ("information_types", ListProperty(StringProperty)),
+        ("x_opencti_workflow_id", StringProperty()),
+        ("x_opencti_assignee_ids", ListProperty(StringProperty)),
+        (
+            "object_refs",
+            ListProperty(
+                ReferenceProperty(valid_types=["SCO", "SDO", "SRO"], spec_version="2.1")
+            ),
+        ),
+    ],
+)
+class CustomObjectCaseRfit:
+    """Case-Rfi object."""
+
+    pass
+
+
+@CustomObject(
     "task",
     [
         ("name", StringProperty(required=True)),
         ("spec_version", StringProperty(fixed="2.1")),
         ("description", StringProperty()),
         (
             "due_date",
             TimestampProperty(
                 default=lambda: NOW, precision="millisecond", precision_constraint="min"
             ),
         ),
+        ("x_opencti_workflow_id", StringProperty()),
+        ("x_opencti_assignee_ids", ListProperty(StringProperty)),
         (
             "object_refs",
             ListProperty(
                 ReferenceProperty(valid_types=["SCO", "SDO", "SRO"], spec_version="2.1")
             ),
         ),
     ],
```

### Comparing `pycti-5.9.4/pycti/utils/opencti_stix2.py` & `pycti-5.9.5/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.9.5/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/utils/opencti_stix2_update.py` & `pycti-5.9.5/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti/utils/opencti_stix2_utils.py` & `pycti-5.9.5/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti.egg-info/PKG-INFO` & `pycti-5.9.5/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.9.4
+Version: 5.9.5
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
-Metadata-Version: 2.1 Name: pycti Version: 5.9.4 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.9.5 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.9.4/pycti.egg-info/SOURCES.txt` & `pycti-5.9.5/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pycti.egg-info/requires.txt` & `pycti-5.9.5/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/pyproject.toml` & `pycti-5.9.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.9.4/setup.cfg` & `pycti-5.9.5/setup.cfg`

 * *Files identical despite different names*

