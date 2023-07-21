# Comparing `tmp/rasa-3.7.0b1.tar.gz` & `tmp/rasa-3.7.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa-3.7.0b1.tar", max compression
+gzip compressed data, was "rasa-3.7.0b2.tar", max compression
```

## Comparing `rasa-3.7.0b1.tar` & `rasa-3.7.0b2.tar`

### file list

```diff
@@ -1,317 +1,317 @@
--rw-r--r--   0        0        0    11352 2023-07-06 19:05:30.052939 rasa-3.7.0b1/LICENSE.txt
--rw-r--r--   0        0        0    21489 2023-07-06 19:05:30.052939 rasa-3.7.0b1/README.md
--rw-r--r--   0        0        0     9566 2023-07-06 19:05:30.284940 rasa-3.7.0b1/pyproject.toml
--rw-r--r--   0        0        0      280 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/__init__.py
--rw-r--r--   0        0        0     5441 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/__main__.py
--rw-r--r--   0        0        0     5314 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/api.py
--rw-r--r--   0        0        0      115 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/__init__.py
--rw-r--r--   0        0        0     2388 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/data.py
--rw-r--r--   0        0        0     5242 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/default_arguments.py
--rw-r--r--   0        0        0     2199 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/evaluate.py
--rw-r--r--   0        0        0     1499 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/export.py
--rw-r--r--   0        0        0     2685 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/interactive.py
--rw-r--r--   0        0        0     5674 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/run.py
--rw-r--r--   0        0        0      367 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/shell.py
--rw-r--r--   0        0        0     6853 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/test.py
--rw-r--r--   0        0        0     8279 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/train.py
--rw-r--r--   0        0        0      861 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/visualize.py
--rw-r--r--   0        0        0     1027 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/arguments/x.py
--rw-r--r--   0        0        0     9722 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/data.py
--rw-r--r--   0        0        0     7948 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/evaluate.py
--rw-r--r--   0        0        0     8204 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/export.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/actions/__init__.py
--rw-r--r--   0        0        0      742 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/actions/actions.py
--rw-r--r--   0        0        0     1505 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/config.yml
--rw-r--r--   0        0        0      998 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/credentials.yml
--rw-r--r--   0        0        0     1433 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/data/nlu.yml
--rw-r--r--   0        0        0      244 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/data/rules.yml
--rw-r--r--   0        0        0      542 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/data/stories.yml
--rw-r--r--   0        0        0      565 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/domain.yml
--rw-r--r--   0        0        0     1411 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/endpoints.yml
--rw-r--r--   0        0        0     1664 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/initial_project/tests/test_stories.yml
--rw-r--r--   0        0        0     5943 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/interactive.py
--rw-r--r--   0        0        0     4196 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/run.py
--rw-r--r--   0        0        0     6846 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/scaffold.py
--rw-r--r--   0        0        0     4264 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/shell.py
--rw-r--r--   0        0        0     3118 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/telemetry.py
--rw-r--r--   0        0        0     8888 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/test.py
--rw-r--r--   0        0        0     7798 2023-07-06 19:05:30.284940 rasa-3.7.0b1/rasa/cli/train.py
--rw-r--r--   0        0        0    12508 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/cli/utils.py
--rw-r--r--   0        0        0     1256 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/cli/visualize.py
--rw-r--r--   0        0        0     6785 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/cli/x.py
--rw-r--r--   0        0        0     1172 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/constants.py
--rw-r--r--   0        0        0      123 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/__init__.py
--rw-r--r--   0        0        0    48450 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/action.py
--rw-r--r--   0        0        0       78 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/constants.py
--rw-r--r--   0        0        0    26651 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/forms.py
--rw-r--r--   0        0        0     3401 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/loops.py
--rw-r--r--   0        0        0     6078 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/actions/two_stage_fallback.py
--rw-r--r--   0        0        0    20445 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/agent.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/__init__.py
--rw-r--r--   0        0        0     4398 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/broker.py
--rw-r--r--   0        0        0     1801 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/file.py
--rw-r--r--   0        0        0    12002 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/kafka.py
--rw-r--r--   0        0        0    14160 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/pika.py
--rw-r--r--   0        0        0     2754 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/brokers/sql.py
--rw-r--r--   0        0        0     1656 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/__init__.py
--rw-r--r--   0        0        0    11669 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/botframework.py
--rw-r--r--   0        0        0     2746 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/callback.py
--rw-r--r--   0        0        0    13331 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/channel.py
--rw-r--r--   0        0        0     8073 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/console.py
--rw-r--r--   0        0        0    15812 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/facebook.py
--rw-r--r--   0        0        0    11560 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/hangouts.py
--rw-r--r--   0        0        0     7743 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/mattermost.py
--rw-r--r--   0        0        0     4814 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/rasa_chat.py
--rw-r--r--   0        0        0     6949 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/rest.py
--rw-r--r--   0        0        0     5999 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/rocketchat.py
--rw-r--r--   0        0        0    24405 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/slack.py
--rw-r--r--   0        0        0    10163 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/socketio.py
--rw-r--r--   0        0        0    10630 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/telegram.py
--rw-r--r--   0        0        0     5938 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/twilio.py
--rw-r--r--   0        0        0    13181 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/twilio_voice.py
--rw-r--r--   0        0        0     4845 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/channels/webexteams.py
--rw-r--r--   0        0        0     3047 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/constants.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/__init__.py
--rw-r--r--   0        0        0     9154 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker.py
--rw-r--r--   0        0        0    38043 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker_base.py
--rw-r--r--   0        0        0    12086 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker_stats.py
--rw-r--r--   0        0        0     3658 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/evaluation/marker_tracker_loader.py
--rw-r--r--   0        0        0      901 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/exceptions.py
--rw-r--r--   0        0        0    10220 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/exporter.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/featurizers/__init__.py
--rw-r--r--   0        0        0    17964 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/featurizers/precomputation.py
--rw-r--r--   0        0        0    15447 2023-07-06 19:05:30.288940 rasa-3.7.0b1/rasa/core/featurizers/single_state_featurizer.py
--rw-r--r--   0        0        0    43363 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/featurizers/tracker_featurizers.py
--rw-r--r--   0        0        0     3024 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/http_interpreter.py
--rw-r--r--   0        0        0     2018 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/jobs.py
--rw-r--r--   0        0        0     4719 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/lock.py
--rw-r--r--   0        0        0    11678 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/lock_store.py
--rw-r--r--   0        0        0    14821 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/migrate.py
--rw-r--r--   0        0        0      240 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/__init__.py
--rw-r--r--   0        0        0     3870 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/callback.py
--rw-r--r--   0        0        0     3285 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/generator.py
--rw-r--r--   0        0        0     2635 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/interpolator.py
--rw-r--r--   0        0        0     7503 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/nlg/response.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/__init__.py
--rw-r--r--   0        0        0    12959 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/ensemble.py
--rw-r--r--   0        0        0    19295 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/memoization.py
--rw-r--r--   0        0        0    25038 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/policy.py
--rw-r--r--   0        0        0    50315 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/rule_policy.py
--rw-r--r--   0        0        0    86521 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/ted_policy.py
--rw-r--r--   0        0        0    39329 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/policies/unexpected_intent_policy.py
--rw-r--r--   0        0        0    41906 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/processor.py
--rw-r--r--   0        0        0     9243 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/run.py
--rw-r--r--   0        0        0    48935 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/test.py
--rw-r--r--   0        0        0    58040 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/tracker_store.py
--rw-r--r--   0        0        0     3543 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/train.py
--rw-r--r--   0        0        0     3218 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/converters/__init__.py
--rw-r--r--   0        0        0     3889 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/converters/responses_prefix_converter.py
--rw-r--r--   0        0        0    59595 2023-07-06 19:05:30.292940 rasa-3.7.0b1/rasa/core/training/interactive.py
--rw-r--r--   0        0        0    13604 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/training/story_conflict.py
--rw-r--r--   0        0        0     3067 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/training/training.py
--rw-r--r--   0        0        0    10995 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/utils.py
--rw-r--r--   0        0        0     2125 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/core/visualize.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/__init__.py
--rw-r--r--   0        0        0    16744 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/caching.py
--rw-r--r--   0        0        0      469 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/constants.py
--rw-r--r--   0        0        0      437 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/exceptions.py
--rw-r--r--   0        0        0    22105 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/graph.py
--rw-r--r--   0        0        0     1384 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/loader.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/__init__.py
--rw-r--r--   0        0        0     1139 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/config_files/default_config.yml
--rw-r--r--   0        0        0     3244 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/default_components.py
--rw-r--r--   0        0        0    43587 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/default_recipe.py
--rw-r--r--   0        0        0     3301 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/graph_recipe.py
--rw-r--r--   0        0        0     3354 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/recipes/recipe.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/runner/__init__.py
--rw-r--r--   0        0        0     4302 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/runner/dask.py
--rw-r--r--   0        0        0     1672 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/runner/interface.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/__init__.py
--rw-r--r--   0        0        0     9581 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/local_model_storage.py
--rw-r--r--   0        0        0     3931 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/resource.py
--rw-r--r--   0        0        0     6923 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/storage/storage.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/__init__.py
--rw-r--r--   0        0        0     6524 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/components.py
--rw-r--r--   0        0        0     1848 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/fingerprinting.py
--rw-r--r--   0        0        0    10516 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/graph_trainer.py
--rw-r--r--   0        0        0     5036 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/training/hooks.py
--rw-r--r--   0        0        0    22697 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/engine/validation.py
--rw-r--r--   0        0        0     2132 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/converters/__init__.py
--rw-r--r--   0        0        0     1576 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/converters/nlu_message_converter.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/__init__.py
--rw-r--r--   0        0        0     3832 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/domain_for_core_training_provider.py
--rw-r--r--   0        0        0     2571 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/domain_provider.py
--rw-r--r--   0        0        0     1294 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/forms_provider.py
--rw-r--r--   0        0        0     2119 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/nlu_training_data_provider.py
--rw-r--r--   0        0        0     1354 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/responses_provider.py
--rw-r--r--   0        0        0     1540 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/rule_only_provider.py
--rw-r--r--   0        0        0     1466 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/story_graph_provider.py
--rw-r--r--   0        0        0     1965 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/providers/training_tracker_provider.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/validators/__init__.py
--rw-r--r--   0        0        0    22668 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/validators/default_recipe_validator.py
--rw-r--r--   0        0        0    12863 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/graph_components/validators/finetuning_validator.py
--rw-r--r--   0        0        0     1782 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/jupyter.py
--rw-r--r--   0        0        0      101 2023-07-06 19:05:53.169073 rasa-3.7.0b1/rasa/keys
--rw-r--r--   0        0        0     3490 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/model.py
--rw-r--r--   0        0        0    14961 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/model_testing.py
--rw-r--r--   0        0        0    16836 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/model_training.py
--rw-r--r--   0        0        0      123 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/nlu/__init__.py
--rw-r--r--   0        0        0      118 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/nlu/classifiers/__init__.py
--rw-r--r--   0        0        0      133 2023-07-06 19:05:30.296940 rasa-3.7.0b1/rasa/nlu/classifiers/classifier.py
--rw-r--r--   0        0        0    71637 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/diet_classifier.py
--rw-r--r--   0        0        0     7150 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/fallback_classifier.py
--rw-r--r--   0        0        0     7581 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/keyword_intent_classifier.py
--rw-r--r--   0        0        0     7568 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/logistic_regression_classifier.py
--rw-r--r--   0        0        0     5559 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/mitie_intent_classifier.py
--rw-r--r--   0        0        0     1989 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/regex_message_handler.py
--rw-r--r--   0        0        0    11915 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/classifiers/sklearn_intent_classifier.py
--rw-r--r--   0        0        0     2757 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/constants.py
--rw-r--r--   0        0        0     1317 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/convert.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/__init__.py
--rw-r--r--   0        0        0     1748 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/dialogflow.py
--rw-r--r--   0        0        0     1367 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/emulator.py
--rw-r--r--   0        0        0     3032 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/luis.py
--rw-r--r--   0        0        0      334 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/no_emulator.py
--rw-r--r--   0        0        0     1930 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/emulators/wit.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/__init__.py
--rw-r--r--   0        0        0    26499 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/crf_entity_extractor.py
--rw-r--r--   0        0        0     7685 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/duckling_entity_extractor.py
--rw-r--r--   0        0        0     7160 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/entity_synonyms.py
--rw-r--r--   0        0        0    17530 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/extractor.py
--rw-r--r--   0        0        0    10973 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/mitie_entity_extractor.py
--rw-r--r--   0        0        0     8289 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/regex_entity_extractor.py
--rw-r--r--   0        0        0     3366 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/extractors/spacy_entity_extractor.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/__init__.py
--rw-r--r--   0        0        0    17142 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
--rw-r--r--   0        0        0     2433 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
--rw-r--r--   0        0        0    30361 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
--rw-r--r--   0        0        0     5861 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
--rw-r--r--   0        0        0     4888 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
--rw-r--r--   0        0        0     3347 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/featurizer.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/__init__.py
--rw-r--r--   0        0        0    33295 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
--rw-r--r--   0        0        0    21810 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
--rw-r--r--   0        0        0    10289 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
--rw-r--r--   0        0        0      220 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
--rw-r--r--   0        0        0      557 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/model.py
--rw-r--r--   0        0        0     8333 2023-07-06 19:05:30.300940 rasa-3.7.0b1/rasa/nlu/persistor.py
--rw-r--r--   0        0        0      803 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/run.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/selectors/__init__.py
--rw-r--r--   0        0        0    39012 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/selectors/response_selector.py
--rw-r--r--   0        0        0    67726 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/test.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/__init__.py
--rw-r--r--   0        0        0     5374 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/jieba_tokenizer.py
--rw-r--r--   0        0        0     2618 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/mitie_tokenizer.py
--rw-r--r--   0        0        0     2378 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/spacy_tokenizer.py
--rw-r--r--   0        0        0     8196 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     3750 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0      928 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/__init__.py
--rw-r--r--   0        0        0    14703 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/bilou_utils.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/hugging_face/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/hugging_face/registry.py
--rw-r--r--   0        0        0     9143 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
--rw-r--r--   0        0        0     3887 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/mitie_utils.py
--rw-r--r--   0        0        0     5386 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/pattern_utils.py
--rw-r--r--   0        0        0    11795 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/nlu/utils/spacy_utils.py
--rw-r--r--   0        0        0     4921 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/plugin.py
--rw-r--r--   0        0        0    55589 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/server.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/__init__.py
--rw-r--r--   0        0        0     4337 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/constants.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/__init__.py
--rw-r--r--   0        0        0     4416 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/constants.py
--rw-r--r--   0        0        0     1366 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/conversation.py
--rw-r--r--   0        0        0    77445 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/domain.py
--rw-r--r--   0        0        0    66276 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/events.py
--rw-r--r--   0        0        0    35597 2023-07-06 19:05:30.304941 rasa-3.7.0b1/rasa/shared/core/generator.py
--rw-r--r--   0        0        0     8286 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/slot_mappings.py
--rw-r--r--   0        0        0    16371 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/slots.py
--rw-r--r--   0        0        0    34744 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/trackers.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/__init__.py
--rw-r--r--   0        0        0     2895 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/loading.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/__init__.py
--rw-r--r--   0        0        0     4449 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_reader.py
--rw-r--r--   0        0        0     6671 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_step_builder.py
--rw-r--r--   0        0        0    32976 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/__init__.py
--rw-r--r--   0        0        0     2543 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/story_writer.py
--rw-r--r--   0        0        0    14903 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
--rw-r--r--   0        0        0    29313 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/structures.py
--rw-r--r--   0        0        0     3500 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/visualization.html
--rw-r--r--   0        0        0    20341 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/core/training_data/visualization.py
--rw-r--r--   0        0        0     5479 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/data.py
--rw-r--r--   0        0        0     3633 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/__init__.py
--rw-r--r--   0        0        0    21866 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/importer.py
--rw-r--r--   0        0        0     7836 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/multi_project.py
--rw-r--r--   0        0        0     3388 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/rasa.py
--rw-r--r--   0        0        0      861 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/importers/utils.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/__init__.py
--rw-r--r--   0        0        0     1388 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/constants.py
--rw-r--r--   0        0        0      188 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/interpreter.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/__init__.py
--rw-r--r--   0        0        0     6759 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/entities_parser.py
--rw-r--r--   0        0        0    14835 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/features.py
--rw-r--r--   0        0        0      453 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/__init__.py
--rw-r--r--   0        0        0     6123 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/dialogflow.py
--rw-r--r--   0        0        0     3014 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/luis.py
--rw-r--r--   0        0        0     4495 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa.py
--rw-r--r--   0        0        0    22353 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa_yaml.py
--rw-r--r--   0        0        0     8540 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/readerwriter.py
--rw-r--r--   0        0        0     1820 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/wit.py
--rw-r--r--   0        0        0     4258 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/loading.py
--rw-r--r--   0        0        0     1116 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/lookup_tables_parser.py
--rw-r--r--   0        0        0    16662 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/message.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/__init__.py
--rw-r--r--   0        0        0     2565 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/data_schema.py
--rw-r--r--   0        0        0     1179 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/nlu.yml
--rw-r--r--   0        0        0     1661 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/responses.yml
--rw-r--r--   0        0        0     1476 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/synonyms_parser.py
--rw-r--r--   0        0        0    28493 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/training_data.py
--rw-r--r--   0        0        0     7040 2023-07-06 19:05:30.308941 rasa-3.7.0b1/rasa/shared/nlu/training_data/util.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/__init__.py
--rw-r--r--   0        0        0     2078 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/cli.py
--rw-r--r--   0        0        0     8731 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/common.py
--rw-r--r--   0        0        0    20533 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/io.py
--rw-r--r--   0        0        0      883 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/pykwalify_extensions.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/__init__.py
--rw-r--r--   0        0        0       27 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/config.yml
--rw-r--r--   0        0        0     3267 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/domain.yml
--rw-r--r--   0        0        0     5569 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/events.py
--rw-r--r--   0        0        0      998 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/model_config.yml
--rw-r--r--   0        0        0     4034 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/schemas/stories.yml
--rw-r--r--   0        0        0    10317 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/shared/utils/validation.py
--rw-r--r--   0        0        0    36273 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/telemetry.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/__init__.py
--rw-r--r--   0        0        0    19532 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/common.py
--rw-r--r--   0        0        0     1647 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/converter.py
--rw-r--r--   0        0        0     8796 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/endpoints.py
--rw-r--r--   0        0        0     7831 2023-07-06 19:05:30.312940 rasa-3.7.0b1/rasa/utils/io.py
--rw-r--r--   0        0        0     2018 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/llm.py
--rw-r--r--   0        0        0     4482 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/log_utils.py
--rw-r--r--   0        0        0    12246 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/plotting.py
--rw-r--r--   0        0        0        0 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/__init__.py
--rw-r--r--   0        0        0     4036 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/callback.py
--rw-r--r--   0        0        0     3140 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/constants.py
--rw-r--r--   0        0        0    19658 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/crf.py
--rw-r--r--   0        0        0    15526 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/data_generator.py
--rw-r--r--   0        0        0     5576 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/environment.py
--rw-r--r--   0        0        0      168 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/exceptions.py
--rw-r--r--   0        0        0    59263 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/layers.py
--rw-r--r--   0        0        0     3319 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/layers_utils.py
--rw-r--r--   0        0        0    10055 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/metrics.py
--rw-r--r--   0        0        0    34572 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/model_data.py
--rw-r--r--   0        0        0    18667 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/model_data_utils.py
--rw-r--r--   0        0        0    36004 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/models.py
--rw-r--r--   0        0        0    49066 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/rasa_layers.py
--rw-r--r--   0        0        0    25509 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/transformer.py
--rw-r--r--   0        0        0      204 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/tensorflow/types.py
--rw-r--r--   0        0        0    20999 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/utils/train_utils.py
--rw-r--r--   0        0        0    17708 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/validator.py
--rw-r--r--   0        0        0      118 2023-07-06 19:05:30.316941 rasa-3.7.0b1/rasa/version.py
--rw-r--r--   0        0        0    28128 1970-01-01 00:00:00.000000 rasa-3.7.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11352 2023-07-20 16:16:53.899925 rasa-3.7.0b2/LICENSE.txt
+-rw-r--r--   0        0        0    21519 2023-07-20 16:16:53.899925 rasa-3.7.0b2/README.md
+-rw-r--r--   0        0        0     9559 2023-07-20 16:16:54.075926 rasa-3.7.0b2/pyproject.toml
+-rw-r--r--   0        0        0      280 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/__init__.py
+-rw-r--r--   0        0        0     5441 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/__main__.py
+-rw-r--r--   0        0        0     5314 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/api.py
+-rw-r--r--   0        0        0      115 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/__init__.py
+-rw-r--r--   0        0        0     2388 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/data.py
+-rw-r--r--   0        0        0     5242 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/default_arguments.py
+-rw-r--r--   0        0        0     2199 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/evaluate.py
+-rw-r--r--   0        0        0     1499 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/export.py
+-rw-r--r--   0        0        0     2685 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/interactive.py
+-rw-r--r--   0        0        0     5674 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/run.py
+-rw-r--r--   0        0        0      367 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/shell.py
+-rw-r--r--   0        0        0     6853 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/test.py
+-rw-r--r--   0        0        0     8279 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/train.py
+-rw-r--r--   0        0        0      861 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/visualize.py
+-rw-r--r--   0        0        0     1027 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/arguments/x.py
+-rw-r--r--   0        0        0     9722 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/data.py
+-rw-r--r--   0        0        0     7948 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/evaluate.py
+-rw-r--r--   0        0        0     8204 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/export.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/actions/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/actions/actions.py
+-rw-r--r--   0        0        0     1505 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/config.yml
+-rw-r--r--   0        0        0      998 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/credentials.yml
+-rw-r--r--   0        0        0     1433 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/data/nlu.yml
+-rw-r--r--   0        0        0      244 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/data/rules.yml
+-rw-r--r--   0        0        0      542 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/data/stories.yml
+-rw-r--r--   0        0        0      565 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/domain.yml
+-rw-r--r--   0        0        0     1411 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/endpoints.yml
+-rw-r--r--   0        0        0     1664 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/initial_project/tests/test_stories.yml
+-rw-r--r--   0        0        0     5943 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/interactive.py
+-rw-r--r--   0        0        0     4196 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/run.py
+-rw-r--r--   0        0        0     6846 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/scaffold.py
+-rw-r--r--   0        0        0     4264 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/shell.py
+-rw-r--r--   0        0        0     3118 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/telemetry.py
+-rw-r--r--   0        0        0     8888 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/test.py
+-rw-r--r--   0        0        0     7798 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/train.py
+-rw-r--r--   0        0        0    12508 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/utils.py
+-rw-r--r--   0        0        0     1256 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/visualize.py
+-rw-r--r--   0        0        0     6785 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/cli/x.py
+-rw-r--r--   0        0        0     1172 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/constants.py
+-rw-r--r--   0        0        0      123 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/actions/__init__.py
+-rw-r--r--   0        0        0    48450 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/actions/action.py
+-rw-r--r--   0        0        0       78 2023-07-20 16:16:54.075926 rasa-3.7.0b2/rasa/core/actions/constants.py
+-rw-r--r--   0        0        0    26679 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/actions/forms.py
+-rw-r--r--   0        0        0     3401 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/actions/loops.py
+-rw-r--r--   0        0        0     6078 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/actions/two_stage_fallback.py
+-rw-r--r--   0        0        0    20445 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/agent.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/__init__.py
+-rw-r--r--   0        0        0     4398 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/broker.py
+-rw-r--r--   0        0        0     1801 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/file.py
+-rw-r--r--   0        0        0    12002 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/kafka.py
+-rw-r--r--   0        0        0    14160 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/pika.py
+-rw-r--r--   0        0        0     2754 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/brokers/sql.py
+-rw-r--r--   0        0        0     1656 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/__init__.py
+-rw-r--r--   0        0        0    11669 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/botframework.py
+-rw-r--r--   0        0        0     2746 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/callback.py
+-rw-r--r--   0        0        0    13331 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/channel.py
+-rw-r--r--   0        0        0     8073 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/console.py
+-rw-r--r--   0        0        0    15819 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/facebook.py
+-rw-r--r--   0        0        0    11568 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/hangouts.py
+-rw-r--r--   0        0        0     7743 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/mattermost.py
+-rw-r--r--   0        0        0     4814 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/rasa_chat.py
+-rw-r--r--   0        0        0     6957 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/rest.py
+-rw-r--r--   0        0        0     5999 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/rocketchat.py
+-rw-r--r--   0        0        0    24405 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/slack.py
+-rw-r--r--   0        0        0    10163 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/socketio.py
+-rw-r--r--   0        0        0    10630 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/telegram.py
+-rw-r--r--   0        0        0     5938 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/twilio.py
+-rw-r--r--   0        0        0    13181 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/twilio_voice.py
+-rw-r--r--   0        0        0     4845 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/channels/webexteams.py
+-rw-r--r--   0        0        0     3047 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/constants.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/__init__.py
+-rw-r--r--   0        0        0     9154 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker.py
+-rw-r--r--   0        0        0    38043 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker_base.py
+-rw-r--r--   0        0        0    12086 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker_stats.py
+-rw-r--r--   0        0        0     3658 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/evaluation/marker_tracker_loader.py
+-rw-r--r--   0        0        0      901 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/exceptions.py
+-rw-r--r--   0        0        0    10220 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/exporter.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/__init__.py
+-rw-r--r--   0        0        0    17964 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/precomputation.py
+-rw-r--r--   0        0        0    15447 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/single_state_featurizer.py
+-rw-r--r--   0        0        0    43363 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/featurizers/tracker_featurizers.py
+-rw-r--r--   0        0        0     3084 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/http_interpreter.py
+-rw-r--r--   0        0        0     2018 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/jobs.py
+-rw-r--r--   0        0        0     4719 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/lock.py
+-rw-r--r--   0        0        0    11678 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/lock_store.py
+-rw-r--r--   0        0        0    14821 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/migrate.py
+-rw-r--r--   0        0        0      240 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/__init__.py
+-rw-r--r--   0        0        0     3870 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/callback.py
+-rw-r--r--   0        0        0     3285 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/generator.py
+-rw-r--r--   0        0        0     2897 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/interpolator.py
+-rw-r--r--   0        0        0     7503 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/nlg/response.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/__init__.py
+-rw-r--r--   0        0        0    12959 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/ensemble.py
+-rw-r--r--   0        0        0    19295 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/memoization.py
+-rw-r--r--   0        0        0    25038 2023-07-20 16:16:54.079926 rasa-3.7.0b2/rasa/core/policies/policy.py
+-rw-r--r--   0        0        0    50315 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/policies/rule_policy.py
+-rw-r--r--   0        0        0    86521 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/policies/ted_policy.py
+-rw-r--r--   0        0        0    39329 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/policies/unexpected_intent_policy.py
+-rw-r--r--   0        0        0    41906 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/processor.py
+-rw-r--r--   0        0        0     9243 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/run.py
+-rw-r--r--   0        0        0    48935 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/test.py
+-rw-r--r--   0        0        0    58040 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/tracker_store.py
+-rw-r--r--   0        0        0     3543 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/train.py
+-rw-r--r--   0        0        0     3218 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/converters/__init__.py
+-rw-r--r--   0        0        0     3889 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/converters/responses_prefix_converter.py
+-rw-r--r--   0        0        0    59595 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/interactive.py
+-rw-r--r--   0        0        0    13604 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/story_conflict.py
+-rw-r--r--   0        0        0     3067 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/training/training.py
+-rw-r--r--   0        0        0    10995 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/utils.py
+-rw-r--r--   0        0        0     2125 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/core/visualize.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/__init__.py
+-rw-r--r--   0        0        0    16744 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/caching.py
+-rw-r--r--   0        0        0      469 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/constants.py
+-rw-r--r--   0        0        0      437 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/exceptions.py
+-rw-r--r--   0        0        0    22105 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/graph.py
+-rw-r--r--   0        0        0     1384 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/loader.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/__init__.py
+-rw-r--r--   0        0        0     1139 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/config_files/default_config.yml
+-rw-r--r--   0        0        0     3244 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/default_components.py
+-rw-r--r--   0        0        0    43587 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/default_recipe.py
+-rw-r--r--   0        0        0     3301 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/graph_recipe.py
+-rw-r--r--   0        0        0     3354 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/recipes/recipe.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/runner/__init__.py
+-rw-r--r--   0        0        0     4302 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/runner/dask.py
+-rw-r--r--   0        0        0     1672 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/runner/interface.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/__init__.py
+-rw-r--r--   0        0        0     9581 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/local_model_storage.py
+-rw-r--r--   0        0        0     3931 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/resource.py
+-rw-r--r--   0        0        0     6923 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/storage/storage.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/__init__.py
+-rw-r--r--   0        0        0     6524 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/components.py
+-rw-r--r--   0        0        0     1848 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/fingerprinting.py
+-rw-r--r--   0        0        0    10516 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/graph_trainer.py
+-rw-r--r--   0        0        0     5036 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/training/hooks.py
+-rw-r--r--   0        0        0    22697 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/engine/validation.py
+-rw-r--r--   0        0        0     2132 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/converters/__init__.py
+-rw-r--r--   0        0        0     1576 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/converters/nlu_message_converter.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.083926 rasa-3.7.0b2/rasa/graph_components/providers/__init__.py
+-rw-r--r--   0        0        0     3832 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/domain_for_core_training_provider.py
+-rw-r--r--   0        0        0     2571 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/domain_provider.py
+-rw-r--r--   0        0        0     1294 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/forms_provider.py
+-rw-r--r--   0        0        0     2119 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/nlu_training_data_provider.py
+-rw-r--r--   0        0        0     1354 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/responses_provider.py
+-rw-r--r--   0        0        0     1540 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/rule_only_provider.py
+-rw-r--r--   0        0        0     1466 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/story_graph_provider.py
+-rw-r--r--   0        0        0     1965 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/providers/training_tracker_provider.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/validators/__init__.py
+-rw-r--r--   0        0        0    22668 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/validators/default_recipe_validator.py
+-rw-r--r--   0        0        0    12863 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/graph_components/validators/finetuning_validator.py
+-rw-r--r--   0        0        0     1782 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/jupyter.py
+-rw-r--r--   0        0        0      101 2023-07-20 16:17:14.656082 rasa-3.7.0b2/rasa/keys
+-rw-r--r--   0        0        0     3490 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/model.py
+-rw-r--r--   0        0        0    14961 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/model_testing.py
+-rw-r--r--   0        0        0    16836 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/model_training.py
+-rw-r--r--   0        0        0      123 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/__init__.py
+-rw-r--r--   0        0        0      118 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/__init__.py
+-rw-r--r--   0        0        0      133 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/classifier.py
+-rw-r--r--   0        0        0    71637 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/diet_classifier.py
+-rw-r--r--   0        0        0     7150 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/fallback_classifier.py
+-rw-r--r--   0        0        0     7581 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/keyword_intent_classifier.py
+-rw-r--r--   0        0        0     7568 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/logistic_regression_classifier.py
+-rw-r--r--   0        0        0     5559 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/mitie_intent_classifier.py
+-rw-r--r--   0        0        0     1989 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/regex_message_handler.py
+-rw-r--r--   0        0        0    11915 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/classifiers/sklearn_intent_classifier.py
+-rw-r--r--   0        0        0     2757 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/constants.py
+-rw-r--r--   0        0        0     1317 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/convert.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/__init__.py
+-rw-r--r--   0        0        0     1748 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/dialogflow.py
+-rw-r--r--   0        0        0     1367 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/emulator.py
+-rw-r--r--   0        0        0     3032 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/luis.py
+-rw-r--r--   0        0        0      334 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/no_emulator.py
+-rw-r--r--   0        0        0     1930 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/emulators/wit.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/__init__.py
+-rw-r--r--   0        0        0    26499 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/crf_entity_extractor.py
+-rw-r--r--   0        0        0     7685 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/duckling_entity_extractor.py
+-rw-r--r--   0        0        0     7160 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/entity_synonyms.py
+-rw-r--r--   0        0        0    17530 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/extractor.py
+-rw-r--r--   0        0        0    10973 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/mitie_entity_extractor.py
+-rw-r--r--   0        0        0     8289 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/regex_entity_extractor.py
+-rw-r--r--   0        0        0     3366 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/extractors/spacy_entity_extractor.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/__init__.py
+-rw-r--r--   0        0        0    17142 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py
+-rw-r--r--   0        0        0     2433 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py
+-rw-r--r--   0        0        0    30361 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py
+-rw-r--r--   0        0        0     5861 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py
+-rw-r--r--   0        0        0     4888 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py
+-rw-r--r--   0        0        0     3347 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/featurizer.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/__init__.py
+-rw-r--r--   0        0        0    33295 2023-07-20 16:16:54.087926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py
+-rw-r--r--   0        0        0    21810 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py
+-rw-r--r--   0        0        0    10289 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py
+-rw-r--r--   0        0        0      220 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/sparse_featurizer.py
+-rw-r--r--   0        0        0      557 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/model.py
+-rw-r--r--   0        0        0     8333 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/persistor.py
+-rw-r--r--   0        0        0      803 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/run.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/selectors/__init__.py
+-rw-r--r--   0        0        0    39012 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/selectors/response_selector.py
+-rw-r--r--   0        0        0    67726 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/test.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/__init__.py
+-rw-r--r--   0        0        0     5374 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/jieba_tokenizer.py
+-rw-r--r--   0        0        0     2618 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/mitie_tokenizer.py
+-rw-r--r--   0        0        0     2378 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/spacy_tokenizer.py
+-rw-r--r--   0        0        0     8196 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     3750 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      928 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/__init__.py
+-rw-r--r--   0        0        0    14703 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/bilou_utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/hugging_face/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/hugging_face/registry.py
+-rw-r--r--   0        0        0     9143 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py
+-rw-r--r--   0        0        0     3887 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/mitie_utils.py
+-rw-r--r--   0        0        0     5386 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/pattern_utils.py
+-rw-r--r--   0        0        0    11795 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/nlu/utils/spacy_utils.py
+-rw-r--r--   0        0        0     4921 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/plugin.py
+-rw-r--r--   0        0        0    55589 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/server.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/__init__.py
+-rw-r--r--   0        0        0     4337 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/constants.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/__init__.py
+-rw-r--r--   0        0        0     4416 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/constants.py
+-rw-r--r--   0        0        0     1366 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/conversation.py
+-rw-r--r--   0        0        0    77445 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/domain.py
+-rw-r--r--   0        0        0    66276 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/events.py
+-rw-r--r--   0        0        0    35597 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/generator.py
+-rw-r--r--   0        0        0     8286 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/slot_mappings.py
+-rw-r--r--   0        0        0    16371 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/slots.py
+-rw-r--r--   0        0        0    34744 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/trackers.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/__init__.py
+-rw-r--r--   0        0        0     2895 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/loading.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/__init__.py
+-rw-r--r--   0        0        0     4449 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_reader.py
+-rw-r--r--   0        0        0     6671 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_step_builder.py
+-rw-r--r--   0        0        0    32976 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/yaml_story_reader.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/__init__.py
+-rw-r--r--   0        0        0     2543 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/story_writer.py
+-rw-r--r--   0        0        0    14903 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/yaml_story_writer.py
+-rw-r--r--   0        0        0    29313 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/structures.py
+-rw-r--r--   0        0        0     3500 2023-07-20 16:16:54.091926 rasa-3.7.0b2/rasa/shared/core/training_data/visualization.html
+-rw-r--r--   0        0        0    20341 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/core/training_data/visualization.py
+-rw-r--r--   0        0        0     5479 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/data.py
+-rw-r--r--   0        0        0     3633 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/__init__.py
+-rw-r--r--   0        0        0    21866 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/importer.py
+-rw-r--r--   0        0        0     7836 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/multi_project.py
+-rw-r--r--   0        0        0     3388 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/rasa.py
+-rw-r--r--   0        0        0      861 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/importers/utils.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/__init__.py
+-rw-r--r--   0        0        0     1388 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/constants.py
+-rw-r--r--   0        0        0      188 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/interpreter.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/__init__.py
+-rw-r--r--   0        0        0     6759 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/entities_parser.py
+-rw-r--r--   0        0        0    14835 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/features.py
+-rw-r--r--   0        0        0      453 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/__init__.py
+-rw-r--r--   0        0        0     6123 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/dialogflow.py
+-rw-r--r--   0        0        0     3014 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/luis.py
+-rw-r--r--   0        0        0     4495 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa.py
+-rw-r--r--   0        0        0    22353 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa_yaml.py
+-rw-r--r--   0        0        0     8540 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/readerwriter.py
+-rw-r--r--   0        0        0     1820 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/wit.py
+-rw-r--r--   0        0        0     4258 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/loading.py
+-rw-r--r--   0        0        0     1116 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/lookup_tables_parser.py
+-rw-r--r--   0        0        0    16662 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/message.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/__init__.py
+-rw-r--r--   0        0        0     2565 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/data_schema.py
+-rw-r--r--   0        0        0     1179 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/nlu.yml
+-rw-r--r--   0        0        0     1661 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/responses.yml
+-rw-r--r--   0        0        0     1476 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/synonyms_parser.py
+-rw-r--r--   0        0        0    28493 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/training_data.py
+-rw-r--r--   0        0        0     7040 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/nlu/training_data/util.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/__init__.py
+-rw-r--r--   0        0        0     2078 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/cli.py
+-rw-r--r--   0        0        0     8731 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/common.py
+-rw-r--r--   0        0        0    20606 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/io.py
+-rw-r--r--   0        0        0      883 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/pykwalify_extensions.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/config.yml
+-rw-r--r--   0        0        0     3267 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/domain.yml
+-rw-r--r--   0        0        0     5569 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/events.py
+-rw-r--r--   0        0        0      998 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/model_config.yml
+-rw-r--r--   0        0        0     4034 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/schemas/stories.yml
+-rw-r--r--   0        0        0    10317 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/shared/utils/validation.py
+-rw-r--r--   0        0        0    36273 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/telemetry.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/__init__.py
+-rw-r--r--   0        0        0    19532 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/common.py
+-rw-r--r--   0        0        0     1647 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/converter.py
+-rw-r--r--   0        0        0     8796 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/endpoints.py
+-rw-r--r--   0        0        0     7831 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/io.py
+-rw-r--r--   0        0        0     2018 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/llm.py
+-rw-r--r--   0        0        0     5036 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/log_utils.py
+-rw-r--r--   0        0        0    12246 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/plotting.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/__init__.py
+-rw-r--r--   0        0        0     4036 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/callback.py
+-rw-r--r--   0        0        0     3140 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/constants.py
+-rw-r--r--   0        0        0    19658 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/crf.py
+-rw-r--r--   0        0        0    15526 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/data_generator.py
+-rw-r--r--   0        0        0     5576 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/environment.py
+-rw-r--r--   0        0        0      168 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/exceptions.py
+-rw-r--r--   0        0        0    59263 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/layers.py
+-rw-r--r--   0        0        0     3319 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/layers_utils.py
+-rw-r--r--   0        0        0    10055 2023-07-20 16:16:54.095926 rasa-3.7.0b2/rasa/utils/tensorflow/metrics.py
+-rw-r--r--   0        0        0    34572 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/model_data.py
+-rw-r--r--   0        0        0    18667 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/model_data_utils.py
+-rw-r--r--   0        0        0    36004 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/models.py
+-rw-r--r--   0        0        0    49066 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/rasa_layers.py
+-rw-r--r--   0        0        0    25509 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/transformer.py
+-rw-r--r--   0        0        0      204 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/tensorflow/types.py
+-rw-r--r--   0        0        0    20999 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/utils/train_utils.py
+-rw-r--r--   0        0        0    17708 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/validator.py
+-rw-r--r--   0        0        0      118 2023-07-20 16:16:54.099926 rasa-3.7.0b2/rasa/version.py
+-rw-r--r--   0        0        0    28151 1970-01-01 00:00:00.000000 rasa-3.7.0b2/PKG-INFO
```

### Comparing `rasa-3.7.0b1/LICENSE.txt` & `rasa-3.7.0b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/README.md` & `rasa-3.7.0b2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <div align="center">
 
 [![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![PyPI version](https://badge.fury.io/py/rasa.svg)](https://badge.fury.io/py/rasa)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/rasa.svg)](https://pypi.python.org/pypi/rasa)
 [![Build Status](https://github.com/RasaHQ/rasa/workflows/Continuous%20Integration/badge.svg)](https://github.com/RasaHQ/rasa/actions)
-[![Coverage Status](https://api.codeclimate.com/v1/badges/756dc6fea1d5d3e127f7/test_coverage)](https://codeclimate.com/github/RasaHQ/rasa/)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=RasaHQ_rasa&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=RasaHQ_rasa)
 [![Documentation Status](https://img.shields.io/badge/docs-stable-brightgreen.svg)](https://rasa.com/docs)
 ![Documentation Build](https://img.shields.io/netlify/d2e447e4-5a5e-4dc7-be5d-7c04ae7ff706?label=Documentation%20Build)
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B8141%2Fgit%40github.com%3ARasaHQ%2Frasa.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B8141%2Fgit%40github.com%3ARasaHQ%2Frasa.git?ref=badge_shield)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/orgs/RasaHQ/projects/23)
 
 </div>
```

### Comparing `rasa-3.7.0b1/pyproject.toml` & `rasa-3.7.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa"
-version = "3.7.0b1"
+version = "3.7.0b2"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
@@ -98,15 +98,15 @@
 apscheduler = ">=3.6,<3.10"
 tqdm = "^4.31"
 networkx = ">=2.4,<2.7"
 fbmessenger = "~6.0.0"
 pykwalify = ">=1.7,<1.9"
 coloredlogs = ">=10,<16"
 "ruamel.yaml" = ">=0.16.5,<0.17.22"
-pyyaml = ">=5.3.1,<6.0"
+pyyaml = ">=6.0"
 twilio = ">=6.26,<8.4"
 webexteamssdk = ">=1.1.1,<1.7.0"
 mattermostwrapper = "~2.2"
 rocketchat_API = ">=0.6.31,<1.31.0"
 colorhash = ">=1.0.2,<1.3.0"
 jsonschema = ">=3.2,<4.18"
 packaging = ">=20.0,<21.0"
```

### Comparing `rasa-3.7.0b1/rasa/__main__.py` & `rasa-3.7.0b2/rasa/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/api.py` & `rasa-3.7.0b2/rasa/api.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/data.py` & `rasa-3.7.0b2/rasa/cli/arguments/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/default_arguments.py` & `rasa-3.7.0b2/rasa/cli/arguments/default_arguments.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/evaluate.py` & `rasa-3.7.0b2/rasa/cli/arguments/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/export.py` & `rasa-3.7.0b2/rasa/cli/arguments/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/interactive.py` & `rasa-3.7.0b2/rasa/cli/arguments/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/run.py` & `rasa-3.7.0b2/rasa/cli/arguments/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/test.py` & `rasa-3.7.0b2/rasa/cli/arguments/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/train.py` & `rasa-3.7.0b2/rasa/cli/arguments/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/visualize.py` & `rasa-3.7.0b2/rasa/cli/arguments/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/arguments/x.py` & `rasa-3.7.0b2/rasa/cli/arguments/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/data.py` & `rasa-3.7.0b2/rasa/cli/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/evaluate.py` & `rasa-3.7.0b2/rasa/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/export.py` & `rasa-3.7.0b2/rasa/cli/export.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/actions/actions.py` & `rasa-3.7.0b2/rasa/cli/initial_project/actions/actions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/config.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/credentials.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/credentials.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/data/nlu.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/data/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/data/stories.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/data/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/domain.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/endpoints.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/endpoints.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/initial_project/tests/test_stories.yml` & `rasa-3.7.0b2/rasa/cli/initial_project/tests/test_stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/interactive.py` & `rasa-3.7.0b2/rasa/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/run.py` & `rasa-3.7.0b2/rasa/cli/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/scaffold.py` & `rasa-3.7.0b2/rasa/cli/scaffold.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/shell.py` & `rasa-3.7.0b2/rasa/cli/shell.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/telemetry.py` & `rasa-3.7.0b2/rasa/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/test.py` & `rasa-3.7.0b2/rasa/cli/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/train.py` & `rasa-3.7.0b2/rasa/cli/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/utils.py` & `rasa-3.7.0b2/rasa/cli/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/visualize.py` & `rasa-3.7.0b2/rasa/cli/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/cli/x.py` & `rasa-3.7.0b2/rasa/cli/x.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/constants.py` & `rasa-3.7.0b2/rasa/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/actions/action.py` & `rasa-3.7.0b2/rasa/core/actions/action.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/actions/forms.py` & `rasa-3.7.0b2/rasa/core/actions/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,16 @@
             if not self._should_request_slot(tracker, slot_name):
                 prefilled_slots[slot_name] = tracker.get_slot(slot_name)
 
         if not prefilled_slots:
             logger.debug("No pre-filled required slots to validate.")
         else:
             structlogger.debug(
-                "forms.activate.form", prefilled_slots=copy.deepcopy(prefilled_slots)
+                "forms.validate.prefilled_slots",
+                prefilled_slots=copy.deepcopy(prefilled_slots),
             )
 
         validate_name = f"validate_{self.name()}"
 
         if validate_name not in domain.action_names_or_texts:
             logger.debug(
                 f"There is no validation action '{validate_name}' "
```

### Comparing `rasa-3.7.0b1/rasa/core/actions/loops.py` & `rasa-3.7.0b2/rasa/core/actions/loops.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/actions/two_stage_fallback.py` & `rasa-3.7.0b2/rasa/core/actions/two_stage_fallback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/agent.py` & `rasa-3.7.0b2/rasa/core/agent.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/brokers/broker.py` & `rasa-3.7.0b2/rasa/core/brokers/broker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/brokers/file.py` & `rasa-3.7.0b2/rasa/core/brokers/file.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/brokers/kafka.py` & `rasa-3.7.0b2/rasa/core/brokers/kafka.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/brokers/pika.py` & `rasa-3.7.0b2/rasa/core/brokers/pika.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/brokers/sql.py` & `rasa-3.7.0b2/rasa/core/brokers/sql.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/__init__.py` & `rasa-3.7.0b2/rasa/core/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/botframework.py` & `rasa-3.7.0b2/rasa/core/channels/botframework.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/callback.py` & `rasa-3.7.0b2/rasa/core/channels/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/channel.py` & `rasa-3.7.0b2/rasa/core/channels/channel.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/console.py` & `rasa-3.7.0b2/rasa/core/channels/console.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/facebook.py` & `rasa-3.7.0b2/rasa/core/channels/facebook.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             attachment = message["message"]["attachments"][0]
             text = attachment["payload"]["url"]
         elif self._is_file_message(message):
             attachment = message["message"]["attachments"][0]
             text = attachment["payload"]["url"]
         else:
             structlogger.warning(
-                "facebook.message.handle", message=copy.deepcopy(message)
+                "facebook.message.cannot.handle", message=copy.deepcopy(message)
             )
             return
 
         await self._handle_user_message(text, self.get_user_id(), metadata)
 
     async def postback(
         self, message: Dict[Text, Any], metadata: Optional[Dict[Text, Any]]
```

### Comparing `rasa-3.7.0b1/rasa/core/channels/hangouts.py` & `rasa-3.7.0b2/rasa/core/channels/hangouts.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
                         sender_id,
                         input_channel=input_channel,
                         metadata={"room": room_name},
                     )
                 )
             except CancelledError:
                 structlogger.error(
-                    "hangouts.message.blueprint", text=copy.deepcopy(text)
+                    "hangouts.message.blueprint.timeout", text=copy.deepcopy(text)
                 )
             except Exception:
                 structlogger.exception(
                     "hangouts.message.blueprint.failure", text=copy.deepcopy(text)
                 )
 
             return response.json(collector.messages)
```

### Comparing `rasa-3.7.0b1/rasa/core/channels/mattermost.py` & `rasa-3.7.0b2/rasa/core/channels/mattermost.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/rasa_chat.py` & `rasa-3.7.0b2/rasa/core/channels/rasa_chat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/rest.py` & `rasa-3.7.0b2/rasa/core/channels/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
                             sender_id,
                             input_channel=input_channel,
                             metadata=metadata,
                         )
                     )
                 except CancelledError:
                     structlogger.error(
-                        "rest.message.received", text=copy.deepcopy(text)
+                        "rest.message.received.timeout", text=copy.deepcopy(text)
                     )
                 except Exception:
                     structlogger.exception(
                         "rest.message.received.failure", text=copy.deepcopy(text)
                     )
 
                 return response.json(collector.messages)
```

### Comparing `rasa-3.7.0b1/rasa/core/channels/rocketchat.py` & `rasa-3.7.0b2/rasa/core/channels/rocketchat.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/slack.py` & `rasa-3.7.0b2/rasa/core/channels/slack.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/socketio.py` & `rasa-3.7.0b2/rasa/core/channels/socketio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/telegram.py` & `rasa-3.7.0b2/rasa/core/channels/telegram.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/twilio.py` & `rasa-3.7.0b2/rasa/core/channels/twilio.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/twilio_voice.py` & `rasa-3.7.0b2/rasa/core/channels/twilio_voice.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/channels/webexteams.py` & `rasa-3.7.0b2/rasa/core/channels/webexteams.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/constants.py` & `rasa-3.7.0b2/rasa/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/evaluation/marker.py` & `rasa-3.7.0b2/rasa/core/evaluation/marker.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/evaluation/marker_base.py` & `rasa-3.7.0b2/rasa/core/evaluation/marker_base.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/evaluation/marker_stats.py` & `rasa-3.7.0b2/rasa/core/evaluation/marker_stats.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/evaluation/marker_tracker_loader.py` & `rasa-3.7.0b2/rasa/core/evaluation/marker_tracker_loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/exceptions.py` & `rasa-3.7.0b2/rasa/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/exporter.py` & `rasa-3.7.0b2/rasa/core/exporter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/featurizers/precomputation.py` & `rasa-3.7.0b2/rasa/core/featurizers/precomputation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/featurizers/single_state_featurizer.py` & `rasa-3.7.0b2/rasa/core/featurizers/single_state_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/featurizers/tracker_featurizers.py` & `rasa-3.7.0b2/rasa/core/featurizers/tracker_featurizers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/http_interpreter.py` & `rasa-3.7.0b2/rasa/core/http_interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         Return `None` on failure.
         """
         if not self.endpoint_config or self.endpoint_config.url is None:
             structlogger.error(
                 "http.parse.text",
                 text=copy.deepcopy(text),
+                event_info="No rasa NLU server specified!",
             )
             return None
 
         params = {
             "token": self.endpoint_config.token,
             "text": text,
             "message_id": message_id,
```

### Comparing `rasa-3.7.0b1/rasa/core/jobs.py` & `rasa-3.7.0b2/rasa/core/jobs.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/lock.py` & `rasa-3.7.0b2/rasa/core/lock.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/lock_store.py` & `rasa-3.7.0b2/rasa/core/lock_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/migrate.py` & `rasa-3.7.0b2/rasa/core/migrate.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/nlg/callback.py` & `rasa-3.7.0b2/rasa/core/nlg/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/nlg/generator.py` & `rasa-3.7.0b2/rasa/core/nlg/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/nlg/interpolator.py` & `rasa-3.7.0b2/rasa/core/nlg/interpolator.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,18 +34,24 @@
             # in double curly and format func simply escaped it.
             # we don't want to return {0[SLOTNAME]} thus
             # restoring original value with { being escaped.
             return response.format({})
 
         return text
     except KeyError as e:
+        event_info = (
+            "The specified slot name does not exist, "
+            "and no explicit value was provided during the response invocation. "
+            "Return the response without populating it."
+        )
         structlogger.exception(
             "interpolator.interpolate.text",
             response=copy.deepcopy(response),
             placeholder_key=e.args[0],
+            event_info=event_info,
         )
         return response
 
 
 def interpolate(
     response: Union[List[Any], Dict[Text, Any], Text], values: Dict[Text, Text]
 ) -> Union[List[Any], Dict[Text, Any], Text]:
```

### Comparing `rasa-3.7.0b1/rasa/core/nlg/response.py` & `rasa-3.7.0b2/rasa/core/nlg/response.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/policies/ensemble.py` & `rasa-3.7.0b2/rasa/core/policies/ensemble.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/policies/memoization.py` & `rasa-3.7.0b2/rasa/core/policies/memoization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/policies/policy.py` & `rasa-3.7.0b2/rasa/core/policies/policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/policies/rule_policy.py` & `rasa-3.7.0b2/rasa/core/policies/rule_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/policies/ted_policy.py` & `rasa-3.7.0b2/rasa/core/policies/ted_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/policies/unexpected_intent_policy.py` & `rasa-3.7.0b2/rasa/core/policies/unexpected_intent_policy.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/processor.py` & `rasa-3.7.0b2/rasa/core/processor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/run.py` & `rasa-3.7.0b2/rasa/core/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/test.py` & `rasa-3.7.0b2/rasa/core/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/tracker_store.py` & `rasa-3.7.0b2/rasa/core/tracker_store.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/train.py` & `rasa-3.7.0b2/rasa/core/train.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/training/__init__.py` & `rasa-3.7.0b2/rasa/core/training/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/training/converters/responses_prefix_converter.py` & `rasa-3.7.0b2/rasa/core/training/converters/responses_prefix_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/training/interactive.py` & `rasa-3.7.0b2/rasa/core/training/interactive.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/training/story_conflict.py` & `rasa-3.7.0b2/rasa/core/training/story_conflict.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/training/training.py` & `rasa-3.7.0b2/rasa/core/training/training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/utils.py` & `rasa-3.7.0b2/rasa/core/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/core/visualize.py` & `rasa-3.7.0b2/rasa/core/visualize.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/caching.py` & `rasa-3.7.0b2/rasa/engine/caching.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/graph.py` & `rasa-3.7.0b2/rasa/engine/graph.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/loader.py` & `rasa-3.7.0b2/rasa/engine/loader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/recipes/config_files/default_config.yml` & `rasa-3.7.0b2/rasa/engine/recipes/config_files/default_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/recipes/default_components.py` & `rasa-3.7.0b2/rasa/engine/recipes/default_components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/recipes/default_recipe.py` & `rasa-3.7.0b2/rasa/engine/recipes/default_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/recipes/graph_recipe.py` & `rasa-3.7.0b2/rasa/engine/recipes/graph_recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/recipes/recipe.py` & `rasa-3.7.0b2/rasa/engine/recipes/recipe.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/runner/dask.py` & `rasa-3.7.0b2/rasa/engine/runner/dask.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/runner/interface.py` & `rasa-3.7.0b2/rasa/engine/runner/interface.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/storage/local_model_storage.py` & `rasa-3.7.0b2/rasa/engine/storage/local_model_storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/storage/resource.py` & `rasa-3.7.0b2/rasa/engine/storage/resource.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/storage/storage.py` & `rasa-3.7.0b2/rasa/engine/storage/storage.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/training/components.py` & `rasa-3.7.0b2/rasa/engine/training/components.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/training/fingerprinting.py` & `rasa-3.7.0b2/rasa/engine/training/fingerprinting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/training/graph_trainer.py` & `rasa-3.7.0b2/rasa/engine/training/graph_trainer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/training/hooks.py` & `rasa-3.7.0b2/rasa/engine/training/hooks.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/engine/validation.py` & `rasa-3.7.0b2/rasa/engine/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/exceptions.py` & `rasa-3.7.0b2/rasa/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/converters/nlu_message_converter.py` & `rasa-3.7.0b2/rasa/graph_components/converters/nlu_message_converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/domain_for_core_training_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/domain_for_core_training_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/domain_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/domain_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/forms_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/forms_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/nlu_training_data_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/nlu_training_data_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/responses_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/responses_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/rule_only_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/rule_only_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/story_graph_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/story_graph_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/providers/training_tracker_provider.py` & `rasa-3.7.0b2/rasa/graph_components/providers/training_tracker_provider.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/validators/default_recipe_validator.py` & `rasa-3.7.0b2/rasa/graph_components/validators/default_recipe_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/graph_components/validators/finetuning_validator.py` & `rasa-3.7.0b2/rasa/graph_components/validators/finetuning_validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/jupyter.py` & `rasa-3.7.0b2/rasa/jupyter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/model.py` & `rasa-3.7.0b2/rasa/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         model_path = os.path.dirname(model_path)
 
     list_of_files = glob.glob(os.path.join(model_path, "*.tar.gz"))
 
     if len(list_of_files) == 0:
         return None
 
-    return max(list_of_files, key=os.path.getctime)
+    return max(list_of_files, key=os.path.getmtime)
 
 
 def get_model_for_finetuning(
     previous_model_file_or_dir: Union[Path, Text]
 ) -> Optional[Path]:
     """Gets validated path for model to finetune.
```

### Comparing `rasa-3.7.0b1/rasa/model_testing.py` & `rasa-3.7.0b2/rasa/model_testing.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/model_training.py` & `rasa-3.7.0b2/rasa/model_training.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/diet_classifier.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/diet_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/fallback_classifier.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/fallback_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/keyword_intent_classifier.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/keyword_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/logistic_regression_classifier.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/logistic_regression_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/mitie_intent_classifier.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/mitie_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/regex_message_handler.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/regex_message_handler.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/classifiers/sklearn_intent_classifier.py` & `rasa-3.7.0b2/rasa/nlu/classifiers/sklearn_intent_classifier.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/constants.py` & `rasa-3.7.0b2/rasa/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/convert.py` & `rasa-3.7.0b2/rasa/nlu/convert.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/emulators/dialogflow.py` & `rasa-3.7.0b2/rasa/nlu/emulators/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/emulators/emulator.py` & `rasa-3.7.0b2/rasa/nlu/emulators/emulator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/emulators/luis.py` & `rasa-3.7.0b2/rasa/nlu/emulators/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/emulators/wit.py` & `rasa-3.7.0b2/rasa/nlu/emulators/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/crf_entity_extractor.py` & `rasa-3.7.0b2/rasa/nlu/extractors/crf_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/duckling_entity_extractor.py` & `rasa-3.7.0b2/rasa/nlu/extractors/duckling_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/entity_synonyms.py` & `rasa-3.7.0b2/rasa/nlu/extractors/entity_synonyms.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/extractor.py` & `rasa-3.7.0b2/rasa/nlu/extractors/extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/mitie_entity_extractor.py` & `rasa-3.7.0b2/rasa/nlu/extractors/mitie_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/regex_entity_extractor.py` & `rasa-3.7.0b2/rasa/nlu/extractors/regex_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/extractors/spacy_entity_extractor.py` & `rasa-3.7.0b2/rasa/nlu/extractors/spacy_entity_extractor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/convert_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/dense_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/lm_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/mitie_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/dense_featurizer/spacy_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/count_vectors_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/lexical_syntactic_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py` & `rasa-3.7.0b2/rasa/nlu/featurizers/sparse_featurizer/regex_featurizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/model.py` & `rasa-3.7.0b2/rasa/nlu/model.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/persistor.py` & `rasa-3.7.0b2/rasa/nlu/persistor.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/run.py` & `rasa-3.7.0b2/rasa/nlu/run.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/selectors/response_selector.py` & `rasa-3.7.0b2/rasa/nlu/selectors/response_selector.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/test.py` & `rasa-3.7.0b2/rasa/nlu/test.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/tokenizers/jieba_tokenizer.py` & `rasa-3.7.0b2/rasa/nlu/tokenizers/jieba_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/tokenizers/mitie_tokenizer.py` & `rasa-3.7.0b2/rasa/nlu/tokenizers/mitie_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/tokenizers/spacy_tokenizer.py` & `rasa-3.7.0b2/rasa/nlu/tokenizers/spacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/tokenizers/tokenizer.py` & `rasa-3.7.0b2/rasa/nlu/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/tokenizers/whitespace_tokenizer.py` & `rasa-3.7.0b2/rasa/nlu/tokenizers/whitespace_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/__init__.py` & `rasa-3.7.0b2/rasa/nlu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/bilou_utils.py` & `rasa-3.7.0b2/rasa/nlu/utils/bilou_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/hugging_face/registry.py` & `rasa-3.7.0b2/rasa/nlu/utils/hugging_face/registry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py` & `rasa-3.7.0b2/rasa/nlu/utils/hugging_face/transformers_pre_post_processors.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/mitie_utils.py` & `rasa-3.7.0b2/rasa/nlu/utils/mitie_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/pattern_utils.py` & `rasa-3.7.0b2/rasa/nlu/utils/pattern_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/nlu/utils/spacy_utils.py` & `rasa-3.7.0b2/rasa/nlu/utils/spacy_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/plugin.py` & `rasa-3.7.0b2/rasa/plugin.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/server.py` & `rasa-3.7.0b2/rasa/server.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/constants.py` & `rasa-3.7.0b2/rasa/shared/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/constants.py` & `rasa-3.7.0b2/rasa/shared/core/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/conversation.py` & `rasa-3.7.0b2/rasa/shared/core/conversation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/domain.py` & `rasa-3.7.0b2/rasa/shared/core/domain.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/events.py` & `rasa-3.7.0b2/rasa/shared/core/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/generator.py` & `rasa-3.7.0b2/rasa/shared/core/generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/slot_mappings.py` & `rasa-3.7.0b2/rasa/shared/core/slot_mappings.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/slots.py` & `rasa-3.7.0b2/rasa/shared/core/slots.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/trackers.py` & `rasa-3.7.0b2/rasa/shared/core/trackers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/loading.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_reader.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/story_step_builder.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/story_step_builder.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/story_reader/yaml_story_reader.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/story_reader/yaml_story_reader.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/story_writer.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/story_writer/yaml_story_writer.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/story_writer/yaml_story_writer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/structures.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/structures.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/visualization.html` & `rasa-3.7.0b2/rasa/shared/core/training_data/visualization.html`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/core/training_data/visualization.py` & `rasa-3.7.0b2/rasa/shared/core/training_data/visualization.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/data.py` & `rasa-3.7.0b2/rasa/shared/data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/exceptions.py` & `rasa-3.7.0b2/rasa/shared/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/importers/importer.py` & `rasa-3.7.0b2/rasa/shared/importers/importer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/importers/multi_project.py` & `rasa-3.7.0b2/rasa/shared/importers/multi_project.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/importers/rasa.py` & `rasa-3.7.0b2/rasa/shared/importers/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/importers/utils.py` & `rasa-3.7.0b2/rasa/shared/importers/utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/constants.py` & `rasa-3.7.0b2/rasa/shared/nlu/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/entities_parser.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/entities_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/features.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/features.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/dialogflow.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/dialogflow.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/luis.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/luis.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/rasa_yaml.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/rasa_yaml.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/readerwriter.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/readerwriter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/formats/wit.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/formats/wit.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/loading.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/loading.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/lookup_tables_parser.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/lookup_tables_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/message.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/message.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/data_schema.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/data_schema.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/nlu.yml` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/nlu.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/schemas/responses.yml` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/schemas/responses.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/synonyms_parser.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/synonyms_parser.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/training_data.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/training_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/nlu/training_data/util.py` & `rasa-3.7.0b2/rasa/shared/nlu/training_data/util.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/cli.py` & `rasa-3.7.0b2/rasa/shared/utils/cli.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/common.py` & `rasa-3.7.0b2/rasa/shared/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/io.py` & `rasa-3.7.0b2/rasa/shared/utils/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,15 @@
         [deep_container_fingerprint(element, encoding) for element in elements]
     )
     return get_text_hash(stringified, encoding)
 
 
 def get_text_hash(text: Text, encoding: Text = DEFAULT_ENCODING) -> Text:
     """Calculate the md5 hash for a text."""
+    # deepcode ignore InsecureHash: Not used for a cryptographic purpose
     return md5(text.encode(encoding)).hexdigest()  # nosec
 
 
 def json_to_string(obj: Any, **kwargs: Any) -> Text:
     """Dumps a JSON-serializable object to string.
 
     Args:
```

### Comparing `rasa-3.7.0b1/rasa/shared/utils/pykwalify_extensions.py` & `rasa-3.7.0b2/rasa/shared/utils/pykwalify_extensions.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/schemas/domain.yml` & `rasa-3.7.0b2/rasa/shared/utils/schemas/domain.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/schemas/events.py` & `rasa-3.7.0b2/rasa/shared/utils/schemas/events.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/schemas/model_config.yml` & `rasa-3.7.0b2/rasa/shared/utils/schemas/model_config.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/schemas/stories.yml` & `rasa-3.7.0b2/rasa/shared/utils/schemas/stories.yml`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/shared/utils/validation.py` & `rasa-3.7.0b2/rasa/shared/utils/validation.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/telemetry.py` & `rasa-3.7.0b2/rasa/telemetry.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/common.py` & `rasa-3.7.0b2/rasa/utils/common.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/converter.py` & `rasa-3.7.0b2/rasa/utils/converter.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/endpoints.py` & `rasa-3.7.0b2/rasa/utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/io.py` & `rasa-3.7.0b2/rasa/utils/io.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/llm.py` & `rasa-3.7.0b2/rasa/utils/llm.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/log_utils.py` & `rasa-3.7.0b2/rasa/utils/log_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,36 @@
 import os
 import logging
 import sys
 from typing import Any, Dict, Optional
 
 import structlog
 from structlog_sentry import SentryProcessor
+from structlog.dev import ConsoleRenderer
+from structlog.typing import EventDict, WrappedLogger
 from rasa.shared.constants import ENV_LOG_LEVEL, DEFAULT_LOG_LEVEL
 from rasa.plugin import plugin_manager
 
 
 FORCE_JSON_LOGGING = os.environ.get("FORCE_JSON_LOGGING")
 
 
+class HumanConsoleRenderer(ConsoleRenderer):
+    """Console renderer that outputs human-readable logs."""
+
+    def __call__(self, logger: WrappedLogger, name: str, event_dict: EventDict) -> str:
+        if "event_info" in event_dict:
+            event_key = event_dict["event"]
+            event_dict["event"] = event_dict["event_info"]
+            event_dict["event_key"] = event_key
+            del event_dict["event_info"]
+
+        return super().__call__(logger, name, event_dict)
+
+
 def _anonymizer(
     _: structlog.BoundLogger, __: str, event_dict: Dict[str, Any]
 ) -> Dict[str, Any]:
     """Anonymizes event dict."""
     anonymizable_keys = [
         "text",
         "response_text",
@@ -39,15 +54,14 @@
         "successes",
         "current_entity",
         "next_entity",
         "states",
         "entity",
         "token_text",
         "user_message",
-        "activity",
         "json_message",
     ]
     anonymization_pipeline = plugin_manager().hook.get_anonymization_pipeline()
 
     if anonymization_pipeline:
         for key in anonymizable_keys:
             if key in event_dict:
@@ -94,15 +108,15 @@
         SentryProcessor(event_level=logging.FATAL),
     ]
 
     if not FORCE_JSON_LOGGING and sys.stderr.isatty():
         # Pretty printing when we run in a terminal session.
         # Automatically prints pretty tracebacks when "rich" is installed
         processors = shared_processors + [
-            structlog.dev.ConsoleRenderer(),
+            HumanConsoleRenderer(),
         ]
     else:
         # Print JSON when we run, e.g., in a Docker container.
         # Also print structured tracebacks.
         processors = shared_processors + [
             structlog.processors.dict_tracebacks,
             structlog.processors.JSONRenderer(),
```

### Comparing `rasa-3.7.0b1/rasa/utils/plotting.py` & `rasa-3.7.0b2/rasa/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/callback.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/callback.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/constants.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/constants.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/crf.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/crf.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/data_generator.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/data_generator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/environment.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/environment.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/layers.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/layers_utils.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/layers_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/metrics.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/metrics.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/model_data.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/model_data.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/model_data_utils.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/model_data_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/models.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/models.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/rasa_layers.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/rasa_layers.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/tensorflow/transformer.py` & `rasa-3.7.0b2/rasa/utils/tensorflow/transformer.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/utils/train_utils.py` & `rasa-3.7.0b2/rasa/utils/train_utils.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/rasa/validator.py` & `rasa-3.7.0b2/rasa/validator.py`

 * *Files identical despite different names*

### Comparing `rasa-3.7.0b1/PKG-INFO` & `rasa-3.7.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa
-Version: 3.7.0b1
+Version: 3.7.0b2
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
@@ -65,15 +65,15 @@
 Requires-Dist: pydot (>=1.4,<1.5)
 Requires-Dist: pykwalify (>=1.7,<1.9)
 Requires-Dist: pymongo[srv,tls] (>=3.8,<4.4)
 Requires-Dist: python-dateutil (>=2.8,<2.9)
 Requires-Dist: python-engineio (>=4,<6,!=5.0.0)
 Requires-Dist: python-socketio (>=4.4,<6)
 Requires-Dist: pytz (>=2019.1,<2023.0)
-Requires-Dist: pyyaml (>=5.3.1,<6.0)
+Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: questionary (>=1.5.1,<1.11.0)
 Requires-Dist: randomname (>=0.1.5,<0.2.0)
 Requires-Dist: rasa-sdk (>=3.7.0b1,<3.8.0)
 Requires-Dist: redis (>=4.5.3,<5.0)
 Requires-Dist: regex (>=2020.6,<2022.11)
 Requires-Dist: requests (>=2.23,<3.0)
 Requires-Dist: rocketchat_API (>=0.6.31,<1.31.0)
@@ -123,15 +123,15 @@
 
 <div align="center">
 
 [![Join the chat on Rasa Community Forum](https://img.shields.io/badge/forum-join%20discussions-brightgreen.svg)](https://forum.rasa.com/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
 [![PyPI version](https://badge.fury.io/py/rasa.svg)](https://badge.fury.io/py/rasa)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/rasa.svg)](https://pypi.python.org/pypi/rasa)
 [![Build Status](https://github.com/RasaHQ/rasa/workflows/Continuous%20Integration/badge.svg)](https://github.com/RasaHQ/rasa/actions)
-[![Coverage Status](https://api.codeclimate.com/v1/badges/756dc6fea1d5d3e127f7/test_coverage)](https://codeclimate.com/github/RasaHQ/rasa/)
+[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=RasaHQ_rasa&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=RasaHQ_rasa)
 [![Documentation Status](https://img.shields.io/badge/docs-stable-brightgreen.svg)](https://rasa.com/docs)
 ![Documentation Build](https://img.shields.io/netlify/d2e447e4-5a5e-4dc7-be5d-7c04ae7ff706?label=Documentation%20Build)
 [![FOSSA Status](https://app.fossa.com/api/projects/custom%2B8141%2Fgit%40github.com%3ARasaHQ%2Frasa.git.svg?type=shield)](https://app.fossa.com/projects/custom%2B8141%2Fgit%40github.com%3ARasaHQ%2Frasa.git?ref=badge_shield)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://github.com/orgs/RasaHQ/projects/23)
 
 </div>
```

