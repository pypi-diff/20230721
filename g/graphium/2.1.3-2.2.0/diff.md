# Comparing `tmp/graphium-2.1.3.tar.gz` & `tmp/graphium-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphium-2.1.3.tar", last modified: Tue Jul 11 19:58:50 2023, max compression
+gzip compressed data, was "graphium-2.2.0.tar", last modified: Fri Jul 21 15:27:54 2023, max compression
```

## Comparing `graphium-2.1.3.tar` & `graphium-2.2.0.tar`

### file list

```diff
@@ -1,330 +1,356 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.387511 graphium-2.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.315511 graphium-2.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.315511 graphium-2.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 19:53:38.000000 graphium-2.1.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-11 19:53:38.000000 graphium-2.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-11 19:53:38.000000 graphium-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:58:50.387511 graphium-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-11 19:53:38.000000 graphium-2.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:53:38.000000 graphium-2.1.3/cleanup_files.sh
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 19:53:38.000000 graphium-2.1.3/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.315511 graphium-2.1.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.307511 graphium-2.1.3/docs/_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/_assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/_assets/css/custom-graphium.css
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/_assets/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/_assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/_assets/js/google-analytics.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.config.md
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.data.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.features.md
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.ipu.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/api/graphium.nn/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/architectures.md
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/encoders.md
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/graphium.nn.md
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.nn/pyg_layers.md
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.trainer.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.utils.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/api/graphium.visualization.md
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/baseline.md
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/cli_references.md
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/datasets.md
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/design.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.319511 graphium-2.1.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/datamodule.png
--rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/full_graph_network.png
--rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/pretrained_models.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.307511 graphium-2.1.3/docs/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/docs/tutorials/feature_processing/
--rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/choosing_parallelization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/csv_to_parquet.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/feature_processing/timing_parallel.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/docs/tutorials/gnn/
--rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/gnn/add_new_gnn_layers.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/gnn/making_gnn_networks.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/gnn/using_gnn_layers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/docs/tutorials/model_training/
--rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/model_training/running-multitask-ipu.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-11 19:53:38.000000 graphium-2.1.3/docs/tutorials/model_training/simple-molecular-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 19:53:38.000000 graphium-2.1.3/env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.323511 graphium-2.1.3/expts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m_mod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_gpspp_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_mpnn_10M_b3lyp.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_mpnn_10M_pcqm4m.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/configs/config_mpnn_pcqm4m.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/data/micro_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/data/tiny_zinc_splits.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4492 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/dataset_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_get_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/main_run_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/neurips2023_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.327511 graphium-2.1.3/expts/neurips2023_configs/baseline/
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_classifigression_l1000.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13812 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_large_mpnn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_luis_jama.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gated_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gcn.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_gine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/config_small_mpnn.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/debug/
--rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/debug/config_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13909 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/run_validation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-11 19:53:38.000000 graphium-2.1.3/expts/test_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.331511 graphium-2.1.3/graphium/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.335511 graphium-2.1.3/graphium/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.339511 graphium-2.1.3/graphium/config/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/_load.py
--rw-r--r--   0 runner    (1001) docker     (123)    20164 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/config_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/fake_multilevel_multitask_pyg.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/config/zinc_default_multitask_pyg.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.339511 graphium-2.1.3/graphium/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.339511 graphium-2.1.3/graphium/data/L1000/
--rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/QM9/
--rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/QM9/micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/QM9/micro_qm9.parquet
--rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/QM9/norm_micro_qm9.csv
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)   108384 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    28207 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/make_data_splits/
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/micro_ZINC/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/micro_ZINC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/micro_ZINC/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multilevel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/multitask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/tiny_ZINC_SA.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/tiny_ZINC_logp.csv
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/multitask/tiny_ZINC_score.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/sdf2csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/data/single_atom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/single_atom_dataset/single_atom_dataset.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/smiles_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.343511 graphium-2.1.3/graphium/expts/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/expts/pyg_batching_sparse.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.347511 graphium-2.1.3/graphium/features/
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/commute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/electrostatic.py
--rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/graphormer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/nmp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/periodic_table.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/test_new_pes.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/features/transfer_pos_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.347511 graphium-2.1.3/graphium/ipu/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_simple_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/ipu_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/ipu/to_dense_batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.351511 graphium-2.1.3/graphium/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.351511 graphium-2.1.3/graphium/nn/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/encoder_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    73133 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/global_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/architectures/pyg_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/base_graph_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/base_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.351511 graphium-2.1.3/graphium/nn/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/bessel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/laplace_pos_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/mlp_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/encoders/signnet_pos_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.355511 graphium-2.1.3/graphium/nn/pyg_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/dimenet_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gated_gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gcn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gin_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/gps_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/mpnn_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/pna_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12706 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/pooling_pyg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/pyg_layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.355511 graphium-2.1.3/graphium/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/predictor_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/trainer/predictor_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.359511 graphium-2.1.3/graphium/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/arg_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/custom_lr.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/moving_average_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/mup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13672 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/read_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/safe_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/utils/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.359511 graphium-2.1.3/graphium/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/visualization/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 19:53:38.000000 graphium-2.1.3/graphium/visualization/vis_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.335511 graphium-2.1.3/graphium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 19:58:50.000000 graphium-2.1.3/graphium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-11 19:53:38.000000 graphium-2.1.3/lightning.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-11 19:53:38.000000 graphium-2.1.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.363511 graphium-2.1.3/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-datamodule-invalidate-cache.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-datamodule-ogb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-datamodule.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-pretrained.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev-training-loop.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/dev.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/running-fingerprints-from-pretrained-model.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-11 19:53:38.000000 graphium-2.1.3/notebooks/running-model-from-config.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.363511 graphium-2.1.3/profiling/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/configs_profiling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/profile_mol_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/profile_one_of_k_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-11 19:53:38.000000 graphium-2.1.3/profiling/profile_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-11 19:53:38.000000 graphium-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-11 19:53:38.000000 graphium-2.1.3/requirements_ipu.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.363511 graphium-2.1.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-11 19:53:38.000000 graphium-2.1.3/scripts/convert_yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:53:38.000000 graphium-2.1.3/scripts/ipu_start.sh
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 19:53:38.000000 graphium-2.1.3/scripts/ipu_venv.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:58:50.387511 graphium-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.383511 graphium-2.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/config_test_ipu_dataloader.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/converted_fake_multilevel_data.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:58:50.383511 graphium-2.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/config_micro_ZINC.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_corrupt.csv
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_1.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/micro_ZINC_shard_2.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/data/pcqm4mv2-2k.csv
--rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/fake_and_missing_multilevel_data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_base_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_dict_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_ipu_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_ipu_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35726 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_ipu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_mtl_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_multitask_datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_mup.py
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_packing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pe_nodepair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pe_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pe_spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pos_transfer_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_positional_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_positional_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_pyg_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_residual_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-11 19:53:38.000000 graphium-2.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.604559 graphium-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.560558 graphium-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-21 15:23:32.000000 graphium-2.2.0/.github/workflows/test_ipu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-21 15:23:32.000000 graphium-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-07-21 15:23:32.000000 graphium-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-21 15:27:54.600559 graphium-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-21 15:23:32.000000 graphium-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 15:23:32.000000 graphium-2.2.0/cleanup_files.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-21 15:23:32.000000 graphium-2.2.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.556558 graphium-2.2.0/docs/_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/docs/_assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/_assets/css/custom-graphium.css
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/_assets/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/docs/_assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/_assets/js/google-analytics.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.config.md
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.features.md
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.ipu.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/docs/api/graphium.nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.nn/architectures.md
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.nn/encoders.md
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.nn/graphium.nn.md
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.nn/pyg_layers.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.trainer.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.utils.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/api/graphium.visualization.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/baseline.md
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/cli_references.md
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/datasets.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/design.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.564558 graphium-2.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   269957 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/images/datamodule.png
+-rw-r--r--   0 runner    (1001) docker     (123)   270126 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/images/full_graph_network.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46468 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/pretrained_models.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.556558 graphium-2.2.0/docs/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/docs/tutorials/feature_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)    12699 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/feature_processing/choosing_parallelization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/feature_processing/csv_to_parquet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/feature_processing/timing_parallel.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/docs/tutorials/gnn/
+-rw-r--r--   0 runner    (1001) docker     (123)    23274 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/gnn/add_new_gnn_layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/gnn/making_gnn_networks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/gnn/using_gnn_layers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/docs/tutorials/model_training/
+-rw-r--r--   0 runner    (1001) docker     (123)    24708 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/model_training/running-multitask-ipu.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-21 15:23:32.000000 graphium-2.2.0/docs/tutorials/model_training/simple-molecular-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-21 15:23:32.000000 graphium-2.2.0/env.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_gps_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_gps_10M_pcqm4m_mod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_gpspp_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_mpnn_10M_b3lyp.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_mpnn_10M_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7654 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_mpnn_pcqm4m.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/configs/config_tdc_admet_demo.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/data/micro_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/data/tiny_zinc_splits.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/dataset_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/debug_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/hydra-configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/hydra-configs/accelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/accelerator/cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/accelerator/gpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/accelerator/ipu.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/hydra-configs/dataset/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/hydra-configs/dataset/accelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/dataset/accelerator/toymix_cpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/dataset/accelerator/toymix_gpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/dataset/accelerator/toymix_ipu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/dataset/toymix.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/hydra-configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/experiment/toymix_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/experiment/toymix_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/main.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.568558 graphium-2.2.0/expts/hydra-configs/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/model/gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/hydra-configs/model/gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/main_run_get_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/main_run_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/main_run_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/main_run_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.572558 graphium-2.2.0/expts/neurips2023_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.572558 graphium-2.2.0/expts/neurips2023_configs/baseline/
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_classifigression_l1000.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14345 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_large_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_large_gcn_gpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_large_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_large_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_large_mpnn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_luis_jama.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_small_gated_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11432 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_small_gcn.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_small_gcn_gpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_small_gin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_small_gine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/config_small_mpnn.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.572558 graphium-2.2.0/expts/neurips2023_configs/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/debug/config_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    14405 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.572558 graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.572558 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8458 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8226 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9903 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8664 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-07-21 15:23:32.000000 graphium-2.2.0/expts/run_validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/graphium/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/graphium/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/cli/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/cli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/graphium/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/config_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5228 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/fake_multilevel_multitask_pyg.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/config/zinc_default_multitask_pyg.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/graphium/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/graphium/data/L1000/
+-rw-r--r--   0 runner    (1001) docker     (123)   450311 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.580558 graphium-2.2.0/graphium/data/QM9/
+-rw-r--r--   0 runner    (1001) docker     (123)   225339 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/QM9/micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   191173 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/QM9/micro_qm9.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)   396078 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/QM9/norm_micro_qm9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13677 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118056 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27435 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.580558 graphium-2.2.0/graphium/data/make_data_splits/
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.580558 graphium-2.2.0/graphium/data/micro_ZINC/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/micro_ZINC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76831 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/micro_ZINC/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/multilevel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.580558 graphium-2.2.0/graphium/data/multitask/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/multitask/tiny_ZINC_SA.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/multitask/tiny_ZINC_logp.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/multitask/tiny_ZINC_score.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/sdf2csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.580558 graphium-2.2.0/graphium/data/single_atom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/single_atom_dataset/single_atom_dataset.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/smiles_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.580558 graphium-2.2.0/graphium/expts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/expts/pyg_batching_sparse.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.584559 graphium-2.2.0/graphium/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/commute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/electrostatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47012 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/graphormer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/nmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/periodic_table.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51424 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/test_new_pes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/features/transfer_pos_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.584559 graphium-2.2.0/graphium/ipu/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36460 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/ipu_simple_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/ipu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/ipu_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/ipu/to_dense_batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.584559 graphium-2.2.0/graphium/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.584559 graphium-2.2.0/graphium/nn/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/architectures/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12326 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/architectures/encoder_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73339 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/architectures/global_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/architectures/pyg_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/base_graph_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27672 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/base_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.588559 graphium-2.2.0/graphium/nn/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/bessel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/gaussian_kernel_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9931 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/laplace_pos_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/mlp_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/encoders/signnet_pos_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.588559 graphium-2.2.0/graphium/nn/pyg_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/dimenet_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/gated_gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/gcn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/gin_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/gps_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13289 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/mpnn_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10582 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/pna_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12710 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/pooling_pyg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/pyg_layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19115 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.588559 graphium-2.2.0/graphium/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30800 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/predictor_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/trainer/predictor_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.592559 graphium-2.2.0/graphium/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/arg_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/custom_lr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10154 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/moving_average_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/read_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/safe_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/utils/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.592559 graphium-2.2.0/graphium/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/visualization/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-21 15:23:32.000000 graphium-2.2.0/graphium/visualization/vis_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.576558 graphium-2.2.0/graphium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-21 15:27:54.000000 graphium-2.2.0/graphium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-07-21 15:27:54.000000 graphium-2.2.0/graphium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 15:27:54.000000 graphium-2.2.0/graphium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 15:27:54.000000 graphium-2.2.0/graphium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-21 15:27:54.000000 graphium-2.2.0/graphium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 15:27:54.000000 graphium-2.2.0/graphium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-07-21 15:23:32.000000 graphium-2.2.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.592559 graphium-2.2.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    15328 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/dev-datamodule-invalidate-cache.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12792 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/dev-datamodule-ogb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/dev-datamodule.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/dev-pretrained.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/dev-training-loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/dev.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    51885 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/finetuning-on-tdc-admet-benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/running-fingerprints-from-pretrained-model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-21 15:23:32.000000 graphium-2.2.0/notebooks/running-model-from-config.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.592559 graphium-2.2.0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-21 15:23:32.000000 graphium-2.2.0/profiling/configs_profiling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-21 15:23:32.000000 graphium-2.2.0/profiling/profile_mol_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-21 15:23:32.000000 graphium-2.2.0/profiling/profile_one_of_k_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-21 15:23:32.000000 graphium-2.2.0/profiling/profile_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-21 15:23:32.000000 graphium-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-21 15:23:32.000000 graphium-2.2.0/requirements_ipu.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.592559 graphium-2.2.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-21 15:23:32.000000 graphium-2.2.0/scripts/convert_yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-21 15:23:32.000000 graphium-2.2.0/scripts/ipu_start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-21 15:23:32.000000 graphium-2.2.0/scripts/ipu_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 15:27:54.604559 graphium-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.600559 graphium-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/config_test_ipu_dataloader.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/config_test_ipu_dataloader_multitask.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   934751 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/converted_fake_multilevel_data.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 15:27:54.600559 graphium-2.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/config_micro_ZINC.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    76617 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/micro_ZINC.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33023 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/micro_ZINC_corrupt.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/micro_ZINC_shard_1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/micro_ZINC_shard_1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/micro_ZINC_shard_2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/micro_ZINC_shard_2.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1504570 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/data/pcqm4mv2-2k.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   931712 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/fake_and_missing_multilevel_data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)    29755 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_base_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17091 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_dict_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_ipu_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_ipu_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35757 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_ipu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_ipu_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_ipu_to_dense_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_mtl_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_multitask_datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_mup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_packing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_pe_nodepair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_pe_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_pe_spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_pos_transfer_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_positional_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_positional_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_pyg_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_residual_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-21 15:23:32.000000 graphium-2.2.0/tests/test_utils.py
```

### Comparing `graphium-2.1.3/.github/CODE_OF_CONDUCT.md` & `graphium-2.2.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/.github/PULL_REQUEST_TEMPLATE.md` & `graphium-2.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/.github/workflows/code-check.yml` & `graphium-2.2.0/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/.github/workflows/doc.yml` & `graphium-2.2.0/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/.github/workflows/release.yml` & `graphium-2.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/.github/workflows/test.yml` & `graphium-2.2.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -13,26 +13,27 @@
 
 jobs:
   test:
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10"]
-        pytorch-version: ["1.13"]
+        pytorch-version: ["2.0"]
 
     runs-on: "ubuntu-latest"
     timeout-minutes: 30
 
     defaults:
       run:
         shell: bash -l {0}
 
     name: |
-      python=${{ matrix.python-version }} -
-      pytorch=${{ matrix.pytorch-version }}
+        regular_env -
+        python=${{ matrix.python-version }} -
+        pytorch=${{ matrix.pytorch-version }}
 
     steps:
       - name: Checkout the code
         uses: actions/checkout@v3
 
       - name: Setup mamba
         uses: mamba-org/setup-micromamba@v1
@@ -45,24 +46,24 @@
             python=${{ matrix.python-version }}
             pytorch=${{ matrix.pytorch-version }}
 
       - name: Install library
         run: python -m pip install --no-deps -e . # `-e` required for correct `coverage` run.
 
       - name: Run tests
-        run: pytest
+        run: pytest -m 'not ipu'
+
+      - name: Test CLI
+        run: graphium --help
+
+      - name: Test building the doc
+        run: mkdocs build
 
       - name: Codecov Upload
         uses: codecov/codecov-action@v3
         with:
           files: ./coverage.xml
           flags: unittests
           name: codecov-umbrella
           fail_ci_if_error: false
           verbose: false
           env_vars: ${{ matrix.python-version }},${{ matrix.pytorch-version }}
-
-      - name: Test CLI
-        run: graphium --help
-
-      - name: Test building the doc
-        run: mkdocs build
```

### Comparing `graphium-2.1.3/.gitignore` & `graphium-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/LICENSE` & `graphium-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/PKG-INFO` & `graphium-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,7 @@
-Metadata-Version: 2.1
-Name: graphium
-Version: 2.1.3
-Summary: Graphium: Scaling molecular GNNs to infinity.
-Author-email: Dominique Beaini <dominique@valencediscovery.com>
-Project-URL: Website, https://graphium.datamol.io/
-Project-URL: Source Code, https://github.com/datamol-io/graphium
-Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
-Project-URL: Documentation, https://graphium-docs.datamol.io/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Healthcare Industry
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
     <img src="docs/images/logo.png" height="200px">
     <h3>Scaling molecular GNNs to infinity</h3>
 </div>
 
 ---
 
@@ -39,18 +10,20 @@
 [![Conda](https://img.shields.io/conda/v/conda-forge/graphium?label=conda&color=success)](https://anaconda.org/conda-forge/graphium)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/graphium)](https://pypi.org/project/graphium/)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/graphium)](https://anaconda.org/conda-forge/graphium)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/graphium/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/graphium)](https://github.com/datamol-io/graphium/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/graphium)](https://github.com/datamol-io/graphium/network/members)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
+[![test-ipu](https://github.com/datamol-io/graphium/actions/workflows/test_ipu.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test_ipu.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
 [![codecov](https://codecov.io/gh/datamol-io/graphium/branch/main/graph/badge.svg?token=bHOkKY5Fze)](https://codecov.io/gh/datamol-io/graphium)
+[![hydra](https://img.shields.io/badge/Config-Hydra_1.3-89b8cd)](https://hydra.cc/)
 
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
@@ -90,27 +63,47 @@
 # Install the PopTorch wheel
 pip install PATH_TO_SDK/poptorch-3.2.0+109946_bb50ce43ab_ubuntu_20_04-cp38-cp38-linux_x86_64.whl
 
 # Enable Poplar SDK (including Poplar and PopART)
 source PATH_TO_SDK/enable
 
 # Install the IPU specific and graphium requirements
-PACKAGE_NAME=pytorch pip install -r requirements_ipu.txt
-pip install -r lightning.txt
+pip install -r requirements_ipu.txt
 
 # Install Graphium in dev mode
 pip install --no-deps -e .
 ```
 
 ## Training a model
 
 To learn how to train a model, we invite you to look at the documentation, or the jupyter notebooks available [here](https://github.com/datamol-io/graphium/tree/master/docs/tutorials/model_training).
 
 If you are not familiar with [PyTorch](https://pytorch.org/docs) or [PyTorch-Lightning](https://pytorch-lightning.readthedocs.io/en/latest/), we highly recommend going through their tutorial first.
 
+## Running an experiment
+We have setup Graphium with `hydra` for managing config files. To run an experiment go to the `expts/` folder. For example, to benchmark a GCN on the ToyMix dataset run
+```bash
+python main_run_multitask.py dataset=toymix model=gcn
+```
+To change parameters specific to this experiment like switching from `fp16` to `fp32` precision, you can either override them directly in the CLI via
+```bash
+python main_run_multitask.py dataset=toymix model=gcn trainer.trainer.precision=32
+```
+or change them permamently in the dedicated experiment config under `expts/hydra-configs/toymix_gcn.yaml`.
+Integrating `hydra` also allows you to quickly switch between accelerators. E.g., running
+```bash
+python main_run_multitask.py dataset=toymix model=gcn accelerator=gpu
+```
+automatically selects the correct configs to run the experiment on GPU.
+To use a config file you built from scratch you can run
+```bash
+python main_run_multitask.py --config-path [PATH] --config-name [CONFIG]
+```
+Thanks to the modular nature of `hydra` you can reuse many of our config settings for your own experiments with Graphium.
+
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
 
 ## Documentation
 
 - Diagram for data processing in molGPS.
```

### Comparing `graphium-2.1.3/docs/_assets/css/custom-graphium.css` & `graphium-2.2.0/docs/_assets/css/custom-graphium.css`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/_assets/css/custom.css` & `graphium-2.2.0/docs/_assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/api/graphium.features.md` & `graphium-2.2.0/docs/api/graphium.features.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/api/graphium.ipu.md` & `graphium-2.2.0/docs/api/graphium.ipu.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/api/graphium.nn/encoders.md` & `graphium-2.2.0/docs/api/graphium.nn/encoders.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/api/graphium.nn/pyg_layers.md` & `graphium-2.2.0/docs/api/graphium.nn/pyg_layers.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/api/graphium.utils.md` & `graphium-2.2.0/docs/api/graphium.utils.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/baseline.md` & `graphium-2.2.0/docs/baseline.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/datasets.md` & `graphium-2.2.0/docs/datasets.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/design.md` & `graphium-2.2.0/docs/design.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/images/datamodule.png` & `graphium-2.2.0/docs/images/datamodule.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/images/full_graph_network.png` & `graphium-2.2.0/docs/images/full_graph_network.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/images/logo.png` & `graphium-2.2.0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/images/logo.svg` & `graphium-2.2.0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/index.md` & `graphium-2.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/pretrained_models.md` & `graphium-2.2.0/docs/pretrained_models.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb` & `graphium-2.2.0/docs/tutorials/feature_processing/add_new_positional_encoding.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/feature_processing/choosing_parallelization.ipynb` & `graphium-2.2.0/docs/tutorials/feature_processing/choosing_parallelization.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/feature_processing/csv_to_parquet.ipynb` & `graphium-2.2.0/docs/tutorials/feature_processing/csv_to_parquet.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/feature_processing/timing_parallel.ipynb` & `graphium-2.2.0/docs/tutorials/feature_processing/timing_parallel.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/gnn/add_new_gnn_layers.ipynb` & `graphium-2.2.0/docs/tutorials/gnn/add_new_gnn_layers.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/gnn/making_gnn_networks.ipynb` & `graphium-2.2.0/docs/tutorials/gnn/making_gnn_networks.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/gnn/using_gnn_layers.ipynb` & `graphium-2.2.0/docs/tutorials/gnn/using_gnn_layers.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/model_training/running-multitask-ipu.ipynb` & `graphium-2.2.0/docs/tutorials/model_training/running-multitask-ipu.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/docs/tutorials/model_training/simple-molecular-model.ipynb` & `graphium-2.2.0/docs/tutorials/model_training/simple-molecular-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/env.yml` & `graphium-2.2.0/env.yml`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   # cloud IO
   - fsspec >=2021.6
   - s3fs >=2021.6
   - gcsfs >=2021.6
 
   # ML packages
   - cudatoolkit # works also with CPU-only system.
-  - pytorch >=1.10.2,<2.0
+  - pytorch >=1.12
   - lightning >=2.0
   - torchmetrics >=0.7.0,<0.11
   - ogb
   - pytorch_geometric >=2.0 # Use `pyg` for Windows instead of `pytorch_geometric`
   - wandb
   - mup
   - pytorch_sparse >=0.6
@@ -67,7 +67,8 @@
   - mkdocs-jupyter
   - mkdocs-click
   - markdown-include
   - mike >=1.0.0
 
   - pip:
       - lightning-graphcore # optional, for using IPUs only
+      - hydra-core>=1.3.2
```

### Comparing `graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m.yaml` & `graphium-2.2.0/expts/configs/config_gps_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/configs/config_gps_10M_pcqm4m_mod.yaml` & `graphium-2.2.0/expts/configs/config_gps_10M_pcqm4m_mod.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/configs/config_gpspp_10M_pcqm4m.yaml` & `graphium-2.2.0/expts/configs/config_gpspp_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/configs/config_mpnn_10M_b3lyp.yaml` & `graphium-2.2.0/expts/configs/config_mpnn_10M_b3lyp.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/configs/config_mpnn_10M_pcqm4m.yaml` & `graphium-2.2.0/expts/configs/config_mpnn_10M_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/configs/config_mpnn_pcqm4m.yaml` & `graphium-2.2.0/expts/configs/config_mpnn_pcqm4m.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/data/micro_zinc_splits.csv` & `graphium-2.2.0/expts/data/micro_zinc_splits.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/dataset_benchmark.py` & `graphium-2.2.0/expts/dataset_benchmark.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from os.path import dirname, abspath
 import yaml
 from omegaconf import DictConfig
 from datetime import datetime
 from copy import deepcopy
 
 import graphium
-from graphium.config._loader import load_datamodule
+from graphium.config._loader import load_datamodule, load_accelerator
 import time
 from typing import Optional, List, Sequence
 import wandb
 import statistics
 import tqdm
 import torch
 import numpy as np
 
 # Set up the working directory
 MAIN_DIR = dirname(dirname(abspath(graphium.__file__)))
 os.chdir(MAIN_DIR)
-CONFIG_FILE = "expts/configs/config_pcqmv2_mpnn.yaml"
+# CONFIG_FILE = "expts/neurips2023_configs/debug/config_large_gcn_debug.yaml"
+CONFIG_FILE = "expts/neurips2023_configs/config_large_gcn.yaml"
+# CONFIG_FILE = "expts/configs/config_pcqmv2_mpnn.yaml"
 # CONFIG_FILE = "expts/configs/config_ipu_qm9.yaml"
 
 
 def benchmark(fn, *args, message="", log2wandb=False, **kwargs):
     start = time.time()
     value = fn(*args, **kwargs)
     duration = time.time() - start
@@ -86,17 +88,19 @@
     if add_date_time:
         run_name += "_" + datetime.now().strftime("%d.%m.%Y_%H.%M.%S")
 
     if log2wandb:
         wandb.init(project="multitask-gnn", name=run_name, config=cfg)
 
     cfg = deepcopy(cfg)
-
+    cfg, accelerator_type = load_accelerator(cfg)
     # Load and initialize the dataset
-    datamodule = benchmark(load_datamodule, cfg, message="Load duration", log2wandb=log2wandb)
+    datamodule = benchmark(
+        load_datamodule, cfg, accelerator_type, message="Load duration", log2wandb=log2wandb
+    )
 
     benchmark(datamodule.prepare_data, message="Prepare duration", log2wandb=log2wandb)
 
     if False:  # stages is not None:
         for stage in stages:
             benchmark(datamodule.setup, stage, message=f"Setup {stage} duration", log2wandb=log2wandb)
     else:
```

### Comparing `graphium-2.1.3/expts/main_run_get_fingerprints.py` & `graphium-2.2.0/expts/main_run_get_fingerprints.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/main_run_multitask.py` & `graphium-2.2.0/expts/run_validation_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,61 +4,61 @@
 from os.path import dirname, abspath
 import yaml
 from copy import deepcopy
 from omegaconf import DictConfig
 import timeit
 from loguru import logger
 from datetime import datetime
-from lightning.pytorch.utilities.model_summary import ModelSummary
+from pytorch_lightning.utilities.model_summary import ModelSummary
 
 # Current project imports
 import graphium
 from graphium.config._loader import (
     load_datamodule,
     load_metrics,
     load_architecture,
     load_predictor,
     load_trainer,
     save_params_to_wandb,
     load_accelerator,
     load_yaml_config,
 )
 from graphium.utils.safe_run import SafeRun
-from graphium.utils.command_line_utils import update_config, get_anchors_and_aliases
 
 
 # WandB
 import wandb
 
 # Set up the working directory
 MAIN_DIR = dirname(dirname(abspath(graphium.__file__)))
 
 # CONFIG_FILE = "expts/configs/config_mpnn_10M_b3lyp.yaml"
 # CONFIG_FILE = "expts/configs/config_mpnn_10M_pcqm4m.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_debug.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_large_mpnn.yaml"
-CONFIG_FILE = "expts/neurips2023_configs/debug/config_small_gcn_debug.yaml"
-# CONFIG_FILE = "expts/neurips2023_configs/config_large_gin.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_large_gcn.yaml"
+CONFIG_FILE = "expts/neurips2023_configs/debug/config_large_gcn_debug.yaml"
+# CONFIG_FILE = "expts/neurips2023_configs/config_large_gin.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_large_gine.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_small_gcn.yaml"
-# CONFIG_FILE = "expts/neurips2023_configs/config_small_gin.yaml"
+# CONFIG_FILE = "expts/neurips2023_configs/config_large_gcn.yaml"
+# CONFIG_FILE = "exptas/neurips2023_configs/config_small_gin.yaml"
 # CONFIG_FILE = "expts/neurips2023_configs/config_small_gine.yaml"
-
 os.chdir(MAIN_DIR)
 
 
-def main(cfg: dict, run_name: str = "main", add_date_time: bool = True) -> None:
+def main(cfg: DictConfig, run_name: str = "main", add_date_time: bool = True) -> None:
     st = timeit.default_timer()
 
     date_time_suffix = ""
     if add_date_time:
         date_time_suffix = datetime.now().strftime("%d.%m.%Y_%H.%M.%S")
 
-    wandb.init(entity="multitask-gnn", project=cfg["constants"]["name"], config=cfg)
+    cfg = deepcopy(cfg)
+    wandb.init(project=cfg["constants"]["name"], config=cfg)
 
     # Initialize the accelerator
     cfg, accelerator_type = load_accelerator(cfg)
 
     # Load and initialize the dataset
     datamodule = load_datamodule(cfg, accelerator_type)
 
@@ -72,35 +72,38 @@
 
     metrics = load_metrics(cfg)
     logger.info(metrics)
 
     predictor = load_predictor(
         cfg, model_class, model_kwargs, metrics, accelerator_type, datamodule.task_norms
     )
-
     logger.info(predictor.model)
     logger.info(ModelSummary(predictor, max_depth=4))
 
     trainer = load_trainer(cfg, run_name, accelerator_type, date_time_suffix)
     save_params_to_wandb(trainer.logger, cfg, predictor, datamodule)
 
     # Determine the max num nodes and edges in training and validation
-    logger.info("About to set the max nodes etc.")
-    predictor.set_max_nodes_edges_per_graph(datamodule, stages=["train", "val"])
-
-    # Run the model training
-    with SafeRun(name="TRAINING", raise_error=cfg["constants"]["raise_train_error"], verbose=True):
-        trainer.fit(model=predictor, datamodule=datamodule)
+    predictor.set_max_nodes_edges_per_graph(datamodule, stages=["val"])
 
-    # Determine the max num nodes and edges in testing
-    predictor.set_max_nodes_edges_per_graph(datamodule, stages=["test"])
+    # Run the model validation
+    with SafeRun(name="VALIDATING", raise_error=cfg["constants"]["raise_train_error"], verbose=True):
+        trainer.validate(
+            model=predictor,
+            ckpt_path=f'{cfg["trainer"]["model_checkpoint"]["dirpath"]}{cfg["trainer"]["seed"]}/{cfg["trainer"]["model_checkpoint"]["filename"]}.ckpt',
+            datamodule=datamodule,
+        )
 
     # Run the model testing
     with SafeRun(name="TESTING", raise_error=cfg["constants"]["raise_train_error"], verbose=True):
-        trainer.test(model=predictor, datamodule=datamodule)  # , ckpt_path=ckpt_path)
+        trainer.test(
+            model=predictor,
+            ckpt_path=f'{cfg["trainer"]["model_checkpoint"]["dirpath"]}{cfg["trainer"]["seed"]}/{cfg["trainer"]["model_checkpoint"]["filename"]}.ckpt',
+            datamodule=datamodule,
+        )
 
     logger.info("--------------------------------------------")
     logger.info("total computation used", timeit.default_timer() - st)
     logger.info("--------------------------------------------")
     wandb.finish()
 
     return trainer.callback_metrics
```

### Comparing `graphium-2.1.3/expts/main_run_predict.py` & `graphium-2.2.0/expts/main_run_predict.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/main_run_test.py` & `graphium-2.2.0/expts/main_run_test.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml` & `graphium-2.2.0/expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml` & `graphium-2.2.0/expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml` & `graphium-2.2.0/expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_classifigression_l1000.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_classifigression_l1000.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_large_gcn.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_large_gcn.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,53 +1,62 @@
-# Testing the gcn model with the PCQMv2 dataset on IPU.
+# Running the gcn model with the largemix dataset on IPU.
 constants:
   name: &name neurips2023_large_data_gcn
   seed: &seed 42
   raise_train_error: true   # Whether the code should raise an error if it crashes during training
 
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 60 # train max nodes: 20, max_edges: 54
+          max_num_nodes_per_graph: 30 # train max nodes: 20, max_edges: 54
           max_num_edges_per_graph: 100
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 60 # valid max nodes: 51, max_edges: 118
+          max_num_nodes_per_graph: 30 # valid max nodes: 51, max_edges: 118
           max_num_edges_per_graph: 100
         # Data handling-related
-        batch_size_training: 10
-        batch_size_inference: 10
+        batch_size_training: 30
+        batch_size_inference: 30
     predictor:
+      metrics_every_n_train_steps: 1000
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
-        precision: 32
-        accumulate_grad_batches: 8
+        precision: 16-true
+        accumulate_grad_batches: 2
 
   ipu_config:
-    - deviceIterations(10) # IPU would require large batches to be ready for the model.
+    - deviceIterations(30) # IPU would require large batches to be ready for the model.
     - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
-    - _Popart.set("defaultBufferingDepth", 128)
+    - _Popart.set("defaultBufferingDepth", 96)
     - Precision.enableStochasticRounding(True)
     # - Precision.enableFloatingPointExceptions(True)
 
+  ipu_inference_config:
+  # set device iteration and replication factor to 1 during inference
+  # gradient accumulation was set to 1 in the code
+    - deviceIterations(1)
+    - replicationFactor(1)
+    - Precision.enableStochasticRounding(False)
+
 # accelerator:
 #   type: cpu  # cpu or ipu or gpu
 #   config_override:
 #     datamodule:
-#       batch_size_training: 64
-#       batch_size_inference: 256
+#       args:
+#         batch_size_training: 64
+#         batch_size_inference: 256
 #     trainer:
 #       trainer:
 #         precision: 32
 #         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
@@ -60,50 +69,54 @@
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_vcap_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_vcap_random_splits.pt`
+        epoch_sampling_fraction: 1.0
 
       l1000_mcf7:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_mcf7_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_mcf7_random_splits.pt`
+        epoch_sampling_fraction: 1.0
 
       pcba_1328:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCBA_1328_1564k.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCBA_1328_1564k.parquet
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: assayID-*  # assayID-* means all columns starting with "assayID-"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcba_1328_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcba_1328_random_splits.pt`
+        epoch_sampling_fraction: 1.0
 
       pcqm4m_g25:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
         label_cols: graph_*  # graph_* means all columns starting with "graph_"
         # sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         label_normalization:
           normalize_val_test: True
           method: "normal"
+        epoch_sampling_fraction: 1.0
 
       pcqm4m_n4:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
@@ -111,14 +124,15 @@
         # sample_size: 2000 # use sample_size for test
         task_level: node
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         seed: *seed
         label_normalization:
           normalize_val_test: True
           method: "normal"
+        epoch_sampling_fraction: 1.0
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
     processed_graph_data_path: "../datacache/neurips2023-large/"
@@ -150,15 +164,15 @@
           rw_pos: # use same name as pe_encoder
             pos_level: node
             pos_type: rw_return_probs
             ksteps: 16
 
     # cache_data_path: .
     num_workers: 30 # -1 to use all
-    persistent_workers: False # if use persistent worker at the start of each epoch.
+    persistent_workers: True # if use persistent worker at the start of each epoch.
     # Using persistent_workers false might make the start of each epoch very long.
     featurization_backend: "loky"
 
 
 architecture:
   model_type: FullGraphMultiTaskNetwork
   mup_base_path: null
@@ -269,15 +283,15 @@
       residual_type: none
     pcba_1328:
       task_level: graph
       out_dim: 1328
       hidden_dims: 64
       depth: 2
       activation: relu
-      last_activation: sigmoid
+      last_activation: none
       dropout: *dropout
       normalization: *normalization
       last_normalization: "none"
       residual_type: none
     pcqm4m_g25:
       task_level: graph
       out_dim: 25
@@ -315,18 +329,20 @@
     pcba_1328: []
     pcqm4m_g25: []
     pcqm4m_n4: []
   loss_fun:
     l1000_vcap:
       name: hybrid_ce_ipu
       n_brackets: 5
+      alpha: 0.5
     l1000_mcf7:
       name: hybrid_ce_ipu
       n_brackets: 5
-    pcba_1328: bce_ipu
+      alpha: 0.5
+    pcba_1328: bce_logits_ipu
     pcqm4m_g25: mae_ipu
     pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
     lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
@@ -401,8 +417,8 @@
     # monitor: *monitor
     # mode: *mode
     # save_top_k: 1
     save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
-    check_val_every_n_epoch: 10
+    check_val_every_n_epoch: 20
```

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_large_gin.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_large_gin.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Testing the gin model with the PCQMv2 dataset on IPU.
+# Running the gin model with the largemix dataset on IPU.
 constants:
   name: &name neurips2023_large_data_gin
   config_override: "expts/neurips2023_configs/config_large_gcn.yaml"
 
 architecture:
   gnn:  # Set as null to avoid a post-nn network
     out_dim: &gnn_dim 704
```

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_large_gine.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_large_gine.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Testing the gine model with the PCQMv2 dataset on IPU.
+# Running the gine model with the largemix dataset on IPU.
 constants:
   name: &name neurips2023_large_data_gine
   config_override: "expts/neurips2023_configs/config_large_gcn.yaml"
 
 architecture:
   pre_nn_edges:   # Set as null to avoid a pre-nn network
     out_dim: 32
```

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_large_mpnn.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_large_mpnn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_luis_jama.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_luis_jama.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_small_gated_gcn.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_small_gated_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_small_gcn.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_small_gcn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_small_gine.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_small_gine.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 architecture:
   pre_nn_edges:   # Set as null to avoid a pre-nn network
     out_dim: 32
     hidden_dims: 128
     depth: 2
     activation: relu
     last_activation: none
-    dropout: *dropout
-    normalization: *normalization
+    dropout: 0.1
+    normalization: &normalization layer_norm
     last_normalization: *normalization
     residual_type: none
 
   gnn:  # Set as null to avoid a post-nn network
     layer_type: 'pyg:gine' #pyg:gine #'pyg:gps' # pyg:gated-gcn, pyg:gine,pyg:gps
 
 trainer:
```

### Comparing `graphium-2.1.3/expts/neurips2023_configs/config_small_mpnn.yaml` & `graphium-2.2.0/expts/neurips2023_configs/config_small_mpnn.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/debug/config_debug.yaml` & `graphium-2.2.0/expts/neurips2023_configs/debug/config_debug.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml` & `graphium-2.2.0/expts/neurips2023_configs/debug/config_large_gcn_debug.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -7,46 +7,55 @@
 accelerator:
   type: ipu  # cpu or ipu or gpu
   config_override:
     datamodule:
       args:
         ipu_dataloader_training_opts:
           mode: async
-          max_num_nodes_per_graph: 40 # train max nodes: 20, max_edges: 54
+          max_num_nodes_per_graph: 30 # train max nodes: 20, max_edges: 54
           max_num_edges_per_graph: 80
         ipu_dataloader_inference_opts:
           mode: async
-          max_num_nodes_per_graph: 40 # valid max nodes: 51, max_edges: 118
+          max_num_nodes_per_graph: 30 # valid max nodes: 51, max_edges: 118
           max_num_edges_per_graph: 80
         # Data handling-related
-        batch_size_training: 20
-        batch_size_inference: 20
+        batch_size_training: 40
+        batch_size_inference: 40
     predictor:
+      metrics_every_n_train_steps: 100
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
-        precision: 16
-        accumulate_grad_batches: 4
+        precision: 16-true
+        accumulate_grad_batches: 2
 
   ipu_config:
     - deviceIterations(2) # IPU would require large batches to be ready for the model.
-    - replicationFactor(4)
+    - replicationFactor(16)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
     - TensorLocations.numIOTiles(128)
-    - _Popart.set("defaultBufferingDepth", 128)
+    - _Popart.set("defaultBufferingDepth", 96)
     - Precision.enableStochasticRounding(True)
 
+  ipu_inference_config:
+  # set device iteration and replication factor to 1 during inference
+  # gradient accumulation was set to be 1 in the code
+    - deviceIterations(1)
+    - replicationFactor(1)
+    - Precision.enableStochasticRounding(False)
+
 # accelerator:
 #   type: cpu  # cpu or ipu or gpu
 #   config_override:
 #     datamodule:
-#       batch_size_training: 64
-#       batch_size_inference: 256
+#       args:
+#         batch_size_training: 320
+#         batch_size_inference: 256
 #     trainer:
 #       trainer:
 #         precision: 32
 #         accumulate_grad_batches: 1
 
 datamodule:
   module_type: "MultitaskFromSmilesDataModule"
@@ -56,53 +65,57 @@
       l1000_vcap:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_VCAP_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_vcap_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_vcap_random_splits.pt`
+        epoch_sampling_fraction: 1.0
 
       l1000_mcf7:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/LINCS_L1000_MCF7_0-4.csv.gz
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: geneID-*  # geneID-* means all columns starting with "geneID-"
-        # sample_size: 2000 # use sample_size for test
+        sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/l1000_mcf7_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/l1000_mcf7_random_splits.pt`
+        epoch_sampling_fraction: 1.0
 
       pcba_1328:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCBA_1328_1564k.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCBA_1328_1564k.parquet
         # or set path as the URL directly
         smiles_col: "SMILES"
         label_cols: assayID-*  # assayID-* means all columns starting with "assayID-"
         sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcba_1328_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcba_1328_random_splits.pt`
+        epoch_sampling_fraction: 1.0
 
       pcqm4m_g25:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
         label_cols: graph_*  # graph_* means all columns starting with "graph_"
         sample_size: 2000 # use sample_size for test
         task_level: graph
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         label_normalization:
           normalize_val_test: True
           method: "normal"
+        epoch_sampling_fraction: 1.0
 
       pcqm4m_n4:
         df: null
         df_path: graphium/data/neurips2023/large-dataset/PCQM4M_G25_N4.parquet
         # wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/PCQM4M_G25_N4.parquet
         # or set path as the URL directly
         smiles_col: "ordered_smiles"
@@ -110,14 +123,15 @@
         sample_size: 2000 # use sample_size for test
         task_level: node
         splits_path: graphium/data/neurips2023/large-dataset/pcqm4m_g25_n4_random_splits.pt  # Download with `wget https://storage.googleapis.com/graphium-public/datasets/neurips_2023/Large-dataset/pcqm4m_g25_n4_random_splits.pt`
         seed: *seed
         label_normalization:
           normalize_val_test: True
           method: "normal"
+        epoch_sampling_fraction: 1.0
 
     # Featurization
     prepare_dict_or_graph: pyg:graph
     featurization_n_jobs: 30
     featurization_progress: True
     featurization_backend: "loky"
     processed_graph_data_path: "../datacache/neurips2023-large/"
@@ -314,30 +328,30 @@
     pcba_1328: []
     pcqm4m_g25: []
     pcqm4m_n4: [] 
   loss_fun:
     l1000_vcap:
       name: hybrid_ce_ipu
       n_brackets: 5
-      alpha: 0.5
+      alpha: 0.9
     l1000_mcf7:
       name: hybrid_ce_ipu
       n_brackets: 5
-      alpha: 0.5
+      alpha: 0.9
     pcba_1328: bce_ipu
     pcqm4m_g25: mae_ipu
     pcqm4m_n4: mae_ipu
   random_seed: *seed
   optim_kwargs:
     lr: 1.e-4 # warmup can be scheduled using torch_scheduler_kwargs
     # weight_decay: 1.e-7
   torch_scheduler_kwargs:
     module_type: WarmUpLinearLR
     max_num_epochs: &max_epochs 10
-    warmup_epochs: 5
+    warmup_epochs: 10
     verbose: False
   scheduler_kwargs:
   #  monitor: &monitor qm9/mae/train
   #  mode: min
   #  frequency: 1
   target_nan_mask: null # null: no mask, 0: 0 mask, ignore-flatten, ignore-mean-per-label
   multitask_handling: flatten # flatten, mean-per-label
@@ -403,13 +417,13 @@
   #  mode: &mode min
   model_checkpoint:
     dirpath: models_checkpoints/neurips2023-large-gcn-debug/
     filename: *name
     # monitor: *monitor
     # mode: *mode
     # save_top_k: 1
-    every_n_epochs: 5
+    every_n_epochs: 20
     save_last: True
   trainer:
     max_epochs: *max_epochs
     min_epochs: 1
     check_val_every_n_epoch: 10
```

### Comparing `graphium-2.1.3/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml` & `graphium-2.2.0/expts/neurips2023_configs/debug/config_small_gcn_debug.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         batch_size_training: 50
         batch_size_inference: 50
     predictor:
       optim_kwargs:
         loss_scaling: 1024
     trainer:
       trainer:
-        precision: 16
+        precision: 16-true
         accumulate_grad_batches: 1
 
   ipu_config:
     - deviceIterations(5) # IPU would require large batches to be ready for the model.
     - replicationFactor(2)
     # - enableProfiling("graph_analyser")       # The folder where the profile will be stored
     # - enableExecutableCaching("pop_compiler_cache")
```

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gcn/config_large_gcn_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_g25.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_n4.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_pcq.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gin/config_large_gin_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_g25.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_mcf7.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_n4.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcba.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_pcq.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml` & `graphium-2.2.0/expts/neurips2023_configs/single_task_gine/config_large_gine_vcap.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/expts/test_yaml.py` & `graphium-2.2.0/expts/debug_yaml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/cli/data.py` & `graphium-2.2.0/graphium/cli/data.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/config/_loader.py` & `graphium-2.2.0/graphium/config/_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,23 +41,27 @@
     """
 
     # Get the accelerator type
     accelerator_type = config_acc["type"]
 
     # Get the GPU info
     if (accelerator_type == "gpu") and (not torch.cuda.is_available()):
-        logger.warning(f"GPUs selected, but will be ignored since no GPU are available on this device")
-        accelerator_type = "cpu"
+        raise ValueError(f"GPUs selected, but GPUs are not available on this device")
 
     # Get the IPU info
     if accelerator_type == "ipu":
         poptorch = import_poptorch()
+        if poptorch is None:
+            raise ValueError("IPUs selected, but PopTorch is not available")
         if not poptorch.ipuHardwareIsAvailable():
-            logger.warning(f"IPUs selected, but will be ignored since no IPU are available on this device")
-            accelerator_type = "cpu"
+            raise ValueError(
+                "IPUs selected, but no IPU is available/visible on this device. "
+                "If you do have IPUs, please check that the IPUOF_VIPU_API_PARTITION_ID and "
+                "IPUOF_VIPU_API_HOST environment variables are set."
+            )
 
     # Fall on cpu at the end
     if accelerator_type is None:
         accelerator_type = "cpu"
     return accelerator_type
 
 
@@ -105,24 +109,25 @@
         return datamodule
 
     # IPU specific adjustments
     else:
         ipu_opts, ipu_inference_opts = _get_ipu_opts(config)
 
         # Default empty values for the IPU configurations
-        ipu_training_opts, ipu_inference_opts = None, None
+        ipu_training_opts = None
 
         ipu_dataloader_training_opts = cfg_data.pop("ipu_dataloader_training_opts", {})
         ipu_dataloader_inference_opts = cfg_data.pop("ipu_dataloader_inference_opts", {})
         ipu_training_opts, ipu_inference_opts = load_ipu_options(
             ipu_opts=ipu_opts,
             seed=config["constants"]["seed"],
             model_name=config["constants"]["name"],
             gradient_accumulation=config["trainer"]["trainer"].get("accumulate_grad_batches", None),
             ipu_inference_opts=ipu_inference_opts,
+            precision=config["trainer"]["trainer"].get("precision"),
         )
         # Define the Dataloader options for the IPU on the training sets
         bz_train = cfg_data["batch_size_training"]
         ipu_dataloader_training_opts = IPUDataloaderOptions(
             batch_size=bz_train, **ipu_dataloader_training_opts
         )
         ipu_dataloader_training_opts.set_kwargs()
@@ -358,14 +363,15 @@
 
         training_opts, inference_opts = load_ipu_options(
             ipu_opts=ipu_opts,
             ipu_inference_opts=ipu_inference_opts,
             seed=config["constants"]["seed"],
             model_name=config["constants"]["name"],
             gradient_accumulation=config["trainer"]["trainer"].get("accumulate_grad_batches", None),
+            precision=config["trainer"]["trainer"].get("precision"),
         )
 
         from lightning_graphcore import IPUStrategy
 
         strategy = IPUStrategy(training_opts=training_opts, inference_opts=inference_opts)
 
     # Get devices
@@ -451,14 +457,19 @@
     config_acc = config.get("accelerator", {})
 
     # Merge the accelerator config with the main config
     config_override = config_acc.get("config_override", {})
     merge_dicts(config, config_override)
     accelerator_type = get_accelerator(config_acc)
 
+    if accelerator_type == "gpu":
+        precision = config_acc.get("float32_matmul_precision", None)
+        if precision is not None:
+            torch.set_float32_matmul_precision(precision)
+
     return config, accelerator_type
 
 
 def load_config_override(
     config: Union[omegaconf.DictConfig, Dict[str, Any]], main_dir: Optional[Union[str, os.PathLike]] = None
 ) -> Dict[str, Any]:
     config = deepcopy(config)
```

### Comparing `graphium-2.1.3/graphium/config/config_convert.py` & `graphium-2.2.0/graphium/config/config_convert.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml` & `graphium-2.2.0/graphium/config/fake_and_missing_multilevel_multitask_pyg.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -4,44 +4,44 @@
     task_specific_args:   # To be replaced by a new class "DatasetParams"
       score:
         df: null
         task_level: "edge"
         df_path: "./tests/fake_and_missing_multilevel_data.parquet"
         smiles_col: "ordered_smiles"
         label_cols: ["edge_label_list", "edge_label_np"]
-        split_val: 0.2
-        split_test: 0.2
+        split_val: 0.0
+        split_test: 0.0
         seed: 19
         splits_path: null
         sample_size: null
         idx_col: null
         weights_col: null
         weights_type: null
       logp:
         df: null
         task_level: "node"
         df_path: "./tests/fake_and_missing_multilevel_data.parquet"
         smiles_col: "ordered_smiles"
         label_cols: ["node_label_list", "node_label_np"]
-        split_val: 0.2
-        split_test: 0.2
+        split_val: 0.0
+        split_test: 0.0
         seed: 19
         splits_path: null
         sample_size: null
         idx_col: null
         weights_col: null
         weights_type: null
       SA:
         df: null
         task_level: "graph"
         df_path: "./tests/fake_and_missing_multilevel_data.parquet"
         smiles_col: "ordered_smiles"
         label_cols: ["graph_label"]
-        split_val: 0.2
-        split_test: 0.2
+        split_val: 0.0
+        split_test: 0.0
         seed: 19
         splits_path: null                 # This may not always be provided
         sample_size: null                 # This may not always be provided
         idx_col: null                     # This may not always be provided
         weights_col: null                 # This may not always be provided
 
     # Featurization
```

### Comparing `graphium-2.1.3/graphium/config/fake_multilevel_multitask_pyg.yaml` & `graphium-2.2.0/graphium/config/fake_multilevel_multitask_pyg.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -4,44 +4,44 @@
     task_specific_args:   # To be replaced by a new class "DatasetParams"
       score:
         df: null
         task_level: "edge"
         df_path: "./tests/converted_fake_multilevel_data.parquet"
         smiles_col: "ordered_smiles"
         label_cols: ["edge_label_list", "edge_label_np"]
-        split_val: 0.2
-        split_test: 0.2
+        split_val: 0.0
+        split_test: 0.0
         seed: 19
         splits_path: null
         sample_size: null
         idx_col: null
         weights_col: null
         weights_type: null
       logp:
         df: null
         task_level: "node"
         df_path: "./tests/converted_fake_multilevel_data.parquet"
         smiles_col: "ordered_smiles"
         label_cols: ["node_label_list", "node_label_np"]
-        split_val: 0.2
-        split_test: 0.2
+        split_val: 0.0
+        split_test: 0.0
         seed: 19
         splits_path: null
         sample_size: null
         idx_col: null
         weights_col: null
         weights_type: null
       SA:
         df: null
         task_level: "graph"
         df_path: "./tests/converted_fake_multilevel_data.parquet"
         smiles_col: "ordered_smiles"
         label_cols: ["graph_label"]
-        split_val: 0.2
-        split_test: 0.2
+        split_val: 0.0
+        split_test: 0.0
         seed: 19
         splits_path: null                 # This may not always be provided
         sample_size: null                 # This may not always be provided
         idx_col: null                     # This may not always be provided
         weights_col: null                 # This may not always be provided
 
     # Featurization
```

### Comparing `graphium-2.1.3/graphium/config/zinc_default_multitask_pyg.yaml` & `graphium-2.2.0/graphium/config/zinc_default_multitask_pyg.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb` & `graphium-2.2.0/graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/QM9/micro_qm9.csv` & `graphium-2.2.0/graphium/data/QM9/micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/QM9/micro_qm9.parquet` & `graphium-2.2.0/graphium/data/QM9/micro_qm9.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/QM9/norm_micro_qm9.csv` & `graphium-2.2.0/graphium/data/QM9/norm_micro_qm9.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/README.md` & `graphium-2.2.0/graphium/data/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/collate.py` & `graphium-2.2.0/graphium/data/collate.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/datamodule.py` & `graphium-2.2.0/graphium/data/datamodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+import tempfile
+from contextlib import redirect_stderr, redirect_stdout
 from typing import Type, List, Dict, Union, Any, Callable, Optional, Tuple, Iterable, Literal
 
 import os
-import glob
 from functools import partial
 import importlib.resources
 import zipfile
 from copy import deepcopy
 import time
 import gc
-from rdkit import Chem
+
+import platformdirs
 import re
 from graphium.data.utils import get_keys
 
 from loguru import logger
 import fsspec
 import omegaconf
 
@@ -25,25 +27,26 @@
 
 from sklearn.model_selection import train_test_split
 
 import lightning
 from lightning.pytorch.trainer.states import RunningStage
 
 import torch
-from torch_geometric.data import Data
 from torch.utils.data.dataloader import DataLoader, Dataset
 from torch.utils.data import Subset
 
 from graphium.utils import fs
 from graphium.features import (
     mol_to_graph_dict,
     GraphDict,
     mol_to_pyggraph,
 )
-from graphium.data.utils import graphium_package_path
+
+from graphium.data.sampler import DatasetSubSampler
+from graphium.data.utils import graphium_package_path, found_size_mismatch
 from graphium.utils.arg_checker import check_arg_iterator
 from graphium.utils.hashing import get_md5_hash
 from graphium.data.smiles_transform import (
     did_featurization_fail,
     BatchingSmilesTransform,
     smiles_to_unique_mol_ids,
 )
@@ -638,26 +641,28 @@
 
         return max_num_edges
 
 
 class DatasetProcessingParams:
     def __init__(
         self,
-        task_level: str = None,
-        df: pd.DataFrame = None,
+        task_level: Optional[str] = None,
+        df: Optional[pd.DataFrame] = None,
         df_path: Optional[Union[str, os.PathLike]] = None,
-        smiles_col: str = None,
+        smiles_col: Optional[str] = None,
         label_cols: List[str] = None,
-        weights_col: str = None,  # Not needed
-        weights_type: str = None,  # Not needed
-        idx_col: str = None,
+        weights_col: Optional[str] = None,  # Not needed
+        weights_type: Optional[str] = None,  # Not needed
+        idx_col: Optional[str] = None,
+        mol_ids_col: Optional[str] = None,
         sample_size: Union[int, float, Type[None]] = None,
         split_val: float = 0.2,
         split_test: float = 0.2,
         seed: int = None,
+        epoch_sampling_fraction: float = 1.0,
         splits_path: Optional[Union[str, os.PathLike]] = None,
         split_names: Optional[List[str]] = ["train", "val", "test"],
         label_normalization: Optional[Union[Dict[str, Any], omegaconf.DictConfig]] = None,
     ):
         """
         object to store the parameters for the dataset processing
         Parameters:
@@ -665,35 +670,44 @@
             df: The dataframe containing the data
             df_path: The path to the dataframe containing the data
             smiles_col: The column name of the smiles
             label_cols: The column names of the labels
             weights_col: The column name of the weights
             weights_type: The type of weights
             idx_col: The column name of the indices
+            mol_ids_col: The column name of the molecule ids
             sample_size: The size of the sample
             split_val: The fraction of the data to use for validation
             split_test: The fraction of the data to use for testing
             seed: The seed to use for the splits and subsampling
             splits_path: The path to the splits
         """
+
+        if df is None and df_path is None:
+            raise ValueError("Either `df` or `df_path` must be provided")
+        if epoch_sampling_fraction <= 0 or epoch_sampling_fraction > 1:
+            raise ValueError("The value of epoch_sampling_fraction must be in the range of (0, 1].")
+
         self.df = df
         self.task_level = task_level
         self.df_path = df_path
         self.smiles_col = smiles_col
         self.label_cols = label_cols
         self.weights_col = weights_col
         self.weights_type = weights_type
         self.idx_col = idx_col
+        self.mol_ids_col = mol_ids_col
         self.sample_size = sample_size
         self.split_val = split_val
         self.split_test = split_test
         self.seed = seed
         self.splits_path = splits_path
         self.split_names = split_names
         self.label_normalization = label_normalization
+        self.epoch_sampling_fraction = epoch_sampling_fraction
 
 
 class IPUDataModuleModifier:
     def __init__(
         self,
         ipu_inference_opts: Optional["poptorch.Options"] = None,
         ipu_training_opts: Optional["poptorch.Options"] = None,
@@ -748,15 +762,15 @@
 
         return loader
 
 
 class MultitaskFromSmilesDataModule(BaseDataModule, IPUDataModuleModifier):
     def __init__(
         self,
-        task_specific_args: Dict[str, Any],  # TODO: Replace this with DatasetParams
+        task_specific_args: Union[DatasetProcessingParams, Dict[str, Any]],
         cache_data_path: Optional[Union[str, os.PathLike]] = None,
         processed_graph_data_path: Optional[Union[str, os.PathLike]] = None,
         featurization: Optional[Union[Dict[str, Any], omegaconf.DictConfig]] = None,
         batch_size_training: int = 16,
         batch_size_inference: int = 16,
         batch_size_per_pack: Optional[int] = None,
         num_workers: int = 0,
@@ -855,19 +869,29 @@
             persistent_workers=persistent_workers,
             collate_fn=collate_fn,
         )
         IPUDataModuleModifier.__init__(self, **kwargs)
 
         self.task_specific_args = task_specific_args
 
-        # TODO: Have the input argument to the Data Module be of type DatasetParams
-        self.task_dataset_processing_params = {
-            self._get_task_key(ds_args["task_level"], task): DatasetProcessingParams(**ds_args)
-            for task, ds_args in task_specific_args.items()
+        self.task_dataset_processing_params = {}
+        for task, ds_args in task_specific_args.items():
+            if not isinstance(ds_args, DatasetProcessingParams):
+                # This is needed as long as not all classes have been migrated
+                # to use the new `DatasetProcessingParams` class
+                ds_args = DatasetProcessingParams(**ds_args)
+
+            key = self._get_task_key(ds_args.task_level, task)
+            self.task_dataset_processing_params[key] = ds_args
+
+        self.sampler_task_dict = {
+            task: self.task_dataset_processing_params[task].epoch_sampling_fraction
+            for task in self.task_dataset_processing_params.keys()
         }
+
         self.featurization_n_jobs = featurization_n_jobs
         self.featurization_progress = featurization_progress
         self.featurization_backend = featurization_backend
         self.featurization_batch_size = featurization_batch_size
 
         self.task_train_indices = None
         self.task_val_indices = None
@@ -995,17 +1019,14 @@
             sample_size = self.task_dataset_processing_params[task].sample_size
             df = self._sub_sample_df(df, sample_size, self.task_dataset_processing_params[task].seed)
 
             logger.info(f"Prepare single-task dataset for task '{task}' with {len(df)} data points.")
 
             logger.info("Filtering the molecules for Hydrogen")
             logger.info(f"Looking at column {df.columns[0]}")
-            # Filter the DataFrame based on the function
-            # need this for pcba dataset
-            # df = df[df[df.columns[0]].apply(lambda x: has_atoms_after_h_removal(x))]
             logger.info("Filtering done")
             # Extract smiles, labels, extras
             args = self.task_dataset_processing_params[task]
             smiles, labels, sample_idx, extras = self._extract_smiles_labels(
                 df,
                 task_level=args.task_level,
                 smiles_col=args.smiles_col,
@@ -1030,47 +1051,51 @@
             all_smiles.extend(dataset_args["smiles"])
             num_smiles = len(dataset_args["smiles"])
             idx_per_task[task] = (total_len, total_len + num_smiles)
             total_len += num_smiles
             for count in range(len(dataset_args["smiles"])):
                 all_tasks.append(task)
         # Get all unique mol ids
-        all_mol_ids = smiles_to_unique_mol_ids(
+        all_unique_mol_ids = smiles_to_unique_mol_ids(
             all_smiles,
             n_jobs=self.featurization_n_jobs,
             featurization_batch_size=self.featurization_batch_size,
             backend=self.featurization_backend,
         )
-        unique_mol_ids, unique_idx, inv = np.unique(all_mol_ids, return_index=True, return_inverse=True)
+        _, unique_ids_idx, unique_ids_inv = np.unique(
+            all_unique_mol_ids, return_index=True, return_inverse=True
+        )
 
-        smiles_to_featurize = [all_smiles[ii] for ii in unique_idx]
+        smiles_to_featurize = [all_smiles[ii] for ii in unique_ids_idx]
 
         # Convert SMILES to features
         features, _ = self._featurize_molecules(smiles_to_featurize)
 
         # Store the features (including Nones, which will be filtered in the next step)
         for task in task_dataset_args.keys():
             task_dataset_args[task]["features"] = []
             task_dataset_args[task]["idx_none"] = []
         # Create a list of features matching up with the original smiles
-        all_features = [features[unique_idx] for unique_idx in inv]
+        all_features = [features[unique_idx] for unique_idx in unique_ids_inv]
 
         # Add the features to the task-specific data
         for all_idx, task in enumerate(all_tasks):
             task_dataset_args[task]["features"].append(all_features[all_idx])
 
         """Filter data based on molecules which failed featurization. Create single task datasets as well."""
         self.single_task_datasets = {}
         for task, args in task_dataset_args.items():
             # Find out which molecule failed featurization, and filter them out
             idx_none = []
-            for idx, feat in enumerate(args["features"]):
-                if did_featurization_fail(feat):
+            for idx, (feat, labels, smiles) in enumerate(
+                zip(args["features"], args["labels"], args["smiles"])
+            ):
+                if did_featurization_fail(feat) or found_size_mismatch(task, feat, labels, smiles):
                     idx_none.append(idx)
-            this_unique_ids = all_mol_ids[idx_per_task[task][0] : idx_per_task[task][1]]
+            this_unique_ids = all_unique_mol_ids[idx_per_task[task][0] : idx_per_task[task][1]]
             df, features, smiles, labels, sample_idx, extras, this_unique_ids = self._filter_none_molecules(
                 idx_none,
                 task_df[task],
                 args["features"],
                 args["smiles"],
                 args["labels"],
                 args["sample_idx"],
@@ -1085,14 +1110,15 @@
 
             # We have the necessary components to create single-task datasets.
             self.single_task_datasets[task] = Datasets.SingleTaskDataset(
                 features=task_dataset_args[task]["features"],
                 labels=task_dataset_args[task]["labels"],
                 smiles=task_dataset_args[task]["smiles"],
                 unique_ids=this_unique_ids,
+                indices=task_dataset_args[task]["sample_idx"],
                 **task_dataset_args[task]["extras"],
             )
 
         """We split the data up to create train, val and test datasets"""
         self.task_train_indices = {}
         self.task_val_indices = {}
         self.task_test_indices = {}
@@ -1457,19 +1483,29 @@
             shuffle: set to ``True`` to have the data reshuffled at every epoch.
             stage: Whether in Training, Validating, Testing, Sanity-checking, Predicting, or Tuning phase.
 
         Returns:
             The poptorch dataloader to sample from
         """
         kwargs = self.get_dataloader_kwargs(stage=stage, shuffle=shuffle)
+        sampler = None
+        # use sampler only when sampler_task_dict is set in the config and during training
+        if DatasetSubSampler.check_sampling_required(self.sampler_task_dict) and stage in [
+            RunningStage.TRAINING
+        ]:
+            sampler = DatasetSubSampler(
+                dataset, self.sampler_task_dict, self.processed_graph_data_path, self.data_hash
+            )
+            # turn shuffle off when sampler is used as sampler option is mutually exclusive with shuffle
+            kwargs["shuffle"] = False
         is_ipu = ("ipu_options" in kwargs.keys()) and (kwargs.get("ipu_options") is not None)
         if is_ipu:
-            loader = IPUDataModuleModifier._dataloader(self, dataset=dataset, **kwargs)
+            loader = IPUDataModuleModifier._dataloader(self, dataset=dataset, sampler=sampler, **kwargs)
         else:
-            loader = BaseDataModule._dataloader(self, dataset=dataset, **kwargs)
+            loader = BaseDataModule._dataloader(self, dataset=dataset, sampler=sampler, **kwargs)
 
         return loader
 
     def get_collate_fn(self, collate_fn):
         if collate_fn is None:
             # Some values become `inf` when changing data type. `mask_nan` deals with that
             collate_fn = partial(
@@ -1708,31 +1744,33 @@
     def _load_from_cache(self):
         raise NotImplementedError()
 
     def _extract_smiles_labels(
         self,
         df: pd.DataFrame,
         task_level: str,
-        smiles_col: str = None,
+        smiles_col: Optional[str] = None,
         label_cols: List[str] = [],
-        idx_col: str = None,
-        weights_col: str = None,
-        weights_type: str = None,
+        idx_col: Optional[str] = None,
+        mol_ids_col: Optional[str] = None,
+        weights_col: Optional[str] = None,
+        weights_type: Optional[str] = None,
     ) -> Tuple[
         np.ndarray, np.ndarray, Union[Type[None], np.ndarray], Dict[str, Union[Type[None], np.ndarray]]
     ]:
         """
         For a given dataframe extract the SMILES and labels columns. Smiles is returned as a list
         of string while labels are returned as a 2D numpy array.
 
         Parameters:
             df: Pandas dataframe
             smiles_col: Name of the column containing the SMILES
             label_cols: List of column names containing the labels
             idx_col: Name of the column containing the index
+            mol_ids_col: Name of the column containing the molecule ids
             weights_col: Name of the column containing the weights
             weights_type: Type of weights to use.
         Returns:
             smiles, labels, sample_idx, extras
         """
 
         if smiles_col is None:  # Should we specify which dataset has caused the potential issue?
@@ -1761,20 +1799,24 @@
             elif task_level == "nodepair":
                 labels = extract_labels(df, "nodepair", label_cols)
             else:
                 raise ValueError(f"Unknown task level: {task_level}")
         else:
             labels = float("nan") + np.zeros([len(smiles), 0])
 
-        indices = None  # What are indices for?
+        # Get the indices, used for sub-sampling and splitting the dataset
         if idx_col is not None:
-            indices = df[idx_col].values
-
+            df = df.set_index(idx_col)
         sample_idx = df.index.values
 
+        # Get the molecule ids
+        mol_ids = None
+        if mol_ids_col is not None:
+            mol_ids = df[mol_ids_col].values
+
         # Extract the weights
         weights = None
         if weights_col is not None:
             weights = df[weights_col].values
         elif weights_type is not None:
             if not np.all((labels == 0) | (labels == 1)):
                 raise ValueError("Labels must be binary for `weights_type`")
@@ -1793,15 +1835,15 @@
                 weights = np.prod(weights, axis=1)
 
             else:
                 raise ValueError(f"Undefined `weights_type` {weights_type}")
 
             weights /= np.max(weights)  # Put the max weight to 1
 
-        extras = {"indices": indices, "weights": weights}
+        extras = {"weights": weights, "mol_ids": mol_ids}
         return smiles, labels, sample_idx, extras
 
     def _get_split_indices(
         self,
         dataset_size: int,
         split_val: float,
         split_test: float,
@@ -1855,23 +1897,25 @@
             file_type = self._get_data_file_type(splits_path)
 
             if file_type == "pt":
                 splits = torch.load(splits_path)
             elif file_type in ["csv", "tsv"]:
                 with fsspec.open(str(splits_path)) as f:
                     splits = self._read_csv(splits_path)
-                splits = splits.dropna()
             else:
                 raise ValueError(
                     f"file type `{file_type}` for `{splits_path}` not recognised, please use .pt, .csv or .tsv"
                 )
             train, val, test = split_names
-            train_indices = np.asarray(splits[train]).astype("int").tolist()
-            val_indices = np.asarray(splits[val]).astype("int").tolist()
-            test_indices = np.asarray(splits[test]).astype("int").tolist()
+            train_indices = np.asarray(splits[train]).astype("int")
+            train_indices = train_indices[~np.isnan(train_indices)].tolist()
+            val_indices = np.asarray(splits[val]).astype("int")
+            val_indices = val_indices[~np.isnan(val_indices)].tolist()
+            test_indices = np.asarray(splits[test]).astype("int")
+            test_indices = test_indices[~np.isnan(test_indices)].tolist()
 
         # Filter train, val and test indices
         _, train_idx, _ = np.intersect1d(sample_idx, train_indices, return_indices=True)
         train_indices = train_idx.tolist()
         _, valid_idx, _ = np.intersect1d(sample_idx, val_indices, return_indices=True)
         val_indices = valid_idx.tolist()
         _, test_idx, _ = np.intersect1d(sample_idx, test_indices, return_indices=True)
@@ -1906,17 +1950,24 @@
         return df
 
     def get_data_hash(self):
         """
         Get a hash specific to a dataset and smiles_transformer.
         Useful to cache the pre-processed data.
         """
+        args = deepcopy(self.task_specific_args)
+        # pop epoch_sampling_fraction out when creating hash
+        # so that the data cache does not need to be regenerated
+        # when epoch_sampling_fraction has changed.
+        for task in self.task_specific_args.keys():
+            if "epoch_sampling_fraction" in args[task].keys():
+                args[task].pop("epoch_sampling_fraction")
         hash_dict = {
             "smiles_transformer": self.smiles_transformer,
-            "task_specific_args": self.task_specific_args,
+            "task_specific_args": args,
         }
         data_hash = get_md5_hash(hash_dict)
         return data_hash
 
     def get_data_cache_fullname(self, compress: bool = False) -> str:
         """
         Create a hash for the dataset, and use it to generate a file name
@@ -2110,15 +2161,15 @@
         """
         return omegaconf.OmegaConf.to_yaml(self.to_dict())
 
 
 class GraphOGBDataModule(MultitaskFromSmilesDataModule):
     def __init__(
         self,
-        task_specific_args: Dict[str, Dict[str, Any]],  # TODO: Replace this with DatasetParams
+        task_specific_args: Dict[str, Union[DatasetProcessingParams, Dict[str, Any]]],
         cache_data_path: Optional[Union[str, os.PathLike]] = None,
         featurization: Optional[Union[Dict[str, Any], omegaconf.DictConfig]] = None,
         batch_size_training: int = 16,
         batch_size_inference: int = 16,
         batch_size_per_pack: Optional[int] = None,
         num_workers: int = 0,
         pin_memory: bool = True,
@@ -2168,20 +2219,20 @@
 
         new_task_specific_args = {}
         self.metadata = {}
         for task_name, task_args in task_specific_args.items():
             # Get OGB metadata
             this_metadata = self._get_dataset_metadata(task_args["dataset_name"])
             # Get dataset
-            df, idx_col, smiles_col, label_cols, splits_path = self._load_dataset(
+            df, mol_ids_col, smiles_col, label_cols, splits_path = self._load_dataset(
                 this_metadata, sample_size=task_args.get("sample_size", None)
             )
             new_task_specific_args[task_name] = {
                 "df": df,
-                "idx_col": idx_col,
+                "mol_ids_col": mol_ids_col,
                 "smiles_col": smiles_col,
                 "label_cols": label_cols,
                 "splits_path": splits_path,
                 "task_level": task_args["task_level"],
             }
             self.metadata[task_name] = this_metadata
 
@@ -2227,15 +2278,15 @@
         Download, extract and load an OGB dataset.
         Parameters:
             metadata: Metadata for the dataset to load.
             sample_size: The number of molecules to sample from the dataset. Default=None,
                 meaning that all molecules will be considered.
         Returns:
             df: Pandas dataframe containing the dataset.
-            idx_col: Name of the column containing the molecule index.
+            mol_ids_col: Name of the column containing the molecule ids.
             smiles_col: Name of the column containing the SMILES.
             label_cols: List of column names containing the labels.
             splits_path: Path to the file containing the train/val/test splits.
         """
 
         base_dir = fs.get_cache_dir("ogb")
         dataset_dir = base_dir / metadata["download_name"]
@@ -2296,23 +2347,23 @@
             splits_path = dataset_dir / "split" / f"{split_name}.csv.gz"
 
         logger.info(f"Saving splits to {splits_path}")
         splits.to_csv(splits_path, index=None)
 
         # Get column names: OGB columns are predictable
         if metadata["download_name"].startswith("pcqm4m"):
-            idx_col = df.columns[0]
+            mol_ids_col = df.columns[0]
             smiles_col = df.columns[-2]
             label_cols = df.columns[-1:].to_list()
         else:
-            idx_col = df.columns[-1]
+            mol_ids_col = df.columns[-1]
             smiles_col = df.columns[-2]
             label_cols = df.columns[:-2].to_list()
 
-        return df, idx_col, smiles_col, label_cols, splits_path
+        return df, mol_ids_col, smiles_col, label_cols, splits_path
 
     def _get_dataset_metadata(self, dataset_name: str) -> Dict[str, Any]:
         ogb_metadata = self._get_ogb_metadata()
         if dataset_name not in ogb_metadata.index:
             raise ValueError(f"'{dataset_name}' is not a valid dataset name.")
 
         return ogb_metadata.loc[dataset_name].to_dict()
@@ -2333,14 +2384,179 @@
 
         # Only keep datasets of type 'mol'
         ogb_metadata = ogb_metadata[ogb_metadata["data type"] == "mol"]
 
         return ogb_metadata
 
 
+class ADMETBenchmarkDataModule(MultitaskFromSmilesDataModule):
+    """
+    Wrapper to use the ADMET benchmark group from the TDC (Therapeutics Data Commons).
+
+    !!! warning "Dependency"
+
+        This class requires [PyTDC](https://pypi.org/project/PyTDC/) to be installed.
+
+    !!! note "Citation"
+
+        Huang, K., Fu, T., Gao, W., Zhao, Y., Roohani, Y., Leskovec, J., Coley, C., Xiao, C., Sun, J., & Zitnik, M. (2021).
+        Therapeutics Data Commons: Machine Learning Datasets and Tasks for Drug Discovery and Development.
+        Proceedings of Neural Information Processing Systems, NeurIPS Datasets and Benchmarks.
+
+
+    Parameters:
+        tdc_benchmark_names: This can be any subset of the benchmark names that make up the ADMET benchmarking group.
+            If `None`, uses the complete benchmarking group. For all full list of options, see
+            [the TDC website](https://tdcommons.ai/benchmark/admet_group/overview/) or use:
+
+           ```python
+           import tdc.utils.retrieve_benchmark_names
+           retrieve_benchmark_names("admet_group")
+           ```
+        tdc_train_val_seed: TDC recommends a default splitting method for the train-val split. This parameter
+          is used to seed that splitting method.
+    """
+
+    def __init__(
+        self,
+        # TDC-specific
+        tdc_benchmark_names: Optional[Union[str, List[str]]] = None,
+        tdc_train_val_seed: int = 0,
+        # Inherited arguments from superclass
+        cache_data_path: Optional[Union[str, os.PathLike]] = None,
+        featurization: Optional[Union[Dict[str, Any], omegaconf.DictConfig]] = None,
+        batch_size_training: int = 16,
+        batch_size_inference: int = 16,
+        batch_size_per_pack: Optional[int] = None,
+        num_workers: int = 0,
+        pin_memory: bool = True,
+        persistent_workers: bool = False,
+        featurization_n_jobs: int = -1,
+        featurization_progress: bool = False,
+        featurization_backend: str = "loky",
+        collate_fn: Optional[Callable] = None,
+        prepare_dict_or_graph: str = "pyg:graph",
+        **kwargs,
+    ):
+        try:
+            from tdc.benchmark_group import admet_group
+            from tdc.utils import retrieve_benchmark_names
+        except ImportError as error:
+            # To make sure we use the exact same train-test set and preprocessing as other benchmark entries,
+            # we rely on the PyTDC library.
+            raise RuntimeError(
+                f"To use {self.__class__.__name__}, `PyTDC` needs to be installed. "
+                f"Please install it with `pip install PyTDC`"
+            ) from error
+
+        # Pick a path to save the TDC data to
+        tdc_cache_dir = fs.get_cache_dir("tdc")
+        tdc_cache_dir = fs.join(tdc_cache_dir, "ADMET_Benchmark")
+        fs.mkdir(tdc_cache_dir, exist_ok=True)
+
+        # Create the benchmark group object
+        # NOTE (cwognum): We redirect stderr and stdout to a file since TDC uses print statements,
+        #  which quickly pollute the logs. Ideally, we would use `redirect_stderr(None)`, but that breaks TQDM.
+        with tempfile.TemporaryFile("w") as f:
+            with redirect_stderr(f):
+                with redirect_stdout(f):
+                    self.group = admet_group(path=tdc_cache_dir)
+
+        # By default, use all available benchmarks in a benchmark group
+        if tdc_benchmark_names is None:
+            tdc_benchmark_names = retrieve_benchmark_names("admet_group")
+        if isinstance(tdc_benchmark_names, str):
+            tdc_benchmark_names = [tdc_benchmark_names]
+
+        # Create the task-specific arguments
+        logger.info(
+            f"Preparing the TDC ADMET Benchmark Group splits for each of the {len(tdc_benchmark_names)} benchmarks."
+        )
+
+        task_specific_args = {
+            t: self._get_task_specific_arguments(t, tdc_train_val_seed, tdc_cache_dir)
+            for t in tdc_benchmark_names
+        }
+
+        super().__init__(
+            task_specific_args=task_specific_args,
+            cache_data_path=cache_data_path,
+            featurization=featurization,
+            batch_size_training=batch_size_training,
+            batch_size_inference=batch_size_inference,
+            batch_size_per_pack=batch_size_per_pack,
+            num_workers=num_workers,
+            pin_memory=pin_memory,
+            persistent_workers=persistent_workers,
+            featurization_n_jobs=featurization_n_jobs,
+            featurization_progress=featurization_progress,
+            featurization_backend=featurization_backend,
+            collate_fn=collate_fn,
+            prepare_dict_or_graph=prepare_dict_or_graph,
+            **kwargs,
+        )
+
+    def _get_task_specific_arguments(self, name: str, seed: int, cache_dir: str) -> DatasetProcessingParams:
+        """
+        Loads the data and split from the TDC benchmark group object.
+
+        For the train-test split, this is fixed.
+
+        For the train-val split, this does not have to be fixed. Here we use the default splitting method
+        from TDC to do the train-val split and allow the seed to be changed. This is likely to best match
+        other entries in the benchmarking group.
+        """
+
+        benchmark = self.group.get(name)
+
+        # Get the default train-val-test split
+
+        # NOTE (cwognum): TDC prints by default to stderr, which pollutes the logs quite a bit.
+        #  This context manager mutes these by temporarily writing to a file.
+        #  Ideally, we would use `redirect_stderr(None)`, but that breaks TQDM.
+
+        with tempfile.TemporaryFile("w") as f:
+            with redirect_stderr(f):
+                train, val = self.group.get_train_valid_split(seed, name)
+        test = benchmark["test"]
+
+        # Convert to the Graphium format
+        n_val = len(val)
+        n_test = len(test)
+        n_train = len(train)
+        max_len = max(n_train, n_val, n_test)
+        total_len = n_train + n_val + n_test
+
+        data = pd.concat([train, val, test], ignore_index=True)
+
+        # NOTE (cwognum): We need to convert the labels to float, since we use NaNs down the line.
+        #  If you uncomment this line, collating the labels will raise an overflow by converting a NaN to the int dtype.
+        data["Y"] = data["Y"].astype(float)
+
+        split = pd.DataFrame(
+            {
+                "train": list(range(n_train)),
+                "val": list(range(n_train, n_train + n_val)) + [float("nan")] * (max_len - n_val),
+                "test": list(range(n_train + n_val, total_len)) + [float("nan")] * (max_len - n_test),
+            }
+        )
+        split_path = fs.join(cache_dir, f"{name}_split.csv")
+        split.to_csv(split_path, index=False)
+
+        return DatasetProcessingParams(
+            df=data,
+            idx_col=None,
+            smiles_col="Drug",
+            label_cols=["Y"],
+            splits_path=split_path,
+            split_names=["train", "val", "test"],
+            task_level="graph",
+        )
+
+
 class FakeDataModule(MultitaskFromSmilesDataModule):
     """
     A fake datamodule that generates artificial data by mimicking the true data coming
     from the provided dataset.
     It is useful to test the speed and performance of the model on a dataset without
     having to featurize it and wait for the workers to load it.
     """
@@ -2467,15 +2683,15 @@
         total_len = 0
         for task, dataset_args in task_dataset_args.items():
             all_smiles.extend(dataset_args["smiles"])
             num_smiles = len(dataset_args["smiles"])
             idx_per_task[task] = (total_len, total_len + num_smiles)
             total_len += num_smiles
         # Get all unique mol ids
-        all_mol_ids = smiles_to_unique_mol_ids(
+        all_unique_mol_ids = smiles_to_unique_mol_ids(
             all_smiles,
             n_jobs=self.featurization_n_jobs,
             featurization_batch_size=self.featurization_batch_size,
             backend=self.featurization_backend,
         )
         # Convert SMILES to features
         features, _ = self._featurize_molecules(all_smiles)
@@ -2483,15 +2699,16 @@
         """Filter data based on molecules which failed featurization. Create single task datasets as well."""
         self.single_task_datasets = {}
         for task, args in task_dataset_args.items():
             self.single_task_datasets[task] = Datasets.SingleTaskDataset(
                 features=task_dataset_args[task]["features"],
                 labels=task_dataset_args[task]["labels"],
                 smiles=task_dataset_args[task]["smiles"],
-                unique_ids=all_mol_ids[idx_per_task[task][0] : idx_per_task[task][1]],
+                indices=task_dataset_args[task]["sample_idx"],
+                unique_ids=all_unique_mol_ids[idx_per_task[task][0] : idx_per_task[task][1]],
                 **task_dataset_args[task]["extras"],
             )
 
         """We split the data up to create train, val and test datasets"""
         self.train_singletask_datasets = {}
         self.val_singletask_datasets = {}
         self.test_singletask_datasets = {}
```

### Comparing `graphium-2.1.3/graphium/data/dataset.py` & `graphium-2.2.0/graphium/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,51 +18,46 @@
 
 class SingleTaskDataset(Dataset):
     def __init__(
         self,
         labels: List[Union[torch.Tensor, np.ndarray]],
         features: Optional[List[Union[Data, "GraphDict"]]] = None,
         smiles: Optional[List[str]] = None,
-        indices: Optional[List[str]] = None,
+        indices: Optional[List[int]] = None,
         weights: Optional[Union[torch.Tensor, np.ndarray]] = None,
         unique_ids: Optional[List[str]] = None,
+        mol_ids: Optional[List[str]] = None,
     ):
         r"""
         dataset for a single task
         Parameters:
             labels: A list of labels for the given task (one per graph)
             features: A list of graphs
             smiles: A list of smiles
             indices: A list of indices
             weights: A list of weights
-            unique_ids: A list of unique ids
+            unique_ids: A list of unique ids for each molecule generated from `datamol.unique_id`
+            mol_ids: A list of ids coming from the original dataset. Useful to identify the molecule in the original dataset.
         """
 
         # Verify that all lists are the same length
         numel = len(labels)
-        if features is not None:
-            assert (
-                len(features) == numel
-            ), f"features must be the same length as labels, got {len(features)} and {numel}"
-        if smiles is not None:
-            assert (
-                len(smiles) == numel
-            ), f"smiles must be the same length as labels, got {len(smiles)} and {numel}"
-        if indices is not None:
-            assert (
-                len(indices) == numel
-            ), f"indices must be the same length as labels, got {len(indices)} and {numel}"
-        if weights is not None:
-            assert (
-                len(weights) == numel
-            ), f"weights must be the same length as labels, got {len(weights)} and {numel}"
-        if unique_ids is not None:
-            assert (
-                len(unique_ids) == numel
-            ), f"unique_ids must be the same length as labels, got {len(unique_ids)} and {numel}"
+
+        def _check_if_same_length(to_check, label):
+            """Simple utility method to throw an error if the length is not as expected."""
+            if to_check is not None and len(to_check) != numel:
+                raise ValueError(
+                    f"{label} must be the same length as `labels`, got {len(to_check)} and {numel}"
+                )
+
+        _check_if_same_length(features, "features")
+        _check_if_same_length(indices, "indices")
+        _check_if_same_length(weights, "weights")
+        _check_if_same_length(unique_ids, "unique_ids")
+        _check_if_same_length(mol_ids, "mol_ids")
 
         self.labels = labels
         if smiles is not None:
             manager = Manager()  # Avoid memory leaks with `num_workers > 0` by using the Manager
             self.smiles = manager.list(smiles)
         else:
             self.smiles = None
@@ -70,14 +65,15 @@
         self.indices = indices
         if self.indices is not None:
             self.indices = np.array(
                 self.indices
             )  # Avoid memory leaks with `num_workers > 0` by using numpy array
         self.weights = weights
         self.unique_ids = unique_ids
+        self.mol_ids = mol_ids
 
     def __len__(self):
         r"""
         return the size of the dataset
         Returns:
             size: the size of the dataset
         """
@@ -107,25 +103,29 @@
 
         if self.weights is not None:
             datum["weights"] = self.weights[idx]
 
         if self.unique_ids is not None:
             datum["unique_ids"] = self.unique_ids[idx]
 
+        if self.mol_ids is not None:
+            datum["mol_ids"] = self.mol_ids[idx]
+
         return datum
 
     def __getstate__(self):
         """Serialize the class for pickling."""
         state = {}
         state["labels"] = self.labels
         state["smiles"] = list(self.smiles) if self.smiles is not None else None
         state["features"] = self.features
         state["indices"] = self.indices
         state["weights"] = self.weights
         state["unique_ids"] = self.unique_ids
+        state["mol_ids"] = self.mol_ids
         return state
 
     def __setstate__(self, state: dict):
         """Reload the class from pickling."""
         if state["smiles"] is not None:
             manager = Manager()
             state["smiles"] = manager.list(state["smiles"])
@@ -167,14 +167,16 @@
             backend: Parallelization backend
             featurization_batch_size: The batch size to use for the parallelization of the featurization
             progress: Whether to display the progress bar
             save_smiles_and_ids: Whether to save the smiles and ids for the dataset. If `False`, `mol_ids` and `smiles` are set to `None`
             about: A description of the dataset
             progress: Whether to display the progress bar
             about: A description of the dataset
+            data_path: The location of the data if saved on disk
+            load_from_file: Whether to load the data from disk
             files_ready: Whether the files to load from were prepared ahead of time
         """
         super().__init__()
         # self.datasets = datasets
         self.n_jobs = n_jobs
         self.backend = backend
         self.featurization_batch_size = featurization_batch_size
@@ -374,25 +376,14 @@
         Returns:
             A dictionary containing the data for the specified index with keys "mol_ids", "smiles", "labels", and "features"
         """
         datum = {}
         if self.load_from_file:
             data_dict = self.load_graph_from_index(idx)
             datum["features"] = data_dict["graph_with_features"]
-            # these type changes are necessary for label dtype match of the largmix
-            # if hasattr(data_dict["labels"], "graph_l1000_vcap"):
-            #     data_dict["labels"].graph_l1000_vcap = data_dict["labels"].graph_l1000_vcap.astype(np.float32)
-            # if hasattr(data_dict["labels"], "graph_l1000_mcf7"):
-            #     data_dict["labels"].graph_l1000_mcf7 = data_dict["labels"].graph_l1000_mcf7.astype(np.float32)
-            # if hasattr(data_dict["labels"], "graph_pcba_1328"):
-            #     data_dict["labels"].graph_pcba_1328 = data_dict["labels"].graph_pcba_1328.astype(np.float32)
-            # if hasattr(data_dict["labels"], "graph_pcqm4m_g25"):
-            #     data_dict["labels"].graph_pcqm4m_g25 = data_dict["labels"].graph_pcqm4m_g25.astype(np.float32)
-            # if hasattr(data_dict["labels"], "node_pcqm4m_n4"):
-            #     data_dict["labels"].node_pcqm4m_n4 = data_dict["labels"].node_pcqm4m_n4.astype(np.float32)
             datum["labels"] = data_dict["labels"]
             if "smiles" in data_dict.keys():
                 datum["smiles"] = data_dict["smiles"]
         else:
             if self.mol_ids is not None:
                 datum["mol_ids"] = self.mol_ids[idx]
```

### Comparing `graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb` & `graphium-2.2.0/graphium/data/make_data_splits/make_train_val_test_splits_large.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb` & `graphium-2.2.0/graphium/data/make_data_splits/make_train_val_test_splits_small.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/micro_ZINC/micro_ZINC.csv` & `graphium-2.2.0/graphium/data/micro_ZINC/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/multilevel_utils.py` & `graphium-2.2.0/graphium/data/multilevel_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,19 @@
             graph_data_list = ast.literal_eval(graph_data)
             return np.array(graph_data_list)
         elif isinstance(graph_data, (int, float)):
             return np.array([graph_data])
         elif isinstance(graph_data, list):
             return np.array(graph_data)
         elif isinstance(graph_data, np.ndarray):
+            if len(graph_data.shape) == 0:
+                graph_data = np.expand_dims(graph_data, 0)
+            if graph_data.shape[0] == 0:
+                graph_data = np.array([np.nan])
+                # TODO: Warning
             return graph_data
         else:
             raise ValueError(
                 f"Graph data should be one of str, float, int, list, np.ndarray, got {type(graph_data)}"
             )
 
     def unpack_column(data: pd.Series):
```

### Comparing `graphium-2.1.3/graphium/data/multitask/tiny_ZINC_SA.csv` & `graphium-2.2.0/graphium/data/multitask/tiny_ZINC_SA.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/multitask/tiny_ZINC_logp.csv` & `graphium-2.2.0/graphium/data/multitask/tiny_ZINC_logp.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/multitask/tiny_ZINC_score.csv` & `graphium-2.2.0/graphium/data/multitask/tiny_ZINC_score.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/normalization.py` & `graphium-2.2.0/graphium/data/normalization.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/sdf2csv.py` & `graphium-2.2.0/graphium/data/sdf2csv.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/data/smiles_transform.py` & `graphium-2.2.0/graphium/data/smiles_transform.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/expts/pyg_batching_sparse.ipynb` & `graphium-2.2.0/graphium/expts/pyg_batching_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/README.md` & `graphium-2.2.0/graphium/features/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/commute.py` & `graphium-2.2.0/graphium/features/commute.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/electrostatic.py` & `graphium-2.2.0/graphium/features/electrostatic.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/featurizer.py` & `graphium-2.2.0/graphium/features/featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/graphormer.py` & `graphium-2.2.0/graphium/features/graphormer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/nmp.py` & `graphium-2.2.0/graphium/features/nmp.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/periodic_table.csv` & `graphium-2.2.0/graphium/features/periodic_table.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/positional_encoding.py` & `graphium-2.2.0/graphium/features/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/properties.py` & `graphium-2.2.0/graphium/features/properties.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/rw.py` & `graphium-2.2.0/graphium/features/rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/spectral.py` & `graphium-2.2.0/graphium/features/spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/test_new_pes.ipynb` & `graphium-2.2.0/graphium/features/test_new_pes.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/features/transfer_pos_level.py` & `graphium-2.2.0/graphium/features/transfer_pos_level.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/ipu/ipu_dataloader.py` & `graphium-2.2.0/graphium/ipu/ipu_dataloader.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/ipu/ipu_losses.py` & `graphium-2.2.0/graphium/ipu/ipu_losses.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,60 @@
 import torch
 from torch import Tensor
-from torch.nn import BCELoss, MSELoss, L1Loss
+from torch.nn import BCELoss, BCEWithLogitsLoss, MSELoss, L1Loss
 from torch._C import _infer_size
 from loguru import logger
 from graphium.trainer.losses import HybridCELoss
 
 
+class BCEWithLogitsLossIPU(BCEWithLogitsLoss):
+    """
+    A modified version of the `torch.nn.BCEWithLogitsLoss` that can ignore NaNs
+    by giving them a weight of `0`. This allows it to work with compilation
+    and IPUs since it doesn't modify the tensor's shape.
+    """
+
+    def forward(self, input: Tensor, target: Tensor) -> Tensor:
+        prev_weight = None
+
+        target = target.clone().to(input.dtype)
+        weight = self.weight
+
+        # Get the original weight matrix. If None, set all weights = 1
+        if weight is not None:
+            prev_weight = self.weight.clone()
+            new_size = _infer_size(target.size(), weight.size())
+            weight = weight.expand(new_size).clone()
+        else:
+            weight = torch.ones(target.shape, dtype=input.dtype, device=input.device)
+
+        # Replace the nan-targets by 0 or 1. Take the value closest to the input.
+        # Give a weight of 0 where there are nan-targets
+        nan_targets = target.isnan()
+        nan_targets_0 = (input < 0.5) & nan_targets
+        nan_targets_1 = (input >= 0.5) & nan_targets
+        target[nan_targets_0] = 0.0
+        target[nan_targets_1] = 1.0
+        weight[nan_targets] = 0.0
+
+        # Compute the loss, and rescale by the number of nan elements
+        self.weight = weight
+        loss = super().forward(input, target)
+
+        num_real_targets = (~nan_targets).sum()
+        factor1 = torch.where(num_real_targets > 0, 1, 0)
+        factor2 = torch.where(num_real_targets > 0, 0, 1)
+        loss = factor1 * loss * nan_targets.numel() / (num_real_targets + factor2)
+
+        # Reset the self.weight to its original value
+        self.weight = prev_weight
+
+        return loss
+
+
 class BCELossIPU(BCELoss):
     """
     A modified version of the `torch.nn.BCELoss` that can ignore NaNs
     by giving them a weight of `0`. This allows it to work with compilation
     and IPUs since it doesn't modify the tensor's shape.
     """
 
@@ -127,18 +172,11 @@
         """
 
         target = target.clone().to(input.dtype)
         input = input.clone()
 
         # Replace the nan-targets in the input/target tensors by 0
         nan_targets = target.isnan()
-        input[nan_targets] = 0.0
-        target[nan_targets] = 0.0
 
         # Compute the loss, and rescale by the number of nan elements
-        loss = super().forward(input, target)
-        num_real_targets = (~nan_targets).sum()
-        factor1 = torch.where(num_real_targets > 0, 1, 0)
-        factor2 = torch.where(num_real_targets > 0, 0, 1)
-        loss = factor1 * loss * nan_targets.numel() / (num_real_targets + factor2)
-
+        loss = super().forward(input, target, nan_targets)
         return loss
```

### Comparing `graphium-2.1.3/graphium/ipu/ipu_metrics.py` & `graphium-2.2.0/graphium/ipu/ipu_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/ipu/ipu_simple_lightning.py` & `graphium-2.2.0/graphium/ipu/ipu_simple_lightning.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/ipu/ipu_utils.py` & `graphium-2.2.0/graphium/ipu/ipu_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,27 +109,26 @@
     if gradient_accumulation is not None:
         current = ipu_options.Training.gradient_accumulation
         assert (current == 1) or (
             current == gradient_accumulation
         ), f"Received inconsistent gradient accumulation `{current}` and `{gradient_accumulation}"
         ipu_options.Training.gradientAccumulation(gradient_accumulation)
 
-    ipu_options.anchorTensor("input", "input")
-    if precision == 16:
+    if precision == "16-true":
         # IPUOptions.loadFromFile currently doesn't support setting half partials, doing it here
         ipu_options.Precision.setPartialsType(torch.half)
     training_opts = ipu_options
 
     # Change the inference options to remove gradient accumulation
     inference_opts = deepcopy(ipu_options)
     inference_opts.Training.gradientAccumulation(1)
     if ipu_inference_opts is not None:
         ipu_inference_opts_file = ipu_options_list_to_file(ipu_inference_opts)
         inference_opts.loadFromFile(ipu_inference_opts_file.name)
-        inference_opts.close()
+        ipu_inference_opts_file.close()
 
     return training_opts, inference_opts
 
 
 def ipu_options_list_to_file(ipu_opts: Optional[List[str]]) -> tempfile._TemporaryFileWrapper:
     """
     Create a temporary file from a list of ipu configs, such that it can be read by `poptorch.Options.loadFromFile`
```

### Comparing `graphium-2.1.3/graphium/ipu/ipu_wrapper.py` & `graphium-2.2.0/graphium/ipu/ipu_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     ) -> Tuple[Tensor, Dict[str, Tensor]]:
         return PredictorModule.compute_loss(
             preds, targets, weights, loss_fun, target_nan_mask, multitask_handling
         )
 
     def on_train_batch_end(self, outputs, batch, batch_idx):
         outputs = self.convert_from_fp16(outputs)
-        outputs["loss"] = outputs["loss"].mean()
+        outputs["loss"] = outputs["loss"][outputs["loss"] != 0].mean()
         super().on_train_batch_end(outputs, batch, batch_idx)
 
     def training_step(self, batch, batch_idx) -> Dict[str, Any]:
         features, labels = batch["features"], batch["labels"]
         features, labels = self.squeeze_input_dims(features, labels)
         dict_input = {"features": features, "labels": labels}
         step_dict = super().training_step(dict_input, to_cpu=False)
```

### Comparing `graphium-2.1.3/graphium/ipu/to_dense_batch.py` & `graphium-2.2.0/graphium/ipu/to_dense_batch.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/README.md` & `graphium-2.2.0/graphium/nn/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/architectures/encoder_manager.py` & `graphium-2.2.0/graphium/nn/architectures/encoder_manager.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/architectures/global_architectures.py` & `graphium-2.2.0/graphium/nn/architectures/global_architectures.py`

 * *Files 1% similar despite different names*

```diff
@@ -987,23 +987,27 @@
 
         # Initialize the pre-processing neural net for nodes (applied directly on node features)
         if pre_nn_kwargs is not None:
             name = pre_nn_kwargs.pop("name", "pre-NN")
             self.pre_nn = FeedForwardNN(**pre_nn_kwargs, name=name)
             next_in_dim = self.pre_nn.out_dim
             gnn_kwargs.setdefault("in_dim", next_in_dim)
-            assert next_in_dim == gnn_kwargs["in_dim"], "Inconsistent input/output dimensions"
+            assert (
+                next_in_dim == gnn_kwargs["in_dim"]
+            ), f"Inconsistent dimensions between pre-NN output ({next_in_dim}) and GNN input ({gnn_kwargs['in_dim']})"
 
         # Initialize the pre-processing neural net for edges (applied directly on edge features)
         if pre_nn_edges_kwargs is not None:
             name = pre_nn_edges_kwargs.pop("name", "pre-NN-edges")
             self.pre_nn_edges = FeedForwardNN(**pre_nn_edges_kwargs, name=name)
             next_in_dim = self.pre_nn_edges.out_dim
             gnn_kwargs.setdefault("in_dim_edges", next_in_dim)
-            assert next_in_dim == gnn_kwargs["in_dim_edges"], "Inconsistent input/output dimensions"
+            assert (
+                next_in_dim == gnn_kwargs["in_dim_edges"]
+            ), f"Inconsistent dimensions between pre-NN-edges output ({next_in_dim}) and GNN input ({gnn_kwargs['in_dim_edges']})"
 
         # Initialize the graph neural net (applied after the pre_nn)
         name = gnn_kwargs.pop("name", "GNN")
         gnn_class = self._parse_feed_forward_gnn(gnn_kwargs)
         gnn_kwargs.setdefault(
             "last_layer_is_readout", self.last_layer_is_readout and (task_heads_kwargs is None)
         )
```

### Comparing `graphium-2.1.3/graphium/nn/architectures/pyg_architectures.py` & `graphium-2.2.0/graphium/nn/architectures/pyg_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/base_graph_layer.py` & `graphium-2.2.0/graphium/nn/base_graph_layer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/base_layers.py` & `graphium-2.2.0/graphium/nn/base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/README.md` & `graphium-2.2.0/graphium/nn/encoders/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/base_encoder.py` & `graphium-2.2.0/graphium/nn/encoders/base_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/bessel_pos_encoder.py` & `graphium-2.2.0/graphium/nn/encoders/bessel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/gaussian_kernel_pos_encoder.py` & `graphium-2.2.0/graphium/nn/encoders/gaussian_kernel_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/laplace_pos_encoder.py` & `graphium-2.2.0/graphium/nn/encoders/laplace_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/mlp_encoder.py` & `graphium-2.2.0/graphium/nn/encoders/mlp_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/encoders/signnet_pos_encoder.py` & `graphium-2.2.0/graphium/nn/encoders/signnet_pos_encoder.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/README.md` & `graphium-2.2.0/graphium/nn/pyg_layers/README.md`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/dimenet_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/dimenet_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/gated_gcn_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/gated_gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/gcn_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/gcn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/gin_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/gin_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/gps_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/gps_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/mpnn_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/mpnn_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/pna_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/pna_pyg.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/pooling_pyg.py` & `graphium-2.2.0/graphium/nn/pyg_layers/pooling_pyg.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         batch (LongTensor): Batch vector :math:`\mathbf{b} \in {\{ 0, \ldots,
             B-1\}}^N`, which assigns each node to a specific example.
         size (int, optional): Batch-size :math:`B`.
             Automatically calculated if not given. (default: :obj:`None`)
     Returns:
         the pooled features tensor
     """
-    dim_size = int(batch.max().item() + 1) if dim_size is None else dim_size
+    dim_size = int(batch.max().detach() + 1) if dim_size is None else dim_size
     mean_pool = scatter(x, batch, dim=dim, dim_size=dim_size, reduce="mean")
     num_nodes = scatter(
         torch.ones(x.shape[:-1], dtype=x.dtype, device=x.device),
         batch,
         dim=dim,
         dim_size=dim_size,
         reduce="sum",
@@ -61,15 +61,15 @@
             B-1\}}^N`, which assigns each node to a specific example.
         size (int, optional): Batch-size :math:`B`.
             Automatically calculated if not given. (default: :obj:`None`)
 
     Returns:
         the pooled features tensor
     """
-    dim_size = int(batch.max().item() + 1) if dim_size is None else dim_size
+    dim_size = int(batch.max().detach() + 1) if dim_size is None else dim_size
     mean = scatter(x, batch, dim=dim, out=None, dim_size=dim_size, reduce="mean")
     mean_squares = scatter(x * x, batch, dim=dim, out=None, dim_size=dim_size, reduce="mean")
     out = mean_squares - mean * mean
     return torch.sqrt(torch.relu(out) + 1e-5)
 
 
 class PoolingWrapperPyg(ModuleWrap):
```

### Comparing `graphium-2.1.3/graphium/nn/pyg_layers/utils.py` & `graphium-2.2.0/graphium/nn/pyg_layers/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/residual_connections.py` & `graphium-2.2.0/graphium/nn/residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/nn/utils.py` & `graphium-2.2.0/graphium/nn/utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/trainer/metrics.py` & `graphium-2.2.0/graphium/trainer/metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/trainer/predictor.py` & `graphium-2.2.0/graphium/trainer/predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         target_nan_mask: Optional[Union[str, int]] = None,
         multitask_handling: Optional[str] = None,
         metrics: Dict[str, Callable] = None,
         metrics_on_progress_bar: Dict[str, List[str]] = [],
         metrics_on_training_set: Optional[Dict[str, List[str]]] = None,
         flag_kwargs: Dict[str, Any] = None,
         task_norms: Optional[Dict[Callable, Any]] = None,
+        metrics_every_n_train_steps: Optional[int] = None,
     ):
         """
         The Lightning module responsible for handling the predictions, losses, metrics, optimization, etc.
         It works in a multi-task setting, with different losses and metrics per class
 
         Parameters:
             model_class: The torch Module containing the main forward function
@@ -54,14 +55,16 @@
             scheduler_kwargs: The lightning scheduler arguments. See class `OptimOptions`
             target_nan_mask: How to handle the NaNs. See `MetricsWrapper` for options
             metrics: A `dict[str, fun]`, where `str` is the task name and `fun` the metric function
             metrics_on_progress_bar: A `dict[str, list[str2]`, where `str` is the task name and `str2` the metrics to include on the progress bar
             metrics_on_training_set: A `dict[str, list[str2]`, where `str` is the task name and `str2` the metrics to include on the training set
             flag_kwargs: Arguments related to using the FLAG adversarial augmentation
             task_norms: the normalization for each task
+            metrics_every_n_train_steps: Compute and log metrics every n training steps.
+                Set to `None` to never log the training metrics and statistics (the default). Set to `1` to log at every step.
         """
         self.save_hyperparameters()
 
         self.random_seed = random_seed
         torch.random.manual_seed(self.random_seed)
         np.random.seed(self.random_seed)
 
@@ -158,14 +161,19 @@
         # throughput estimation
         self.mean_val_time_tracker = MovingAverageTracker()
         self.mean_val_tput_tracker = MovingAverageTracker()
         self.validation_step_outputs = []
         self.test_step_outputs = []
         self.epoch_start_time = None
 
+        # Decide whether to log every step or once at the end
+        # of the epoch.
+        self.metrics_every_n_train_steps = metrics_every_n_train_steps
+        # Wether save preds and targets for each training step.
+
     def forward(
         self, inputs: Dict
     ) -> Dict[str, Union[Tensor, Dict[str, Tensor], Dict[str, Dict[str, Tensor]]]]:
         r"""
         Returns the result of `self.model.forward(*inputs)` on the inputs.
         If the output of `out = self.model.forward` is a dictionary with a `"preds"` key,
         it is returned directly. Otherwise, a new dictionary is created and
@@ -435,48 +443,68 @@
         step_dict[f"loss/{step_name}"] = loss.detach().cpu()
         step_dict["loss"] = loss
         step_dict["task_losses"] = task_losses
         return step_dict
 
     def on_train_batch_start(self, batch: Any, batch_idx: int) -> Optional[int]:
         self.train_batch_start_time = time.time()
+        self.skip_log_train_metrics = (self.metrics_every_n_train_steps is None) or (
+            (batch_idx % self.metrics_every_n_train_steps) != 0
+        )
         return super().on_train_batch_start(batch, batch_idx)
 
     def on_train_batch_end(self, outputs, batch: Any, batch_idx: int) -> None:
-        train_batch_time = time.time() - self.train_batch_start_time
+        train_batch_time = time.time() - self.train_batch_start_time  # To be used for throughput calculation
+
+        # Get the metrics that are logged at every step (loss, grad_norm, batch_time, batch_tput)
+        concatenated_metrics_logs = {}
+        concatenated_metrics_logs["train/loss"] = outputs["loss"]
+
+        # report the training loss for each individual tasks
+        for task in self.tasks:
+            concatenated_metrics_logs[f"train/loss/{task}"] = outputs["task_losses"][task]
+
+        # get the mean loss value for individual tasks as they are a tensor of size --> gradient accumulation * replication * device_iter
+        for key in concatenated_metrics_logs:
+            if isinstance(concatenated_metrics_logs[key], torch.Tensor):
+                if concatenated_metrics_logs[key].numel() > 1:
+                    concatenated_metrics_logs[key] = concatenated_metrics_logs[key][
+                        concatenated_metrics_logs[key] != 0
+                    ].mean()
+
+        # If logging is skipped for this step, then log the important metrics anyway and return
+        if self.skip_log_train_metrics:
+            if self.logger is not None:
+                self.logger.log_metrics(
+                    concatenated_metrics_logs, step=self.global_step
+                )  # This is a pytorch lightning function call
+            return
+
+        ### The code below is not executed if the logging is skipped for this step ###
+
+        # Get the throughput of the batch
         num_graphs = self.get_num_graphs(batch["features"])
         tput = num_graphs / train_batch_time
+        concatenated_metrics_logs["train/batch_time"] = train_batch_time
+        concatenated_metrics_logs["train/batch_tput"] = tput
 
-        # this code is likely repeated for validation and testing, this should be moved to a function
+        # Compute all the metrics for the training set
         self.task_epoch_summary.update_predictor_state(
             step_name="train",
             targets=outputs["targets"],
             predictions=outputs["preds"],
             loss=outputs["loss"],  # This is the weighted loss for now, but change to task-specific loss
             task_losses=outputs["task_losses"],
             n_epochs=self.current_epoch,
         )
         metrics_logs = self.task_epoch_summary.get_metrics_logs()  # Dict[task, metric_logs]
         metrics_logs["_global"]["grad_norm"] = self.get_gradient_norm()
-        outputs.update(metrics_logs)  # Dict[task, metric_logs]. Concatenate them?
+        concatenated_metrics_logs.update(metrics_logs)
 
-        concatenated_metrics_logs = {}  # self.task_epoch_summary.concatenate_metrics_logs(metrics_logs)
-        concatenated_metrics_logs["train/loss"] = outputs["loss"]
-        outputs["grad_norm"] = self.get_gradient_norm()
-        concatenated_metrics_logs["train/grad_norm"] = outputs["grad_norm"]
-        concatenated_metrics_logs["train/batch_time"] = train_batch_time
-        concatenated_metrics_logs["train/batch_tput"] = tput
-        # report the training loss for each individual tasks
-        for task in self.tasks:
-            concatenated_metrics_logs[f"train/loss/{task}"] = outputs["task_losses"][task]
-        # get the mean loss value for individual tasks as they are a tensor of size --> gradient accumulation * replication * device_iter
-        for key in concatenated_metrics_logs:
-            if isinstance(concatenated_metrics_logs[key], torch.Tensor):
-                if concatenated_metrics_logs[key].numel() > 1:
-                    concatenated_metrics_logs[key] = concatenated_metrics_logs[key].mean()
+        # Log the metrics
         if self.logger is not None:
             self.logger.log_metrics(
                 concatenated_metrics_logs, step=self.global_step
             )  # This is a pytorch lightning function call
 
     def training_step(self, batch: Dict[str, Tensor], to_cpu: bool = True) -> Dict[str, Any]:
         step_dict = None
@@ -485,23 +513,27 @@
         if self.flag_kwargs["n_steps"] > 0:
             step_dict = self.flag_step(batch=batch, step_name="train", to_cpu=to_cpu)
         # Train normally, without using FLAG
         elif self.flag_kwargs["n_steps"] == 0:
             # step_dict = self._general_step(batch=batch, step_name="train", to_cpu=True)
             step_dict = self._general_step(batch=batch, step_name="train", to_cpu=to_cpu)
 
+        # Remove the preds and targets if no logging is required
+        if self.skip_log_train_metrics:
+            step_dict.pop("preds")
+            step_dict.pop("targets")
         return step_dict  # Returning the metrics_logs with the loss
 
     def get_gradient_norm(self):
         # compute the norm
         total_norm = torch.tensor(0.0)
         for p in self.parameters():
             if p.grad is not None:
                 param_norm = p.grad.detach().data.norm(2)
-                total_norm += param_norm.item() ** 2
+                total_norm += param_norm.detach().cpu() ** 2
         total_norm = total_norm**0.5
         return total_norm
 
     def validation_step(self, batch: Dict[str, Tensor], to_cpu: bool = True) -> Dict[str, Any]:
         return self._general_step(batch=batch, step_name="val", to_cpu=to_cpu)
 
     def test_step(self, batch: Dict[str, Tensor], to_cpu: bool = True) -> Dict[str, Any]:
@@ -606,15 +638,15 @@
         hparams_log = deepcopy(self.hparams)
         hparams_log["n_params"] = self.n_params
         if self.logger is not None:
             self.logger.log_hyperparams(hparams_log)
 
     def get_progress_bar_dict(self) -> Dict[str, float]:
         prog_dict = {}
-        prog_dict["loss"] = self.task_epoch_summary.weighted_loss.item()
+        prog_dict["loss"] = self.task_epoch_summary.weighted_loss.detach().cpu()
         results_on_progress_bar = self.task_epoch_summary.get_results_on_progress_bar("val")
         for task in self.tasks:
             prog_dict[self.task_epoch_summary.metric_log_name(task, "loss", "val")] = (
                 self.task_epoch_summary.task_summaries[task].summaries["val"].loss
             )
             prog_dict.update(results_on_progress_bar)
         return prog_dict
```

### Comparing `graphium-2.1.3/graphium/trainer/predictor_options.py` & `graphium-2.2.0/graphium/trainer/predictor_options.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/trainer/predictor_summaries.py` & `graphium-2.2.0/graphium/trainer/predictor_summaries.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/arg_checker.py` & `graphium-2.2.0/graphium/utils/arg_checker.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/command_line_utils.py` & `graphium-2.2.0/graphium/utils/command_line_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/custom_lr.py` & `graphium-2.2.0/graphium/utils/custom_lr.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/dict_tensor.py` & `graphium-2.2.0/graphium/utils/dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/fs.py` & `graphium-2.2.0/graphium/utils/fs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/mup.py` & `graphium-2.2.0/graphium/utils/mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/packing.py` & `graphium-2.2.0/graphium/utils/packing.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,21 +133,21 @@
             if we collect `num_nodes` from the indices, then each pack has roughly the
             same total number of atoms.
     """
     num_nodes = np.asarray(num_nodes)
     argsort_num_nodes = np.argsort(num_nodes)
     ipu_batch_size = int(len(num_nodes) / batch_size)
 
-    groups = []
-    for ii in range(batch_size):
-        group = argsort_num_nodes[ii * ipu_batch_size : (ii + 1) * ipu_batch_size]
-        np.random.shuffle(group)
-        groups.append(group)
-
-    packed_indices = np.stack(groups, axis=1).tolist()
+    packed_indices = np.stack(
+        [
+            np.random.permutation(argsort_num_nodes[ii * ipu_batch_size : (ii + 1) * ipu_batch_size])
+            for ii in range(batch_size)
+        ],
+        axis=0,
+    ).T.tolist()
     return packed_indices
 
 
 def hybrid_packing(num_nodes: List[int], batch_size: int) -> List[List[int]]:
     """
     Uses a combination of the `smart_packing` `O(n^2)` on the most important data points,
     and the `fast_packing` `O(n)` on the average-sized data points.
@@ -170,20 +170,16 @@
 
     # Determine the parameters based on the complexity of the smart-packing.
     # The bigger the complexity, the more the `fast_packing` algorithm becomes
     # statistically powerful, and the more speed benefits it provides.
     smart_packing_complexity = len(num_nodes) ** 2 / batch_size
     if smart_packing_complexity < 1e4:
         return smart_packing(num_nodes=num_nodes, batch_size=batch_size)
-    elif smart_packing_complexity < 1e6:
+    elif smart_packing_complexity < 1e5:
         big, small = 3, 6
-    elif smart_packing_complexity < 1e8:
-        big, small = 2, 4
-    elif smart_packing_complexity < 1e10:
-        big, small = 1, 2
     else:
         return fast_packing(num_nodes=num_nodes, batch_size=batch_size)
 
     # Small datasets benefit from smart-packing, without compute burden
     ipu_batch_size = int(len(num_nodes) / batch_size)
     if len(num_nodes) < (big + small) * ipu_batch_size:
         return smart_packing(num_nodes=num_nodes, batch_size=batch_size)
```

### Comparing `graphium-2.1.3/graphium/utils/read_file.py` & `graphium-2.2.0/graphium/utils/read_file.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/safe_run.py` & `graphium-2.2.0/graphium/utils/safe_run.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium/utils/spaces.py` & `graphium-2.2.0/graphium/utils/spaces.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 LOSS_DICT = {
     "mse": torch.nn.MSELoss,
     "bce": torch.nn.BCELoss,
     "l1": torch.nn.L1Loss,
     "mae": torch.nn.L1Loss,
     "hybrid_ce": Losses.HybridCELoss,
     "bce_ipu": IPULosses.BCELossIPU,
+    "bce_logits_ipu": IPULosses.BCEWithLogitsLossIPU,
     "mse_ipu": IPULosses.MSELossIPU,
     "mae_ipu": IPULosses.L1LossIPU,
     "l1_ipu": IPULosses.L1LossIPU,
     "hybrid_ce_ipu": IPULosses.HybridCELossIPU,
 }
 
 
@@ -115,9 +116,10 @@
 METRICS_DICT = deepcopy(METRICS_CLASSIFICATION)
 METRICS_DICT.update(METRICS_REGRESSION)
 
 
 DATAMODULE_DICT = {
     "GraphOGBDataModule": Datamodules.GraphOGBDataModule,
     "MultitaskFromSmilesDataModule": Datamodules.MultitaskFromSmilesDataModule,
+    "ADMETBenchmarkDataModule": Datamodules.ADMETBenchmarkDataModule,
     "FakeDataModule": Datamodules.FakeDataModule,
 }
```

### Comparing `graphium-2.1.3/graphium/utils/tensor.py` & `graphium-2.2.0/graphium/utils/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         input = input.flatten(-len(dim))
         median, _ = torch.nanmedian(input, dim=-1, keepdim=False)
         if not keepdim:
             for d in dim[::-1]:
                 median = median.squeeze(d)
     else:
         if dim is None:
-            median = torch.nanmedian(input.flatten())
+            median = torch.nanmedian(input.flatten().float()).to(input.dtype)
         else:
             median, _ = torch.nanmedian(input, dim=dim, keepdim=keepdim)
 
     return median
 
 
 def nan_var(input: Tensor, unbiased: bool = True, **kwargs) -> Tensor:
@@ -246,16 +246,16 @@
             The desired data type of returned tensor.
             If specified, the input tensor is casted to dtype before the operation is performed.
             This is useful for preventing data type overflows. Default: None.
 
     Returns:
         output: The resulting standard deviation of the tensor
     """
-
-    return torch.sqrt(nan_var(input=input, unbiased=unbiased, **kwargs))
+    variances = nan_var(input=input, unbiased=unbiased, **kwargs)
+    return torch.sqrt(variances.float()).to(variances.dtype)
 
 
 def nan_mad(input: Tensor, normal: bool = True, **kwargs) -> Tensor:
     r"""
     Return the median absolute deviation of all elements, while ignoring the NaNs.
 
     Parameters:
```

### Comparing `graphium-2.1.3/graphium/visualization/vis_utils.py` & `graphium-2.2.0/graphium/visualization/vis_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/graphium.egg-info/PKG-INFO` & `graphium-2.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphium
-Version: 2.1.3
+Version: 2.2.0
 Summary: Graphium: Scaling molecular GNNs to infinity.
 Author-email: Dominique Beaini <dominique@valencediscovery.com>
 Project-URL: Website, https://graphium.datamol.io/
 Project-URL: Source Code, https://github.com/datamol-io/graphium
 Project-URL: Bug Tracker, https://github.com/datamol-io/graphium/issues
 Project-URL: Documentation, https://graphium-docs.datamol.io/
 Classifier: Development Status :: 5 - Production/Stable
@@ -39,18 +39,20 @@
 [![Conda](https://img.shields.io/conda/v/conda-forge/graphium?label=conda&color=success)](https://anaconda.org/conda-forge/graphium)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/graphium)](https://pypi.org/project/graphium/)
 [![Conda](https://img.shields.io/conda/dn/conda-forge/graphium)](https://anaconda.org/conda-forge/graphium)
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/datamol-io/graphium/blob/main/LICENSE)
 [![GitHub Repo stars](https://img.shields.io/github/stars/datamol-io/graphium)](https://github.com/datamol-io/graphium/stargazers)
 [![GitHub Repo stars](https://img.shields.io/github/forks/datamol-io/graphium)](https://github.com/datamol-io/graphium/network/members)
 [![test](https://github.com/datamol-io/graphium/actions/workflows/test.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test.yml)
+[![test-ipu](https://github.com/datamol-io/graphium/actions/workflows/test_ipu.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/test_ipu.yml)
 [![release](https://github.com/datamol-io/graphium/actions/workflows/release.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/release.yml)
 [![code-check](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/code-check.yml)
 [![doc](https://github.com/datamol-io/graphium/actions/workflows/doc.yml/badge.svg)](https://github.com/datamol-io/graphium/actions/workflows/doc.yml)
 [![codecov](https://codecov.io/gh/datamol-io/graphium/branch/main/graph/badge.svg?token=bHOkKY5Fze)](https://codecov.io/gh/datamol-io/graphium)
+[![hydra](https://img.shields.io/badge/Config-Hydra_1.3-89b8cd)](https://hydra.cc/)
 
 A deep learning library focused on graph representation learning for real-world chemical tasks.
 
 - ✅ State-of-the-art GNN architectures.
 - 🐍 Extensible API: build your own GNN model and train it with ease.
 - ⚗️ Rich featurization: powerful and flexible built-in molecular featurization.
 - 🧠 Pretrained models: for fast and easy inference or transfer learning.
@@ -90,27 +92,47 @@
 # Install the PopTorch wheel
 pip install PATH_TO_SDK/poptorch-3.2.0+109946_bb50ce43ab_ubuntu_20_04-cp38-cp38-linux_x86_64.whl
 
 # Enable Poplar SDK (including Poplar and PopART)
 source PATH_TO_SDK/enable
 
 # Install the IPU specific and graphium requirements
-PACKAGE_NAME=pytorch pip install -r requirements_ipu.txt
-pip install -r lightning.txt
+pip install -r requirements_ipu.txt
 
 # Install Graphium in dev mode
 pip install --no-deps -e .
 ```
 
 ## Training a model
 
 To learn how to train a model, we invite you to look at the documentation, or the jupyter notebooks available [here](https://github.com/datamol-io/graphium/tree/master/docs/tutorials/model_training).
 
 If you are not familiar with [PyTorch](https://pytorch.org/docs) or [PyTorch-Lightning](https://pytorch-lightning.readthedocs.io/en/latest/), we highly recommend going through their tutorial first.
 
+## Running an experiment
+We have setup Graphium with `hydra` for managing config files. To run an experiment go to the `expts/` folder. For example, to benchmark a GCN on the ToyMix dataset run
+```bash
+python main_run_multitask.py dataset=toymix model=gcn
+```
+To change parameters specific to this experiment like switching from `fp16` to `fp32` precision, you can either override them directly in the CLI via
+```bash
+python main_run_multitask.py dataset=toymix model=gcn trainer.trainer.precision=32
+```
+or change them permamently in the dedicated experiment config under `expts/hydra-configs/toymix_gcn.yaml`.
+Integrating `hydra` also allows you to quickly switch between accelerators. E.g., running
+```bash
+python main_run_multitask.py dataset=toymix model=gcn accelerator=gpu
+```
+automatically selects the correct configs to run the experiment on GPU.
+To use a config file you built from scratch you can run
+```bash
+python main_run_multitask.py --config-path [PATH] --config-name [CONFIG]
+```
+Thanks to the modular nature of `hydra` you can reuse many of our config settings for your own experiments with Graphium.
+
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
 
 ## Documentation
 
 - Diagram for data processing in molGPS.
```

### Comparing `graphium-2.1.3/graphium.egg-info/SOURCES.txt` & `graphium-2.2.0/graphium.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 .gitignore
 LICENSE
 README.md
 cleanup_files.sh
 codecov.yml
 env.yml
-lightning.txt
 mkdocs.yml
 pyproject.toml
 requirements_ipu.txt
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/workflows/code-check.yml
 .github/workflows/doc.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
+.github/workflows/test_ipu.yml
 docs/baseline.md
 docs/cli_references.md
 docs/contribute.md
 docs/datasets.md
 docs/design.md
 docs/index.md
 docs/license.md
@@ -47,36 +47,51 @@
 docs/tutorials/feature_processing/timing_parallel.ipynb
 docs/tutorials/gnn/add_new_gnn_layers.ipynb
 docs/tutorials/gnn/making_gnn_networks.ipynb
 docs/tutorials/gnn/using_gnn_layers.ipynb
 docs/tutorials/model_training/running-multitask-ipu.ipynb
 docs/tutorials/model_training/simple-molecular-model.ipynb
 expts/dataset_benchmark.py
+expts/debug_yaml.py
 expts/main_run_get_fingerprints.py
 expts/main_run_multitask.py
 expts/main_run_predict.py
 expts/main_run_test.py
 expts/run_validation_test.py
-expts/test_yaml.py
 expts/configs/config_gps_10M_pcqm4m.yaml
 expts/configs/config_gps_10M_pcqm4m_mod.yaml
 expts/configs/config_gpspp_10M_pcqm4m.yaml
 expts/configs/config_mpnn_10M_b3lyp.yaml
 expts/configs/config_mpnn_10M_pcqm4m.yaml
 expts/configs/config_mpnn_pcqm4m.yaml
+expts/configs/config_tdc_admet_demo.yaml
 expts/data/micro_zinc_splits.csv
 expts/data/tiny_zinc_splits.csv
+expts/hydra-configs/main.yaml
+expts/hydra-configs/accelerator/cpu.yaml
+expts/hydra-configs/accelerator/gpu.yaml
+expts/hydra-configs/accelerator/ipu.yaml
+expts/hydra-configs/dataset/toymix.yaml
+expts/hydra-configs/dataset/accelerator/toymix_cpu.yaml
+expts/hydra-configs/dataset/accelerator/toymix_gpu.yaml
+expts/hydra-configs/dataset/accelerator/toymix_ipu.yaml
+expts/hydra-configs/experiment/toymix_gcn.yaml
+expts/hydra-configs/experiment/toymix_gin.yaml
+expts/hydra-configs/model/gcn.yaml
+expts/hydra-configs/model/gin.yaml
 expts/neurips2023_configs/config_classifigression_l1000.yaml
 expts/neurips2023_configs/config_large_gcn.yaml
+expts/neurips2023_configs/config_large_gcn_gpu.yaml
 expts/neurips2023_configs/config_large_gin.yaml
 expts/neurips2023_configs/config_large_gine.yaml
 expts/neurips2023_configs/config_large_mpnn.yaml
 expts/neurips2023_configs/config_luis_jama.yaml
 expts/neurips2023_configs/config_small_gated_gcn.yaml
 expts/neurips2023_configs/config_small_gcn.yaml
+expts/neurips2023_configs/config_small_gcn_gpu.yaml
 expts/neurips2023_configs/config_small_gin.yaml
 expts/neurips2023_configs/config_small_gine.yaml
 expts/neurips2023_configs/config_small_mpnn.yaml
 expts/neurips2023_configs/baseline/config_small_gcn_baseline.yaml
 expts/neurips2023_configs/baseline/config_small_gin_baseline.yaml
 expts/neurips2023_configs/baseline/config_small_gine_baseline.yaml
 expts/neurips2023_configs/debug/config_debug.yaml
@@ -120,14 +135,15 @@
 graphium/data/README.md
 graphium/data/__init__.py
 graphium/data/collate.py
 graphium/data/datamodule.py
 graphium/data/dataset.py
 graphium/data/multilevel_utils.py
 graphium/data/normalization.py
+graphium/data/sampler.py
 graphium/data/sdf2csv.py
 graphium/data/smiles_transform.py
 graphium/data/utils.py
 graphium/data/L1000/datasets_goli-L1000_parse_gctx_to_csv.ipynb
 graphium/data/QM9/micro_qm9.csv
 graphium/data/QM9/micro_qm9.parquet
 graphium/data/QM9/norm_micro_qm9.csv
@@ -222,25 +238,27 @@
 graphium/visualization/vis_utils.py
 notebooks/dev-datamodule-invalidate-cache.ipynb
 notebooks/dev-datamodule-ogb.ipynb
 notebooks/dev-datamodule.ipynb
 notebooks/dev-pretrained.ipynb
 notebooks/dev-training-loop.ipynb
 notebooks/dev.ipynb
+notebooks/finetuning-on-tdc-admet-benchmark.ipynb
 notebooks/running-fingerprints-from-pretrained-model.ipynb
 notebooks/running-model-from-config.ipynb
 profiling/configs_profiling.yaml
 profiling/profile_mol_to_graph.py
 profiling/profile_one_of_k_encoding.py
 profiling/profile_predictor.py
 scripts/convert_yml.py
 scripts/ipu_start.sh
 scripts/ipu_venv.sh
 tests/.gitignore
 tests/config_test_ipu_dataloader.yaml
+tests/config_test_ipu_dataloader_multitask.yaml
 tests/conftest.py
 tests/converted_fake_multilevel_data.parquet
 tests/fake_and_missing_multilevel_data.parquet
 tests/test_architectures.py
 tests/test_attention.py
 tests/test_base_layers.py
 tests/test_collate.py
@@ -248,14 +266,16 @@
 tests/test_datamodule.py
 tests/test_dataset.py
 tests/test_dict_tensor.py
 tests/test_featurizer.py
 tests/test_ipu_dataloader.py
 tests/test_ipu_losses.py
 tests/test_ipu_metrics.py
+tests/test_ipu_options.py
+tests/test_ipu_to_dense_batch.py
 tests/test_loaders.py
 tests/test_losses.py
 tests/test_metrics.py
 tests/test_mtl_architecture.py
 tests/test_multitask_datamodule.py
 tests/test_mup.py
 tests/test_packing.py
```

### Comparing `graphium-2.1.3/mkdocs.yml` & `graphium-2.2.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/dev-datamodule-invalidate-cache.ipynb` & `graphium-2.2.0/notebooks/dev-datamodule-invalidate-cache.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/dev-datamodule-ogb.ipynb` & `graphium-2.2.0/notebooks/dev-datamodule-ogb.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/dev-datamodule.ipynb` & `graphium-2.2.0/notebooks/dev-datamodule.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/dev-pretrained.ipynb` & `graphium-2.2.0/notebooks/dev-pretrained.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/dev-training-loop.ipynb` & `graphium-2.2.0/notebooks/dev-training-loop.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/dev.ipynb` & `graphium-2.2.0/notebooks/dev.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/running-fingerprints-from-pretrained-model.ipynb` & `graphium-2.2.0/notebooks/running-fingerprints-from-pretrained-model.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/notebooks/running-model-from-config.ipynb` & `graphium-2.2.0/notebooks/running-model-from-config.ipynb`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/profiling/configs_profiling.yaml` & `graphium-2.2.0/profiling/configs_profiling.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/profiling/profile_mol_to_graph.py` & `graphium-2.2.0/profiling/profile_mol_to_graph.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/profiling/profile_predictor.py` & `graphium-2.2.0/profiling/profile_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/pyproject.toml` & `graphium-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -98,14 +98,17 @@
 filterwarnings = [
     "ignore::DeprecationWarning:ray.*:",
     "ignore::DeprecationWarning:numba.*:",
     "ignore::DeprecationWarning:lightning_fabric.*:",
     "ignore::DeprecationWarning:pytorch_lightning.*:",
     "ignore::DeprecationWarning:pkg_resources.*:",
 ]
+markers = [
+    "ipu: marks tests that are specific to the IPU (deselect with '-m \"not ipu\"')",
+]
 
 [tool.coverage.run]
 source = ["graphium/"]
 disable_warnings = ["no-data-collected"]
 data_file = ".coverage/coverage"
 
 [tool.coverage.report]
```

### Comparing `graphium-2.1.3/requirements_ipu.txt` & `graphium-2.2.0/requirements_ipu.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,24 @@
---find-links https://data.pyg.org/whl/torch-1.13.0+cpu.html
---find-links https://download.pytorch.org/whl/cpu/torch_stable.html
+--find-links https://data.pyg.org/whl/torch-2.0.1+cpu.html
 
 pip
 click
 loguru
 tqdm
 numpy
 scipy >==1.4
 sympy
 pandas >==1.0
 scikit-learn
 seaborn
-fsspec >==2021.6
-s3fs >==2021.6
-gcsfs >==2021.6
+fsspec >==2023.6.0
+s3fs >==2023.6.0
+gcsfs >==2023.6.0
 appdirs
 tensorboard
-torch <2.0
 torchmetrics >=0.7.0,<0.11
 hydra-core >==1.0
 ogb
 rdkit >==2020.09
 umap-learn
 pytest >==6.0
 pytest-cov
@@ -45,13 +43,14 @@
 tk
 datamol
 PyYAML
 wandb
 optuna
 google-cloud-storage
 mup
+networkx
 pyg-nightly
 fastparquet
-torch-scatter==2.1.0
-torch-sparse==0.6.15
-torchvision==0.14.1+cpu
+torch-scatter==2.1.1
+torch-sparse==0.6.17
+lightning @ git+https://github.com/Lightning-AI/lightning@ca30fd7752582201a3966806c92e3acbbaf2a045
 lightning-graphcore @ git+https://github.com/Lightning-AI/lightning-Graphcore
```

### Comparing `graphium-2.1.3/scripts/convert_yml.py` & `graphium-2.2.0/scripts/convert_yml.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/scripts/ipu_venv.sh` & `graphium-2.2.0/scripts/ipu_venv.sh`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/config_test_ipu_dataloader.yaml` & `graphium-2.2.0/tests/config_test_ipu_dataloader.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/converted_fake_multilevel_data.parquet` & `graphium-2.2.0/tests/converted_fake_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/config_micro_ZINC.yaml` & `graphium-2.2.0/tests/data/config_micro_ZINC.yaml`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/micro_ZINC.csv` & `graphium-2.2.0/tests/data/micro_ZINC.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/micro_ZINC_corrupt.csv` & `graphium-2.2.0/tests/data/micro_ZINC_corrupt.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/micro_ZINC_shard_1.csv` & `graphium-2.2.0/tests/data/micro_ZINC_shard_1.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/micro_ZINC_shard_1.parquet` & `graphium-2.2.0/tests/data/micro_ZINC_shard_1.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/micro_ZINC_shard_2.csv` & `graphium-2.2.0/tests/data/micro_ZINC_shard_2.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/micro_ZINC_shard_2.parquet` & `graphium-2.2.0/tests/data/micro_ZINC_shard_2.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/data/pcqm4mv2-2k.csv` & `graphium-2.2.0/tests/data/pcqm4mv2-2k.csv`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/fake_and_missing_multilevel_data.parquet` & `graphium-2.2.0/tests/fake_and_missing_multilevel_data.parquet`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_architectures.py` & `graphium-2.2.0/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_attention.py` & `graphium-2.2.0/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_base_layers.py` & `graphium-2.2.0/tests/test_base_layers.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_collate.py` & `graphium-2.2.0/tests/test_collate.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_data_utils.py` & `graphium-2.2.0/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_datamodule.py` & `graphium-2.2.0/tests/test_datamodule.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_dataset.py` & `graphium-2.2.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_dict_tensor.py` & `graphium-2.2.0/tests/test_dict_tensor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_featurizer.py` & `graphium-2.2.0/tests/test_featurizer.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_ipu_metrics.py` & `graphium-2.2.0/tests/test_ipu_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     r2_score,
     f1_score,
     fbeta_score,
     mean_squared_error,
     mean_absolute_error,
 )
 from copy import deepcopy
+import pytest
 
 from graphium.ipu.ipu_metrics import (
     auroc_ipu,
     average_precision_ipu,
     precision_ipu,
     accuracy_ipu,
     recall_ipu,
@@ -28,14 +29,15 @@
     f1_score_ipu,
     fbeta_score_ipu,
     mean_squared_error_ipu,
     mean_absolute_error_ipu,
 )
 
 
+@pytest.mark.ipu
 class test_Metrics(ut.TestCase):
     torch.manual_seed(42)
     preds = torch.rand((100, 10), dtype=torch.float32)
     target = torch.rand((100, 10), dtype=torch.float32)
 
     th = 0.7
     nan_th = 0.2
```

### Comparing `graphium-2.1.3/tests/test_loaders.py` & `graphium-2.2.0/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_losses.py` & `graphium-2.2.0/tests/test_losses.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_metrics.py` & `graphium-2.2.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_mtl_architecture.py` & `graphium-2.2.0/tests/test_mtl_architecture.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_multitask_datamodule.py` & `graphium-2.2.0/tests/test_multitask_datamodule.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+import shutil
+import tempfile
 import unittest as ut
+
+import pytest
 from omegaconf import OmegaConf
 import pandas as pd
 import numpy as np
 import graphium
 
 
 class Test_Multitask_DataModule(ut.TestCase):
+    def setUp(self):
+        # Create a temporary directory
+        self.tmp_test_dir = tempfile.mkdtemp()
+
+    def tearDown(self):
+        # Remove the directory after the test
+        shutil.rmtree(self.tmp_test_dir)
+
     def test_multitask_fromsmiles_dm(
         self,
     ):  # TODO: I think we can remove this as it tests tiny_zinc which only contain graph level labels
         """Cover similar testing as for the original data module."""
         df = graphium.data.load_tiny_zinc()  # 100 molecules
 
         # Here we take the microzinc dataset and split the labels up into 'SA', 'logp' and 'score' in order to simulate having multiple single-task datasets
@@ -206,72 +218,60 @@
 
         dm_args = OmegaConf.to_container(config.datamodule.args, resolve=True)
         dm = graphium.data.MultitaskFromSmilesDataModule(**dm_args)
 
         dm.prepare_data()
         dm.setup()
 
-        # self.assertEqual(len(dm), 100)                      # Should this have a fixed value for when it's initialized? MTL dataset only gets created after.
-        self.assertEqual(len(dm.train_ds), 602)  # type: ignore
-        self.assertEqual(len(dm.val_ds), 201)  # type: ignore
-        self.assertEqual(len(dm.test_ds), 201)  # type: ignore
-        # assert dm.num_node_feats == 50
-        # assert dm.num_edge_feats == 6
-
-        for dl in [dm.train_dataloader(), dm.val_dataloader(), dm.test_dataloader()]:
-            dl = dm.train_dataloader()
-            it = iter(dl)
-            batch = next(it)
-
-            assert set(batch.keys()) == {"labels", "features"}
+        self.assertEqual(len(dm.train_ds), 1004)  # type: ignore
 
-            # assert batch["labels"].shape == (16, 1)            # Single-task case
-            assert batch["labels"]["graph_SA"].shape == (16, 1)
-            assert batch["labels"]["node_logp"].shape == (
-                batch["features"].feat.size(0),
-                2,
-            )  # test node level
-            assert batch["labels"]["edge_score"].shape == (
-                batch["features"].edge_feat.size(0),
-                2,
-            )  # test edge level
+        dl = dm.train_dataloader()
+        it = iter(dl)
+        batch = next(it)
+
+        assert set(batch.keys()) == {"labels", "features"}
+
+        # assert batch["labels"].shape == (16, 1)            # Single-task case
+        assert batch["labels"]["graph_SA"].shape == (16, 1)
+        assert batch["labels"]["node_logp"].shape == (
+            batch["features"].feat.size(0),
+            2,
+        )  # test node level
+        assert batch["labels"]["edge_score"].shape == (
+            batch["features"].edge_feat.size(0),
+            2,
+        )  # test edge level
 
     def test_multitask_with_missing_fromsmiles_from_config_parquet(self):
         config = graphium.load_config(name="fake_and_missing_multilevel_multitask_pyg")
 
         dm_args = OmegaConf.to_container(config.datamodule.args, resolve=True)
         dm = graphium.data.MultitaskFromSmilesDataModule(**dm_args)
 
         dm.prepare_data()
         dm.setup()
 
-        # self.assertEqual(len(dm), 100)                      # Should this have a fixed value for when it's initialized? MTL dataset only gets created after.
-        self.assertEqual(len(dm.train_ds), 602)  # type: ignore
-        self.assertEqual(len(dm.val_ds), 201)  # type: ignore
-        self.assertEqual(len(dm.test_ds), 201)  # type: ignore
-        # assert dm.num_node_feats == 50
-        # assert dm.num_edge_feats == 6
-
-        for dl in [dm.train_dataloader(), dm.val_dataloader(), dm.test_dataloader()]:
-            dl = dm.train_dataloader()
-            it = iter(dl)
-            batch = next(it)
-
-            assert set(batch.keys()) == {"labels", "features"}
+        self.assertEqual(len(dm.train_ds), 1004)  # type: ignore
 
-            # assert batch["labels"].shape == (16, 1)            # Single-task case
-            assert batch["labels"]["graph_SA"].shape == (16, 1)
-            assert batch["labels"]["node_logp"].shape == (
-                batch["features"].feat.size(0),
-                2,
-            )  # test node level
-            assert batch["labels"]["edge_score"].shape == (
-                batch["features"].edge_feat.size(0),
-                2,
-            )  # test edge level
+        dl = dm.train_dataloader()
+        it = iter(dl)
+        batch = next(it)
+
+        assert set(batch.keys()) == {"labels", "features"}
+
+        # assert batch["labels"].shape == (16, 1)            # Single-task case
+        assert batch["labels"]["graph_SA"].shape == (16, 1)
+        assert batch["labels"]["node_logp"].shape == (
+            batch["features"].feat.size(0),
+            2,
+        )  # test node level
+        assert batch["labels"]["edge_score"].shape == (
+            batch["features"].edge_feat.size(0),
+            2,
+        )  # test edge level
 
     def test_extract_graph_level_singletask(self):
         df = pd.read_parquet(f"tests/converted_fake_multilevel_data.parquet")
         num_graphs = len(df)
         label_cols = ["graph_label"]
         output = graphium.data.datamodule.extract_labels(df, "graph", label_cols)
 
@@ -336,10 +336,60 @@
                     assert output[idx].shape[1] == len(label_cols)
 
                     # Check that number of labels is adjusted correctly
                     if replace == 1:
                         non_missing_col = label_cols[1]
                         assert output[idx].shape[0] == len(df[non_missing_col][idx])
 
+    def test_tdc_admet_benchmark_data_module(self):
+        """
+        Verifies that the ADMET-specific subclass of the MultiTaskDataModule works.
+        Checks if all main endpoints can be run and if the split is correct.
+        """
+
+        try:
+            from tdc.benchmark_group import admet_group
+            from tdc.utils import retrieve_benchmark_names
+        except ImportError:
+            self.skipTest("PyTDC needs to be installed to run this test. Use `pip install PyTDC`.")
+            raise
+
+        # Make sure we can initialize the module and run the main endpoints
+        data_module = graphium.data.ADMETBenchmarkDataModule()
+        data_module.prepare_data()
+        data_module.setup()
+
+        for dl in [
+            data_module.train_dataloader(),
+            data_module.val_dataloader(),
+            data_module.test_dataloader(),
+        ]:
+            batch = next(iter(dl))
+            assert set(batch.keys()) == {"labels", "features"}
+
+        # # Validate the split
+        group = admet_group(path=self.tmp_test_dir)
+        benchmark_names = retrieve_benchmark_names("admet_group")
+
+        # For each of the endpoints...
+        for name in benchmark_names:
+            # Get the split from the benchmark group (ground truth)
+            benchmark = group.get(name)
+            train, val = group.get_train_valid_split(0, name)
+            test = benchmark["test"]
+
+            # Get the split from the data module
+            params = data_module._get_task_specific_arguments(name, 0, self.tmp_test_dir)
+            split = pd.read_csv(params.splits_path)
+            data = params.df
+
+            # Check that the split is the same
+            for ground_truth, label in [(train, "train"), (val, "val"), (test, "test")]:
+                y_true = ground_truth["Y"].values
+                y_module = data.loc[split[label].dropna(), "Y"].values
+
+                assert len(y_true) == len(y_module)
+                assert np.allclose(np.sort(y_true), np.sort(y_module))
+
 
 if __name__ == "__main__":
     ut.main()
```

### Comparing `graphium-2.1.3/tests/test_mup.py` & `graphium-2.2.0/tests/test_mup.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_packing.py` & `graphium-2.2.0/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_pe_nodepair.py` & `graphium-2.2.0/tests/test_pe_nodepair.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_pe_rw.py` & `graphium-2.2.0/tests/test_pe_rw.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_pe_spectral.py` & `graphium-2.2.0/tests/test_pe_spectral.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_pos_transfer_funcs.py` & `graphium-2.2.0/tests/test_pos_transfer_funcs.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_positional_encoders.py` & `graphium-2.2.0/tests/test_positional_encoders.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_positional_encodings.py` & `graphium-2.2.0/tests/test_positional_encodings.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_predictor.py` & `graphium-2.2.0/tests/test_predictor.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_pyg_layers.py` & `graphium-2.2.0/tests/test_pyg_layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 import numpy as np
 import torch
 import unittest as ut
 from torch_geometric.data import Data, Batch
 from copy import deepcopy
+import pytest
 
 from graphium.nn.pyg_layers import (
     GINConvPyg,
     GINEConvPyg,
     MPNNPlusPyg,
     GatedGCNPyg,
     PNAMessagePassingPyg,
@@ -212,14 +213,15 @@
         self.assertEqual(layer.out_dim_factor, 1)
 
         bg2 = layer.forward(bg)
         self.assertEqual(bg2.feat.shape[0], feat_in.shape[0])
         self.assertEqual(bg2.feat.shape[1], self.out_dim * layer.out_dim_factor)
         self.assertTrue((bg2.edge_feat == self.bg.edge_feat).all)
 
+    @pytest.mark.skip_ipu
     def test_dimenetlayer(self):
         from graphium.nn.encoders.bessel_pos_encoder import BesselSphericalPosEncoder
 
         bg = deepcopy(self.bg)
         # dummy input pos
         bg.pos = torch.randn((bg.feat.shape[0], 3), dtype=torch.float32)
```

### Comparing `graphium-2.1.3/tests/test_residual_connections.py` & `graphium-2.2.0/tests/test_residual_connections.py`

 * *Files identical despite different names*

### Comparing `graphium-2.1.3/tests/test_utils.py` & `graphium-2.2.0/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 from graphium.utils.tensor import nan_mad, nan_mean, nan_std, nan_var, nan_median
 from graphium.utils.safe_run import SafeRun
 import torch
 import numpy as np
 import scipy as sp
 import unittest as ut
+import gzip
+from graphium.utils.read_file import file_opener
 
 
 class test_nan_statistics(ut.TestCase):
     torch.manual_seed(42)
 
     dims = [
         None,
@@ -121,14 +123,40 @@
 
                 # Compare the nan-median
                 torch_mad = nan_mad(tensor, **torch_kwargs)
                 numpy_mad = sp.stats.median_abs_deviation(tensor.numpy(), **numpy_kwargs)
                 np.testing.assert_almost_equal(torch_mad.numpy(), numpy_mad, decimal=4, err_msg=err_msg)
 
 
+def test_file_opener(tmp_path):
+    # Create a temporary file
+    txt_file = tmp_path / "test.txt"
+    txt_file.write_text("Hello, World!")
+
+    # Test opening file in read mode
+    with file_opener(txt_file, "r") as f:
+        assert f.read() == "Hello, World!"
+
+    # Test opening file in write mode
+    with file_opener(txt_file, "w") as f:
+        f.write("New text")
+
+    with file_opener(txt_file, "r") as f:
+        assert f.read() == "New text"
+
+    # Create a temporary gzip file
+    gzip_file = tmp_path / "test.txt.gz"
+    with gzip.open(gzip_file, "wt") as f:
+        f.write("Hello, Gzip!")
+
+    # Test opening gzip file in read mode
+    with file_opener(gzip_file, "r") as f:
+        assert f.read() == "Hello, Gzip!"
+
+
 class test_SafeRun(ut.TestCase):
     def test_safe_run(self):
         # Error is caught
         with SafeRun(name="bob", raise_error=False, verbose=0):
             raise ValueError("This is an error")
 
         # Error is caught
```

