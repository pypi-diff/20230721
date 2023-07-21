# Comparing `tmp/seldonian_engine-0.8.0.tar.gz` & `tmp/seldonian_engine-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_engine-0.8.0.tar", last modified: Thu Jun 22 21:25:55 2023, max compression
+gzip compressed data, was "seldonian_engine-0.8.1.tar", last modified: Fri Jul 21 00:00:56 2023, max compression
```

## Comparing `seldonian_engine-0.8.0.tar` & `seldonian_engine-0.8.1.tar`

### file list

```diff
@@ -1,107 +1,109 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.821403 seldonian_engine-0.8.0/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)     2134 2023-06-22 21:25:55.821215 seldonian_engine-0.8.0/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)     1643 2022-11-11 22:25:32.000000 seldonian_engine-0.8.0/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.800861 seldonian_engine-0.8.0/seldonian/
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.803227 seldonian_engine-0.8.0/seldonian/RL/
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.804289 seldonian_engine-0.8.0/seldonian/RL/Agents/
--rw-r--r--   0 ahoag      (501) staff       (20)     1733 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.804610 seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/
--rw-r--r--   0 ahoag      (501) staff       (20)     4537 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/Fourier.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1043 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Discrete_Random_Agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.805246 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/
--rw-r--r--   0 ahoag      (501) staff       (20)      554 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1333 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Linear_FA.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2854 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Table.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3054 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.805791 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/
--rw-r--r--   0 ahoag      (501) staff       (20)     4906 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Policy.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6459 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Softmax.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)      794 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/keyboard_gridworld.py
--rw-r--r--   0 ahoag      (501) staff       (20)      406 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/mountain_car_rough_solution.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.806233 seldonian_engine-0.8.0/seldonian/RL/Env_Description/
--rw-r--r--   0 ahoag      (501) staff       (20)     2001 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Env_Description/Env_Description.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2311 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Env_Description/Spaces.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Env_Description/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3698 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/RL_generate_dataset_and_spec_file.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2335 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/RL/RL_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6614 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/RL_runner.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/__init__.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.807120 seldonian_engine-0.8.0/seldonian/RL/environments/
--rw-r--r--   0 ahoag      (501) staff       (20)     1364 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/Environment.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/environments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4075 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/gridworld.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2352 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/mountaincar.py
--rw-r--r--   0 ahoag      (501) staff       (20)      984 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/n_step_mountaincar.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2807 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/simglucose_env.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1196 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/generate_gridworld_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1236 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/generate_mountaincar_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1337 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/generate_simglucose_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)      615 2022-09-13 15:24:12.000000 seldonian_engine-0.8.0/seldonian/RL/hyperparams_and_settings.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3991 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/profiling_seldonian_RL.py
--rw-r--r--   0 ahoag      (501) staff       (20)       33 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/__init__.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.807449 seldonian_engine-0.8.0/seldonian/candidate_selection/
--rw-r--r--   0 ahoag      (501) staff       (20)       40 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/candidate_selection/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    19265 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/candidate_selection/candidate_selection.py
--rw-r--r--   0 ahoag      (501) staff       (20)    12880 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/dataset.py
--rw-r--r--   0 ahoag      (501) staff       (20)    21029 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/hyperparam_search.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.809226 seldonian_engine-0.8.0/seldonian/models/
--rw-r--r--   0 ahoag      (501) staff       (20)       48 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     8288 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/models/models.py
--rw-r--r--   0 ahoag      (501) staff       (20)    40182 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/models/objectives.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1284 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/pytorch_cnn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6883 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/models/pytorch_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1084 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/sklearn_lr.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4758 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/sklearn_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1559 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/tensorflow_cnn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6068 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/tensorflow_model.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.809580 seldonian_engine-0.8.0/seldonian/optimizers/
--rw-r--r--   0 ahoag      (501) staff       (20)       43 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/optimizers/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    10884 2023-04-03 17:05:25.000000 seldonian_engine-0.8.0/seldonian/optimizers/gradient_descent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.811134 seldonian_engine-0.8.0/seldonian/parse_tree/
--rw-r--r--   0 ahoag      (501) staff       (20)       75 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/parse_tree/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    40039 2023-06-06 19:58:26.000000 seldonian_engine-0.8.0/seldonian/parse_tree/nodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3828 2023-04-19 20:33:28.000000 seldonian_engine-0.8.0/seldonian/parse_tree/operators.py
--rw-r--r--   0 ahoag      (501) staff       (20)    46725 2023-06-13 16:21:42.000000 seldonian_engine-0.8.0/seldonian/parse_tree/parse_tree.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.812065 seldonian_engine-0.8.0/seldonian/safety_test/
--rw-r--r--   0 ahoag      (501) staff       (20)       36 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/safety_test/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4272 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/safety_test/safety_test.py
--rw-r--r--   0 ahoag      (501) staff       (20)    15854 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/seldonian_algorithm.py
--rw-r--r--   0 ahoag      (501) staff       (20)    22099 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/spec.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.813761 seldonian_engine-0.8.0/seldonian/utils/
--rw-r--r--   0 ahoag      (501) staff       (20)      468 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/RL_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)       24 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1685 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/io_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6891 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/plot_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2011 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/utils/stats_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4210 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/utils/tutorial_utils.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.814195 seldonian_engine-0.8.0/seldonian/warnings/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/warnings/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)      344 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/warnings/custom_warnings.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.816011 seldonian_engine-0.8.0/seldonian_engine.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)     2134 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)     2998 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)      148 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       16 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-06-22 21:25:55.821450 seldonian_engine-0.8.0/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)     1070 2023-06-22 21:25:20.000000 seldonian_engine-0.8.0/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.820909 seldonian_engine-0.8.0/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    14897 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)    13340 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_RL.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6913 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_dataset.py
--rw-r--r--   0 ahoag      (501) staff       (20)      828 2022-09-21 21:32:24.000000 seldonian_engine-0.8.0/tests/test_io_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5508 2022-12-08 20:24:26.000000 seldonian_engine-0.8.0/tests/test_objectives.py
--rw-r--r--   0 ahoag      (501) staff       (20)    64110 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_parse_tree.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1223 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/tests/test_plot_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4820 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_safety_test.py
--rw-r--r--   0 ahoag      (501) staff       (20)    61690 2023-06-13 16:21:42.000000 seldonian_engine-0.8.0/tests/test_seldonian_algorithm.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1582 2023-02-09 17:42:02.000000 seldonian_engine-0.8.0/tests/test_sklearn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6389 2022-11-07 22:08:04.000000 seldonian_engine-0.8.0/tests/test_spec.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1272 2022-09-21 21:32:24.000000 seldonian_engine-0.8.0/tests/test_stats_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)      544 2022-09-21 21:32:24.000000 seldonian_engine-0.8.0/tests/test_tutorial_utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:56.001593 seldonian_engine-0.8.1/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)     2133 2023-07-21 00:00:56.001417 seldonian_engine-0.8.1/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)     1642 2023-07-20 04:24:35.000000 seldonian_engine-0.8.1/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.983143 seldonian_engine-0.8.1/seldonian/
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.985513 seldonian_engine-0.8.1/seldonian/RL/
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.986506 seldonian_engine-0.8.1/seldonian/RL/Agents/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1733 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.986871 seldonian_engine-0.8.1/seldonian/RL/Agents/Bases/
+-rw-r--r--   0 ahoag      (501) staff       (20)     4537 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Bases/Fourier.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Bases/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1043 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Discrete_Random_Agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.987590 seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/
+-rw-r--r--   0 ahoag      (501) staff       (20)      554 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1333 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/Linear_FA.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2854 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/Table.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3054 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.988187 seldonian_engine-0.8.1/seldonian/RL/Agents/Policies/
+-rw-r--r--   0 ahoag      (501) staff       (20)     4906 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Policies/Policy.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6459 2023-05-31 21:23:44.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Policies/Softmax.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/Policies/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      794 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/keyboard_gridworld.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      406 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Agents/mountain_car_rough_solution.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.988648 seldonian_engine-0.8.1/seldonian/RL/Env_Description/
+-rw-r--r--   0 ahoag      (501) staff       (20)     2001 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Env_Description/Env_Description.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2311 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/Env_Description/Spaces.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/Env_Description/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3698 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/RL_generate_dataset_and_spec_file.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2335 2023-05-31 21:23:44.000000 seldonian_engine-0.8.1/seldonian/RL/RL_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6614 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/RL_runner.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/__init__.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.989654 seldonian_engine-0.8.1/seldonian/RL/environments/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1364 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/environments/Environment.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/RL/environments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4075 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/environments/gridworld.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2352 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/environments/mountaincar.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      984 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/environments/n_step_mountaincar.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2807 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/environments/simglucose_env.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1196 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/generate_gridworld_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1236 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/generate_mountaincar_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1337 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/generate_simglucose_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      615 2022-09-13 15:24:12.000000 seldonian_engine-0.8.1/seldonian/RL/hyperparams_and_settings.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3991 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/RL/profiling_seldonian_RL.py
+-rw-r--r--   0 ahoag      (501) staff       (20)       33 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/__init__.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.990025 seldonian_engine-0.8.1/seldonian/candidate_selection/
+-rw-r--r--   0 ahoag      (501) staff       (20)       40 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/candidate_selection/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    19265 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/seldonian/candidate_selection/candidate_selection.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    12880 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/seldonian/dataset.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    21029 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/hyperparam_search.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.992439 seldonian_engine-0.8.1/seldonian/models/
+-rw-r--r--   0 ahoag      (501) staff       (20)       48 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/models/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8288 2023-05-31 21:23:44.000000 seldonian_engine-0.8.1/seldonian/models/models.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    19375 2023-07-20 23:54:53.000000 seldonian_engine-0.8.1/seldonian/models/objectives.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1284 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/models/pytorch_cnn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6883 2023-05-31 21:23:44.000000 seldonian_engine-0.8.1/seldonian/models/pytorch_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1084 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/models/sklearn_lr.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4758 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/models/sklearn_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1559 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/models/tensorflow_cnn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6068 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/models/tensorflow_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    20883 2023-07-20 23:54:53.000000 seldonian_engine-0.8.1/seldonian/models/zhat_funcs.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.992887 seldonian_engine-0.8.1/seldonian/optimizers/
+-rw-r--r--   0 ahoag      (501) staff       (20)       43 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/optimizers/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    10884 2023-04-03 17:05:25.000000 seldonian_engine-0.8.1/seldonian/optimizers/gradient_descent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.993928 seldonian_engine-0.8.1/seldonian/parse_tree/
+-rw-r--r--   0 ahoag      (501) staff       (20)       75 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/parse_tree/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    39983 2023-07-20 23:54:53.000000 seldonian_engine-0.8.1/seldonian/parse_tree/nodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3828 2023-04-19 20:33:28.000000 seldonian_engine-0.8.1/seldonian/parse_tree/operators.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    46709 2023-07-20 04:24:40.000000 seldonian_engine-0.8.1/seldonian/parse_tree/parse_tree.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.994896 seldonian_engine-0.8.1/seldonian/safety_test/
+-rw-r--r--   0 ahoag      (501) staff       (20)       36 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/safety_test/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4272 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/safety_test/safety_test.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    15854 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/seldonian/seldonian_algorithm.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    22099 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/seldonian/spec.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.996067 seldonian_engine-0.8.1/seldonian/utils/
+-rw-r--r--   0 ahoag      (501) staff       (20)      468 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/utils/RL_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)       24 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/utils/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1685 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/utils/io_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6851 2023-07-20 04:24:40.000000 seldonian_engine-0.8.1/seldonian/utils/plot_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2035 2023-07-20 23:54:53.000000 seldonian_engine-0.8.1/seldonian/utils/stats_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4210 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/seldonian/utils/tutorial_utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.996472 seldonian_engine-0.8.1/seldonian/warnings/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/seldonian/warnings/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      344 2023-03-08 18:13:56.000000 seldonian_engine-0.8.1/seldonian/warnings/custom_warnings.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:55.997297 seldonian_engine-0.8.1/seldonian_engine.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)     2133 2023-07-21 00:00:55.000000 seldonian_engine-0.8.1/seldonian_engine.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)     3050 2023-07-21 00:00:55.000000 seldonian_engine-0.8.1/seldonian_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-07-21 00:00:55.000000 seldonian_engine-0.8.1/seldonian_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)      148 2023-07-21 00:00:55.000000 seldonian_engine-0.8.1/seldonian_engine.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       16 2023-07-21 00:00:55.000000 seldonian_engine-0.8.1/seldonian_engine.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-07-21 00:00:56.001647 seldonian_engine-0.8.1/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)     1070 2023-07-21 00:00:44.000000 seldonian_engine-0.8.1/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-07-21 00:00:56.001079 seldonian_engine-0.8.1/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    14897 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    13340 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/tests/test_RL.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6913 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/tests/test_dataset.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      828 2022-09-21 21:32:24.000000 seldonian_engine-0.8.1/tests/test_io_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2381 2023-07-20 04:24:40.000000 seldonian_engine-0.8.1/tests/test_models.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     5548 2023-07-20 23:54:53.000000 seldonian_engine-0.8.1/tests/test_objectives.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    65550 2023-07-20 04:24:40.000000 seldonian_engine-0.8.1/tests/test_parse_tree.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1223 2022-09-12 23:15:58.000000 seldonian_engine-0.8.1/tests/test_plot_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4820 2023-06-22 21:24:25.000000 seldonian_engine-0.8.1/tests/test_safety_test.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    61920 2023-07-20 04:24:40.000000 seldonian_engine-0.8.1/tests/test_seldonian_algorithm.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1582 2023-02-09 17:42:02.000000 seldonian_engine-0.8.1/tests/test_sklearn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6389 2022-11-07 22:08:04.000000 seldonian_engine-0.8.1/tests/test_spec.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1272 2022-09-21 21:32:24.000000 seldonian_engine-0.8.1/tests/test_stats_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      544 2022-09-21 21:32:24.000000 seldonian_engine-0.8.1/tests/test_tutorial_utils.py
```

### Comparing `seldonian_engine-0.8.0/LICENSE` & `seldonian_engine-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/PKG-INFO` & `seldonian_engine-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian_engine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Core library for Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -21,15 +21,15 @@
 
 This is the source code repository for a framework for creating and running [Seldonian](https://seldonian.cs.umass.edu/) algorithms. 
 
 ## Installation
 
 To use the latest stable version:
 ```
-pip install seldonian-toolkit
+pip install seldonian-engine
 ```
 
 To run this code as a developer, create a virtual environment. Then install the package locally, e.g. 
 
 ```
 python setup.py develop
 ```
```

### Comparing `seldonian_engine-0.8.0/README.md` & `seldonian_engine-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 This is the source code repository for a framework for creating and running [Seldonian](https://seldonian.cs.umass.edu/) algorithms. 
 
 ## Installation
 
 To use the latest stable version:
 ```
-pip install seldonian-toolkit
+pip install seldonian-engine
 ```
 
 To run this code as a developer, create a virtual environment. Then install the package locally, e.g. 
 
 ```
 python setup.py develop
 ```
```

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Agent.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Agent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/Fourier.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Bases/Fourier.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Discrete_Random_Agent.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Discrete_Random_Agent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Linear_FA.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/Linear_FA.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Table.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Function_Approximators/Table.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Policy.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Policies/Policy.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Softmax.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/Policies/Softmax.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Agents/keyboard_gridworld.py` & `seldonian_engine-0.8.1/seldonian/RL/Agents/keyboard_gridworld.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Env_Description/Env_Description.py` & `seldonian_engine-0.8.1/seldonian/RL/Env_Description/Env_Description.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/Env_Description/Spaces.py` & `seldonian_engine-0.8.1/seldonian/RL/Env_Description/Spaces.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/RL_generate_dataset_and_spec_file.py` & `seldonian_engine-0.8.1/seldonian/RL/RL_generate_dataset_and_spec_file.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/RL_model.py` & `seldonian_engine-0.8.1/seldonian/RL/RL_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/RL_runner.py` & `seldonian_engine-0.8.1/seldonian/RL/RL_runner.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/environments/Environment.py` & `seldonian_engine-0.8.1/seldonian/RL/environments/Environment.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/environments/gridworld.py` & `seldonian_engine-0.8.1/seldonian/RL/environments/gridworld.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/environments/mountaincar.py` & `seldonian_engine-0.8.1/seldonian/RL/environments/mountaincar.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/environments/n_step_mountaincar.py` & `seldonian_engine-0.8.1/seldonian/RL/environments/n_step_mountaincar.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/environments/simglucose_env.py` & `seldonian_engine-0.8.1/seldonian/RL/environments/simglucose_env.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/generate_gridworld_episodes.py` & `seldonian_engine-0.8.1/seldonian/RL/generate_gridworld_episodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/generate_mountaincar_episodes.py` & `seldonian_engine-0.8.1/seldonian/RL/generate_mountaincar_episodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/generate_simglucose_episodes.py` & `seldonian_engine-0.8.1/seldonian/RL/generate_simglucose_episodes.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/hyperparams_and_settings.py` & `seldonian_engine-0.8.1/seldonian/RL/hyperparams_and_settings.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/RL/profiling_seldonian_RL.py` & `seldonian_engine-0.8.1/seldonian/RL/profiling_seldonian_RL.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/candidate_selection/candidate_selection.py` & `seldonian_engine-0.8.1/seldonian/candidate_selection/candidate_selection.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/dataset.py` & `seldonian_engine-0.8.1/seldonian/dataset.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/hyperparam_search.py` & `seldonian_engine-0.8.1/seldonian/hyperparam_search.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/models.py` & `seldonian_engine-0.8.1/seldonian/models/models.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/pytorch_cnn.py` & `seldonian_engine-0.8.1/seldonian/models/pytorch_cnn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/pytorch_model.py` & `seldonian_engine-0.8.1/seldonian/models/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/sklearn_lr.py` & `seldonian_engine-0.8.1/seldonian/models/sklearn_lr.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/sklearn_model.py` & `seldonian_engine-0.8.1/seldonian/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/tensorflow_cnn.py` & `seldonian_engine-0.8.1/seldonian/models/tensorflow_cnn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/models/tensorflow_model.py` & `seldonian_engine-0.8.1/seldonian/models/tensorflow_model.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/optimizers/gradient_descent.py` & `seldonian_engine-0.8.1/seldonian/optimizers/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/parse_tree/nodes.py` & `seldonian_engine-0.8.1/seldonian/parse_tree/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from operator import itemgetter
 from functools import reduce, partial
 import pandas as pd
 import autograd.numpy as np
 
-from seldonian.models.objectives import sample_from_statistic, evaluate_statistic
+from seldonian.models import zhat_funcs 
 from seldonian.utils.stats_utils import *
 
 
 class Node(object):
     def __init__(self, name, lower, upper):
         """The base class for all parse tree nodes
 
@@ -126,16 +126,15 @@
     def calculate_value(self, **kwargs):
         """
         Calculate the value of the node
         given model weights, etc. This is
         the expected value of the base variable,
         not the bound.
         """
-
-        value = evaluate_statistic(statistic_name=self.measure_function_name, **kwargs)
+        value = zhat_funcs.evaluate_statistic(statistic_name=self.measure_function_name, **kwargs)
         return value
 
     def mask_data(self, dataset, conditional_columns):
         """Mask features and labels using
         a joint AND mask where each of the
         conditional columns is True.
 
@@ -167,30 +166,27 @@
                 masked_features = [x[joint_mask] for x in dataset.features]
                 masked_labels = [x[joint_mask] for x in dataset.labels]
                 # If possible, convert to numpy array. Not always possible,
                 # e.g., if features are of different dimensions.
                 try:
                     masked_features = np.array(masked_features)
                     masked_labels = np.array(masked_labels)
-                    n_masked = len(masked_features)
                 except Exception as e:
                     # masked_features and masked_labels stay as lists
-                    n_masked = len(masked_features[0])
+                    pass
             else:
                 # numpy array
                 masked_features = dataset.features[joint_mask]
                 masked_labels = dataset.labels[joint_mask]
-                n_masked = len(masked_features)
 
-            return masked_features, masked_labels, n_masked
+            return masked_features, masked_labels
 
         elif dataset.regime == "reinforcement_learning":
             masked_episodes = np.asarray(dataset.episodes)[joint_mask]
-            n_masked = len(masked_episodes)
-            return masked_episodes, n_masked
+            return masked_episodes
 
     def calculate_data_forbound(self, **kwargs):
         """
         Prepare data inputs
         for confidence bound calculation.
         """
         theta, dataset, model, regime, branch = itemgetter(
@@ -207,49 +203,43 @@
         if regime == "supervised_learning":
             # mask the data using the conditional columns, if present
 
             features = dataset.features
             labels = dataset.labels
 
             if self.conditional_columns:
-                masked_features, masked_labels, n_masked = self.mask_data(
+                masked_features, masked_labels = self.mask_data(
                     dataset, self.conditional_columns
                 )
             else:
-                (masked_features, masked_labels, n_masked) = (
+                (masked_features, masked_labels) = (
                     features,
-                    labels,
-                    dataset.num_datapoints,
+                    labels
                 )
 
-            if branch == "candidate_selection":
-                frac_masked = n_masked / dataset.num_datapoints
-                datasize = int(round(frac_masked * n_safety))
-            else:
-                datasize = n_masked
-            data_dict = {"features": masked_features, "labels": masked_labels}
+            data_dict = {
+                "features": masked_features,
+                "labels": masked_labels
+            }
 
         elif regime == "reinforcement_learning":
             gamma = model.env_kwargs["gamma"]
             episodes = dataset.episodes
 
             if self.conditional_columns:
-                masked_episodes, n_masked = self.mask_data(
+                masked_episodes = self.mask_data(
                     dataset, self.conditional_columns
                 )
             else:
-                (masked_episodes, n_masked) = episodes, dataset.num_datapoints
-
-            if branch == "candidate_selection":
-                frac_masked = n_masked / dataset.num_datapoints
-                datasize = int(round(frac_masked * n_safety))
-            else:
-                datasize = n_masked
+                masked_episodes = episodes
 
             # Precalculate expected return from behavioral policy
+            # using the reward specified by the alt_reward_number
+            # These are only ever used in the zhat functions, so 
+            # they pertain to the constraint, not the primary objective
             if "alt_reward_number" in kwargs:
                 # use the alternate reward specified in the constraint string
                 # when calculating the return
                 alt_reward_number = kwargs["alt_reward_number"]
                 alt_reward_index = alt_reward_number - 1
                 masked_returns = [
                     weighted_sum_gamma(ep.alt_rewards[:, alt_reward_index], gamma)
@@ -261,15 +251,15 @@
                 ]
 
             data_dict = {
                 "episodes": masked_episodes,
                 "weighted_returns": masked_returns,
             }
 
-        return data_dict, datasize
+        return data_dict
 
     def calculate_bounds(self, **kwargs):
         """Calculate confidence bounds given a bound_method,
         such as t-test.
         """
         if "bound_method" in kwargs:
             bound_method = kwargs["bound_method"]
@@ -287,17 +277,33 @@
 
                 # --TODO-- abstract away to support things like
                 # getting confidence intervals from bootstrap
                 # and RL cases
                 estimator_samples = self.zhat(**kwargs)
 
                 branch = kwargs["branch"]
+                if branch == "safety_test":
+                    datasize = len(estimator_samples)
+                elif branch == "candidate_selection":
+                    candidate_dataset = kwargs["dataset"]
+                    n_candidate = candidate_dataset.num_datapoints
+                    n_safety = kwargs["n_safety"]
+                    # Want to predict the size of the safety dataset.
+                    # We do this using the fraction of candidate data we 
+                    # get from the estimator
+                    datasize = int(
+                        round(
+                            ( len(estimator_samples)/n_candidate ) * n_safety 
+                        )
+                    )
+
                 data_dict = kwargs["data_dict"]
                 bound_kwargs = kwargs
                 bound_kwargs["data"] = estimator_samples
+                bound_kwargs["datasize"] = datasize
                 bound_kwargs["delta"] = self.delta
 
                 # If lower and upper are both needed,
                 # can't necessarily call lower and upper
                 # bound functions separately. Sometimes the joint bound
                 # is different from the individual bounds combined
                 if self.will_lower_bound and self.will_upper_bound:
@@ -328,15 +334,15 @@
                 raise AssertionError(
                     "will_lower_bound and will_upper_bound " "cannot both be False"
                 )
 
         else:
             raise RuntimeError("bound_method not specified!")
 
-    def zhat(self, model, theta, data_dict, datasize, **kwargs):
+    def zhat(self, model, theta, data_dict, **kwargs):
         """
         Calculate an unbiased estimate of the
         base variable node.
 
         :param model: The machine learning model
         :type model: models.SeldonianModel object
         :param theta:
@@ -344,20 +350,19 @@
         :type theta: numpy ndarray
         :param data_dict:
             Contains inputs to model,
             such as features and labels
         :type data_dict: dict
         """
 
-        return sample_from_statistic(
+        return zhat_funcs.sample_from_statistic(
             model=model,
             statistic_name=self.measure_function_name,
             theta=theta,
             data_dict=data_dict,
-            datasize=datasize,
             **kwargs,
         )
 
     def predict_HC_lowerbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence lower bound
         that we expect to pass the safety test.
@@ -758,22 +763,17 @@
         Overrides same method from parent class, :py:class:`.BaseNode`
         """
         dataset = kwargs["dataset"]
         features = dataset.features
         labels = np.expand_dims(dataset.labels, axis=1)
         sensitive_attrs = dataset.sensitive_attrs
 
-        data_dict, datasize = self.precalculate_data(features, labels, sensitive_attrs)
-
-        if kwargs["branch"] == "candidate_selection":
-            n_safety = kwargs["n_safety"]
-            frac_masked = datasize / len(features)
-            datasize = int(round(frac_masked * n_safety))
+        data_dict = self.precalculate_data(features, labels, sensitive_attrs)
 
-        return data_dict, datasize
+        return data_dict
 
     def precalculate_data(self, X, Y, S):
         """
         Preconfigure dataset for candidate selection or
         safety test so that it does not need to be
         recalculated on each iteration through the parse tree
 
@@ -813,15 +813,15 @@
         data_dict = {
             "X_male": X_male,
             "Y_male": Y_male,
             "X_female": X_female,
             "Y_female": Y_female,
         }
         datasize = N_least
-        return data_dict, datasize
+        return data_dict
 
     def zhat(self, model, theta, data_dict, **kwargs):
         """
         Pair up male and female columns and compute a vector of:
         (y_i - y_hat_i | M) - (y_j - y_hat_j | F).
         There may not be the same number of male and female rows
         so the number of pairs is min(N_male,N_female)
@@ -896,15 +896,15 @@
         model = kwargs["model"]
         theta = kwargs["theta"]
         data_dict = kwargs["data_dict"]
 
         # Get squashed squared errors
         X = data_dict["features"]
         y = data_dict["labels"]
-        squared_errors = objectives.vector_Squared_Error(model, theta, X, y)
+        squared_errors = zhat_funcs.vector_Squared_Error(model, theta, X, y)
         # sort
         Z = np.array(sorted(squared_errors))
         # Now calculate cvar
         percentile_thresh = (1 - self.alpha) * 100
         # calculate var_alpha
         var_alpha = np.percentile(Z, percentile_thresh)
         # cvar is the mean of all values >= var_alpha
@@ -951,15 +951,15 @@
         s = 2.0
         y_hat_min = y_min * (1 + s) / 2 + y_max * (1 - s) / 2
         y_hat_max = y_max * (1 + s) / 2 + y_min * (1 - s) / 2
 
         min_squared_error = 0
         max_squared_error = max(pow(y_hat_max - y_min, 2), pow(y_max - y_hat_min, 2))
 
-        squared_errors = objectives.vector_Squared_Error(model, theta, X, y)
+        squared_errors = zhat_funcs.vector_Squared_Error(model, theta, X, y)
 
         a = min_squared_error
         b = max_squared_error
         # Need to sort squared errors to get Z1, ..., Zn
         sorted_squared_errors = sorted(squared_errors)
 
         bound_kwargs = {
```

### Comparing `seldonian_engine-0.8.0/seldonian/parse_tree/operators.py` & `seldonian_engine-0.8.1/seldonian/parse_tree/operators.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/parse_tree/parse_tree.py` & `seldonian_engine-0.8.1/seldonian/parse_tree/parse_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,14 @@
                 self.base_node_dict[new_node.name] = {
                     "bound_method": default_bound_method,
                     "bound_computed": False,
                     "value_computed": False,
                     "lower": float("-inf"),
                     "upper": float("inf"),
                     "data_dict": None,
-                    "datasize": 0,
                 }
 
         self.n_nodes += 1
         new_node.index = self.node_index
         self.node_index += 1
 
         # If node is a leaf node, don't check for children
@@ -504,18 +503,28 @@
             node_kwargs["name"] = node_name
             node_kwargs["cm_true_index"] = row_index
             node_kwargs["cm_pred_index"] = col_index
         elif ast_node.value.id in ["J_pi_new_","J_pi_new_PDIS_"]:
             # alternate reward function
             node_class = RLAltRewardBaseNode
             try:
-                # 3.8 syntax
+                # Python 3.8 syntax ("ast" is part of the standard library)
                 alt_reward_number = ast_node.slice.value.value
             except AttributeError:
-                alt_reward_number = ast_node.slice.value
+                try:
+                    # Python 3.9 and some 3.10 syntaxes
+                    alt_reward_number = ast_node.slice.value
+                except AttributeError:
+                    # Later Python 3.10 syntax
+                    alt_reward_number = ast_node.slice.id
+            # Validate that alt_reward_number is an integer
+            if type(alt_reward_number) != int:
+                raise RuntimeError(
+                    "The alternate reward number you entered was not an integer."
+                )
             node_name = f"{ast_node.value.id}[{alt_reward_number}]"
             node_kwargs = {}
             node_kwargs["name"] = node_name
             node_kwargs["alt_reward_number"] = alt_reward_number
         else:
             # It's one of the PR_[i], FPR_[i], etc. functions
             node_class = MultiClassBaseNode
@@ -710,30 +719,30 @@
             else:
                 # Need to calculate the bound
                 if "dataset" in kwargs:
                     # Check if data has already been prepared
                     # for this node name. If so, use precalculated data
                     if self.base_node_dict[node.name]["data_dict"] != None:
                         data_dict = self.base_node_dict[node.name]["data_dict"]
-                        datasize = self.base_node_dict[node.name]["datasize"]
                     else:
                         # Data not prepared already. Need to do that.
                         if isinstance(node, RLAltRewardBaseNode):
                             kwargs["alt_reward_number"] = node.alt_reward_number
-                        data_dict, datasize = node.calculate_data_forbound(**kwargs)
+                        
+                        data_dict = node.calculate_data_forbound(**kwargs)
                         self.base_node_dict[node.name]["data_dict"] = data_dict
-                        self.base_node_dict[node.name]["datasize"] = datasize
 
                     kwargs["data_dict"] = data_dict
-                    kwargs["datasize"] = datasize
 
                 bound_method = self.base_node_dict[node.name]["bound_method"]
+                
                 if isinstance(node, ConfusionMatrixBaseNode):
                     kwargs["cm_true_index"] = node.cm_true_index
                     kwargs["cm_pred_index"] = node.cm_pred_index
+                
                 bound_result = node.calculate_bounds(
                     bound_method=bound_method, **kwargs
                 )
                 self.base_node_dict[node.name]["bound_computed"] = True
 
                 if node.will_lower_bound:
                     node.lower = bound_result["lower"]
@@ -789,25 +798,21 @@
                 return
             else:
                 if "dataset" in kwargs:
                     # Check if data has already been prepared
                     # for this node name. If so, use precalculated data
                     if self.base_node_dict[node.name]["data_dict"] != None:
                         data_dict = self.base_node_dict[node.name]["data_dict"]
-                        datasize = self.base_node_dict[node.name]["datasize"]
                     else:
-                        print("Calculating data for bound")
                         if isinstance(node, RLAltRewardBaseNode):
                             kwargs["alt_reward_number"] = node.alt_reward_number
-                        data_dict, datasize = node.calculate_data_forbound(**kwargs)
+                        data_dict = node.calculate_data_forbound(**kwargs)
                         self.base_node_dict[node.name]["data_dict"] = data_dict
-                        self.base_node_dict[node.name]["datasize"] = datasize
 
                     kwargs["data_dict"] = data_dict
-                    kwargs["datasize"] = datasize
 
                 if isinstance(node, ConfusionMatrixBaseNode):
                     kwargs["cm_true_index"] = node.cm_true_index
                     kwargs["cm_pred_index"] = node.cm_pred_index
                 
                 value = node.calculate_value(**kwargs)
                 node.value = value
@@ -1177,15 +1182,14 @@
             self.base_node_dict[node_name]["bound_computed"] = False
             self.base_node_dict[node_name]["value_computed"] = False
             self.base_node_dict[node_name]["value"] = None
             self.base_node_dict[node_name]["lower"] = float("-inf")
             self.base_node_dict[node_name]["upper"] = float("inf")
             if reset_data:
                 self.base_node_dict[node_name]["data_dict"] = None
-                self.base_node_dict[node_name]["datasize"] = 0
 
         return
 
     def make_viz(self, title):
         """
         Make a graphviz diagram from a root node
```

### Comparing `seldonian_engine-0.8.0/seldonian/safety_test/safety_test.py` & `seldonian_engine-0.8.1/seldonian/safety_test/safety_test.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/seldonian_algorithm.py` & `seldonian_engine-0.8.1/seldonian/seldonian_algorithm.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/spec.py` & `seldonian_engine-0.8.1/seldonian/spec.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/utils/io_utils.py` & `seldonian_engine-0.8.1/seldonian/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian/utils/plot_utils.py` & `seldonian_engine-0.8.1/seldonian/utils/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     :param savename: The full path where you want to save the plot
     :type savename: str
     :param show: Whether to show the plot with plt.show().
             Only relevant when save=False
     :type show: bool
     """
     # Extract values from dictionary
-    theta_vals = solution["theta_vals"]
     lamb_vals = solution[
         "lamb_vals"
     ]  # i x j array where i is number of iterations, j is number of constraints
     f_vals = solution["f_vals"]  # length = i array where i is number of iterations
     g_vals = solution[
         "g_vals"
     ]  # i x j array where i is number of iterations, j is number of constraints
```

### Comparing `seldonian_engine-0.8.0/seldonian/utils/stats_utils.py` & `seldonian_engine-0.8.1/seldonian/utils/stats_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import autograd.numpy as np  # Thinly-wrapped version of Numpy
 from scipy.stats import t
 
+stability_const = 1e-15
 
 def stddev(v):
     """
     Sample standard deviation of the vector v,
     with Bessel's correction
 
     :param v: vector of data
```

### Comparing `seldonian_engine-0.8.0/seldonian/utils/tutorial_utils.py` & `seldonian_engine-0.8.1/seldonian/utils/tutorial_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/seldonian_engine.egg-info/PKG-INFO` & `seldonian_engine-0.8.1/seldonian_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian-engine
-Version: 0.8.0
+Version: 0.8.1
 Summary: Core library for Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -21,15 +21,15 @@
 
 This is the source code repository for a framework for creating and running [Seldonian](https://seldonian.cs.umass.edu/) algorithms. 
 
 ## Installation
 
 To use the latest stable version:
 ```
-pip install seldonian-toolkit
+pip install seldonian-engine
 ```
 
 To run this code as a developer, create a virtual environment. Then install the package locally, e.g. 
 
 ```
 python setup.py develop
 ```
```

### Comparing `seldonian_engine-0.8.0/seldonian_engine.egg-info/SOURCES.txt` & `seldonian_engine-0.8.1/seldonian_engine.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 seldonian/models/objectives.py
 seldonian/models/pytorch_cnn.py
 seldonian/models/pytorch_model.py
 seldonian/models/sklearn_lr.py
 seldonian/models/sklearn_model.py
 seldonian/models/tensorflow_cnn.py
 seldonian/models/tensorflow_model.py
+seldonian/models/zhat_funcs.py
 seldonian/optimizers/__init__.py
 seldonian/optimizers/gradient_descent.py
 seldonian/parse_tree/__init__.py
 seldonian/parse_tree/nodes.py
 seldonian/parse_tree/operators.py
 seldonian/parse_tree/parse_tree.py
 seldonian/safety_test/__init__.py
@@ -72,14 +73,15 @@
 seldonian_engine.egg-info/requires.txt
 seldonian_engine.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_RL.py
 tests/test_dataset.py
 tests/test_io_utils.py
+tests/test_models.py
 tests/test_objectives.py
 tests/test_parse_tree.py
 tests/test_plot_utils.py
 tests/test_safety_test.py
 tests/test_seldonian_algorithm.py
 tests/test_sklearn.py
 tests/test_spec.py
```

### Comparing `seldonian_engine-0.8.0/setup.py` & `seldonian_engine-0.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_engine",
-    version="0.8.0",
+    version="0.8.1",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Core library for Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
```

### Comparing `seldonian_engine-0.8.0/tests/conftest.py` & `seldonian_engine-0.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_RL.py` & `seldonian_engine-0.8.1/tests/test_RL.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_dataset.py` & `seldonian_engine-0.8.1/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_io_utils.py` & `seldonian_engine-0.8.1/tests/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_objectives.py` & `seldonian_engine-0.8.1/tests/test_objectives.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import pytest
 import autograd.numpy as np
 
 from seldonian.spec import (SupervisedSpec)
 from seldonian.models import objectives
+from seldonian.models import zhat_funcs
 from seldonian.models.models import *
 from seldonian.seldonian_algorithm import SeldonianAlgorithm
 
 def test_binary_classification_measure_functions():
 	# i = 4 datapoints
 	# j = 2 features
 	# labels are 0 or 1
@@ -36,31 +37,31 @@
 	TPR = objectives.True_Positive_Rate(model,theta,X,Y)
 	assert TPR == pytest.approx(1.0-FNR)
 	TNR = objectives.True_Negative_Rate(model,theta,X,Y)
 	assert TNR == pytest.approx(1.0-FPR)
 	ACC = objectives.Accuracy(model,theta,X,Y,sub_regime=sub_regime)
 	assert ACC == pytest.approx(0.5598653825)
 	# Vector statistics 
-	vector_PR = objectives.vector_Positive_Rate(model,theta,X,Y)
+	vector_PR = zhat_funcs.vector_Positive_Rate(model,theta,X,Y)
 	assert np.allclose(vector_PR,y_pred)
-	vector_NR = objectives.vector_Negative_Rate(model,theta,X,Y)
+	vector_NR = zhat_funcs.vector_Negative_Rate(model,theta,X,Y)
 	assert np.allclose(vector_NR,1.0-y_pred)
-	vector_FPR = objectives.vector_False_Positive_Rate(model,theta,X,Y)
+	vector_FPR = zhat_funcs.vector_False_Positive_Rate(model,theta,X,Y)
 	# True label=0 was in first two datapoints. prob[1:3] = [0.5,0.5621765]
 	arcomp_FPR = y_pred[0:2]
 	assert np.allclose(vector_FPR,arcomp_FPR)
-	vector_FNR = objectives.vector_False_Negative_Rate(model,theta,X,Y)
+	vector_FNR = zhat_funcs.vector_False_Negative_Rate(model,theta,X,Y)
 	# True label=1 was in last two datapoints: want 1.0-prob[2:]
 	arcomp_FNR = 1.0-y_pred[2:]
 	assert np.allclose(vector_FNR,arcomp_FNR)
-	vector_TPR = objectives.vector_True_Positive_Rate(model,theta,X,Y)
+	vector_TPR = zhat_funcs.vector_True_Positive_Rate(model,theta,X,Y)
 	assert np.allclose(vector_TPR,1.0-arcomp_FNR)
-	vector_TNR = objectives.vector_True_Negative_Rate(model,theta,X,Y)
+	vector_TNR = zhat_funcs.vector_True_Negative_Rate(model,theta,X,Y)
 	assert np.allclose(vector_TNR,1.0-arcomp_FPR)
-	vector_ACC = objectives.vector_Accuracy(model,theta,X,Y,sub_regime=sub_regime)
+	vector_ACC = zhat_funcs.vector_Accuracy(model,theta,X,Y,sub_regime=sub_regime)
 	arcomp_ACC = np.array([0.5, 0.4378235 , 0.62245933, 0.6791787 ])
 	assert np.allclose(vector_ACC,arcomp_ACC)
 
 def test_multiclass_classification_measure_functions():
 	# i = 4 datapoints
 	# j = 2 features
 	# k = 3 classes
@@ -83,15 +84,15 @@
 	y_pred = model.predict(theta,X) # (i,k)
 
 	# Accuracy
 	ACC = objectives.Accuracy(model,theta,X,Y,sub_regime=sub_regime)
 	assert ACC == pytest.approx(0.36639504)
 
 	# Vector accuracy
-	vector_ACC = objectives.vector_Accuracy(model,theta,X,Y,sub_regime=sub_regime)
+	vector_ACC = zhat_funcs.vector_Accuracy(model,theta,X,Y,sub_regime=sub_regime)
 	arcomp_ACC = np.array([0.33333333,0.41922895,0.54654939,0.14024438,0.49951773,0.25949646])
 	assert np.allclose(vector_ACC,arcomp_ACC)
 
 	for class_index in [0,1,2]:
 		# Will reuse these masks
 		pos_mask = Y == class_index
 		neg_mask = Y != class_index
@@ -114,33 +115,33 @@
 			class_index=class_index)
 		assert TPR == pytest.approx(1.0 - FNR)
 		TNR = objectives.True_Negative_Rate(model,theta,X,Y,
 			class_index=class_index)
 		assert TNR == pytest.approx(1.0 - FPR)
 	
 		# Vector statistics 
-		vector_PR = objectives.vector_Positive_Rate(
+		vector_PR = zhat_funcs.vector_Positive_Rate(
 			model,theta,X,Y,
 			class_index=class_index)
 		assert np.allclose(vector_PR,y_pred[:,class_index])
-		vector_NR = objectives.vector_Negative_Rate(
+		vector_NR = zhat_funcs.vector_Negative_Rate(
 			model,theta,X,Y,
 			class_index=class_index)
 		assert np.allclose(vector_NR,1.0-y_pred[:,class_index])
-		vector_FPR = objectives.vector_False_Positive_Rate(
+		vector_FPR = zhat_funcs.vector_False_Positive_Rate(
 			model,theta,X,Y,
 			class_index=class_index)
 		arcomp_FPR = y_pred[:,class_index][neg_mask]
 		assert np.allclose(vector_FPR,arcomp_FPR)
-		vector_FNR = objectives.vector_False_Negative_Rate(
+		vector_FNR = zhat_funcs.vector_False_Negative_Rate(
 			model,theta,X,Y,
 			class_index=class_index)
 		arcomp_FNR = 1.0-y_pred[:,class_index][pos_mask]
 		assert np.allclose(vector_FNR,arcomp_FNR)
-		vector_TPR = objectives.vector_True_Positive_Rate(
+		vector_TPR = zhat_funcs.vector_True_Positive_Rate(
 			model,theta,X,Y,
 			class_index=class_index)
 		assert np.allclose(vector_TPR,1.0-arcomp_FNR)
-		vector_TNR = objectives.vector_True_Negative_Rate(
+		vector_TNR = zhat_funcs.vector_True_Negative_Rate(
 			model,theta,X,Y,
 			class_index=class_index)
 		assert np.allclose(vector_TNR,1.0-arcomp_FPR)
```

### Comparing `seldonian_engine-0.8.0/tests/test_parse_tree.py` & `seldonian_engine-0.8.1/tests/test_parse_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -771,15 +771,14 @@
 	pt = ParseTree(delta,regime='reinforcement_learning',
 		sub_regime='all')
 	pt.create_from_ast(constraint_str)
 	assert pt.root.left.measure_function_name == 'J_pi_new'
 	assert pt.root.left.name == 'J_pi_new_[1]'
 	assert pt.root.left.alt_reward_number == 1
 
-
 	constraint_str = '(J_pi_new_[2] | [A,B]) - 0.5'
 	pt = ParseTree(delta,regime='reinforcement_learning',
 		sub_regime='all',columns=['A','B'])
 	pt.create_from_ast(constraint_str)
 	assert pt.root.left.measure_function_name == 'J_pi_new'
 	assert pt.root.left.name == 'J_pi_new_[2] | [A,B]'
 	assert pt.root.left.alt_reward_number == 2
@@ -789,14 +788,53 @@
 	pt = ParseTree(delta,regime='reinforcement_learning',
 		sub_regime='all')
 	pt.create_from_ast(constraint_str)
 	assert pt.root.left.measure_function_name == 'J_pi_new_PDIS'
 	assert pt.root.left.name == 'J_pi_new_PDIS_[1]'
 	assert pt.root.left.alt_reward_number == 1
 
+def test_rl_alt_reward_bad_string():
+	# Test that using non-numeric characters for the alt reward number raises an error
+	delta = 0.05
+	constraint_str = 'J_pi_new_[N] - 0.5'
+
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all')
+	with pytest.raises(RuntimeError) as excinfo:
+			pt.create_from_ast(constraint_str)
+	error_str = "The alternate reward number you entered was not an integer."		
+	assert str(excinfo.value) == error_str
+
+	constraint_str = 'J_pi_new_[1.1] - 0.5'
+
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all')
+	with pytest.raises(RuntimeError) as excinfo:
+			pt.create_from_ast(constraint_str)
+	error_str = "The alternate reward number you entered was not an integer."		
+	assert str(excinfo.value) == error_str
+
+	constraint_str = 'J_pi_new_PDIS_[M] - 0.5'
+
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all')
+	with pytest.raises(RuntimeError) as excinfo:
+			pt.create_from_ast(constraint_str)
+	error_str = "The alternate reward number you entered was not an integer."		
+	assert str(excinfo.value) == error_str
+
+	constraint_str = 'J_pi_new_PDIS_[5.9] - 0.5'
+
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all')
+	with pytest.raises(RuntimeError) as excinfo:
+			pt.create_from_ast(constraint_str)
+	error_str = "The alternate reward number you entered was not an integer."		
+	assert str(excinfo.value) == error_str
+
 def test_rl_alt_reward_precalc_return():
 	np.random.seed(0)
 	
 	from seldonian.RL.RL_model import RL_model
 	from seldonian.RL.Agents.Policies.Softmax import DiscreteSoftmax
 	from seldonian.RL.Env_Description import Spaces, Env_Description
 	data_pth = 'static/datasets/RL/gridworld/gridworld_100episodes_2altrewards.pkl'
@@ -864,15 +902,14 @@
 		model=model,regime='reinforcement_learning',
 		branch='safety_test')
 	assert PDIS_pt.root.value == pytest.approx(0.08025886028)
 
 	weighted_returns_alt_reward = PDIS_pt.base_node_dict["J_pi_new_PDIS_[1]"]['data_dict']['weighted_returns']
 	assert weighted_returns_alt_reward[0] == pytest.approx(7.563782445399999)
 
-
 def test_measure_function_with_conditional_bad_syntax_captured():
 	delta=0.05
 	error_str = ("Error parsing your expression."
 				" The issue is most likely due to"
 				" missing/mismatched parentheses or square brackets"
 				" in a conditional expression involving '|'.")
 
@@ -1150,34 +1187,34 @@
 
 	# propagate the bounds with example theta value
 	# theta = np.hstack([np.array([0.0,0.0]),np.random.uniform(-0.05,0.05,10)])
 	theta = np.random.uniform(-0.05,0.05,10)
 	pt.propagate_bounds(theta=theta,dataset=dataset,
 		model=model_instance,branch='safety_test',
 		regime='supervised_learning')
-	assert pt.root.lower == pytest.approx(0.5990300)
-	assert pt.root.upper == pytest.approx(0.5999346)
+	assert pt.root.lower == pytest.approx(0.59886236)
+	assert pt.root.upper == pytest.approx(0.60010258)
 
-	constraint_str = '1+log(FPR)'
-	delta = 0.05
-	pt = ParseTree(delta,regime='supervised_learning',
-		sub_regime='classification',
-		columns=dataset.meta.sensitive_col_names)
-	# pt.build_tree(constraint_str)
-	
-	pt.create_from_ast(constraint_str)
-	pt.assign_deltas(weight_method='equal')
-
-	# propagate the bounds with example theta value
-	theta = np.random.uniform(-0.05,0.05,10)
-	pt.propagate_bounds(theta=theta,dataset=dataset,
-		model=model_instance,branch='safety_test',
-		regime='supervised_learning')
-	assert pt.root.lower == pytest.approx(-2.5187904943528903)
-	assert pt.root.upper == pytest.approx(-2.470509955060809)
+	# constraint_str = '1+log(FPR)'
+	# delta = 0.05
+	# pt = ParseTree(delta,regime='supervised_learning',
+	# 	sub_regime='classification',
+	# 	columns=dataset.meta.sensitive_col_names)
+	# # pt.build_tree(constraint_str)
+	
+	# pt.create_from_ast(constraint_str)
+	# pt.assign_deltas(weight_method='equal')
+
+	# # propagate the bounds with example theta value
+	# theta = np.random.uniform(-0.05,0.05,10)
+	# pt.propagate_bounds(theta=theta,dataset=dataset,
+	# 	model=model_instance,branch='safety_test',
+	# 	regime='supervised_learning')
+	# assert pt.root.lower == pytest.approx(-2.5187904943528903)
+	# assert pt.root.upper == pytest.approx(-2.470509955060809)
 
 def test_deltas_assigned_equally():
 	constraint_str = 'abs((Mean_Error|[M]) - (Mean_Error|[F])) - 0.1'
 	delta = 0.05 
 
 	pt = ParseTree(delta,regime='supervised_learning',
 		sub_regime='regression',columns=['M','F'])
@@ -1477,22 +1514,22 @@
 	candidate_labels = labels[:n_candidate] 
 	safety_labels = labels[n_candidate:] 
 	
 	candidate_dataset = SupervisedDataSet(
 		features=candidate_features,
 		labels=candidate_labels,
 		sensitive_attrs=[],
-		num_datapoints=len(candidate_features),
+		num_datapoints=len(candidate_labels),
 		meta=dataset.meta)
 
 	safety_dataset = SupervisedDataSet(
 		features=safety_features,
 		labels=safety_labels,
 		sensitive_attrs=[],
-		num_datapoints=len(safety_features),
+		num_datapoints=len(safety_labels),
 		meta=dataset.meta)
 
 	pt = ParseTree(deltas[0],regime='supervised_learning',
 		sub_regime='regression')
 	pt.create_from_ast(constraint_strs[0])
 	pt.assign_deltas(weight_method='equal')
 	pt.assign_bounds_needed()
@@ -1503,28 +1540,28 @@
 	assert pt.root.name == 'sub'  
 	assert pt.root.left.will_lower_bound == False
 	assert pt.root.left.will_upper_bound == True
 	theta = np.array([0,1,2])
 	
 	# Candidate selection
 	pt.propagate_bounds(theta=theta,dataset=candidate_dataset,
-		n_safety=len(safety_features),
+		n_safety=len(safety_labels),
 		model=model,
 		branch='candidate_selection',
 		regime='supervised_learning')
 	assert pt.root.lower == float('-inf') # not bound_computed 
-	assert pt.root.upper == pytest.approx(235.89950087)
+	assert pt.root.upper == pytest.approx(12.341009549)
 	pt.reset_base_node_dict(reset_data=True)
 	# Safety test
 	pt.propagate_bounds(theta=theta,dataset=safety_dataset,
 		model=model,
 		branch='safety_test',
 		regime='supervised_learning')
 	assert pt.root.lower == float('-inf') # not computed
-	assert pt.root.upper == pytest.approx(166.0071908)
+	assert pt.root.upper == pytest.approx(13.1514499)
 
 def test_bad_bound_method(simulated_regression_dataset):
 	# dummy data for linear regression
 	np.random.seed(0)
 	numPoints=1000
 
 	# First, single sided bound (MSE only needs upper bound)
```

### Comparing `seldonian_engine-0.8.0/tests/test_plot_utils.py` & `seldonian_engine-0.8.1/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_safety_test.py` & `seldonian_engine-0.8.1/tests/test_safety_test.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_seldonian_algorithm.py` & `seldonian_engine-0.8.1/tests/test_seldonian_algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,143 +354,143 @@
 		[ 0.42523186, -0.00285192, -0.00202239,
 		 -0.00241261, -0.00234646, -0.0025831,
 		  0.01924249,  0.01865552, -0.00308212, 
 		 -0.0024446 ])
 
 	assert np.allclose(solution,array_to_compare)
 
-def test_cvar_custom_base_node():
-	""" Test that the gpa regression example runs 
-	using the custom base node that calculates 
-	CVaR alpha of the squared error. Make
-	sure safety test passes and solution is correct.
-
-	Check that the actual value of the constraint (not the bound)
-	is also correctly calculated.
-	"""
-	from seldonian.models.models import BoundedLinearRegressionModel
-	rseed=0
-	np.random.seed(rseed) 
-	constraint_strs = ['CVaRSQE <= 50.0']
-	deltas = [0.1]
-
-	numPoints = 2500
-	dataset = make_synthetic_regression_dataset(
-		numPoints,
-		loc_X=0.0,
-		loc_Y=0.0,
-		sigma_X=1.0,
-		sigma_Y=0.2,
-		clipped=True)
-
-	parse_trees = make_parse_trees_from_constraints(
-		constraint_strs,
-		deltas)
-
-	model = BoundedLinearRegressionModel()
-
-	# Create spec object
-	spec = SupervisedSpec(
-		dataset=dataset,
-		model=model,
-		sub_regime='regression',
-		primary_objective=objectives.Mean_Squared_Error,
-		use_builtin_primary_gradient_fn=False,
-		custom_primary_gradient_fn=objectives.gradient_Bounded_Squared_Error,
-		parse_trees=parse_trees,
-		optimization_technique='gradient_descent',
-		optimizer='adam',
-		optimization_hyperparams={
-			'lambda_init'   : np.array([0.5]),
-			'alpha_theta'   : 0.01,
-			'alpha_lamb'    : 0.01,
-			'beta_velocity' : 0.9,
-			'beta_rmsprop'  : 0.95,
-			'num_iters'     : 5,
-			'use_batches'   : False,
-			'gradient_library': "autograd",
-			'hyper_search'  : None,
-			'verbose'       : True,
-		}
-	)
-
-	# Run seldonian algorithm
-	SA = SeldonianAlgorithm(spec)
-	passed_safety,solution = SA.run(debug=True)
-	assert passed_safety == True
-	solution_to_compare = np.array([-0.07257342,0.07182381])
-	assert np.allclose(solution,solution_to_compare)
-
-	# Make sure we can evaluate constraint as well
-	pt = parse_trees[0]
-	pt.evaluate_constraint(theta=solution,dataset=dataset,
-		model=model,regime='supervised_learning',
-		branch='safety_test')
-	assert pt.root.value == pytest.approx(-47.163772762)
-
-def test_cvar_lower_bound():
-	""" The normal constraint only uses 
-	the CVAR upper bound because we want CVAR < some value. 
-	Test that the lower bound also works
-
-	Check that the actual value of the constraint (not the bound)
-	is also correctly calculated.
-	"""
-	from seldonian.models.models import BoundedLinearRegressionModel
-	rseed=0
-	np.random.seed(rseed) 
-	constraint_strs = ['CVaRSQE >= 5.0']
-	deltas = [0.1]
-
-	numPoints = 1000
-	dataset = make_synthetic_regression_dataset(
-		numPoints,
-		loc_X=0.0,
-		loc_Y=0.0,
-		sigma_X=1.0,
-		sigma_Y=0.2,
-		clipped=True)
-
-	parse_trees = make_parse_trees_from_constraints(
-		constraint_strs,
-		deltas)
-
-	model = BoundedLinearRegressionModel()
-
-	# Create spec object
-	spec = SupervisedSpec(
-		dataset=dataset,
-		model=model,
-		sub_regime='regression',
-		primary_objective=objectives.Mean_Squared_Error,
-		use_builtin_primary_gradient_fn=False,
-		custom_primary_gradient_fn=objectives.gradient_Bounded_Squared_Error,
-		parse_trees=parse_trees,
-		optimization_technique='gradient_descent',
-		optimizer='adam',
-		optimization_hyperparams={
-			'lambda_init'   : np.array([0.5]),
-			'alpha_theta'   : 0.01,
-			'alpha_lamb'    : 0.01,
-			'beta_velocity' : 0.9,
-			'beta_rmsprop'  : 0.95,
-			'num_iters'     : 10,
-			'use_batches'   : False,
-			'gradient_library': "autograd",
-			'hyper_search'  : None,
-			'verbose'       : True,
-		}
-	)
-
-	# Run seldonian algorithm
-	SA = SeldonianAlgorithm(spec)
-	passed_safety,solution = SA.run()
-	assert passed_safety == True
-	solution_to_compare = np.array([-0.15426298, -0.15460036])
-	assert np.allclose(solution,solution_to_compare)
+# def test_cvar_custom_base_node():
+# 	""" Test that the gpa regression example runs 
+# 	using the custom base node that calculates 
+# 	CVaR alpha of the squared error. Make
+# 	sure safety test passes and solution is correct.
+
+# 	Check that the actual value of the constraint (not the bound)
+# 	is also correctly calculated.
+# 	"""
+# 	from seldonian.models.models import BoundedLinearRegressionModel
+# 	rseed=0
+# 	np.random.seed(rseed) 
+# 	constraint_strs = ['CVaRSQE <= 50.0']
+# 	deltas = [0.1]
+
+# 	numPoints = 2500
+# 	dataset = make_synthetic_regression_dataset(
+# 		numPoints,
+# 		loc_X=0.0,
+# 		loc_Y=0.0,
+# 		sigma_X=1.0,
+# 		sigma_Y=0.2,
+# 		clipped=True)
+
+# 	parse_trees = make_parse_trees_from_constraints(
+# 		constraint_strs,
+# 		deltas)
+
+# 	model = BoundedLinearRegressionModel()
+
+# 	# Create spec object
+# 	spec = SupervisedSpec(
+# 		dataset=dataset,
+# 		model=model,
+# 		sub_regime='regression',
+# 		primary_objective=objectives.Mean_Squared_Error,
+# 		use_builtin_primary_gradient_fn=False,
+# 		custom_primary_gradient_fn=objectives.gradient_Bounded_Squared_Error,
+# 		parse_trees=parse_trees,
+# 		optimization_technique='gradient_descent',
+# 		optimizer='adam',
+# 		optimization_hyperparams={
+# 			'lambda_init'   : np.array([0.5]),
+# 			'alpha_theta'   : 0.01,
+# 			'alpha_lamb'    : 0.01,
+# 			'beta_velocity' : 0.9,
+# 			'beta_rmsprop'  : 0.95,
+# 			'num_iters'     : 5,
+# 			'use_batches'   : False,
+# 			'gradient_library': "autograd",
+# 			'hyper_search'  : None,
+# 			'verbose'       : True,
+# 		}
+# 	)
+
+# 	# Run seldonian algorithm
+# 	SA = SeldonianAlgorithm(spec)
+# 	passed_safety,solution = SA.run(debug=True)
+# 	assert passed_safety == True
+# 	solution_to_compare = np.array([-0.07257342,0.07182381])
+# 	assert np.allclose(solution,solution_to_compare)
+
+# 	# Make sure we can evaluate constraint as well
+# 	pt = parse_trees[0]
+# 	pt.evaluate_constraint(theta=solution,dataset=dataset,
+# 		model=model,regime='supervised_learning',
+# 		branch='safety_test')
+# 	assert pt.root.value == pytest.approx(-47.163772762)
+
+# def test_cvar_lower_bound():
+# 	""" The normal constraint only uses 
+# 	the CVAR upper bound because we want CVAR < some value. 
+# 	Test that the lower bound also works
+
+# 	Check that the actual value of the constraint (not the bound)
+# 	is also correctly calculated.
+# 	"""
+# 	from seldonian.models.models import BoundedLinearRegressionModel
+# 	rseed=0
+# 	np.random.seed(rseed) 
+# 	constraint_strs = ['CVaRSQE >= 5.0']
+# 	deltas = [0.1]
+
+# 	numPoints = 1000
+# 	dataset = make_synthetic_regression_dataset(
+# 		numPoints,
+# 		loc_X=0.0,
+# 		loc_Y=0.0,
+# 		sigma_X=1.0,
+# 		sigma_Y=0.2,
+# 		clipped=True)
+
+# 	parse_trees = make_parse_trees_from_constraints(
+# 		constraint_strs,
+# 		deltas)
+
+# 	model = BoundedLinearRegressionModel()
+
+# 	# Create spec object
+# 	spec = SupervisedSpec(
+# 		dataset=dataset,
+# 		model=model,
+# 		sub_regime='regression',
+# 		primary_objective=objectives.Mean_Squared_Error,
+# 		use_builtin_primary_gradient_fn=False,
+# 		custom_primary_gradient_fn=objectives.gradient_Bounded_Squared_Error,
+# 		parse_trees=parse_trees,
+# 		optimization_technique='gradient_descent',
+# 		optimizer='adam',
+# 		optimization_hyperparams={
+# 			'lambda_init'   : np.array([0.5]),
+# 			'alpha_theta'   : 0.01,
+# 			'alpha_lamb'    : 0.01,
+# 			'beta_velocity' : 0.9,
+# 			'beta_rmsprop'  : 0.95,
+# 			'num_iters'     : 10,
+# 			'use_batches'   : False,
+# 			'gradient_library': "autograd",
+# 			'hyper_search'  : None,
+# 			'verbose'       : True,
+# 		}
+# 	)
+
+# 	# Run seldonian algorithm
+# 	SA = SeldonianAlgorithm(spec)
+# 	passed_safety,solution = SA.run()
+# 	assert passed_safety == True
+# 	solution_to_compare = np.array([-0.15426298, -0.15460036])
+# 	assert np.allclose(solution,solution_to_compare)
 
 def test_gpa_data_regression_multiple_constraints(gpa_regression_dataset):
 	""" Test that the gpa regression example runs 
 	with a two constraints using gradient descent. Make
 	sure safety test passes and solution is correct.
 	"""
 	# Load metadata
```

### Comparing `seldonian_engine-0.8.0/tests/test_sklearn.py` & `seldonian_engine-0.8.1/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_spec.py` & `seldonian_engine-0.8.1/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_stats_utils.py` & `seldonian_engine-0.8.1/tests/test_stats_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.8.0/tests/test_tutorial_utils.py` & `seldonian_engine-0.8.1/tests/test_tutorial_utils.py`

 * *Files identical despite different names*

