# Comparing `tmp/d3rlpy-2.0.3.tar.gz` & `tmp/d3rlpy-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3rlpy-2.0.3.tar", last modified: Tue Jul 18 13:52:45 2023, max compression
+gzip compressed data, was "d3rlpy-2.0.4.tar", last modified: Fri Jul 21 08:45:52 2023, max compression
```

## Comparing `d3rlpy-2.0.3.tar` & `d3rlpy-2.0.4.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1068 2022-09-11 02:40:22.000000 d3rlpy-2.0.3/LICENSE
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      125 2022-09-11 02:40:22.000000 d3rlpy-2.0.3/MANIFEST.in
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12192 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/PKG-INFO
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9411 2023-07-18 07:57:09.000000 d3rlpy-2.0.3/README.md
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.002464 d3rlpy-2.0.3/d3rlpy/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      496 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       22 2023-07-18 13:52:25.000000 d3rlpy-2.0.3/d3rlpy/_version.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.002464 d3rlpy-2.0.3/d3rlpy/algos/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       75 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/__init__.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.002464 d3rlpy-2.0.3/d3rlpy/algos/qlearning/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      351 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5973 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/awac.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    32009 2023-07-18 13:42:32.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6171 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/bc.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14962 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/bcq.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10883 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/bear.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12529 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/cql.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7331 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/crr.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5449 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/ddpg.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6647 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/dqn.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4001 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/explorers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6525 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/iql.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3697 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/nfq.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12022 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/plas.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4336 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/random_policy.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12811 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/sac.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6320 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/td3.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5837 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/td3_plus_bc.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      323 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3267 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/awac_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4059 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/bc_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7013 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/bcq_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8012 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/bear_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8546 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/cql_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5466 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/crr_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4252 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/ddpg_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3014 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/dqn_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3549 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/iql_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5343 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/plas_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7320 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/sac_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1936 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/td3_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1546 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1104 2023-07-18 13:43:50.000000 d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/algos/transformer/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       78 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/transformer/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12680 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/transformer/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4813 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/transformer/decision_transformer.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4010 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/transformer/inputs.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/algos/transformer/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       41 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/transformer/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2222 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/transformer/torch/decision_transformer_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4456 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/algos/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12802 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9991 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/cli.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1265 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/constants.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/dataset/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      310 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3071 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/buffers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2032 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/compat.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11090 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/components.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2577 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/episode_generator.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3264 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/io.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7410 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/mini_batch.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15505 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/replay_buffer.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2941 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/trajectory_slicers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5413 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/transition_pickers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      286 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/types.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7796 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/utils.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12332 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/dataset/writers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14906 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/datasets.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/envs/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/envs/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      143 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/envs/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15039 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/envs/wrappers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1041 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/interface.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/itertools.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/logging/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      134 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/logging/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2650 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/logging/file_adapter.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4169 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/logging/logger.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1050 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/logging/noop_adapter.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2457 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/logging/tensorboard_adapter.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2114 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/logging/utils.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/metrics/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       49 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/metrics/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    18066 2023-07-18 13:44:05.000000 d3rlpy-2.0.3/d3rlpy/metrics/evaluators.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2965 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/metrics/utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/models/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      101 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10171 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/builders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10380 2023-07-18 06:51:00.000000 d3rlpy-2.0.3/d3rlpy/models/encoders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5301 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/optimizers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6626 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/q_functions.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/models/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      210 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4284 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/distributions.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11014 2023-07-18 07:05:05.000000 d3rlpy-2.0.3/d3rlpy/models/torch/encoders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7803 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/imitators.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      484 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/parameters.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11312 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/policies.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      198 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1574 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9237 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/ensemble_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9520 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/fqf_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7216 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/iqn_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3194 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/mean_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5040 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/qr_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2552 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12509 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/transformers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      860 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/torch/v_functions.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/models/utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/ope/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       19 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/ope/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8378 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/ope/fqe.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/ope/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       24 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/ope/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3436 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/ope/torch/fqe_impl.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/d3rlpy/preprocessing/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      115 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/preprocessing/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6533 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/preprocessing/action_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3265 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/preprocessing/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    13692 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/preprocessing/observation_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15062 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/preprocessing/reward_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4821 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/serializable_config.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9874 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/d3rlpy/torch_utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 13:52:45.002464 d3rlpy-2.0.3/d3rlpy.egg-info/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12192 2023-07-18 13:52:44.000000 d3rlpy-2.0.3/d3rlpy.egg-info/PKG-INFO
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3747 2023-07-18 13:52:44.000000 d3rlpy-2.0.3/d3rlpy.egg-info/SOURCES.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2023-07-18 13:52:44.000000 d3rlpy-2.0.3/d3rlpy.egg-info/dependency_links.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       43 2023-07-18 13:52:44.000000 d3rlpy-2.0.3/d3rlpy.egg-info/entry_points.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       96 2023-07-18 13:52:44.000000 d3rlpy-2.0.3/d3rlpy.egg-info/requires.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        7 2023-07-18 13:52:44.000000 d3rlpy-2.0.3/d3rlpy.egg-info/top_level.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2023-07-18 13:52:43.000000 d3rlpy-2.0.3/d3rlpy.egg-info/zip-safe
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       38 2023-07-18 13:52:45.006464 d3rlpy-2.0.3/setup.cfg
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1825 2023-07-18 06:25:45.000000 d3rlpy-2.0.3/setup.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1068 2022-09-11 02:40:22.000000 d3rlpy-2.0.4/LICENSE
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12059 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/PKG-INFO
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9286 2023-07-19 14:37:01.000000 d3rlpy-2.0.4/README.md
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.060900 d3rlpy-2.0.4/d3rlpy/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      496 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       22 2023-07-21 08:45:14.000000 d3rlpy-2.0.4/d3rlpy/_version.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.060900 d3rlpy-2.0.4/d3rlpy/algos/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       75 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/__init__.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/algos/qlearning/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      351 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5973 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/awac.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    32009 2023-07-18 13:42:32.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6171 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/bc.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    14962 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/bcq.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10883 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/bear.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12588 2023-07-18 15:26:37.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/cql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7331 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/crr.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5449 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/ddpg.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6647 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/dqn.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4001 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/explorers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6525 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/iql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3697 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/nfq.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12022 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/plas.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4336 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/random_policy.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12811 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/sac.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6320 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/td3.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5837 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/td3_plus_bc.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      323 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3267 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/awac_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4059 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/bc_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7013 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/bcq_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8012 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/bear_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8546 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/cql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5466 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/crr_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4252 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/ddpg_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3014 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/dqn_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3549 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/iql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5343 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/plas_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7320 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/sac_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1936 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/td3_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1546 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1104 2023-07-18 13:43:50.000000 d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/algos/transformer/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       78 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/transformer/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12680 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/transformer/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4813 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/transformer/decision_transformer.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4010 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/transformer/inputs.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/algos/transformer/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       41 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/transformer/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2222 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/transformer/torch/decision_transformer_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4456 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/algos/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12802 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9735 2023-07-21 07:09:38.000000 d3rlpy-2.0.4/d3rlpy/cli.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1265 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/constants.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/dataset/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      310 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3071 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/buffers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2032 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/compat.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11090 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/components.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2577 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/episode_generator.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3487 2023-07-19 13:49:08.000000 d3rlpy-2.0.4/d3rlpy/dataset/io.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7410 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/mini_batch.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15506 2023-07-19 13:55:00.000000 d3rlpy-2.0.4/d3rlpy/dataset/replay_buffer.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2941 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/trajectory_slicers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5413 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/transition_pickers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      286 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/types.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7796 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/utils.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12332 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/dataset/writers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    16065 2023-07-21 08:24:44.000000 d3rlpy-2.0.4/d3rlpy/datasets.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/envs/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/envs/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      143 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/envs/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11749 2023-07-21 06:58:36.000000 d3rlpy-2.0.4/d3rlpy/envs/wrappers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1041 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/interface.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/itertools.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/logging/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      134 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/logging/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2650 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/logging/file_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4169 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/logging/logger.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1050 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/logging/noop_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2457 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/logging/tensorboard_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2114 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/logging/utils.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/metrics/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       49 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/metrics/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    17958 2023-07-21 06:51:28.000000 d3rlpy-2.0.4/d3rlpy/metrics/evaluators.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2719 2023-07-21 06:51:45.000000 d3rlpy-2.0.4/d3rlpy/metrics/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.064900 d3rlpy-2.0.4/d3rlpy/models/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      101 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10171 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/builders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10380 2023-07-18 06:51:00.000000 d3rlpy-2.0.4/d3rlpy/models/encoders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5301 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/optimizers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6626 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/q_functions.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/d3rlpy/models/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      210 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4284 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/distributions.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11014 2023-07-18 07:05:05.000000 d3rlpy-2.0.4/d3rlpy/models/torch/encoders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7803 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/imitators.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      484 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/parameters.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11312 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/policies.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      198 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1574 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9237 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/ensemble_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9520 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/fqf_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7216 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/iqn_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3194 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/mean_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5040 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/qr_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2552 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12509 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/transformers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      860 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/torch/v_functions.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/models/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/d3rlpy/ope/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       19 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/ope/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8378 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/ope/fqe.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/d3rlpy/ope/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       24 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/ope/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3436 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/ope/torch/fqe_impl.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/d3rlpy/preprocessing/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      115 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/preprocessing/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6533 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/preprocessing/action_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3265 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/preprocessing/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    13692 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/preprocessing/observation_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15062 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/preprocessing/reward_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4821 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/serializable_config.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9874 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/d3rlpy/torch_utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-21 08:45:52.060900 d3rlpy-2.0.4/d3rlpy.egg-info/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12059 2023-07-21 08:45:52.000000 d3rlpy-2.0.4/d3rlpy.egg-info/PKG-INFO
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3735 2023-07-21 08:45:52.000000 d3rlpy-2.0.4/d3rlpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2023-07-21 08:45:52.000000 d3rlpy-2.0.4/d3rlpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       43 2023-07-21 08:45:52.000000 d3rlpy-2.0.4/d3rlpy.egg-info/entry_points.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       96 2023-07-21 08:45:52.000000 d3rlpy-2.0.4/d3rlpy.egg-info/requires.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        7 2023-07-21 08:45:52.000000 d3rlpy-2.0.4/d3rlpy.egg-info/top_level.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2023-07-21 08:45:49.000000 d3rlpy-2.0.4/d3rlpy.egg-info/zip-safe
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       38 2023-07-21 08:45:52.068900 d3rlpy-2.0.4/setup.cfg
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1825 2023-07-18 06:25:45.000000 d3rlpy-2.0.4/setup.py
```

### Comparing `d3rlpy-2.0.3/LICENSE` & `d3rlpy-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/PKG-INFO` & `d3rlpy-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d3rlpy
-Version: 2.0.3
+Version: 2.0.4
 Summary: An offline deep reinforcement learning library
 Home-page: https://github.com/takuseno/d3rlpy
 Author: Takuma Seno
 Author-email: takuma.seno@gmail.com
 License: MIT License
 Description: <p align="center"><img align="center" width="300px" src="assets/logo.png"></p>
         
@@ -64,18 +64,17 @@
         [![PyPI version](https://badge.fury.io/py/d3rlpy.svg)](https://badge.fury.io/py/d3rlpy)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/d3rlpy)
         ```
         $ pip install d3rlpy
         ```
         ### Anaconda
         [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/version.svg)](https://anaconda.org/conda-forge/d3rlpy)
-        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/platforms.svg)](https://anaconda.org/conda-forge/d3rlpy)
         [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/downloads.svg)](https://anaconda.org/conda-forge/d3rlpy)
         ```
-        $ conda install -c conda-forge d3rlpy
+        $ conda install conda-forge/noarch::d3rlpy
         ```
         
         ### Docker
         ![Docker Pulls](https://img.shields.io/docker/pulls/takuseno/d3rlpy)
         ```
         $ docker run -it --gpus all --name d3rlpy takuseno/d3rlpy:latest bash
         ```
```

### Comparing `d3rlpy-2.0.3/README.md` & `d3rlpy-2.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,17 @@
 [![PyPI version](https://badge.fury.io/py/d3rlpy.svg)](https://badge.fury.io/py/d3rlpy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/d3rlpy)
 ```
 $ pip install d3rlpy
 ```
 ### Anaconda
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/version.svg)](https://anaconda.org/conda-forge/d3rlpy)
-[![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/platforms.svg)](https://anaconda.org/conda-forge/d3rlpy)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/downloads.svg)](https://anaconda.org/conda-forge/d3rlpy)
 ```
-$ conda install -c conda-forge d3rlpy
+$ conda install conda-forge/noarch::d3rlpy
 ```
 
 ### Docker
 ![Docker Pulls](https://img.shields.io/docker/pulls/takuseno/d3rlpy)
 ```
 $ docker run -it --gpus all --name d3rlpy takuseno/d3rlpy:latest bash
 ```
```

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/awac.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/awac.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/base.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/bc.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/bc.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/bcq.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/bcq.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/bear.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/bear.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/cql.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/cql.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,18 +305,18 @@
             gamma=self._config.gamma,
             alpha=self._config.alpha,
             device=self._device,
         )
 
     def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
-        loss = self._impl.update(batch)
+        loss, conservative_loss = self._impl.update(batch)
         if self._grad_step % self._config.target_update_interval == 0:
             self._impl.update_target()
-        return {"loss": loss}
+        return {"loss": loss, "conservative_loss": conservative_loss}
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.DISCRETE
 
 
 register_learnable(CQLConfig)
 register_learnable(DiscreteCQLConfig)
```

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/crr.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/crr.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/ddpg.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/ddpg.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/dqn.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/dqn.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/explorers.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/explorers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/iql.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/iql.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/nfq.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/nfq.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/plas.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/plas.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/random_policy.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/random_policy.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/sac.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/sac.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/td3.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/td3.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/td3_plus_bc.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/td3_plus_bc.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/awac_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/awac_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/bc_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/bc_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/bcq_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/bcq_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/bear_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/bear_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/cql_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/cql_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/crr_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/crr_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/ddpg_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/ddpg_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/dqn_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/dqn_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/iql_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/iql_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/plas_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/plas_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/sac_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/sac_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/td3_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/td3_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/qlearning/torch/utility.py` & `d3rlpy-2.0.4/d3rlpy/algos/qlearning/torch/utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/transformer/base.py` & `d3rlpy-2.0.4/d3rlpy/algos/transformer/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/transformer/decision_transformer.py` & `d3rlpy-2.0.4/d3rlpy/algos/transformer/decision_transformer.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/transformer/inputs.py` & `d3rlpy-2.0.4/d3rlpy/algos/transformer/inputs.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/transformer/torch/decision_transformer_impl.py` & `d3rlpy-2.0.4/d3rlpy/algos/transformer/torch/decision_transformer_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/algos/utility.py` & `d3rlpy-2.0.4/d3rlpy/algos/utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/base.py` & `d3rlpy-2.0.4/d3rlpy/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/cli.py` & `d3rlpy-2.0.4/d3rlpy/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import json
 import os
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple
 
 import click
 import gym
 import numpy as np
+from gym.wrappers import RecordVideo
 
 from ._version import __version__
 from .algos import (
     QLearningAlgoBase,
     StatefulTransformerWrapper,
     TransformerAlgoBase,
 )
 from .base import load_learnable
-from .envs import Monitor
 from .metrics.utility import (
     evaluate_qlearning_with_environment,
     evaluate_transformer_with_environment,
 )
 
 if TYPE_CHECKING:
     import matplotlib.pyplot
@@ -245,64 +245,55 @@
 @click.option(
     "--env-header", default=None, help="one-liner to create environment."
 )
 @click.option("--out", default="videos", help="output directory path.")
 @click.option(
     "--n-episodes", default=3, help="the number of episodes to record."
 )
-@click.option("--frame-rate", default=60, help="video frame rate.")
-@click.option("--record-rate", default=1, help="record frame rate.")
 @click.option(
     "--target-return",
     default=None,
     help="the target return for Decision Transformer variants.",
 )
 def record(
     model_path: str,
     env_id: Optional[str],
     env_header: Optional[str],
     out: str,
     n_episodes: int,
-    frame_rate: float,
-    record_rate: int,
     target_return: Optional[float],
 ) -> None:
     # load saved model
     print(f"Loading {model_path}...")
     algo = load_learnable(model_path)
 
     # wrap environment with Monitor
     env: gym.Env[Any, Any]
     if env_id is not None:
-        env = gym.make(env_id)
+        env = gym.make(env_id, render_mode="rgb_array")
     elif env_header is not None:
         env = _exec_to_create_env(env_header)
     else:
         raise ValueError("env_id or env_header must be provided.")
 
-    wrapped_env = Monitor(
+    wrapped_env = RecordVideo(
         env,
         out,
-        video_callable=lambda ep: ep % 1 == 0,
-        frame_rate=float(frame_rate),
-        record_rate=int(record_rate),
+        episode_trigger=lambda ep: True,
     )
 
     # run episodes
     if isinstance(algo, QLearningAlgoBase):
-        evaluate_qlearning_with_environment(
-            algo, wrapped_env, n_episodes, render=True
-        )
+        evaluate_qlearning_with_environment(algo, wrapped_env, n_episodes)
     elif isinstance(algo, TransformerAlgoBase):
         assert target_return is not None, "--target-return must be specified."
         evaluate_transformer_with_environment(
             StatefulTransformerWrapper(algo, float(target_return)),
             wrapped_env,
             n_episodes,
-            render=True,
         )
     else:
         raise ValueError("invalid algo type.")
 
 
 @cli.command(short_help="Run evaluation episodes with rendering.")
 @click.argument("model_path")
@@ -326,26 +317,26 @@
     # load saved model
     print(f"Loading {model_path}...")
     algo = load_learnable(model_path)
 
     # wrap environment with Monitor
     env: gym.Env[Any, Any]
     if env_id is not None:
-        env = gym.make(env_id)
+        env = gym.make(env_id, render_mode="human")
     elif env_header is not None:
         env = _exec_to_create_env(env_header)
     else:
         raise ValueError("env_id or env_header must be provided.")
 
     # run episodes
     if isinstance(algo, QLearningAlgoBase):
-        evaluate_qlearning_with_environment(algo, env, n_episodes, render=True)
+        score = evaluate_qlearning_with_environment(algo, env, n_episodes)
     elif isinstance(algo, TransformerAlgoBase):
         assert target_return is not None, "--target-return must be specified."
-        evaluate_transformer_with_environment(
+        score = evaluate_transformer_with_environment(
             StatefulTransformerWrapper(algo, float(target_return)),
             env,
             n_episodes,
-            render=True,
         )
     else:
         raise ValueError("invalid algo type.")
+    print(f"Score: {score}")
```

### Comparing `d3rlpy-2.0.3/d3rlpy/constants.py` & `d3rlpy-2.0.4/d3rlpy/constants.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/buffers.py` & `d3rlpy-2.0.4/d3rlpy/dataset/buffers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/compat.py` & `d3rlpy-2.0.4/d3rlpy/dataset/compat.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/components.py` & `d3rlpy-2.0.4/d3rlpy/dataset/components.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/episode_generator.py` & `d3rlpy-2.0.4/d3rlpy/dataset/episode_generator.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/io.py` & `d3rlpy-2.0.4/d3rlpy/dataset/io.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,37 +5,37 @@
 
 from .components import Episode, EpisodeBase
 from .episode_generator import EpisodeGenerator
 
 __all__ = ["dump", "load", "load_v1", "DATASET_VERSION"]
 
 
-DATASET_VERSION = "2.0"
+DATASET_VERSION = "2.1"
 
 
 def dump(episodes: Sequence[EpisodeBase], f: BinaryIO) -> None:
     r"""Writes episode data to file-like object.
 
     Args:
         episodes: Sequence of episodes.
         f: Binary file-like object.
     """
-    serializedData = [episode.serialize() for episode in episodes]
-    keys = list(serializedData[0].keys())
     with h5py.File(f, "w") as h5:
+        keys = list(episodes[0].serialize().keys())
         h5.create_dataset("columns", data=keys)
-        h5.create_dataset("total_size", data=len(episodes))
-        for key in keys:
-            if isinstance(serializedData[0][key], (list, tuple)):
-                for i in range(len(serializedData[0][key])):
-                    data = [d[key][i] for d in serializedData]
-                    h5.create_dataset(f"{key}_{i}", data=data)
-            else:
-                data = [d[key] for d in serializedData]
-                h5.create_dataset(key, data=data)
+        h5.create_dataset("num_episodes", data=len(episodes))
+        for i, episode in enumerate(episodes):
+            serializedData = episode.serialize()
+            for key in keys:
+                if isinstance(serializedData[key], (list, tuple)):
+                    for j in range(len(serializedData[key])):
+                        elm = serializedData[key][j]
+                        h5.create_dataset(f"{key}_{i}_{j}", data=elm)
+                else:
+                    h5.create_dataset(f"{key}_{i}", data=serializedData[key])
         h5.create_dataset("version", data=DATASET_VERSION)
         h5.flush()
 
 
 def load(episode_cls: Type[EpisodeBase], f: BinaryIO) -> Sequence[EpisodeBase]:
     r"""Constructs episodes from file-like object.
 
@@ -44,30 +44,35 @@
         f: Binary file-like object.
 
     Returns:
         Sequence of episodes.
     """
     episodes = []
     with h5py.File(f, "r") as h5:
+        version = cast(str, h5["version"][()])
+        if version == "2.0":
+            raise ValueError("version=2.0 has been obsolete.")
         keys = cast(
-            Sequence[str], map(lambda s: s.decode("utf-8"), h5["columns"][()])
+            Sequence[str],
+            list(map(lambda s: s.decode("utf-8"), h5["columns"][()])),
         )
-        total_size = cast(int, h5["total_size"][()])
-        for i in range(total_size):
+        num_episodes = cast(int, h5["num_episodes"][()])
+        for i in range(num_episodes):
             data = {}
             for key in keys:
-                if key in h5:
-                    data[key] = h5[key][()][i]
+                path = f"{key}_{i}"
+                if path in h5:
+                    data[key] = h5[path][()]
                 else:
                     j = 0
                     tuple_data = []
                     while True:
-                        tuple_key = f"{key}_{j}"
-                        if tuple_key in h5:
-                            tuple_data.append(h5[tuple_key][()][i])
+                        tuple_path = f"{key}_{i}_{j}"
+                        if tuple_path in h5:
+                            tuple_data.append(h5[tuple_path][()])
                         else:
                             break
                         j += 1
                     data[key] = tuple_data
             episode = episode_cls.deserialize(data)
             episodes.append(episode)
     return episodes
```

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/mini_batch.py` & `d3rlpy-2.0.4/d3rlpy/dataset/mini_batch.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/replay_buffer.py` & `d3rlpy-2.0.4/d3rlpy/dataset/replay_buffer.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         )
 
     def dump(self, f: BinaryIO) -> None:
         """Dumps buffer data.
 
         .. code-block:: python
 
-            with open('dataset.h5', 'wb') as f:
+            with open('dataset.h5', 'w+b') as f:
                 replay_buffer.dump(f)
 
         Args:
             f: IO object to write to.
         """
         dump(self._buffer.episodes, f)
```

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/trajectory_slicers.py` & `d3rlpy-2.0.4/d3rlpy/dataset/trajectory_slicers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/transition_pickers.py` & `d3rlpy-2.0.4/d3rlpy/dataset/transition_pickers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/utils.py` & `d3rlpy-2.0.4/d3rlpy/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/dataset/writers.py` & `d3rlpy-2.0.4/d3rlpy/dataset/writers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/datasets.py` & `d3rlpy-2.0.4/d3rlpy/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     ReplayBuffer,
     TrajectorySlicerProtocol,
     TransitionPickerProtocol,
     create_infinite_replay_buffer,
     load_v1,
 )
 from .envs import ChannelFirst, FrameStack
+from .logging import LOG
 
 __all__ = [
     "DATA_DIRECTORY",
     "DROPBOX_URL",
     "CARTPOLE_URL",
     "CARTPOLE_RANDOM_URL",
     "PENDULUM_URL",
@@ -47,25 +48,27 @@
 PENDULUM_RANDOM_URL = f"{DROPBOX_URL}/hhbq9i6ako24kzz/pendulum_random_v1.1.0.h5?dl=1"  # pylint: disable=line-too-long
 
 
 def get_cartpole(
     dataset_type: str = "replay",
     transition_picker: Optional[TransitionPickerProtocol] = None,
     trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+    render_mode: Optional[str] = None,
 ) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, int]]:
     """Returns cartpole dataset and environment.
 
     The dataset is automatically downloaded to ``d3rlpy_data/cartpole.h5`` if
     it does not exist.
 
     Args:
         dataset_type: dataset type. Available options are
             ``['replay', 'random']``.
         transition_picker: TransitionPickerProtocol object.
         trajectory_slicer: TrajectorySlicerProtocol object.
+        render_mode: Mode of rendering (``human``, ``rgb_array``).
 
     Returns:
         tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     if dataset_type == "replay":
         url = CARTPOLE_URL
         file_name = "cartpole_replay_v1.1.0.h5"
@@ -90,34 +93,36 @@
         InfiniteBuffer(),
         episodes=episodes,
         transition_picker=transition_picker,
         trajectory_slicer=trajectory_slicer,
     )
 
     # environment
-    env = gym.make("CartPole-v1")
+    env = gym.make("CartPole-v1", render_mode=render_mode)
 
     return dataset, env
 
 
 def get_pendulum(
     dataset_type: str = "replay",
     transition_picker: Optional[TransitionPickerProtocol] = None,
     trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+    render_mode: Optional[str] = None,
 ) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, np.ndarray]]:
     """Returns pendulum dataset and environment.
 
     The dataset is automatically downloaded to ``d3rlpy_data/pendulum.h5`` if
     it does not exist.
 
     Args:
         dataset_type: dataset type. Available options are
             ``['replay', 'random']``.
         transition_picker: TransitionPickerProtocol object.
         trajectory_slicer: TrajectorySlicerProtocol object.
+        render_mode: Mode of rendering (``human``, ``rgb_array``).
 
     Returns:
         tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     if dataset_type == "replay":
         url = PENDULUM_URL
         file_name = "pendulum_replay_v1.1.0.h5"
@@ -141,22 +146,23 @@
         InfiniteBuffer(),
         episodes=episodes,
         transition_picker=transition_picker,
         trajectory_slicer=trajectory_slicer,
     )
 
     # environment
-    env = gym.make("Pendulum-v1")
+    env = gym.make("Pendulum-v1", render_mode=render_mode)
 
     return dataset, env
 
 
 def get_atari(
     env_name: str,
     num_stack: Optional[int] = None,
+    render_mode: Optional[str] = None,
 ) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, int]]:
     """Returns atari dataset and envrironment.
 
     The dataset is provided through d4rl-atari. See more details including
     available dataset from its GitHub page.
 
     .. code-block:: python
@@ -167,22 +173,23 @@
 
     References:
         * https://github.com/takuseno/d4rl-atari
 
     Args:
         env_name: environment id of d4rl-atari dataset.
         num_stack: the number of frames to stack (only applied to env).
+        render_mode: Mode of rendering (``human``, ``rgb_array``).
 
     Returns:
         tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     try:
         import d4rl_atari  # type: ignore
 
-        env = gym.make(env_name)
+        env = gym.make(env_name, render_mode=render_mode)
         raw_dataset = env.get_dataset()  # type: ignore
         episode_generator = EpisodeGenerator(**raw_dataset)
         dataset = create_infinite_replay_buffer(
             episodes=episode_generator(),
             transition_picker=FrameStackTransitionPicker(num_stack or 1),
             trajectory_slicer=None,
         )
@@ -199,14 +206,15 @@
 
 
 def get_atari_transitions(
     game_name: str,
     fraction: float = 0.01,
     index: int = 0,
     num_stack: Optional[int] = None,
+    render_mode: Optional[str] = None,
 ) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, int]]:
     """Returns atari dataset as a list of Transition objects and envrironment.
 
     The dataset is provided through d4rl-atari.
     The difference from ``get_atari`` function is that this function will
     sample transitions from all epochs.
     This function is necessary for reproducing Atari experiments.
@@ -222,29 +230,34 @@
         * https://github.com/takuseno/d4rl-atari
 
     Args:
         game_name: Atari 2600 game name in lower_snake_case.
         fraction: fraction of sampled transitions.
         index: index to specify which trial to load.
         num_stack: the number of frames to stack (only applied to env).
+        render_mode: Mode of rendering (``human``, ``rgb_array``).
 
     Returns:
         tuple of a list of :class:`d3rlpy.dataset.Transition` and gym
         environment.
     """
     try:
         import d4rl_atari
 
         # each epoch consists of 1M steps
         num_transitions_per_epoch = int(1000000 * fraction)
 
         copied_episodes = []
         for i in range(50):
+            env_name = f"{game_name}-epoch-{i + 1}-v{index}"
+            LOG.info(f"Collecting {env_name}...")
             env = gym.make(
-                f"{game_name}-epoch-{i + 1}-v{index}", sticky_action=True
+                env_name,
+                sticky_action=True,
+                render_mode=render_mode,
             )
             raw_dataset = env.get_dataset()  # type: ignore
             episode_generator = EpisodeGenerator(**raw_dataset)
             episodes = list(episode_generator())
 
             # copy episode data to release memory of unused data
             random.shuffle(episodes)
@@ -292,14 +305,15 @@
         ) from e
 
 
 def get_d4rl(
     env_name: str,
     transition_picker: Optional[TransitionPickerProtocol] = None,
     trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+    render_mode: Optional[str] = None,
 ) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, np.ndarray]]:
     """Returns d4rl dataset and envrironment.
 
     The dataset is provided through d4rl.
 
     .. code-block:: python
 
@@ -312,14 +326,15 @@
           Learning. <https://arxiv.org/abs/2004.07219>`_
         * https://github.com/rail-berkeley/d4rl
 
     Args:
         env_name: environment id of d4rl dataset.
         transition_picker: TransitionPickerProtocol object.
         trajectory_slicer: TrajectorySlicerProtocol object.
+        render_mode: Mode of rendering (``human``, ``rgb_array``).
 
     Returns:
         tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     try:
         import d4rl  # type: ignore
 
@@ -340,14 +355,15 @@
             timeouts=timeouts,
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
         )
 
         # wrapped by NormalizedBoxEnv that is incompatible with newer Gym
         unwrapped_env: gym.Env[Any, Any] = env.env.env.env.wrapped_env  # type: ignore
+        unwrapped_env.render_mode = render_mode  # overwrite
 
         return dataset, TimeLimit(unwrapped_env, max_episode_steps=1000)
     except ImportError as e:
         raise ImportError(
             "d4rl is not installed.\n"
             "pip install git+https://github.com/rail-berkeley/d4rl"
         ) from e
@@ -419,14 +435,15 @@
 ]
 
 
 def get_dataset(
     env_name: str,
     transition_picker: Optional[TransitionPickerProtocol] = None,
     trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+    render_mode: Optional[str] = None,
 ) -> Tuple[ReplayBuffer, gym.Env[Any, Any]]:
     """Returns dataset and envrironment by guessing from name.
 
     This function returns dataset by matching name with the following datasets.
 
     - cartpole-replay
     - cartpole-random
@@ -452,48 +469,55 @@
        # d4rl dataset
        dataset, env = d3rlpy.datasets.get_dataset('hopper-medium-v0')
 
     Args:
         env_name: environment id of the dataset.
         transition_picker: TransitionPickerProtocol object.
         trajectory_slicer: TrajectorySlicerProtocol object.
+        render_mode: Mode of rendering (``human``, ``rgb_array``).
 
     Returns:
         tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     if env_name == "cartpole-replay":
         return get_cartpole(
             dataset_type="replay",
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
+            render_mode=render_mode,
         )
     elif env_name == "cartpole-random":
         return get_cartpole(
             dataset_type="random",
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
+            render_mode=render_mode,
         )
     elif env_name == "pendulum-replay":
         return get_pendulum(
             dataset_type="replay",
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
+            render_mode=render_mode,
         )
     elif env_name == "pendulum-random":
         return get_pendulum(
             dataset_type="random",
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
+            render_mode=render_mode,
         )
     elif re.match(r"^bullet-.+$", env_name):
         return get_d4rl(
             env_name,
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
+            render_mode=render_mode,
         )
     elif re.match(r"hopper|halfcheetah|walker|ant", env_name):
         return get_d4rl(
             env_name,
             transition_picker=transition_picker,
             trajectory_slicer=trajectory_slicer,
+            render_mode=render_mode,
         )
     raise ValueError(f"Unrecognized env_name: {env_name}.")
```

### Comparing `d3rlpy-2.0.3/d3rlpy/envs/wrappers.py` & `d3rlpy-2.0.4/d3rlpy/envs/wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import json
-import os
 from collections import deque
-from typing import Any, Callable, Deque, Dict, List, Optional, Tuple, TypeVar
+from typing import Any, Deque, Dict, Optional, Tuple, TypeVar
 
 import gym
 import numpy as np
 
 try:
     import cv2  # this is used in AtariPreprocessing
 except ImportError:
@@ -15,15 +13,14 @@
 from gym.wrappers.transform_reward import TransformReward
 
 __all__ = [
     "ChannelFirst",
     "FrameStack",
     "AtariPreprocessing",
     "Atari",
-    "Monitor",
 ]
 
 _ObsType = TypeVar("_ObsType")
 _ActType = TypeVar("_ActType")
 
 
 class ChannelFirst(gym.Wrapper[_ObsType, _ActType]):
@@ -334,104 +331,7 @@
         if not is_eval:
             env = TransformReward(env, lambda r: float(np.clip(r, -1.0, 1.0)))
         if num_stack:
             env = FrameStack(env, num_stack)
         else:
             env = ChannelFirst(env)
         super().__init__(env)
-
-
-class Monitor(gym.Wrapper[_ObsType, _ActType]):
-    """gym.wrappers.Monitor-style Monitor wrapper.
-
-    Args:
-        env (gym.Env): gym environment.
-        directory (str): directory to save.
-        video_callable (callable): callable function that takes episode counter
-            to control record frequency.
-        force (bool): flag to allow existing directory.
-        frame_rate (float): video frame rate.
-        record_rate (int): images are record every ``record_rate`` frames.
-    """
-
-    _directory: str
-    _video_callable: Callable[[int], bool]
-    _frame_rate: float
-    _record_rate: int
-    _episode: int
-    _episode_return: float
-    _episode_step: int
-    _buffer: List[np.ndarray]
-
-    def __init__(
-        self,
-        env: gym.Env[_ObsType, _ActType],
-        directory: str,
-        video_callable: Optional[Callable[[int], bool]] = None,
-        force: bool = False,
-        frame_rate: float = 30.0,
-        record_rate: int = 1,
-    ):
-        super().__init__(env)
-        # prepare directory
-        if os.path.exists(directory) and not force:
-            raise ValueError(f"{directory} already exists.")
-        os.makedirs(directory, exist_ok=True)
-        self._directory = directory
-
-        if video_callable:
-            self._video_callable = video_callable
-        else:
-            self._video_callable = lambda ep: ep % 10 == 0
-
-        self._frame_rate = frame_rate
-        self._record_rate = record_rate
-
-        self._episode = 0
-        self._episode_return = 0.0
-        self._episode_step = 0
-        self._buffer = []
-
-    def step(
-        self, action: _ActType
-    ) -> Tuple[_ObsType, float, bool, bool, Dict[str, Any]]:
-        obs, reward, done, truncated, info = super().step(action)
-
-        if self._video_callable(self._episode):
-            # store rendering
-            frame = cv2.cvtColor(super().render("rgb_array"), cv2.COLOR_BGR2RGB)
-            self._buffer.append(frame)
-            self._episode_step += 1
-            self._episode_return += reward
-            if done:
-                self._save_video()
-                self._save_stats()
-
-        return obs, reward, done, truncated, info
-
-    def reset(self, **kwargs: Any) -> Tuple[_ObsType, Dict[str, Any]]:
-        self._episode += 1
-        self._episode_return = 0.0
-        self._episode_step = 0
-        self._buffer = []
-        return super().reset(**kwargs)
-
-    def _save_video(self) -> None:
-        height, width = self._buffer[0].shape[:2]
-        path = os.path.join(self._directory, f"video{self._episode}.avi")
-        fmt = cv2.VideoWriter_fourcc(*"MJPG")
-        writer = cv2.VideoWriter(path, fmt, self._frame_rate, (width, height))
-        print(f"Saving a recorded video to {path}...")
-        for i, frame in enumerate(self._buffer):
-            if i % self._record_rate == 0:
-                writer.write(frame)
-        writer.release()
-
-    def _save_stats(self) -> None:
-        path = os.path.join(self._directory, f"stats{self._episode}.json")
-        stats = {
-            "episode_step": self._episode_step,
-            "return": self._episode_return,
-        }
-        with open(path, "w") as f:
-            json_str = json.dumps(stats, indent=2)
-            f.write(json_str)
```

### Comparing `d3rlpy-2.0.3/d3rlpy/interface.py` & `d3rlpy-2.0.4/d3rlpy/interface.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/logging/file_adapter.py` & `d3rlpy-2.0.4/d3rlpy/logging/file_adapter.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/logging/logger.py` & `d3rlpy-2.0.4/d3rlpy/logging/logger.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/logging/noop_adapter.py` & `d3rlpy-2.0.4/d3rlpy/logging/noop_adapter.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/logging/tensorboard_adapter.py` & `d3rlpy-2.0.4/d3rlpy/logging/tensorboard_adapter.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/logging/utils.py` & `d3rlpy-2.0.4/d3rlpy/logging/utils.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/metrics/evaluators.py` & `d3rlpy-2.0.4/d3rlpy/metrics/evaluators.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,16 +259,17 @@
         total_values = []
         episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
             for batch in make_batches(
                 episode, WINDOW_SIZE, dataset.transition_picker
             ):
                 # estimate action-value in initial states
-                actions = algo.predict([batch.observations[0]])
-                values = algo.predict_value([batch.observations[0]], actions)
+                first_obs = np.expand_dims(batch.observations[0], axis=0)
+                actions = algo.predict(first_obs)
+                values = algo.predict_value(first_obs, actions)
                 total_values.append(values[0])
         return float(np.mean(total_values))
 
 
 class SoftOPCEvaluator(EvaluatorProtocol):
     r"""Returns Soft Off-Policy Classification metrics.
 
@@ -511,36 +512,31 @@
             \{\text{argmax}_a Q_{\theta_1}(s_t, a)
             = \text{argmax}_a Q_{\theta_2}(s_t, a)\}]
 
     Args:
         env: Gym environment.
         n_trials: Number of episodes to evaluate.
         epsilon: Probability of random action.
-        render: Flag to turn on rendering.
     """
     _env: gym.Env[Any, Any]
     _n_trials: int
     _epsilon: float
-    _render: bool
 
     def __init__(
         self,
         env: gym.Env[Any, Any],
         n_trials: int = 10,
         epsilon: float = 0.0,
-        render: bool = False,
     ):
         self._env = env
         self._n_trials = n_trials
         self._epsilon = epsilon
-        self._render = render
 
     def __call__(
         self, algo: QLearningAlgoProtocol, dataset: ReplayBuffer
     ) -> float:
         return evaluate_qlearning_with_environment(
             algo=algo,
             env=self._env,
             n_trials=self._n_trials,
             epsilon=self._epsilon,
-            render=self._render,
         )
```

### Comparing `d3rlpy-2.0.3/d3rlpy/metrics/utility.py` & `d3rlpy-2.0.4/d3rlpy/metrics/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 
 def evaluate_qlearning_with_environment(
     algo: QLearningAlgoProtocol,
     env: gym.Env[Any, Any],
     n_trials: int = 10,
     epsilon: float = 0.0,
-    render: bool = False,
 ) -> float:
     """Returns average environment score.
 
     .. code-block:: python
 
         import gym
 
@@ -35,15 +34,14 @@
 
 
     Args:
         alg: algorithm object.
         env: gym-styled environment.
         n_trials: the number of trials.
         epsilon: noise factor for epsilon-greedy policy.
-        render: flag to render environment.
 
     Returns:
         average score.
     """
     episode_rewards = []
     for _ in range(n_trials):
         observation, _ = env.reset()
@@ -55,28 +53,24 @@
                 action = env.action_space.sample()
             else:
                 action = algo.predict(np.expand_dims(observation, axis=0))[0]
 
             observation, reward, done, truncated, _ = env.step(action)
             episode_reward += reward
 
-            if render:
-                env.render()
-
             if done or truncated:
                 break
         episode_rewards.append(episode_reward)
     return float(np.mean(episode_rewards))
 
 
 def evaluate_transformer_with_environment(
     algo: StatefulTransformerAlgoProtocol,
     env: gym.Env[Any, Any],
     n_trials: int = 10,
-    render: bool = False,
 ) -> float:
     """Returns average environment score.
 
     .. code-block:: python
 
         import gym
 
@@ -90,15 +84,14 @@
         mean_episode_return = evaluate_with_environment(cql, env)
 
 
     Args:
         alg: algorithm object.
         env: gym-styled environment.
         n_trials: the number of trials.
-        render: flag to render environment.
 
     Returns:
         average score.
     """
     episode_rewards = []
     for _ in range(n_trials):
         algo.reset()
@@ -108,14 +101,11 @@
         while True:
             # take action
             action = algo.predict(observation, reward)
 
             observation, reward, done, truncated, _ = env.step(action)
             episode_reward += reward
 
-            if render:
-                env.render()
-
             if done or truncated:
                 break
         episode_rewards.append(episode_reward)
     return float(np.mean(episode_rewards))
```

### Comparing `d3rlpy-2.0.3/d3rlpy/models/builders.py` & `d3rlpy-2.0.4/d3rlpy/models/builders.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/encoders.py` & `d3rlpy-2.0.4/d3rlpy/models/encoders.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/optimizers.py` & `d3rlpy-2.0.4/d3rlpy/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/q_functions.py` & `d3rlpy-2.0.4/d3rlpy/models/q_functions.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/distributions.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/distributions.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/encoders.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/encoders.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/imitators.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/imitators.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/policies.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/policies.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/base.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/ensemble_q_function.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/ensemble_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/fqf_q_function.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/fqf_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/iqn_q_function.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/iqn_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/mean_q_function.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/mean_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/qr_q_function.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/qr_q_function.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/q_functions/utility.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/q_functions/utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/transformers.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/transformers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/models/torch/v_functions.py` & `d3rlpy-2.0.4/d3rlpy/models/torch/v_functions.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/ope/fqe.py` & `d3rlpy-2.0.4/d3rlpy/ope/fqe.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/ope/torch/fqe_impl.py` & `d3rlpy-2.0.4/d3rlpy/ope/torch/fqe_impl.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/preprocessing/action_scalers.py` & `d3rlpy-2.0.4/d3rlpy/preprocessing/action_scalers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/preprocessing/base.py` & `d3rlpy-2.0.4/d3rlpy/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/preprocessing/observation_scalers.py` & `d3rlpy-2.0.4/d3rlpy/preprocessing/observation_scalers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/preprocessing/reward_scalers.py` & `d3rlpy-2.0.4/d3rlpy/preprocessing/reward_scalers.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/serializable_config.py` & `d3rlpy-2.0.4/d3rlpy/serializable_config.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy/torch_utility.py` & `d3rlpy-2.0.4/d3rlpy/torch_utility.py`

 * *Files identical despite different names*

### Comparing `d3rlpy-2.0.3/d3rlpy.egg-info/PKG-INFO` & `d3rlpy-2.0.4/d3rlpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d3rlpy
-Version: 2.0.3
+Version: 2.0.4
 Summary: An offline deep reinforcement learning library
 Home-page: https://github.com/takuseno/d3rlpy
 Author: Takuma Seno
 Author-email: takuma.seno@gmail.com
 License: MIT License
 Description: <p align="center"><img align="center" width="300px" src="assets/logo.png"></p>
         
@@ -64,18 +64,17 @@
         [![PyPI version](https://badge.fury.io/py/d3rlpy.svg)](https://badge.fury.io/py/d3rlpy)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/d3rlpy)
         ```
         $ pip install d3rlpy
         ```
         ### Anaconda
         [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/version.svg)](https://anaconda.org/conda-forge/d3rlpy)
-        [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/platforms.svg)](https://anaconda.org/conda-forge/d3rlpy)
         [![Anaconda-Server Badge](https://anaconda.org/conda-forge/d3rlpy/badges/downloads.svg)](https://anaconda.org/conda-forge/d3rlpy)
         ```
-        $ conda install -c conda-forge d3rlpy
+        $ conda install conda-forge/noarch::d3rlpy
         ```
         
         ### Docker
         ![Docker Pulls](https://img.shields.io/docker/pulls/takuseno/d3rlpy)
         ```
         $ docker run -it --gpus all --name d3rlpy takuseno/d3rlpy:latest bash
         ```
```

### Comparing `d3rlpy-2.0.3/d3rlpy.egg-info/SOURCES.txt` & `d3rlpy-2.0.4/d3rlpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENSE
-MANIFEST.in
 README.md
 setup.py
 d3rlpy/__init__.py
 d3rlpy/_version.py
 d3rlpy/base.py
 d3rlpy/cli.py
 d3rlpy/constants.py
```

### Comparing `d3rlpy-2.0.3/setup.py` & `d3rlpy-2.0.4/setup.py`

 * *Files identical despite different names*

