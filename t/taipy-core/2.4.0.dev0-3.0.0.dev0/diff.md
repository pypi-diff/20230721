# Comparing `tmp/taipy-core-2.4.0.dev0.tar.gz` & `tmp/taipy-core-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-core-2.4.0.dev0.tar", last modified: Fri Jul 21 11:36:49 2023, max compression
+gzip compressed data, was "taipy-core-3.0.0.dev0.tar", last modified: Fri Jun 23 09:48:19 2023, max compression
```

## Comparing `taipy-core-2.4.0.dev0.tar` & `taipy-core-3.0.0.dev0.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.249166 taipy-core-2.4.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-21 11:36:49.249166 taipy-core-2.4.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 11:36:49.249166 taipy-core-2.4.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-21 11:36:41.000000 taipy-core-2.4.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/taipy/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/taipy/core/_backup/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_backup/_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_core_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/taipy/core/_entity/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_entity_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_labeled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_reload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_entity/_submittable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/taipy/core/_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_manager/_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_manager/_manager_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.229166 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.233166 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.233166 taipy-core-2.4.0.dev0/src/taipy/core/_repository/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/_filesystem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/_repository_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/_sql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_repository/_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.233166 taipy-core-2.4.0.dev0/src/taipy/core/_version/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.233166 taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/_bcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/_version_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_sql_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.233166 taipy-core-2.4.0.dev0/src/taipy/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/_listattributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/_warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/default_custom_document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.237166 taipy-core-2.4.0.dev0/src/taipy/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.237166 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/config.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/core_section.py
--rw-r--r--   0 runner    (1001) docker     (123)    49614 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/data_node_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/job_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/scenario_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10090 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/config/task_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.237166 taipy-core-2.4.0.dev0/src/taipy/core/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/cycle.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/cycle/cycle_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.241166 taipy-core-2.4.0.dev0/src/taipy/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_data_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/abstract_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/data_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/data_node_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/data/sql_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.241166 taipy-core-2.4.0.dev0/src/taipy/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.241166 taipy-core-2.4.0.dev0/src/taipy/core/job/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/_job_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/job.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/job_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/job/status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.241166 taipy-core-2.4.0.dev0/src/taipy/core/notification/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/core_event_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/registration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/notification/topic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.245166 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/pipeline/pipeline_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.245166 taipy-core-2.4.0.dev0/src/taipy/core/scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/scenario/scenario_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/taipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.245166 taipy-core-2.4.0.dev0/src/taipy/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_fs_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_repository_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/_task_sql_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/task/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/src/taipy/core/version.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.245166 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-21 11:36:49.000000 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-21 11:36:49.000000 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:36:49.000000 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:36:42.000000 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-21 11:36:49.000000 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 11:36:49.000000 taipy-core-2.4.0.dev0/src/taipy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:36:49.245166 taipy-core-2.4.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/tests/test_complex_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    33298 2023-07-21 11:36:36.000000 taipy-core-2.4.0.dev0/tests/test_taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-23 09:48:10.000000 taipy-core-3.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.971586 taipy-core-3.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.971586 taipy-core-3.0.0.dev0/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_backup/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_backup/_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_core_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_labeled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_reload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_entity/_submittable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.975586 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_filesystem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_version/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.979586 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_bcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_sql_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.983586 taipy-core-3.0.0.dev0/src/taipy/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_listattributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/default_custom_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.983586 taipy-core-3.0.0.dev0/src/taipy/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.983586 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/config.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/core_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49075 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/data_node_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/job_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/scenario_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/config/task_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.987586 taipy-core-3.0.0.dev0/src/taipy/core/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6080 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.987586 taipy-core-3.0.0.dev0/src/taipy/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_data_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9586 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/data_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/data_node_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13905 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9057 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11994 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/data/sql_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.991586 taipy-core-3.0.0.dev0/src/taipy/core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.991586 taipy-core-3.0.0.dev0/src/taipy/core/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/_job_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9939 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/job/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.991586 taipy-core-3.0.0.dev0/src/taipy/core/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/core_event_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/notification/topic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.995586 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7520 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.995586 taipy-core-3.0.0.dev0/src/taipy/core/scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14080 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27303 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/taipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/src/taipy/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_fs_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/_task_sql_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/task/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/src/taipy/core/version.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 09:48:11.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 09:48:18.000000 taipy-core-3.0.0.dev0/src/taipy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 09:48:18.999586 taipy-core-3.0.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9955 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/tests/test_complex_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33298 2023-06-23 09:48:05.000000 taipy-core-3.0.0.dev0/tests/test_taipy.py
```

### Comparing `taipy-core-2.4.0.dev0/LICENSE` & `taipy-core-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/PKG-INFO` & `taipy-core-3.0.0.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.4.0.dev0/README.md` & `taipy-core-3.0.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/setup.py` & `taipy-core-3.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     version_string = f'{version.get("major", 0)}.{version.get("minor", 0)}.{version.get("patch", 0)}'
     if vext := version.get("ext"):
         version_string = f"{version_string}.{vext}"
 
 requirements = [
     "pyarrow>=10.0.1,<11.0",
     "networkx>=2.6,<3.0",
-    "openpyxl>=3.1.2,<3.2",
-    "modin[dask]>=0.23.0,<1.0",
+    "openpyxl>=3.0.7,<3.1",
+    "modin[dask]>=0.16.2,<1.0",
     "pymongo>=4.2.0,<5.0",
     "sqlalchemy>2.0",
     "toml>=0.10,<0.11",
-    "taipy-config==2.4.0.dev0",
+    "taipy-config==3.0.0.dev0",
 ]
 
 test_requirements = ["pytest>=3.8"]
 
 extras_require = {
     "fastparquet": ["fastparquet==2022.11.0"],
     "mssql": ["pyodbc>=4,<4.1"],
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_backup/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_backup/_backup.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_backup/_backup.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_core.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_core.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_core_cli.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_core_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_dag.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_dag.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_entity.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_entity_ids.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_entity_ids.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_labeled.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_labeled.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,17 @@
         return self._get_explicit_label() or self._generate_label(True)
 
     def _generate_label(self, simple=False) -> str:
         ls = []
         if not simple:
             if owner_id := self._get_owner_id():
                 if getattr(self, "id") != owner_id:
-                    from ... import core
+                    from ... import core as tp
 
-                    owner = core.get(owner_id)
+                    owner = tp.get(owner_id)
                     ls.append(owner.get_label())
         ls.append(self._generate_entity_label())
         return self.__LABEL_SEPARATOR.join(ls)
 
     def _get_explicit_label(self) -> Optional[str]:
         if hasattr(self, "_properties"):
             return getattr(self, "_properties").get("label")
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_properties.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_properties.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_reload.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_reload.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_entity/_submittable.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_entity/_submittable.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_init.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_init.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_manager/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_manager/_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_manager/_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_manager/_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_abstract_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_development_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_dispatcher/_standalone_job_dispatcher.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/_orchestrator_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_orchestrator/utils.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_orchestrator/utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/_filesystem_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_filesystem_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/_repository_adapter.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_adapter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/_sql_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_repository/_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_repository/_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/_bcolor.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_bcolor.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_cli/_version_cli.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_cli/_version_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_utils.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,23 +50,18 @@
 
     @classmethod
     def _get_or_create(cls, id: str, force: bool) -> _Version:
         if version := cls._get(id):
             comparator_result = Config._comparator._find_conflict_config(version.config, Config._applied_config, id)
             if comparator_result.get(_ComparatorResult.CONFLICTED_SECTION_KEY):
                 if force:
-                    cls.__logger.warning(
-                        f"Option --taipy-force is detected, overriding the configuration of version {id} ..."
-                    )
+                    _TaipyLogger._get_logger().warning(f"Overriding version {id} ...")
                     version.config = Config._applied_config
                 else:
-                    cls.__logger.error(
-                        "To force running the application with the changes, run your application with --taipy-force option."
-                    )
-                    raise SystemExit()
+                    raise SystemExit("The application is stopped. Please check the error log for more information.")
         else:
             version = _Version(id=id, config=Config._applied_config)
 
         cls._set(version)
         return version
 
     @classmethod
@@ -133,24 +128,15 @@
                 continue
 
             if version := cls._get(production_version):
                 comparator_result = Config._comparator._find_conflict_config(
                     version.config, Config._applied_config, production_version
                 )
                 if comparator_result.get(_ComparatorResult.CONFLICTED_SECTION_KEY):
-                    if force:
-                        cls.__logger.warning(
-                            f"Option --taipy-force is detected, the conflicted changes"
-                            f" compared to version {version.id} are ignored."
-                        )
-                    else:
-                        cls.__logger.error(
-                            "To force running the application with the changes, run your application with --taipy-force option."
-                        )
-                        raise SystemExit()
+                    raise SystemExit("The application is stopped. Please check the error log for more information.")
 
             else:
                 raise NonExistingVersion(production_version)
 
         if version_number == cls._get_development_version():
             cls._set_development_version(str(uuid.uuid4()))
 
@@ -180,15 +166,15 @@
                 return version_number
             return production_versions
 
         if version_number == cls.__LATEST_VERSION:
             return cls._get_latest_version()
         if version_number in cls.__DEVELOPMENT_VERSION:
             return cls._get_development_version()
-        if version_number == cls.__PRODUCTION_VERSION:
+        if version_number in cls.__PRODUCTION_VERSION:
             return cls._get_production_versions()
         if version_number in cls.__ALL_VERSION:
             return ""
 
         try:
             if version := cls._get(version_number):
                 return version.id
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/_version/_version_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/_version/_version_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/_listattributes.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_listattributes.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/_repr_enum.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/_utils.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_utils.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/_warnings.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/_warnings.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/default_custom_document.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/default_custom_document.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py` & `taipy-core-3.0.0.dev0/src/taipy/core/common/warn_if_inputs_not_ready.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 _inject_section(
     DataNodeConfig,
     "data_nodes",
     DataNodeConfig.default_config(),
     [
         ("configure_data_node", DataNodeConfig._configure),
         ("configure_default_data_node", DataNodeConfig._configure_default),
-        ("set_default_data_node_configuration", DataNodeConfig._set_default_configuration),
         ("configure_csv_data_node", DataNodeConfig._configure_csv),
         ("configure_json_data_node", DataNodeConfig._configure_json),
         ("configure_parquet_data_node", DataNodeConfig._configure_parquet),
         ("configure_sql_table_data_node", DataNodeConfig._configure_sql_table),
         ("configure_sql_data_node", DataNodeConfig._configure_sql),
         ("configure_mongo_collection_data_node", DataNodeConfig._configure_mongo_collection),
         ("configure_in_memory_data_node", DataNodeConfig._configure_in_memory),
@@ -57,38 +56,32 @@
         ("configure_generic_data_node", DataNodeConfig._configure_generic),
     ],
 )
 _inject_section(
     TaskConfig,
     "tasks",
     TaskConfig.default_config(),
-    [
-        ("configure_task", TaskConfig._configure),
-        ("configure_default_task", TaskConfig._configure_default),
-        ("set_default_task_configuration", TaskConfig._set_default_configuration),
-    ],
+    [("configure_task", TaskConfig._configure), ("configure_default_task", TaskConfig._configure_default)],
 )
 _inject_section(
     PipelineConfig,
     "pipelines",
     PipelineConfig.default_config(),
     [
         ("configure_pipeline", PipelineConfig._configure),
         ("configure_default_pipeline", PipelineConfig._configure_default),
-        ("set_default_pipeline_configuration", PipelineConfig._set_default_configuration),
     ],
 )
 _inject_section(
     ScenarioConfig,
     "scenarios",
     ScenarioConfig.default_config(),
     [
         ("configure_scenario", ScenarioConfig._configure),
         ("configure_default_scenario", ScenarioConfig._configure_default),
-        ("set_default_scenario_configuration", ScenarioConfig._set_default_configuration),
         ("configure_scenario_from_tasks", ScenarioConfig._configure_from_tasks),
     ],
 )
 _inject_section(
     CoreSection,
     "core",
     CoreSection.default_config(),
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_config_id_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_data_node_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_global_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_job_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_pipeline_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_scenario_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/checkers/_task_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/config.schema.json` & `taipy-core-3.0.0.dev0/src/taipy/core/config/config.schema.json`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/core_section.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/core_section.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 from taipy.config import Config, UniqueSection
 from taipy.config._config import _Config
 from taipy.config.common._template_handler import _TemplateHandler as _tpl
 
 
 class CoreSection(UniqueSection):
     """
-    Configuration parameters for running the `Core^` service.
+    Configuration fields needed to run the `Core^` service.
 
 
     Attributes:
         mode (str): The Taipy operating mode. By default, the `Core^` service runs in "development" mode.
             An "experiment" and a "production" mode are also available. Please refer to the
-            [Versioning management](../../core/versioning/) documentation page for more details.
+            [Versioning management](../../../manuals/core/versioning/index.md) documentation page.
         version_number (str)): The identifier of the user application version. Please refer to the
-            [Versioning management](../../core/versioning/) documentation page for more details.
-        force (bool): If True, force the application run even if there are some conflicts in the
+            [Versioning management](../../../manuals/core/versioning/index.md) documentation page.
+        force (bool): Parameter to force the application run even if there are some conflicts in the
             configuration.
-        clean_entities(bool): If True, remove all entities (from previous run) before running
+        clean_entities(bool): Parameter to remove all entities (from previous run) before running
             the application.
         **properties (dict[str, any]): A dictionary of additional properties.
     """
 
     name = "CORE"
     _MODE_KEY = "mode"
     _DEVELOPMENT_MODE = "development"
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/data_node_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/data_node_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,25 +357,15 @@
                 if default_value is not None and self._properties.get(optional_property) is None:
                     self._properties[optional_property] = default_value
 
     @staticmethod
     def _configure_default(
         storage_type: str, scope: Optional[Scope] = None, validity_period: Optional[timedelta] = None, **properties
     ) -> "DataNodeConfig":
-        """
-        Deprecated since taipy version 2.3.2. Use set_default_data_node_configuration instead.
-        """
-        _warn_deprecated("configure_default_data_node", suggest="set_default_data_node_configuration")
-        return DataNodeConfig._set_default_configuration(storage_type, scope, validity_period, **properties)
-
-    @staticmethod
-    def _set_default_configuration(
-        storage_type: str, scope: Optional[Scope] = None, validity_period: Optional[timedelta] = None, **properties
-    ) -> "DataNodeConfig":
-        """Set the default values for data node configurations.
+        """Configure the default values for data node configurations.
 
         This function creates the _default data node configuration_ object,
         where all data node configuration objects will find their default
         values when needed.
 
         Parameters:
             storage_type (str): The default storage type for all data node configurations.
@@ -410,20 +400,20 @@
         """Configure a new data node configuration.
 
         Parameters:
             id (str): The unique identifier of the new data node configuration.
             storage_type (Optional[str]): The data node configuration storage type. The possible values
                 are None (which is the default value of *"pickle"*, unless it has been overloaded by the
                 *storage_type* value set in the default data node configuration
-                (see `(Config.)set_default_data_node_configuration()^`)), *"pickle"*, *"csv"*, *"excel"*,
+                (see `(Config.)configure_default_data_node()^`)), *"pickle"*, *"csv"*, *"excel"*,
                 *"sql_table"*, *"sql"*, *"json"*, *"parquet"*, *"mongo_collection"*, *"in_memory"*, or
                 *"generic"*.
             scope (Optional[Scope^]): The scope of the data node configuration.<br/>
                 The default value is `Scope.SCENARIO` (or the one specified in
-                `(Config.)set_default_data_node_configuration()^`).
+                `(Config.)configure_default_data_node()^`).
             validity_period (Optional[timedelta]): The duration since the last edit date for which the data node can be
                 considered up-to-date. Once the validity period has passed, the data node is considered stale and
                 relevant tasks will run even if they are skippable (see the
                 [Task configs page](../core/config/task-config.md) for more details).
                 If *validity_period* is set to None, the data node is always up-to-date.
             **properties (dict[str, any]): A keyworded variable length list of additional arguments.
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/job_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/job_config.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/pipeline_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/pipeline_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,23 +102,15 @@
         section = PipelineConfig(id, task_configs, **properties)
         Config._register(section)
         _warn_deprecated("PipelineConfig")
         return Config.sections[PipelineConfig.name][id]
 
     @staticmethod
     def _configure_default(task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
-        """
-        Deprecated since taipy version 2.3.2. Use set_default_pipeline_configuration() instead.
-        """
-        _warn_deprecated("configure_default_pipeline", suggest="set_default_pipeline_configuration")
-        return PipelineConfig._set_default_configuration(task_configs, **properties)
-
-    @staticmethod
-    def _set_default_configuration(task_configs: Union[TaskConfig, List[TaskConfig]], **properties) -> "PipelineConfig":
-        """Set the default values for pipeline configurations.
+        """Configure the default values for pipeline configurations.
 
         This function creates the *default pipeline configuration* object,
         where all pipeline configuration objects will find their default
         values when needed.
 
         Parameters:
             task_configs (Union[TaskConfig^, List[TaskConfig^]]): The list of the task
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/scenario_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/scenario_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,28 +211,15 @@
     @staticmethod
     def _configure_default(
         pipeline_configs: List[PipelineConfig],
         frequency: Optional[Frequency] = None,
         comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
         **properties,
     ) -> "ScenarioConfig":
-        """
-        Deprecated since taipy version 2.3.2. Use set_default_scenario_configuration() instead.
-        """
-        _warn_deprecated("configure_default_scenario", suggest="set_default_scenario_configuration")
-        return ScenarioConfig._set_default_configuration(pipeline_configs, frequency, comparators, **properties)
-
-    @staticmethod
-    def _set_default_configuration(
-        pipeline_configs: List[PipelineConfig],
-        frequency: Optional[Frequency] = None,
-        comparators: Optional[Dict[str, Union[List[Callable], Callable]]] = None,
-        **properties,
-    ) -> "ScenarioConfig":
-        """Set the default values for scenario configurations.
+        """Configure the default values for scenario configurations.
 
         This function creates the *default scenario configuration* object,
         where all scenario configuration objects will find their default
         values when needed.
 
         Parameters:
             pipeline_configs (List[PipelineConfig^]): The list of pipeline configurations used
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/config/task_config.py` & `taipy-core-3.0.0.dev0/src/taipy/core/config/task_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -188,29 +188,15 @@
     def _configure_default(
         function,
         input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
         skippable: Optional[bool] = False,
         **properties,
     ) -> "TaskConfig":
-        """
-        Deprecated since taipy version 2.3.2. Use set_default_task_configuration() instead.
-        """
-        _warn_deprecated("configure_default_task", suggest="set_default_task_configuration")
-        return TaskConfig._set_default_configuration(function, input, output, skippable, **properties)
-
-    @staticmethod
-    def _set_default_configuration(
-        function,
-        input: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
-        output: Optional[Union[DataNodeConfig, List[DataNodeConfig]]] = None,
-        skippable: Optional[bool] = False,
-        **properties,
-    ) -> "TaskConfig":
-        """Sets the default values for task configurations.
+        """Configure the default values for task configurations.
 
         This function creates the *default task configuration* object,
         where all task configuration objects will find their default
         values when needed.
 
         Parameters:
             function (Callable): The python function called by Taipy to run the task.
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/_cycle_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/cycle.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/cycle/cycle_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/cycle/cycle_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_data_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_data_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/_filter.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/_filter.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/abstract_file.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_file.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/abstract_sql.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/abstract_sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/csv.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/csv.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/data_node.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/data_node.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/data_node_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/data_node_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/excel.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/excel.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/generic.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/generic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/in_memory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/in_memory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/json.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/json.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/mongo.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/mongo.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/operator.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/operator.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/parquet.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/parquet.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/pickle.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/pickle.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/sql.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/sql.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/data/sql_table.py` & `taipy-core-3.0.0.dev0/src/taipy/core/data/sql_table.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/exceptions/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/exceptions/exceptions.py` & `taipy-core-3.0.0.dev0/src/taipy/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/_job_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/_job_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/job.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/job.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/job_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/job_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/job/status.py` & `taipy-core-3.0.0.dev0/src/taipy/core/job/status.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/core_event_consumer.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/core_event_consumer.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/event.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/event.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/notifier.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/registration.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/registration.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/registration_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/registration_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/notification/topic.py` & `taipy-core-3.0.0.dev0/src/taipy/core/notification/topic.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/_pipeline_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/pipeline.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/pipeline/pipeline_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/pipeline/pipeline_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/_scenario_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/scenario.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/scenario/scenario_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/scenario/scenario_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/taipy.py` & `taipy-core-3.0.0.dev0/src/taipy/core/taipy.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/__init__.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_fs_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_fs_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_manager.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_manager_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_manager_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_model.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_model.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_repository_factory.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_repository_factory.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/_task_sql_repository.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/_task_sql_repository.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/task.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/task.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy/core/task/task_id.py` & `taipy-core-3.0.0.dev0/src/taipy/core/task/task_id.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/src/taipy_core.egg-info/PKG-INFO` & `taipy-core-3.0.0.dev0/src/taipy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-core
-Version: 2.4.0.dev0
+Version: 3.0.0.dev0
 Summary: A Python library to build powerful and customized data-driven back-end applications.
 Home-page: https://github.com/avaiga/taipy-core
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-core
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-core-2.4.0.dev0/src/taipy_core.egg-info/SOURCES.txt` & `taipy-core-3.0.0.dev0/src/taipy_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/tests/test_complex_application.py` & `taipy-core-3.0.0.dev0/tests/test_complex_application.py`

 * *Files identical despite different names*

### Comparing `taipy-core-2.4.0.dev0/tests/test_taipy.py` & `taipy-core-3.0.0.dev0/tests/test_taipy.py`

 * *Files identical despite different names*

