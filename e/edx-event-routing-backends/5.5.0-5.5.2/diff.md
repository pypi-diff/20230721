# Comparing `tmp/edx-event-routing-backends-5.5.0.tar.gz` & `tmp/edx-event-routing-backends-5.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-event-routing-backends-5.5.0.tar", last modified: Wed Jun 28 21:08:00 2023, max compression
+gzip compressed data, was "edx-event-routing-backends-5.5.2.tar", last modified: Fri Jul 21 10:54:06 2023, max compression
```

## Comparing `edx-event-routing-backends-5.5.0.tar` & `edx-event-routing-backends-5.5.2.tar`

### file list

```diff
@@ -1,123 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.696477 edx-event-routing-backends-5.5.0/
--rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      222 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-06-28 21:08:00.696477 edx-event-routing-backends-5.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.680477 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4921 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-28 21:08:00.000000 edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.680477 edx-event-routing-backends-5.5.0/event_routing_backends/
--rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.680477 edx-event-routing-backends-5.5.0/event_routing_backends/backends/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8145 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/backends/events_router.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.680477 edx-event-routing-backends-5.5.0/event_routing_backends/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27921 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/backends/tests/test_events_router.py
--rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.680477 edx-event-routing-backends-5.5.0/event_routing_backends/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.680477 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.684477 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/helpers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/helpers/event_log_parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/helpers/queued_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.684477 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    14350 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    10799 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/transform_tracking_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.684477 edx-event-routing-backends-5.5.0/event_routing_backends/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0002_auto_20210503_0648.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0003_auto_20210713_0344.py
--rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0004_auto_20211025_1053.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9144 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.684477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      907 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/envelope_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      598 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     5861 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      302 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/test_caliper.py
--rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/mixins/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/mixins/base_transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/mixins/base_transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/tests/transformers_test_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      165 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.688477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.692477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4420 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.692477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
--rw-r--r--   0 runner    (1001) docker     (122)    10068 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/video_events.py
--rw-r--r--   0 runner    (1001) docker     (122)      293 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.692477 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/tests/test_transformers.py
--rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/transformer_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.692477 edx-event-routing-backends-5.5.0/event_routing_backends/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9014 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.676477 edx-event-routing-backends-5.5.0/event_routing_backends/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.676477 edx-event-routing-backends-5.5.0/event_routing_backends/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.692477 edx-event-routing-backends-5.5.0/event_routing_backends/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (122)      812 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
--rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.676477 edx-event-routing-backends-5.5.0/event_routing_backends/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.692477 edx-event-routing-backends-5.5.0/event_routing_backends/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/templates/admin/router_conf_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.696477 edx-event-routing-backends-5.5.0/event_routing_backends/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      527 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.696477 edx-event-routing-backends-5.5.0/event_routing_backends/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      227 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/event_routing_backends/utils/xapi_lrs_client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-28 21:08:00.696477 edx-event-routing-backends-5.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-06-28 21:08:00.696477 edx-event-routing-backends-5.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-06-28 21:07:55.000000 edx-event-routing-backends-5.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     2859 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      222 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3721 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.183133 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7365 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4995 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-21 10:54:06.000000 edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8145 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/backends/events_router.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27921 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/backends/tests/test_events_router.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8529 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/helpers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/helpers/event_log_parser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5944 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/helpers/queued_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    14350 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10799 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/transform_tracking_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      981 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0002_auto_20210503_0648.py
+-rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0003_auto_20210713_0344.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1938 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0004_auto_20211025_1053.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9144 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/processors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.187133 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/envelope_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)      598 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2035 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3213 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5823 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5778 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4905 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/test_caliper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1290 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/test_envelope_processor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2404 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/mixins/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7022 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/mixins/base_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3018 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/mixins/base_transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/tests/transformers_test_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1059 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/
+-rw-r--r--   0 runner    (1001) docker     (122)     1513 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4899 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1082 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3448 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/forum_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/navigation_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9037 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10068 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/video_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      293 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.191134 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2857 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/tests/test_transformers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4536 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5404 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/transformer_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/event_routing_backends/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1643 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/settings/production.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.183133 edx-event-routing-backends-5.5.2/event_routing_backends/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.183133 edx-event-routing-backends-5.5.2/event_routing_backends/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/event_routing_backends/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (122)      812 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5163 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.183133 edx-event-routing-backends-5.5.2/event_routing_backends/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/event_routing_backends/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/templates/admin/router_conf_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/event_routing_backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      527 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2875 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5261 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/event_routing_backends/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      227 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4148 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4473 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/event_routing_backends/utils/xapi_lrs_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-21 10:54:06.195134 edx-event-routing-backends-5.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-07-21 10:53:58.000000 edx-event-routing-backends-5.5.2/setup.py
```

### Comparing `edx-event-routing-backends-5.5.0/CHANGELOG.rst` & `edx-event-routing-backends-5.5.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/LICENSE.txt` & `edx-event-routing-backends-5.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/PKG-INFO` & `edx-event-routing-backends-5.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.5.0
+Version: 5.5.2
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `edx-event-routing-backends-5.5.0/README.rst` & `edx-event-routing-backends-5.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/PKG-INFO` & `edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: edx-event-routing-backends
-Version: 5.5.0
+Version: 5.5.2
 Summary: Various backends for receiving edX LMS events.
 Home-page: https://github.com/openedx/event-routing-backends
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
```

### Comparing `edx-event-routing-backends-5.5.0/edx_event_routing_backends.egg-info/SOURCES.txt` & `edx-event-routing-backends-5.5.2/edx_event_routing_backends.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 event_routing_backends/processors/xapi/__init__.py
 event_routing_backends/processors/xapi/constants.py
 event_routing_backends/processors/xapi/registry.py
 event_routing_backends/processors/xapi/transformer.py
 event_routing_backends/processors/xapi/transformer_processor.py
 event_routing_backends/processors/xapi/event_transformers/__init__.py
 event_routing_backends/processors/xapi/event_transformers/enrollment_events.py
+event_routing_backends/processors/xapi/event_transformers/forum_events.py
 event_routing_backends/processors/xapi/event_transformers/navigation_events.py
 event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py
 event_routing_backends/processors/xapi/event_transformers/video_events.py
 event_routing_backends/processors/xapi/tests/__init__.py
 event_routing_backends/processors/xapi/tests/test_transformers.py
 event_routing_backends/processors/xapi/tests/test_xapi.py
 event_routing_backends/settings/__init__.py
```

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/admin.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,21 @@
 """
 from config_models.admin import KeyedConfigurationModelAdmin
 from django.contrib import admin
 
 from event_routing_backends.models import RouterConfiguration
 
 
+@admin.register(RouterConfiguration)
 class RouterConfigurationAdmin(KeyedConfigurationModelAdmin):
     """
     Admin model class for RouterConfiguration model.
     """
 
     history_list_display = 'status'
     change_form_template = 'admin/router_conf_change_form.html'
 
     def get_displayable_field_names(self):
         """
         Get the list display.
         """
         return ['backend_name', 'enabled', 'route_url', 'configurations']
-
-
-admin.site.register(RouterConfiguration, RouterConfigurationAdmin)
```

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/apps.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/apps.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/backends/events_router.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/backends/events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/backends/tests/test_events_router.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/backends/tests/test_events_router.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/helpers.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/helpers/event_log_parser.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/helpers/event_log_parser.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/helpers/queued_sender.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/helpers/queued_sender.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/tests/test_transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/management/commands/transform_tracking_logs.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/management/commands/transform_tracking_logs.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0001_initial.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0002_auto_20210503_0648.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0002_auto_20210503_0648.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/migrations/0004_auto_20211025_1053.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/migrations/0004_auto_20211025_1053.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/models.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/__init__.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/envelope_processor.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/__init__.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/event_transformers/video_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/event_transformers/video_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,14 @@
 - edx.video.loaded
 - edx.video.played
 - edx.video.stopped
 - edx.video.paused
 - edx.video.position.changed
 - edx.video.completed (proposed)
 """
-from datetime import timedelta
-
-from isodate import duration_isoformat
-
 from event_routing_backends.helpers import convert_seconds_to_iso, make_video_block_id
 from event_routing_backends.processors.caliper.registry import CaliperTransformersRegistry
 from event_routing_backends.processors.caliper.transformer import CaliperTransformer
 
 EVENTS_ACTION_MAP = {
     'load_video': 'Started',
     'edx.video.loaded': 'Started',
@@ -91,17 +87,17 @@
         course_id = self.get_data('context.course_id', True)
         video_id = self.get_data('data.id', True)
         object_id = make_video_block_id(course_id=course_id, video_id=video_id)
 
         caliper_object.update({
             'id': self.get_object_iri('xblock', object_id),
             'type': 'VideoObject',
-            'duration': duration_isoformat(timedelta(
-                    seconds=data.get('duration', 0)
-            ))
+            'duration': convert_seconds_to_iso(
+                seconds=data.get('duration', 0)
+            )
         })
 
         return caliper_object
 
     def get_target(self):
         """
         Return target for the caliper event.
```

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/test_caliper.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/test_caliper.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/test_envelope_processor.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/test_envelope_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/tests/test_transformers.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/transformer.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/caliper/transformer_processor.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/caliper/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/mixins/base_transformer.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/mixins/base_transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/mixins/base_transformer_processor.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/mixins/base_transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/tests/transformers_test_mixin.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/tests/transformers_test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/registry.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/transformer_utils/tests/test_registry.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/transformer_utils/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/__init__.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/__init__.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/constants.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 XAPI_VERB_REGISTERED = 'http://adlnet.gov/expapi/verbs/registered'
 XAPI_VERB_UNREGISTERED = 'http://id.tincanapi.com/verb/unregistered'
 XAPI_VERB_COMPLETED = 'http://adlnet.gov/expapi/verbs/completed'
 XAPI_VERB_PASSED = 'http://adlnet.gov/expapi/verbs/passed'
 XAPI_VERB_FAILED = 'http://adlnet.gov/expapi/verbs/failed'
 XAPI_VERB_EXPERIENCED = 'http://adlnet.gov/expapi/verbs/experienced'
 XAPI_VERB_NAVIGATED = 'https://w3id.org/xapi/dod-isd/verbs/navigated'
+XAPI_VERB_POSTED = 'https://w3id.org/xapi/acrossx/verbs/posted'
+XAPI_VERB_EDITED = 'https://w3id.org/xapi/acrossx/verbs/edited'
+XAPI_VERB_VIEWED = 'http://id.tincanapi.com/verb/viewed'
+XAPI_VERB_DELETED = 'https://w3id.org/xapi/dod-isd/verbs/deleted'
+XAPI_VERB_VOTED = 'https://w3id.org/xapi/openedx/verb/voted'
 
 XAPI_VERB_TERMINATED = 'http://adlnet.gov/expapi/verbs/terminated'
 XAPI_VERB_ASKED = 'http://adlnet.gov/expapi/verbs/asked'
 
 
 XAPI_VERB_INITIALIZED = 'http://adlnet.gov/expapi/verbs/initialized'
 XAPI_VERB_PLAYED = 'https://w3id.org/xapi/video/verbs/played'
@@ -30,14 +35,15 @@
 XAPI_ACTIVITY_SOLUTION = 'http://id.tincanapi.com/activitytype/solution'
 XAPI_ACTIVITY_RESOURCE = 'http://id.tincanapi.com/activitytype/resource'
 XAPI_ACTIVITY_INTERACTION = 'http://adlnet.gov/expapi/activities/cmi.interaction'
 XAPI_ACTIVITY_SUPPLEMENTAL_INFO = 'https://w3id.org/xapi/acrossx/extensions/supplemental-info'
 XAPI_ACTIVITY_COURSE = 'http://adlnet.gov/expapi/activities/course'
 XAPI_ACTIVITY_MODULE = 'http://adlnet.gov/expapi/activities/module'
 XAPI_ACTIVITY_VIDEO = 'https://w3id.org/xapi/video/activity-type/video'
+XAPI_ACTIVITY_DISCUSSION = 'http://id.tincanapi.com/activitytype/discussion'
 XAPI_ACTIVITY_LINK = 'http://adlnet.gov/expapi/activities/link'
 XAPI_ACTIVITY_POSITION = 'http://id.tincanapi.com/extension/position'
 XAPI_ACTIVITY_TOTAL_COUNT = 'https://w3id.org/xapi/acrossx/extensions/total-items'
 XAPI_ACTIVITY_MODE = 'https://w3id.org/xapi/acrossx/extensions/type'
 XAPI_ACTIVITY_ATTEMPT = 'http://id.tincanapi.com/extension/attempt-id'
 
 # xAPI context
@@ -78,14 +84,19 @@
 INTERACTED = 'interacted'
 PLAYED = 'played'
 PAUSED = 'paused'
 COMPLETED = 'completed'
 PASSED = 'passed'
 FAILED = 'failed'
 SEEKED = 'seeked'
+POSTED = 'posted'
+VIEWED = 'viewed'
+DELETED = 'deleted'
+EDITED = 'edited'
+VOTED = 'voted'
 
 TERMINATED = 'terminated'
 NAVIGATED = 'navigated'
 ASKED = 'asked'
 
 # Open edX
 OPENEDX_OAUTH2_TOKEN_URL = '/oauth2/access_token'
```

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/__init__.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,21 @@
 All xAPI transformers.
 """
 
 from event_routing_backends.processors.xapi.event_transformers.enrollment_events import (
     EnrollmentActivatedTransformer,
     EnrollmentDeactivatedTransformer,
 )
+from event_routing_backends.processors.xapi.event_transformers.forum_events import (
+    ThreadCreatedTransformer,
+    ThreadDeletedTransformer,
+    ThreadEditedTransformer,
+    ThreadViewedTransformer,
+    ThreadVotedTransformer,
+)
 from event_routing_backends.processors.xapi.event_transformers.navigation_events import (
     LinkClickedTransformer,
     OutlineSelectedTransformer,
     TabNavigationTransformer,
 )
 from event_routing_backends.processors.xapi.event_transformers.problem_interaction_events import (
     ProblemCheckTransformer,
```

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/enrollment_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/navigation_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/navigation_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/problem_interaction_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/event_transformers/video_events.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/event_transformers/video_events.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/tests/test_transformers.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/tests/test_xapi.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/transformer.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/transformer.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/processors/xapi/transformer_processor.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/processors/xapi/transformer_processor.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/settings/common.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/settings/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,19 @@
                     {
                         'ENGINE': 'eventtracking.processors.whitelist.NameWhitelistProcessor',
                         'OPTIONS': {
                                 'whitelist': [
                                     'edx.course.enrollment.activated',
                                     'edx.course.enrollment.deactivated',
                                     'edx.course.enrollment.mode_changed',
+                                    'edx.forum.thread.created',
+                                    'edx.forum.thread.deleted',
+                                    'edx.forum.thread.edited',
+                                    'edx.forum.thread.viewed',
+                                    'edx.forum.thread.voted',
                                     'edx.ui.lms.link_clicked',
                                     'edx.ui.lms.sequence.outline.selected',
                                     'edx.ui.lms.outline.selected',
                                     'edx.ui.lms.sequence.next_selected',
                                     'edx.ui.lms.sequence.previous_selected',
                                     'edx.ui.lms.sequence.tab_selected',
                                     'showanswer',
```

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/settings/production.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/settings/production.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js` & `edx-event-routing-backends-5.5.2/event_routing_backends/static/admin/js/EventRoutingBankendsConditionalFieldRenderer.js`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/tasks.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/tests/factories.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/tests/factories.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_helpers.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_mixin.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_models.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/tests/test_settings.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/utils/http_client.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/event_routing_backends/utils/xapi_lrs_client.py` & `edx-event-routing-backends-5.5.2/event_routing_backends/utils/xapi_lrs_client.py`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/requirements/constraints.txt` & `edx-event-routing-backends-5.5.2/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-event-routing-backends-5.5.0/setup.py` & `edx-event-routing-backends-5.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     license="AGPL 3.0",
     zip_safe=False,
     keywords='Python edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
-        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
```

