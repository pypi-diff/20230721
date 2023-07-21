# Comparing `tmp/lightning-template-1.1.0.tar.gz` & `tmp/lightning-template-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-template-1.1.0.tar", last modified: Fri Jul 21 08:03:08 2023, max compression
+gzip compressed data, was "lightning-template-1.1.1.tar", last modified: Fri Jul 21 08:15:46 2023, max compression
```

## Comparing `lightning-template-1.1.0.tar` & `lightning-template-1.1.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.397942 lightning-template-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 08:02:55.000000 lightning-template-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:03:08.397942 lightning-template-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 08:02:55.000000 lightning-template-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.381942 lightning-template-1.1.0/lightning_template/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.385942 lightning-template-1.1.0/lightning_template/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.385942 lightning-template-1.1.0/lightning_template/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.385942 lightning-template-1.1.0/lightning_template/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.385942 lightning-template-1.1.0/lightning_template/tools/model/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/tools/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/tools/model/batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/tools/model/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/tools/model/model_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.385942 lightning-template-1.1.0/lightning_template/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.389942 lightning-template-1.1.0/lightning_template/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/custom_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/save_and_log_config_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/callbacks/set_wandb_logger_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.389942 lightning-template-1.1.0/lightning_template/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.393942 lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/deep_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/json_file_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/instantiate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/cli/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.393942 lightning-template-1.1.0/lightning_template/utils/loggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.393942 lightning-template-1.1.0/lightning_template/utils/loop/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/loop/kfold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.393942 lightning-template-1.1.0/lightning_template/utils/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/mixin/split_name_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.397942 lightning-template-1.1.0/lightning_template/utils/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/optim/configure_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/optim/warmup_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.397942 lightning-template-1.1.0/lightning_template/utils/progress/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/progress/rich_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.397942 lightning-template-1.1.0/lightning_template/utils/timer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 08:02:55.000000 lightning-template-1.1.0/lightning_template/utils/timer/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:03:08.381942 lightning-template-1.1.0/lightning_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:03:08.000000 lightning-template-1.1.0/lightning_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-21 08:03:08.000000 lightning-template-1.1.0/lightning_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:03:08.000000 lightning-template-1.1.0/lightning_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-21 08:03:08.000000 lightning-template-1.1.0/lightning_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 08:03:08.000000 lightning-template-1.1.0/lightning_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 08:03:08.000000 lightning-template-1.1.0/lightning_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:03:08.397942 lightning-template-1.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-07-21 08:02:55.000000 lightning-template-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 08:15:32.000000 lightning-template-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:15:46.172349 lightning-template-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 08:15:32.000000 lightning-template-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template/tools/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/tools/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/tools/model/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/tools/model/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/tools/model/model_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/custom_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/save_and_log_config_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/callbacks/set_wandb_logger_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/deep_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/json_file_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/instantiate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/cli/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/loggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/loop/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/loop/kfold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/mixin/split_name_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/optim/configure_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/optim/warmup_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/progress/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/progress/rich_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.172349 lightning-template-1.1.1/lightning_template/utils/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 08:15:32.000000 lightning-template-1.1.1/lightning_template/utils/timer/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:15:46.168349 lightning-template-1.1.1/lightning_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:15:46.000000 lightning-template-1.1.1/lightning_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-21 08:15:46.000000 lightning-template-1.1.1/lightning_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:15:46.000000 lightning-template-1.1.1/lightning_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-21 08:15:46.000000 lightning-template-1.1.1/lightning_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 08:15:46.000000 lightning-template-1.1.1/lightning_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 08:15:46.000000 lightning-template-1.1.1/lightning_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:15:46.172349 lightning-template-1.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-07-21 08:15:32.000000 lightning-template-1.1.1/setup.py
```

### Comparing `lightning-template-1.1.0/LICENSE` & `lightning-template-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/PKG-INFO` & `lightning-template-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.1.0
+Version: 1.1.1
 Summary: A template wrapper for pytorch-lightning.
 Home-page: https://github.com/shenmishajing/lightning_template
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/lightning_template
 Project-URL: Issue tracker, https://github.com/shenmishajing/lightning_template/issues
```

### Comparing `lightning-template-1.1.0/README.md` & `lightning-template-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/datasets/base.py` & `lightning-template-1.1.1/lightning_template/datasets/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         else:
             sampler = SequentialSampler(dataset)
         return sampler
 
     def _build_batch_sampler(self, batch_sampler_cfg, dataset, *args):
         return instantiate_class(args, batch_sampler_cfg)
 
-    def _handle_batch_sampler(self, dataloader_cfg, dataset, split="train"):
+    def _handle_batch_sampler(self, dataloader_cfg, dataset, *arg, **kwargs):
         if "batch_sampler" in dataloader_cfg:
             if "init_args" not in dataloader_cfg["batch_sampler"]:
                 dataloader_cfg["batch_sampler"]["init_args"] = {}
 
             dataloader_cfg["batch_sampler"]["init_args"][
                 "batch_size"
             ] = dataloader_cfg.pop("batch_size", 1)
@@ -70,15 +70,15 @@
             ] = self._build_sampler(dataloader_cfg, dataset)
 
             dataloader_cfg["batch_sampler"] = self._build_batch_sampler(
                 dataloader_cfg["batch_sampler"], dataset
             )
         return dataloader_cfg
 
-    def _build_dataloader(self, dataset, split="train", set_batch_size=False):
+    def _build_dataloader(self, dataset, split, set_batch_size=False):
         dataloader_cfg = copy.deepcopy(self.dataloader_cfg.get(split, {}))
         if set_batch_size:
             dataloader_cfg["batch_size"] = self.batch_size
         dataloader_cfg["collate_fn"] = self._build_collate_fn(
             dataloader_cfg.get("collate_fn", {}), dataset
         )
         return DataLoader(
@@ -104,24 +104,26 @@
     def setup_folds(self, num_folds: int) -> None:
         self.num_folds = num_folds
         self.splits = [
             split for split in KFold(num_folds).split(range(len(self.dataset)))
         ]
 
     def setup_fold_index(self, fold_index: int) -> None:
-        for indices, fold_name in zip(self.splits[fold_index], ["train", "val"]):
+        for indices, fold_name in zip(
+            self.splits[fold_index], [self.TrainSplit, self.ValidateSplit]
+        ):
             self.folds[fold_name] = Subset(self.dataset, indices)
 
-        for fold_name in ["test", "predict"]:
-            self.folds[fold_name] = self.folds["val"]
+        for fold_name in [self.TestSplit, self.PredictSplit]:
+            self.folds[fold_name] = self.folds[self.ValidateSplit]
 
     def train_dataloader(self):
-        return self._dataloader("train")
+        return self._dataloader(self.TrainSplit)
 
     def val_dataloader(self):
-        return self._dataloader("val")
+        return self._dataloader(self.ValidateSplit)
 
     def test_dataloader(self):
-        return self._dataloader("test")
+        return self._dataloader(self.TestSplit)
 
     def predict_dataloader(self):
-        return self._dataloader("predict")
+        return self._dataloader(self.PredictSplit)
```

### Comparing `lightning-template-1.1.0/lightning_template/models/base.py` & `lightning-template-1.1.1/lightning_template/models/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         # manual step lr scheduler
         for scheduler in self.manual_step_scedulers:
             if self.trainer.global_step % scheduler["frequency"] == 0:
                 scheduler["scheduler"].step()
 
     @staticmethod
-    def flatten_dict(log_dict, prefix="train", sep="/"):
+    def flatten_dict(log_dict, prefix, sep="/"):
         res_dict = {}
 
         for k, v in log_dict.items():
             new_key = prefix + sep + k if prefix else k
             if isinstance(v, Mapping):
                 res_dict[new_key] = LightningModule.flatten_dict(v, new_key, sep=sep)
             else:
@@ -96,21 +96,21 @@
         # calculate loss
         if "loss" not in loss:
             loss["loss"] = torch.sum(
                 torch.stack([v for k, v in loss.items() if "loss" in k])
             )
         return loss
 
-    def metric_step(self, batch, output, *args, split="val", **kwargs):
+    def metric_step(self, batch, output, *args, split, **kwargs):
         if self.evaluators[split]:
             return self.evaluators[split].update(batch, output)
         else:
             return {}
 
-    def on_metric_epoch_end(self, *args, split="val", **kwargs):
+    def on_metric_epoch_end(self, *args, split, **kwargs):
         if self.evaluators[split]:
             return self.evaluators[split].compute()
         else:
             return {}
 
     def forward_step(self, batch, *args, split, **kwargs):
         # forward
@@ -120,42 +120,46 @@
         log_dict = self.loss_step(batch, output, *args, **kwargs)
 
         # metrics
         metrics = self.metric_step(batch, output, split=split, *args, **kwargs)
         log_dict.update(metrics)
 
         # log
-        self.log_dict(self.flatten_dict(log_dict, split), sync_dist=split != "train")
+        self.log_dict(
+            self.flatten_dict(log_dict, split), sync_dist=split != self.TrainSplit
+        )
 
         # return loss
         return log_dict
 
     def on_forward_epoch_end(self, split, *args, **kwargs):
         metrics = self.on_metric_epoch_end(split=split, *args, **kwargs)
 
         if metrics:
-            self.log_dict(self.flatten_dict(metrics, split), sync_dist=split != "train")
+            self.log_dict(
+                self.flatten_dict(metrics, split), sync_dist=split != self.TrainSplit
+            )
 
     def training_step(self, *args, **kwargs):
-        return self.forward_step(split="train", *args, **kwargs)
+        return self.forward_step(split=self.TrainSplit, *args, **kwargs)
 
     def on_training_epoch_end(self, *args, **kwargs):
-        return self.on_forward_epoch_end(split="train", *args, **kwargs)
+        return self.on_forward_epoch_end(split=self.TrainSplit, *args, **kwargs)
 
     def validation_step(self, *args, **kwargs):
-        return self.forward_step(split="val", *args, **kwargs)
+        return self.forward_step(split=self.ValidateSplit, *args, **kwargs)
 
     def on_validation_epoch_end(self, *args, **kwargs):
-        return self.on_forward_epoch_end(split="val", *args, **kwargs)
+        return self.on_forward_epoch_end(split=self.ValidateSplit, *args, **kwargs)
 
     def test_step(self, *args, **kwargs):
-        return self.forward_step(split="test", *args, **kwargs)
+        return self.forward_step(split=self.TestSplit, *args, **kwargs)
 
     def on_test_epoch_end(self, *args, **kwargs):
-        return self.on_forward_epoch_end(split="test", *args, **kwargs)
+        return self.on_forward_epoch_end(split=self.TestSplit, *args, **kwargs)
 
     @staticmethod
     @rank_zero_only
     def rm_and_create(path):
         if os.path.exists(path):
             shutil.rmtree(path)
         os.makedirs(path, exist_ok=True)
```

### Comparing `lightning-template-1.1.0/lightning_template/tools/model/batch_size_finder.py` & `lightning-template-1.1.1/lightning_template/tools/model/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/tools/model/model_statistics.py` & `lightning-template-1.1.1/lightning_template/tools/model/model_statistics.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/callbacks/custom_repr.py` & `lightning-template-1.1.1/lightning_template/utils/callbacks/custom_repr.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/callbacks/model_checkpoint.py` & `lightning-template-1.1.1/lightning_template/utils/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/callbacks/save_and_log_config_callback.py` & `lightning-template-1.1.1/lightning_template/utils/callbacks/save_and_log_config_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py` & `lightning-template-1.1.1/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/callbacks/set_sharing_strategy_callback.py` & `lightning-template-1.1.1/lightning_template/utils/callbacks/set_sharing_strategy_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/callbacks/set_wandb_logger_callback.py` & `lightning-template-1.1.1/lightning_template/utils/callbacks/set_wandb_logger_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/deep_update.py` & `lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/deep_update.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/json_file_action.py` & `lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/json_file_action.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py` & `lightning-template-1.1.1/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/cli/cli.py` & `lightning-template-1.1.1/lightning_template/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/cli/instantiate_class.py` & `lightning-template-1.1.1/lightning_template/utils/cli/instantiate_class.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/cli/trainer.py` & `lightning-template-1.1.1/lightning_template/utils/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/loop/kfold.py` & `lightning-template-1.1.1/lightning_template/utils/loop/kfold.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/mixin/split_name_mixin.py` & `lightning-template-1.1.1/lightning_template/utils/mixin/split_name_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/optim/configure_optimizers.py` & `lightning-template-1.1.1/lightning_template/utils/optim/configure_optimizers.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py` & `lightning-template-1.1.1/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/optim/warmup_lr_scheduler.py` & `lightning-template-1.1.1/lightning_template/utils/optim/warmup_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/progress/rich_progress.py` & `lightning-template-1.1.1/lightning_template/utils/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template/utils/timer/timer.py` & `lightning-template-1.1.1/lightning_template/utils/timer/timer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/lightning_template.egg-info/PKG-INFO` & `lightning-template-1.1.1/lightning_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.1.0
+Version: 1.1.1
 Summary: A template wrapper for pytorch-lightning.
 Home-page: https://github.com/shenmishajing/lightning_template
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/lightning_template
 Project-URL: Issue tracker, https://github.com/shenmishajing/lightning_template/issues
```

### Comparing `lightning-template-1.1.0/lightning_template.egg-info/SOURCES.txt` & `lightning-template-1.1.1/lightning_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.0/setup.py` & `lightning-template-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lightning-template",
-    version="1.1.0",
+    version="1.1.1",
     description="A template wrapper for pytorch-lightning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/lightning_template",
     project_urls={
```

