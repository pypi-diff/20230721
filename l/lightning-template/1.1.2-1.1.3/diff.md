# Comparing `tmp/lightning-template-1.1.2.tar.gz` & `tmp/lightning-template-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-template-1.1.2.tar", last modified: Fri Jul 21 08:28:14 2023, max compression
+gzip compressed data, was "lightning-template-1.1.3.tar", last modified: Fri Jul 21 08:59:11 2023, max compression
```

## Comparing `lightning-template-1.1.2.tar` & `lightning-template-1.1.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.161971 lightning-template-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 08:28:02.000000 lightning-template-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:28:14.161971 lightning-template-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 08:28:02.000000 lightning-template-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.153971 lightning-template-1.1.2/lightning_template/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.153971 lightning-template-1.1.2/lightning_template/datasets/
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/datasets/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/tools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/tools/model/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/tools/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/tools/model/batch_size_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/tools/model/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/tools/model/model_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/utils/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/custom_repr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/save_and_log_config_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/callbacks/set_wandb_logger_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/deep_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/json_file_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/instantiate_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/cli/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/utils/loggers/
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/loggers/wandb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.157971 lightning-template-1.1.2/lightning_template/utils/loop/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/loop/kfold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.161971 lightning-template-1.1.2/lightning_template/utils/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/mixin/split_name_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.161971 lightning-template-1.1.2/lightning_template/utils/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/optim/configure_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/optim/warmup_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.161971 lightning-template-1.1.2/lightning_template/utils/progress/
--rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/progress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/progress/rich_progress.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.161971 lightning-template-1.1.2/lightning_template/utils/timer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 08:28:02.000000 lightning-template-1.1.2/lightning_template/utils/timer/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:28:14.153971 lightning-template-1.1.2/lightning_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:28:14.000000 lightning-template-1.1.2/lightning_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-21 08:28:14.000000 lightning-template-1.1.2/lightning_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:28:14.000000 lightning-template-1.1.2/lightning_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-21 08:28:14.000000 lightning-template-1.1.2/lightning_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 08:28:14.000000 lightning-template-1.1.2/lightning_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 08:28:14.000000 lightning-template-1.1.2/lightning_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:28:14.161971 lightning-template-1.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-07-21 08:28:02.000000 lightning-template-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.527580 lightning-template-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 08:58:56.000000 lightning-template-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:59:11.527580 lightning-template-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-21 08:58:56.000000 lightning-template-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.519580 lightning-template-1.1.3/lightning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.519580 lightning-template-1.1.3/lightning_template/datasets/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/datasets/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.519580 lightning-template-1.1.3/lightning_template/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6651 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/tools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/tools/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/tools/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/tools/model/batch_size_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/tools/model/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/tools/model/model_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      350 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/custom_repr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/save_and_log_config_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/set_sharing_strategy_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/callbacks/set_wandb_logger_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/deep_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/json_file_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/instantiate_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/cli/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/loggers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/loggers/wandb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/loop/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/loop/kfold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/mixin/split_name_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/optim/configure_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/optim/warmup_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.523580 lightning-template-1.1.3/lightning_template/utils/progress/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       16 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/progress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/progress/rich_progress.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.527580 lightning-template-1.1.3/lightning_template/utils/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-21 08:58:56.000000 lightning-template-1.1.3/lightning_template/utils/timer/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:59:11.519580 lightning-template-1.1.3/lightning_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-21 08:59:11.000000 lightning-template-1.1.3/lightning_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-21 08:59:11.000000 lightning-template-1.1.3/lightning_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:59:11.000000 lightning-template-1.1.3/lightning_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-21 08:59:11.000000 lightning-template-1.1.3/lightning_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 08:59:11.000000 lightning-template-1.1.3/lightning_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 08:59:11.000000 lightning-template-1.1.3/lightning_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 08:59:11.527580 lightning-template-1.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-07-21 08:58:56.000000 lightning-template-1.1.3/setup.py
```

### Comparing `lightning-template-1.1.2/LICENSE` & `lightning-template-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/PKG-INFO` & `lightning-template-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.1.2
+Version: 1.1.3
 Summary: A template wrapper for pytorch-lightning.
 Home-page: https://github.com/shenmishajing/lightning_template
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/lightning_template
 Project-URL: Issue tracker, https://github.com/shenmishajing/lightning_template/issues
```

### Comparing `lightning-template-1.1.2/README.md` & `lightning-template-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/datasets/base.py` & `lightning-template-1.1.3/lightning_template/datasets/base.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/models/base.py` & `lightning-template-1.1.3/lightning_template/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,14 +79,20 @@
                 res_dict[new_key] = v
         return res_dict
 
     def forward(self, batch, *args, **kwargs):
         return self.model(batch)
 
     def _loss_step(self, batch, output, *args, **kwargs):
+        if not isinstance(output, Mapping):
+            return {"loss": output}
+        elif "log_dict" in output:
+            return output["log_dict"]
+        elif hasattr(self.model, "loss_step"):
+            return self.model.loss_step(batch, output)
         return output
 
     def loss_step(self, *args, use_loss_weight=True, **kwargs):
         loss = self._loss_step(*args, **kwargs)
         # multi loss weights
         if use_loss_weight and self.loss_weights:
             loss = {
```

### Comparing `lightning-template-1.1.2/lightning_template/tools/model/batch_size_finder.py` & `lightning-template-1.1.3/lightning_template/tools/model/batch_size_finder.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/tools/model/model_statistics.py` & `lightning-template-1.1.3/lightning_template/tools/model/model_statistics.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/callbacks/custom_repr.py` & `lightning-template-1.1.3/lightning_template/utils/callbacks/custom_repr.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/callbacks/model_checkpoint.py` & `lightning-template-1.1.3/lightning_template/utils/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/callbacks/save_and_log_config_callback.py` & `lightning-template-1.1.3/lightning_template/utils/callbacks/save_and_log_config_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py` & `lightning-template-1.1.3/lightning_template/utils/callbacks/set_precision_and_cudnn_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/callbacks/set_sharing_strategy_callback.py` & `lightning-template-1.1.3/lightning_template/utils/callbacks/set_sharing_strategy_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/callbacks/set_wandb_logger_callback.py` & `lightning-template-1.1.3/lightning_template/utils/callbacks/set_wandb_logger_callback.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/deep_update.py` & `lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/deep_update.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/json_file_action.py` & `lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/json_file_action.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py` & `lightning-template-1.1.3/lightning_template/utils/cli/argument_parsers/yaml_with_merge.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/cli/cli.py` & `lightning-template-1.1.3/lightning_template/utils/cli/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/cli/instantiate_class.py` & `lightning-template-1.1.3/lightning_template/utils/cli/instantiate_class.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/cli/trainer.py` & `lightning-template-1.1.3/lightning_template/utils/cli/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/loop/kfold.py` & `lightning-template-1.1.3/lightning_template/utils/loop/kfold.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/mixin/split_name_mixin.py` & `lightning-template-1.1.3/lightning_template/utils/mixin/split_name_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/optim/configure_optimizers.py` & `lightning-template-1.1.3/lightning_template/utils/optim/configure_optimizers.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py` & `lightning-template-1.1.3/lightning_template/utils/optim/keep_and_linearly_decay_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/optim/warmup_lr_scheduler.py` & `lightning-template-1.1.3/lightning_template/utils/optim/warmup_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/progress/rich_progress.py` & `lightning-template-1.1.3/lightning_template/utils/progress/rich_progress.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template/utils/timer/timer.py` & `lightning-template-1.1.3/lightning_template/utils/timer/timer.py`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/lightning_template.egg-info/PKG-INFO` & `lightning-template-1.1.3/lightning_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-template
-Version: 1.1.2
+Version: 1.1.3
 Summary: A template wrapper for pytorch-lightning.
 Home-page: https://github.com/shenmishajing/lightning_template
 Author: shenmishajing
 Author-email: shenmishajing@gmail.com
 License: MIT License
 Project-URL: Code, https://github.com/shenmishajing/lightning_template
 Project-URL: Issue tracker, https://github.com/shenmishajing/lightning_template/issues
```

### Comparing `lightning-template-1.1.2/lightning_template.egg-info/SOURCES.txt` & `lightning-template-1.1.3/lightning_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-template-1.1.2/setup.py` & `lightning-template-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lightning-template",
-    version="1.1.2",
+    version="1.1.3",
     description="A template wrapper for pytorch-lightning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="shenmishajing",
     author_email="shenmishajing@gmail.com",
     url="https://github.com/shenmishajing/lightning_template",
     project_urls={
```

