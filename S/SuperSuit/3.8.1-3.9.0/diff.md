# Comparing `tmp/SuperSuit-3.8.1.tar.gz` & `tmp/SuperSuit-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SuperSuit-3.8.1.tar", last modified: Fri Jul  7 23:49:42 2023, max compression
+gzip compressed data, was "SuperSuit-3.9.0.tar", last modified: Fri Jul 21 01:24:31 2023, max compression
```

## Comparing `SuperSuit-3.8.1.tar` & `SuperSuit-3.9.0.tar`

### file list

```diff
@@ -1,101 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.627312 SuperSuit-3.8.1/SuperSuit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-07 23:49:42.000000 SuperSuit-3.8.1/SuperSuit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.627312 SuperSuit-3.8.1/supersuit/
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.627312 SuperSuit-3.8.1/supersuit/aec_vector/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/async_vector_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/base_aec_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/aec_vector/vector_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/generic_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/basic_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/delay_observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/frame_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/max_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/nan_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/sticky_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/base_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/generic_wrappers/utils/shared_wrapper_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/lambda_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/action_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/observation_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/lambda_wrappers/reward_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/multiagent_wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/agent_indication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/black_death.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/multiagent_wrappers/padding_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/accumulator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/utils/action_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/action_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/action_transforms/homogenize_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/agent_indicator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/base_aec_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.631312 SuperSuit-3.8.1/supersuit/utils/basic_transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/color_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/normalize_obs.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/basic_transforms/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/convert_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/frame_skip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/frame_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/make_defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/obs_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/utils/wrapper_chooser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.635312 SuperSuit-3.8.1/supersuit/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/concat_vec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/constructors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/markov_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/multiproc_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/sb3_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/sb_vector_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/single_vec_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.635312 SuperSuit-3.8.1/supersuit/vector/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/utils/shared_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/utils/space_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/supersuit/vector/vector_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.635312 SuperSuit-3.8.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/aec_mock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/aec_unwrapped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/dummy_aec_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/dummy_gym_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/generated_agents_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/gym_mock_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/gym_unwrapped_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/parallel_env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/pettingzoo_api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_autodep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:42.639312 SuperSuit-3.8.1/test/test_vector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_aec_vector_identity_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_aec_vector_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_env_is_wrapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_gym_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_pettingzoo_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/test_vector/test_vector_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-07 23:49:36.000000 SuperSuit-3.8.1/test/vec_env_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    12201 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.253049 SuperSuit-3.9.0/SuperSuit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-07-21 01:24:31.000000 SuperSuit-3.9.0/SuperSuit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-21 01:24:31.000000 SuperSuit-3.9.0/SuperSuit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:24:31.000000 SuperSuit-3.9.0/SuperSuit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-21 01:24:31.000000 SuperSuit-3.9.0/SuperSuit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-21 01:24:31.000000 SuperSuit-3.9.0/SuperSuit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.253049 SuperSuit-3.9.0/supersuit/
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.253049 SuperSuit-3.9.0/supersuit/aec_vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/aec_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18256 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/aec_vector/async_vector_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/aec_vector/base_aec_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/aec_vector/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/aec_vector/vector_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.253049 SuperSuit-3.9.0/supersuit/generic_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/basic_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/delay_observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7962 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/frame_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/max_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/nan_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/sticky_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.257049 SuperSuit-3.9.0/supersuit/generic_wrappers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/utils/base_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/generic_wrappers/utils/shared_wrapper_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.257049 SuperSuit-3.9.0/supersuit/lambda_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/lambda_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/lambda_wrappers/action_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/lambda_wrappers/observation_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/lambda_wrappers/reward_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.257049 SuperSuit-3.9.0/supersuit/multiagent_wrappers/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/multiagent_wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/multiagent_wrappers/agent_indication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/multiagent_wrappers/black_death.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/multiagent_wrappers/padding_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.257049 SuperSuit-3.9.0/supersuit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/accumulator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.257049 SuperSuit-3.9.0/supersuit/utils/action_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/action_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/action_transforms/homogenize_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/agent_indicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/base_aec_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/supersuit/utils/basic_transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/color_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/normalize_obs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/basic_transforms/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/convert_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/frame_skip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/frame_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/make_defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/obs_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/utils/wrapper_chooser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/supersuit/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/concat_vec_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/constructors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/markov_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8671 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/multiproc_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/sb3_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/sb_vector_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/single_vec_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/supersuit/vector/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/utils/shared_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/utils/space_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/supersuit/vector/vector_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:24:31.261049 SuperSuit-3.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-21 01:24:18.000000 SuperSuit-3.9.0/test/test_autodep.py
```

### Comparing `SuperSuit-3.8.1/LICENSE.txt` & `SuperSuit-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/PKG-INFO` & `SuperSuit-3.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: SuperSuit
-Version: 3.8.1
+Version: 3.9.0
 Summary: Wrappers for Gymnasium and PettingZoo
-Home-page: https://github.com/Farama-Foundation/SuperSuit
-Author: Farama Foundation
-Author-email: contact@farama.org
+Author-email: Farama Foundation <contact@farama.org>
+License: MIT License
+Project-URL: Homepage, https://farama.org
+Project-URL: Repository, https://github.com/Farama-Foundation/SuperSuit
+Project-URL: Bug Report, https://github.com/Farama-Foundation/SuperSuit/issues
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <3.12
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+Provides-Extra: testing
+License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/SuperSuit/master/supersuit-text.png" width="500px"/>
 </p>
 
 
 SuperSuit introduces a collection of small functions which can wrap reinforcement learning environments to do preprocessing ('microwrappers').
@@ -64,7 +66,19 @@
 ```
 python3 -m venv env
 source env/bin/activate
 pip install --upgrade pip
 pip install -e .
 ```
 
+## Citation
+
+If you use this in your research, please cite:
+
+```
+@article{SuperSuit,
+  Title = {SuperSuit: Simple Microwrappers for Reinforcement Learning Environments},
+  Author = {Terry, J. K and Black, Benjamin and Hari, Ananth},
+  journal={arXiv preprint arXiv:2008.08932},
+  year={2020}
+}
+```
```

### Comparing `SuperSuit-3.8.1/README.md` & `SuperSuit-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/SuperSuit.egg-info/PKG-INFO` & `SuperSuit-3.9.0/SuperSuit.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: SuperSuit
-Version: 3.8.1
+Version: 3.9.0
 Summary: Wrappers for Gymnasium and PettingZoo
-Home-page: https://github.com/Farama-Foundation/SuperSuit
-Author: Farama Foundation
-Author-email: contact@farama.org
+Author-email: Farama Foundation <contact@farama.org>
+License: MIT License
+Project-URL: Homepage, https://farama.org
+Project-URL: Repository, https://github.com/Farama-Foundation/SuperSuit
+Project-URL: Bug Report, https://github.com/Farama-Foundation/SuperSuit/issues
 Keywords: Reinforcement Learning,game,RL,AI,gymnasium
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7, <3.12
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+Provides-Extra: testing
+License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/SuperSuit/master/supersuit-text.png" width="500px"/>
 </p>
 
 
 SuperSuit introduces a collection of small functions which can wrap reinforcement learning environments to do preprocessing ('microwrappers').
@@ -64,7 +66,19 @@
 ```
 python3 -m venv env
 source env/bin/activate
 pip install --upgrade pip
 pip install -e .
 ```
 
+## Citation
+
+If you use this in your research, please cite:
+
+```
+@article{SuperSuit,
+  Title = {SuperSuit: Simple Microwrappers for Reinforcement Learning Environments},
+  Author = {Terry, J. K and Black, Benjamin and Hari, Ananth},
+  journal={arXiv preprint arXiv:2008.08932},
+  year={2020}
+}
+```
```

### Comparing `SuperSuit-3.8.1/SuperSuit.egg-info/SOURCES.txt` & `SuperSuit-3.9.0/SuperSuit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-LICENSE.txt
+LICENSE
 README.md
+pyproject.toml
 setup.py
 SuperSuit.egg-info/PKG-INFO
 SuperSuit.egg-info/SOURCES.txt
 SuperSuit.egg-info/dependency_links.txt
 SuperSuit.egg-info/requires.txt
 SuperSuit.egg-info/top_level.txt
 supersuit/__init__.py
@@ -58,27 +59,8 @@
 supersuit/vector/sb3_vector_wrapper.py
 supersuit/vector/sb_vector_wrapper.py
 supersuit/vector/single_vec_env.py
 supersuit/vector/vector_constructors.py
 supersuit/vector/utils/__init__.py
 supersuit/vector/utils/shared_array.py
 supersuit/vector/utils/space_wrapper.py
-test/__init__.py
-test/aec_mock_test.py
-test/aec_unwrapped_test.py
-test/dummy_aec_env.py
-test/dummy_gym_env.py
-test/generated_agents_test.py
-test/gym_mock_test.py
-test/gym_unwrapped_test.py
-test/parallel_env_test.py
-test/pettingzoo_api_test.py
-test/test_autodep.py
-test/vec_env_test.py
-test/test_vector/__init__.py
-test/test_vector/test_aec_vector_identity_env.py
-test/test_vector/test_aec_vector_values.py
-test/test_vector/test_env_is_wrapped.py
-test/test_vector/test_gym_vector.py
-test/test_vector/test_pettingzoo_to_vec.py
-test/test_vector/test_render.py
-test/test_vector/test_vector_dict.py
+test/test_autodep.py
```

### Comparing `SuperSuit-3.8.1/supersuit/__init__.py` & `SuperSuit-3.9.0/supersuit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                     raise DeprecatedWrapper(
                         f"{base}{version_num} is now deprecated, use {base}{act_version_num} instead"
                     )
 
     raise ImportError(f"cannot import name '{wrapper_name}' from 'supersuit'")
 
 
-__version__ = "3.8.1"
+__version__ = "3.9.0"
```

### Comparing `SuperSuit-3.8.1/supersuit/aec_vector/async_vector_env.py` & `SuperSuit-3.9.0/supersuit/aec_vector/async_vector_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/aec_vector/base_aec_vec_env.py` & `SuperSuit-3.9.0/supersuit/aec_vector/base_aec_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/aec_vector/create.py` & `SuperSuit-3.9.0/supersuit/aec_vector/create.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/aec_vector/vector_env.py` & `SuperSuit-3.9.0/supersuit/aec_vector/vector_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/__init__.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/basic_wrappers.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/basic_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/delay_observations.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/delay_observations.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/frame_skip.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/frame_skip.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/frame_stack.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/frame_stack.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/max_observation.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/max_observation.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/nan_wrappers.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/nan_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/sticky_actions.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/sticky_actions.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/utils/base_modifier.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/utils/base_modifier.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/generic_wrappers/utils/shared_wrapper_util.py` & `SuperSuit-3.9.0/supersuit/generic_wrappers/utils/shared_wrapper_util.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/lambda_wrappers/action_lambda.py` & `SuperSuit-3.9.0/supersuit/lambda_wrappers/action_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/lambda_wrappers/observation_lambda.py` & `SuperSuit-3.9.0/supersuit/lambda_wrappers/observation_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/lambda_wrappers/reward_lambda.py` & `SuperSuit-3.9.0/supersuit/lambda_wrappers/reward_lambda.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/multiagent_wrappers/agent_indication.py` & `SuperSuit-3.9.0/supersuit/multiagent_wrappers/agent_indication.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/multiagent_wrappers/black_death.py` & `SuperSuit-3.9.0/supersuit/multiagent_wrappers/black_death.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/multiagent_wrappers/padding_wrappers.py` & `SuperSuit-3.9.0/supersuit/multiagent_wrappers/padding_wrappers.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/accumulator.py` & `SuperSuit-3.9.0/supersuit/utils/accumulator.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/action_transforms/homogenize_ops.py` & `SuperSuit-3.9.0/supersuit/utils/action_transforms/homogenize_ops.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/agent_indicator.py` & `SuperSuit-3.9.0/supersuit/utils/agent_indicator.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/base_aec_wrapper.py` & `SuperSuit-3.9.0/supersuit/utils/base_aec_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/basic_transforms/color_reduction.py` & `SuperSuit-3.9.0/supersuit/utils/basic_transforms/color_reduction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 
 from . import convert_box
 
+
 COLOR_RED_LIST = ["full", "R", "G", "B"]
 GRAYSCALE_WEIGHTS = np.array([0.299, 0.587, 0.114], dtype=np.float32)
 
 
 def check_param(space, color_reduction):
     assert isinstance(
         color_reduction, str
```

### Comparing `SuperSuit-3.8.1/supersuit/utils/basic_transforms/normalize_obs.py` & `SuperSuit-3.9.0/supersuit/utils/basic_transforms/normalize_obs.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/basic_transforms/reshape.py` & `SuperSuit-3.9.0/supersuit/utils/basic_transforms/reshape.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/basic_transforms/resize.py` & `SuperSuit-3.9.0/supersuit/utils/basic_transforms/resize.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/frame_skip.py` & `SuperSuit-3.9.0/supersuit/utils/frame_skip.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/frame_stack.py` & `SuperSuit-3.9.0/supersuit/utils/frame_stack.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/utils/wrapper_chooser.py` & `SuperSuit-3.9.0/supersuit/utils/wrapper_chooser.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/concat_vec_env.py` & `SuperSuit-3.9.0/supersuit/vector/concat_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/constructors.py` & `SuperSuit-3.9.0/supersuit/vector/constructors.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/markov_vector_wrapper.py` & `SuperSuit-3.9.0/supersuit/vector/markov_vector_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/multiproc_vec.py` & `SuperSuit-3.9.0/supersuit/vector/multiproc_vec.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,18 +177,17 @@
     def reset(self, seed=None, options=None):
         for i, pipe in enumerate(self.pipes):
             if seed is not None:
                 pipe.send(("reset", (seed + i, options)))
             else:
                 pipe.send(("reset", (seed, options)))
 
-        self._receive_info()
+        info = self._receive_info()
 
-        # TODO: should this include info
-        return numpy_deepcopy(self.observations_buffers)
+        return numpy_deepcopy(self.observations_buffers), copy.deepcopy(info)
 
     def step_async(self, actions):
         actions = list(iterate(self.action_space, actions))
         for i, pipe in enumerate(self.pipes):
             start, end = self.idx_starts[i : i + 2]
             pipe.send(("step", actions[start:end]))
```

### Comparing `SuperSuit-3.8.1/supersuit/vector/sb3_vector_wrapper.py` & `SuperSuit-3.9.0/supersuit/vector/sb3_vector_wrapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-from typing import Any, List
+import warnings
+from typing import Any, List, Optional
 
 import numpy as np
 from stable_baselines3.common.vec_env import VecEnvWrapper
 from stable_baselines3.common.vec_env.base_vec_env import VecEnvIndices
 
 
 class SB3VecEnvWrapper(VecEnvWrapper):
     def __init__(self, venv):
         self.venv = venv
         self.num_envs = venv.num_envs
         self.observation_space = venv.observation_space
         self.action_space = venv.action_space
-        # self.render_mode = venv.render_mode
+        self.reset_infos = []
 
     def reset(self, seed=None, options=None):
         if seed is not None:
             self.seed(seed=seed)
-        return self.venv.reset()
+        # Note: SB3's vector envs return only observations on reset, and store infos in `self.reset_infos`
+        observations, self.reset_infos = self.venv.reset()
+        return observations
 
     def step_wait(self):
         observations, rewards, terminations, truncations, infos = self.venv.step_wait()
         # Note: SB3 expects dones to be an np.array
         dones = np.array(
             [terminations[i] or truncations[i] for i in range(len(terminations))]
         )
@@ -39,7 +42,13 @@
     def get_attr(self, attr_name: str, indices: VecEnvIndices = None) -> List[Any]:
         attr = self.venv.get_attr(attr_name)
         # Note: SB3 expects render_mode to be returned as an array, with values for each env
         if attr_name == "render_mode":
             return [attr for _ in range(self.num_envs)]
         else:
             return attr
+
+    def render(self, mode: Optional[str] = None) -> Optional[np.ndarray]:
+        warnings.warn(
+            "PettingZoo environments do not take the `render(mode)` argument, to change rendering mode, re-initialize the environment using the `render_mode` argument."
+        )
+        return self.venv.render()
```

### Comparing `SuperSuit-3.8.1/supersuit/vector/sb_vector_wrapper.py` & `SuperSuit-3.9.0/supersuit/vector/sb_vector_wrapper.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/single_vec_env.py` & `SuperSuit-3.9.0/supersuit/vector/single_vec_env.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/utils/shared_array.py` & `SuperSuit-3.9.0/supersuit/vector/utils/shared_array.py`

 * *Files identical despite different names*

### Comparing `SuperSuit-3.8.1/supersuit/vector/vector_constructors.py` & `SuperSuit-3.9.0/supersuit/vector/vector_constructors.py`

 * *Files identical despite different names*

