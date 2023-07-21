# Comparing `tmp/ops-scenario-4.0.3.tar.gz` & `tmp/ops-scenario-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops-scenario-4.0.3.tar", last modified: Fri Jul 21 09:45:24 2023, max compression
+gzip compressed data, was "ops-scenario-4.0.4.tar", last modified: Fri Jul 21 12:08:05 2023, max compression
```

## Comparing `ops-scenario-4.0.3.tar` & `ops-scenario-4.0.4.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.137275 ops-scenario-4.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.121275 ops-scenario-4.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.125275 ops-scenario-4.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/.github/workflows/build_wheels.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/.github/workflows/quality_checks.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    39878 2023-07-21 09:45:24.137275 ops-scenario-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39068 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.125275 ops-scenario-4.0.3/ops_scenario.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    39878 2023-07-21 09:45:23.000000 ops-scenario-4.0.3/ops_scenario.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-21 09:45:24.000000 ops-scenario-4.0.3/ops_scenario.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 09:45:23.000000 ops-scenario-4.0.3/ops_scenario.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 09:45:23.000000 ops-scenario-4.0.3/ops_scenario.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 09:45:23.000000 ops-scenario-4.0.3/ops_scenario.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 09:45:23.000000 ops-scenario-4.0.3/ops_scenario.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.125275 ops-scenario-4.0.3/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    50386 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/resources/state-transition-model.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.129274 ops-scenario-4.0.3/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/capture_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/fs_mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/ops_main_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.129274 ops-scenario-4.0.3/scenario/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/scripts/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/scripts/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    30113 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/scripts/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/scripts/state_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/scripts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/scenario/state.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 09:45:24.137275 ops-scenario-4.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.133274 ops-scenario-4.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.133274 ops-scenario-4.0.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/resources/demo_decorate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_dcbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 09:45:24.137275 ops-scenario-4.0.3/tests/test_e2e/
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_builtin_scenes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_custom_event_triggers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_deferred.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_juju_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_observers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_pebble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_play_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_rubbish_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_stored_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_e2e/test_vroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_emitted_events_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tests/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-21 09:45:12.000000 ops-scenario-4.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.767419 ops-scenario-4.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.755418 ops-scenario-4.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.759418 ops-scenario-4.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/.github/workflows/build_wheels.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/.github/workflows/quality_checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    39878 2023-07-21 12:08:05.767419 ops-scenario-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39068 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.759418 ops-scenario-4.0.4/ops_scenario.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39878 2023-07-21 12:08:05.000000 ops-scenario-4.0.4/ops_scenario.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-21 12:08:05.000000 ops-scenario-4.0.4/ops_scenario.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:08:05.000000 ops-scenario-4.0.4/ops_scenario.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 12:08:05.000000 ops-scenario-4.0.4/ops_scenario.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 12:08:05.000000 ops-scenario-4.0.4/ops_scenario.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 12:08:05.000000 ops-scenario-4.0.4/ops_scenario.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.759418 ops-scenario-4.0.4/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    50386 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/resources/state-transition-model.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.759418 ops-scenario-4.0.4/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/capture_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14394 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/fs_mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13868 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/ops_main_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.763419 ops-scenario-4.0.4/scenario/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/scripts/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/scripts/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30113 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/scripts/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/scripts/state_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/scripts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39685 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/scenario/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:08:05.767419 ops-scenario-4.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.763419 ops-scenario-4.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.763419 ops-scenario-4.0.4/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/resources/demo_decorate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_dcbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:08:05.767419 ops-scenario-4.0.4/tests/test_e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_builtin_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_custom_event_triggers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_deferred.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_juju_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_observers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_pebble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_play_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_rubbish_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_stored_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_e2e/test_vroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_emitted_events_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tests/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-21 12:07:49.000000 ops-scenario-4.0.4/tox.ini
```

### Comparing `ops-scenario-4.0.3/.github/workflows/build_wheels.yaml` & `ops-scenario-4.0.4/.github/workflows/build_wheels.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/.github/workflows/quality_checks.yaml` & `ops-scenario-4.0.4/.github/workflows/quality_checks.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/.pre-commit-config.yaml` & `ops-scenario-4.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/CONTRIBUTING.md` & `ops-scenario-4.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/LICENSE.txt` & `ops-scenario-4.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/PKG-INFO` & `ops-scenario-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 4.0.3
+Version: 4.0.4
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-4.0.3/README.md` & `ops-scenario-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/ops_scenario.egg-info/PKG-INFO` & `ops-scenario-4.0.4/ops_scenario.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-scenario
-Version: 4.0.3
+Version: 4.0.4
 Summary: Python library providing a Scenario-based testing API for Operator Framework charms.
 Author-email: Pietro Pasotti <pietro.pasotti@canonical.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/canonical/ops-scenario
 Project-URL: Bug Tracker, https://github.com/canonical/ops-scenario/issues
 Keywords: juju,test
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ops-scenario-4.0.3/ops_scenario.egg-info/SOURCES.txt` & `ops-scenario-4.0.4/ops_scenario.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/pyproject.toml` & `ops-scenario-4.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,26 +4,26 @@
     "setuptools_scm >= 2.0.0, <3"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ops-scenario"
 
-version = "4.0.3"
+version = "4.0.4"
 
 authors = [
     { name = "Pietro Pasotti", email = "pietro.pasotti@canonical.com" }
 ]
 description = "Python library providing a Scenario-based testing API for Operator Framework charms."
 license.text = "Apache-2.0"
 keywords = ["juju", "test"]
 
 dependencies = [
     "ops>=2.0",
-    "PyYAML==6.0",
+    "PyYAML>=6.0.1",
     "typer==0.7.0",
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `ops-scenario-4.0.3/resources/state-transition-model.png` & `ops-scenario-4.0.4/resources/state-transition-model.png`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/__init__.py` & `ops-scenario-4.0.4/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/capture_events.py` & `ops-scenario-4.0.4/scenario/capture_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/consistency_checker.py` & `ops-scenario-4.0.4/scenario/consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/context.py` & `ops-scenario-4.0.4/scenario/context.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/fs_mocks.py` & `ops-scenario-4.0.4/scenario/fs_mocks.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/mocking.py` & `ops-scenario-4.0.4/scenario/mocking.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/ops_main_mock.py` & `ops-scenario-4.0.4/scenario/ops_main_mock.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/runtime.py` & `ops-scenario-4.0.4/scenario/runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/scripts/main.py` & `ops-scenario-4.0.4/scenario/scripts/main.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/scripts/snapshot.py` & `ops-scenario-4.0.4/scenario/scripts/snapshot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/scripts/state_apply.py` & `ops-scenario-4.0.4/scenario/scripts/state_apply.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/scripts/utils.py` & `ops-scenario-4.0.4/scenario/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/sequences.py` & `ops-scenario-4.0.4/scenario/sequences.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/scenario/state.py` & `ops-scenario-4.0.4/scenario/state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/helpers.py` & `ops-scenario-4.0.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_consistency_checker.py` & `ops-scenario-4.0.4/tests/test_consistency_checker.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_dcbase.py` & `ops-scenario-4.0.4/tests/test_dcbase.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_actions.py` & `ops-scenario-4.0.4/tests/test_e2e/test_actions.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_builtin_scenes.py` & `ops-scenario-4.0.4/tests/test_e2e/test_builtin_scenes.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_config.py` & `ops-scenario-4.0.4/tests/test_e2e/test_config.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_custom_event_triggers.py` & `ops-scenario-4.0.4/tests/test_e2e/test_custom_event_triggers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_deferred.py` & `ops-scenario-4.0.4/tests/test_e2e/test_deferred.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_juju_log.py` & `ops-scenario-4.0.4/tests/test_e2e/test_juju_log.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_network.py` & `ops-scenario-4.0.4/tests/test_e2e/test_network.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_observers.py` & `ops-scenario-4.0.4/tests/test_e2e/test_observers.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_pebble.py` & `ops-scenario-4.0.4/tests/test_e2e/test_pebble.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_play_assertions.py` & `ops-scenario-4.0.4/tests/test_e2e/test_play_assertions.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_relations.py` & `ops-scenario-4.0.4/tests/test_e2e/test_relations.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_rubbish_events.py` & `ops-scenario-4.0.4/tests/test_e2e/test_rubbish_events.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_secrets.py` & `ops-scenario-4.0.4/tests/test_e2e/test_secrets.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_state.py` & `ops-scenario-4.0.4/tests/test_e2e/test_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_status.py` & `ops-scenario-4.0.4/tests/test_e2e/test_status.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_stored_state.py` & `ops-scenario-4.0.4/tests/test_e2e/test_stored_state.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_e2e/test_vroot.py` & `ops-scenario-4.0.4/tests/test_e2e/test_vroot.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_emitted_events_util.py` & `ops-scenario-4.0.4/tests/test_emitted_events_util.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_plugin.py` & `ops-scenario-4.0.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tests/test_runtime.py` & `ops-scenario-4.0.4/tests/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ops-scenario-4.0.3/tox.ini` & `ops-scenario-4.0.4/tox.ini`

 * *Files identical despite different names*

