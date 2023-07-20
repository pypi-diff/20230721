# Comparing `tmp/crowdstrike-falconpy-dev-1.3.0.dev6.tar.gz` & `tmp/crowdstrike-falconpy-dev-1.3.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crowdstrike-falconpy-dev-1.3.0.dev6.tar", last modified: Fri Jul 14 05:22:15 2023, max compression
+gzip compressed data, was "crowdstrike-falconpy-dev-1.3.0.dev7.tar", last modified: Thu Jul 20 23:12:48 2023, max compression
```

## Comparing `crowdstrike-falconpy-dev-1.3.0.dev6.tar` & `crowdstrike-falconpy-dev-1.3.0.dev7.tar`

### file list

```diff
@@ -1,220 +1,220 @@
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.137681 crowdstrike-falconpy-dev-1.3.0.dev6/
--rw-r--r--   0 jhiller    (501) staff       (20)     4906 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/AUTHORS.md
--rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/LICENSE
--rw-r--r--   0 jhiller    (501) staff       (20)    32848 2023-07-14 05:22:15.137284 crowdstrike-falconpy-dev-1.3.0.dev6/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/README.md
--rw-r--r--   0 jhiller    (501) staff       (20)     7201 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/dev_setup.py
--rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-14 05:22:15.137788 crowdstrike-falconpy-dev-1.3.0.dev6/setup.cfg
--rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/setup.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:14.984349 crowdstrike-falconpy-dev-1.3.0.dev6/src/
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.006690 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/
--rw-r--r--   0 jhiller    (501) staff       (20)    32848 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO
--rw-r--r--   0 jhiller    (501) staff       (20)     8224 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt
--rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/dependency_links.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/requires.txt
--rw-r--r--   0 jhiller    (501) staff       (20)       12 2023-07-14 05:22:14.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/top_level.txt
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.055696 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/
--rw-r--r--   0 jhiller    (501) staff       (20)    12107 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.060221 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/
--rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_behavior.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_connection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_payloads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_validator.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.064561 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/
--rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_base_falcon_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_bearer_token.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20647 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_falcon_interface.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_interface_config.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_uber_interface.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.065133 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_constant/
--rw-r--r--   0 jhiller    (501) staff       (20)     2905 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_constant/__init__.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.098407 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/
--rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_prevention_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_update_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.110378 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/
--rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.113080 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/
--rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_container_base_url.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_token_fail_reason.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.114843 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/
--rw-r--r--   0 jhiller    (501) staff       (20)     2662 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6071 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_exceptions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_warnings.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.116038 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/
--rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/_facility.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.128681 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/
--rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_device_control_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_falconx.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_firewall.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_generic.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_response_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sensor_update_policy.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.133404 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/
--rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__base_resource.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_base_dictionary.py
--rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_errors.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_expanded_result.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_headers.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_meta.py
--rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_resources.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_response_component.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16548 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_result.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.134688 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/
--rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_base_service_class.py
--rw-r--r--   0 jhiller    (501) staff       (20)    11426 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_service_class.py
-drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-14 05:22:15.136617 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/
--rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/__init__.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_auth.py
--rw-r--r--   0 jhiller    (501) staff       (20)    33929 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_functions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_uber.py
--rw-r--r--   0 jhiller    (501) staff       (20)     3539 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_version.py
--rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/alerts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/api_complete.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cloud_connect_aws.py
--rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cspm_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/custom_ioa.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/d4c_registration.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/debug.py
--rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/detects.py
--rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/device_control_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/discover.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/event_streams.py
--rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_complete_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_container.py
--rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falconx_sandbox.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/fdr.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/filevantage.py
--rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/host_group.py
--rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/hosts.py
--rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/identity_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/incidents.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/installation_tokens.py
--rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/intel.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioa_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioc.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/iocs.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/kubernetes_protection.py
--rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/malquery.py
--rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/message_center.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ml_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mobile_enrollment.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mssp.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/oauth2.py
--rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ods.py
--rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/overwatch_dashboard.py
--rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/prevention_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quarantine.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quick_scan.py
--rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response.py
--rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response_admin.py
--rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/recon.py
--rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/report_executions.py
--rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/response_policies.py
--rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sample_uploads.py
--rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/scheduled_reports.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_download.py
--rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_update_policy.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_visibility_exclusions.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_evaluation_logic.py
--rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_vulnerabilities.py
--rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/tailored_intelligence.py
--rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/user_management.py
--rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-14 05:22:13.000000 crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.618142 crowdstrike-falconpy-dev-1.3.0.dev7/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4936 2023-07-20 23:12:46.000000 crowdstrike-falconpy-dev-1.3.0.dev7/AUTHORS.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     1211 2023-07-20 23:12:46.000000 crowdstrike-falconpy-dev-1.3.0.dev7/LICENSE
+-rw-r--r--   0 jhiller    (501) staff       (20)    32848 2023-07-20 23:12:48.617810 crowdstrike-falconpy-dev-1.3.0.dev7/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)    29563 2023-07-20 23:12:46.000000 crowdstrike-falconpy-dev-1.3.0.dev7/README.md
+-rw-r--r--   0 jhiller    (501) staff       (20)     7201 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/dev_setup.py
+-rw-r--r--   0 jhiller    (501) staff       (20)       38 2023-07-20 23:12:48.618244 crowdstrike-falconpy-dev-1.3.0.dev7/setup.cfg
+-rw-r--r--   0 jhiller    (501) staff       (20)     4482 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/setup.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.365969 crowdstrike-falconpy-dev-1.3.0.dev7/src/
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.374230 crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/
+-rw-r--r--   0 jhiller    (501) staff       (20)    32848 2023-07-20 23:12:48.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO
+-rw-r--r--   0 jhiller    (501) staff       (20)     8224 2023-07-20 23:12:48.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)        1 2023-07-20 23:12:48.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       83 2023-07-20 23:12:48.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/requires.txt
+-rw-r--r--   0 jhiller    (501) staff       (20)       12 2023-07-20 23:12:48.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/top_level.txt
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.444770 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/
+-rw-r--r--   0 jhiller    (501) staff       (20)    12107 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.449178 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2095 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11250 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5561 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_behavior.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5022 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_connection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3788 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5358 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_payloads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3827 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_validator.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.453187 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2047 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4234 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_base_falcon_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5998 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_bearer_token.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    21566 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_falcon_interface.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4806 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_interface_config.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8624 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_uber_interface.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.453864 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_constant/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2905 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_constant/__init__.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.560351 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/
+-rw-r--r--   0 jhiller    (501) staff       (20)     9054 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7042 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6740 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    30329 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13488 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15447 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6446 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10667 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3167 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12391 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6172 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14991 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3694 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23292 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10008 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9015 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10381 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8008 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6237 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22179 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4594 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11784 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13556 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15790 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5803 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7033 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4457 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2377 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20286 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3611 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12950 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3569 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9960 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_prevention_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4808 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4165 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    24729 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16057 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17960 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9918 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11674 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5275 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15927 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sensor_update_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4678 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4667 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7134 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4885 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16463 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6050 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.568863 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4611 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13207 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5506 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12267 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4091 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17702 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3316 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2273 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5947 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    11312 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2177 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13181 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13678 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13342 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4094 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3816 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1945 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.570924 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1871 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2124 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2063 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/_container_base_url.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2218 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/_token_fail_reason.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.572155 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/
+-rw-r--r--   0 jhiller    (501) staff       (20)     2662 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6071 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/_exceptions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3573 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/_warnings.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.573311 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_log/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1744 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_log/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3809 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_log/_facility.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.584392 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/
+-rw-r--r--   0 jhiller    (501) staff       (20)     5516 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2691 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3624 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5855 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6079 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4604 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2790 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6181 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_device_control_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3666 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_falconx.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16333 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_firewall.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7329 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_generic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4290 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4511 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5808 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7508 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5577 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3774 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2866 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4506 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3118 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4309 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8001 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2615 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_response_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2433 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4519 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_sensor_update_policy.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.613710 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/
+-rw-r--r--   0 jhiller    (501) staff       (20)     4540 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/__base_resource.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2186 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4581 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_base_dictionary.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     1825 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_errors.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2684 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_expanded_result.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3112 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_headers.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3298 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_meta.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     2489 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_resources.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4561 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_response_component.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16736 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_result.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.615252 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/
+-rw-r--r--   0 jhiller    (501) staff       (20)     1827 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12272 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/_base_service_class.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    12083 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/_service_class.py
+drwxr-xr-x   0 jhiller    (501) staff       (20)        0 2023-07-20 23:12:48.617183 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/
+-rw-r--r--   0 jhiller    (501) staff       (20)     3087 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/__init__.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3076 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/_auth.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34041 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/_functions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6161 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/_uber.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     3539 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_version.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    17508 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/alerts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9970 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/api_complete.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15947 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/cloud_connect_aws.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    48601 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/cspm_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34208 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/custom_ioa.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27069 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/d4c_registration.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10750 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/debug.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    15759 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/detects.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    29552 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/device_control_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    22218 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/discover.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5973 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/event_streams.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    37615 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/falcon_complete_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16270 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/falcon_container.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    28300 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/falconx_sandbox.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8668 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/fdr.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5384 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/filevantage.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    79369 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/firewall_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20174 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/firewall_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    18869 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/host_group.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    27450 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/hosts.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     4578 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/identity_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13758 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/incidents.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13613 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/installation_tokens.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    34693 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/intel.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10663 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ioa_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35840 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ioc.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14032 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/iocs.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25074 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/kubernetes_protection.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    16367 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/malquery.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    23565 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/message_center.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10056 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ml_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     5166 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/mobile_enrollment.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43338 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/mssp.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8919 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/oauth2.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    35443 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ods.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    13881 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/overwatch_dashboard.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    20718 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/prevention_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    14372 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/quarantine.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9493 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/quick_scan.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    43159 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/real_time_response.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    25250 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/real_time_response_admin.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    45859 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/recon.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     7687 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/report_executions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    19891 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/response_policies.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    21891 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sample_uploads.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     6764 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/scheduled_reports.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10169 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sensor_download.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    38364 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sensor_update_policy.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9899 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sensor_visibility_exclusions.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8333 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/spotlight_evaluation_logic.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    10652 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/spotlight_vulnerabilities.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     9791 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/tailored_intelligence.py
+-rw-r--r--   0 jhiller    (501) staff       (20)    39321 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/user_management.py
+-rw-r--r--   0 jhiller    (501) staff       (20)     8311 2023-07-20 23:12:47.000000 crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/zero_trust_assessment.py
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/AUTHORS.md` & `crowdstrike-falconpy-dev-1.3.0.dev7/AUTHORS.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,15 @@
 + `@jmillerca`
 + `@davidt99`
 + `@CommonVulnerability`
 + `@Odie71`
 + Chris, `@chrisbvt`
 + Alex, `@khyberspache`
 + Phil Massyn, `@massyn`
++ Russell Snyder, `@rusnyder`
 
 
 ## Sponsors
 Without the support of these executives, the FalconPy project would not have happened.
 
 | Name | Role |
 | :-- | :-- |
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/LICENSE` & `crowdstrike-falconpy-dev-1.3.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/PKG-INFO` & `crowdstrike-falconpy-dev-1.3.0.dev7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy-dev
-Version: 1.3.0.dev6
+Version: 1.3.0.dev7
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/README.md` & `crowdstrike-falconpy-dev-1.3.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/dev_setup.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/dev_setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/setup.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/setup.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crowdstrike-falconpy-dev
-Version: 1.3.0.dev6
+Version: 1.3.0.dev7
 Summary: The CrowdStrike Falcon SDK for Python 3
 Home-page: https://github.com/CrowdStrike/falconpy
 Author: CrowdStrike
 Author-email: falconpy@crowdstrike.com
 Maintainer: Joshua Hiller
 Maintainer-email: falconpy@crowdstrike.com
 Project-URL: Documentation, https://www.falconpy.io
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/crowdstrike_falconpy_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_behavior.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_behavior.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_connection.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_connection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_meta.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_payloads.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_payloads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_api_request/_request_validator.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_api_request/_request_validator.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_base_falcon_auth.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_base_falcon_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_bearer_token.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_bearer_token.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_falcon_interface.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_falcon_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
 import time
+import os
 import warnings
 from json import loads
 try:
     from simplejson import JSONDecodeError
 except ImportError:
     from json.decoder import JSONDecodeError
 from logging import Logger, getLogger
@@ -154,14 +155,28 @@
                                      MIN_TOKEN_RENEW_WINDOW
                                      )
         # Legacy (Token) Authentication (fallback)
         if access_token:
             # Store this non-refreshable token, assuming it was just generated.
             self._token: BearerToken = BearerToken(access_token, 1799)
 
+        # Environment Authentication
+        # When credentials are not provided, attempt to retrieve them from the environment.
+        if not self.cred_format_valid and not self.refreshable:
+            if os.getenv("FALCON_CLIENT_ID") and os.getenv("FALCON_CLIENT_SECRET"):
+                api_id = os.getenv("FALCON_CLIENT_ID") if "client_id" not in self.creds else self.creds["client_id"]
+                if "client_secret" not in self.creds:
+                    api_sec = os.getenv("FALCON_CLIENT_SECRET")
+                else:
+                    api_sec = self.creds["client_secret"]
+                self.creds = {
+                    "client_id": api_id,
+                    "client_secret": api_sec
+                }
+
         # Log the creation of this object if debugging is enabled.
         if debug:
             # Ignored when debugging is disabled.
             _debug_record_count: int = debug_record_count if debug_record_count else None
             # Allow log sanitization to be overridden.
             _sanitize = sanitize_log if isinstance(sanitize_log, bool) else None
             # Logging facility for all classes using this interface, defaults to disabled.
@@ -451,15 +466,19 @@
     def authenticated(self) -> bool:
         """Return if we are authenticated by retrieving the inverse of token_expired."""
         return not self.token_expired
 
     @property
     def cred_format_valid(self) -> bool:
         """Return a boolean that the creds dictionary is valid."""
-        return bool("client_id" in self.creds and "client_secret" in self.creds)
+        _returned = False
+        if "client_id" in self.creds and "client_secret" in self.creds:
+            if isinstance(self.creds["client_id"], str) and isinstance(self.creds["client_secret"], str):
+                _returned = True
+        return _returned
 
     @property
     def log(self) -> Logger:
         """Return the logger from our log facility."""
         return self.log_facility.log
 
     @property
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_interface_config.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_interface_config.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_auth_object/_uber_interface.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_auth_object/_uber_interface.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_constant/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_constant/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_alerts.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_cspm_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_custom_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_detects.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_device_control_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_discover.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_event_streams.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falcon_container.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_fdr.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_filevantage.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_firewall_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_host_group.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_hosts.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_identity_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_incidents.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_installation_tokens.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_intel.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_iocs.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_malquery.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_message_center.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ml_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_mssp.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_oauth2.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_prevention_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_prevention_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quarantine.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_quick_scan.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_recon.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_report_executions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_response_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sample_uploads.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_download.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_update_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sensor_update_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_user_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/_zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_custom_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_discover.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_fdr.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_firewall_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_hosts.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_identity_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_installation_tokens.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_iocs.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_report_executions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_endpoint/deprecated/_zero_trust_assessment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_base_url.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_container_base_url.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/_container_base_url.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_enum/_token_fail_reason.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_enum/_token_fail_reason.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_exceptions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/_exceptions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_error/_warnings.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_error/_warnings.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_log/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_log/_facility.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_log/_facility.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_alerts.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_container.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_cspm_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_detects.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_device_control_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_device_control_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_falconx.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_falconx.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_firewall.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_firewall.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_generic.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_generic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_host_group.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_incidents.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_malquery.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_message_center.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_mssp.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_prevention_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_recon.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_response_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_response_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sample_uploads.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_payload/_sensor_update_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_payload/_sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__base_resource.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/__base_resource.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_base_dictionary.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_base_dictionary.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_errors.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_errors.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_expanded_result.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_expanded_result.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_headers.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_headers.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_meta.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_meta.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_resources.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_resources.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_response_component.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_response_component.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_result/_result.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_result/_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,17 @@
                     # due to the combined response format.
                     self.raw = RawBody(body)
                 elif body.get("data", {}):  # pragma: no cover
                     # GraphQL uses a custom response payload, we will
                     # use RawBody for this return for now. Due to
                     # environment constraints, this is manually tested.
                     self.raw = RawBody(body)
+                elif isinstance(body.get("resources", []), dict):
+                    # Catch unusual response payloads not explicitly handled
+                    self.raw = RawBody(body)
                 else:
                     # Standard API responses
                     self.resources = Resources(body.get("resources", []))
 
     # Iteration handlers
     def __iter__(self):
         """Return this object for iteration handling."""
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_base_service_class.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/_base_service_class.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_service_class/_service_class.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_service_class/_service_class.py`

 * *Files 6% similar despite different names*

```diff
@@ -242,14 +242,32 @@
 
         Changing this value will impact the renew window for all classes
         using this auth_object.
         """
         self.auth_object.renew_window = value
 
     @property
+    def token_renew_window(self) -> int:
+        """Return the current renew window from the auth_object.
+
+        DEPRECATED: This property recreates a legacy attribute.
+        Developers should update code to make use of the `renew_window` property.
+        """
+        return self.auth_object.renew_window
+
+    @token_renew_window.setter
+    def token_renew_window(self, value: int):
+        """Allow the renew_window to be changed.
+
+        DEPRECATED: This property recreates a legacy attribute.
+        Developers should update code to make use of the `renew_window` property.
+        """
+        self.auth_object.renew_window = value
+
+    @property
     def user_agent(self) -> int:
         """Provide the user_agent from the auth_object if it's not been set."""
         if self._override_user_agent:
             returned = self._override_user_agent
         else:
             returned = self.auth_object.user_agent
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/__init__.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_auth.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/_auth.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_functions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -721,30 +721,31 @@
 
     return new_base_url
 
 
 def sanitize_dictionary(dirty: Any, record_max: int = MAX_DEBUG_RECORDS) -> dict:
     """Strip confidential data from logged dictionaries."""
     cleaned = dirty
-    if isinstance(dirty, dict):
+    if isinstance(dirty, dict):  # pylint: disable=R1702
         # cleaned = deepcopy(dict(dirty))
         redacted = ["access_token", "client_id", "client_secret", "member_cid", "token"]
         for redact in redacted:
             if redact in cleaned:
                 cleaned[redact] = "REDACTED"
             if "body" in cleaned:
                 if redact in cleaned["body"]:
                     cleaned["body"][redact] = "REDACTED"
                 if "resources" in cleaned["body"]:
                     # Log results are limited to MAX_DEBUG_RECORDS
                     # number of items within the resources list
                     if cleaned["body"]["resources"]:
-                        del cleaned["body"]["resources"][max(1, min(record_max,
-                                                                    GLOBAL_API_MAX_RETURN
-                                                                    )):]
+                        if isinstance(cleaned["body"]["resources"], list):
+                            del cleaned["body"]["resources"][max(1, min(record_max,
+                                                                        GLOBAL_API_MAX_RETURN
+                                                                        )):]
         if "Authorization" in cleaned:
             cleaned["Authorization"] = "Bearer REDACTED"
 
     return cleaned
 
 
 # Python 3.6 compatibility warning: Cannot properly type the interface.
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_util/_uber.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_util/_uber.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/_version.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
 OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
 OTHER DEALINGS IN THE SOFTWARE.
 
 For more information, please refer to <https://unlicense.org>
 """
-_VERSION = '1.3.0.dev6'
+_VERSION = '1.3.0.dev7'
 _MAINTAINER = 'Joshua Hiller'
 _AUTHOR = 'CrowdStrike'
 _AUTHOR_EMAIL = 'falconpy@crowdstrike.com'
 _CREDITS = 'CrowdStrike'
 _DESCRIPTION = "The CrowdStrike Falcon SDK for Python 3"
 _TITLE = "crowdstrike-falconpy"
 _PROJECT_URL = "https://github.com/CrowdStrike/falconpy"
```

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/alerts.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/alerts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/api_complete.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/api_complete.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cloud_connect_aws.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/cloud_connect_aws.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/cspm_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/cspm_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/custom_ioa.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/custom_ioa.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/d4c_registration.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/d4c_registration.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/debug.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/debug.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/detects.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/detects.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/device_control_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/device_control_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/discover.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/discover.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/event_streams.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/event_streams.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_complete_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/falcon_complete_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falcon_container.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/falcon_container.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/falconx_sandbox.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/falconx_sandbox.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/fdr.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/fdr.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/filevantage.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/filevantage.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/firewall_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/firewall_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/firewall_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/host_group.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/host_group.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/hosts.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/hosts.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/identity_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/identity_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/incidents.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/incidents.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/installation_tokens.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/installation_tokens.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/intel.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/intel.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioa_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ioa_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ioc.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ioc.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/iocs.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/iocs.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/kubernetes_protection.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/kubernetes_protection.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/malquery.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/malquery.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/message_center.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/message_center.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ml_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ml_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mobile_enrollment.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/mobile_enrollment.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/mssp.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/mssp.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/oauth2.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/oauth2.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/ods.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/ods.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/overwatch_dashboard.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/overwatch_dashboard.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/prevention_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/prevention_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quarantine.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/quarantine.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/quick_scan.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/quick_scan.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/real_time_response.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/real_time_response_admin.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/real_time_response_admin.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/recon.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/recon.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/report_executions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/report_executions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/response_policies.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/response_policies.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sample_uploads.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sample_uploads.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/scheduled_reports.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/scheduled_reports.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_download.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sensor_download.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_update_policy.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sensor_update_policy.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/sensor_visibility_exclusions.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/sensor_visibility_exclusions.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_evaluation_logic.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/spotlight_evaluation_logic.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/spotlight_vulnerabilities.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/spotlight_vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/tailored_intelligence.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/tailored_intelligence.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/user_management.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/user_management.py`

 * *Files identical despite different names*

### Comparing `crowdstrike-falconpy-dev-1.3.0.dev6/src/falconpydev/zero_trust_assessment.py` & `crowdstrike-falconpy-dev-1.3.0.dev7/src/falconpydev/zero_trust_assessment.py`

 * *Files identical despite different names*

