# Comparing `tmp/Shimmy-1.2.0.tar.gz` & `tmp/Shimmy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimmy-1.2.0.tar", last modified: Fri Jul 21 01:30:36 2023, max compression
+gzip compressed data, was "Shimmy-1.2.1.tar", last modified: Fri Jul 21 06:25:07 2023, max compression
```

## Comparing `Shimmy-1.2.0.tar` & `Shimmy-1.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 01:30:36.896838 Shimmy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-21 01:30:27.000000 Shimmy-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.892838 Shimmy-1.2.0/Shimmy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 01:30:27.000000 Shimmy-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:30:36.896838 Shimmy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-21 01:30:27.000000 Shimmy-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/shimmy/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/atari_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/bsuite_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/dm_control_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/dm_control_multiagent_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/dm_lab_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/meltingpot_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/openai_gym_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/openspiel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/shimmy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/dm_control_multiagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/envs_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/meltingpot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_atari.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_bsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_dm_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_dm_control_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_meltingpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_openspiel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.895684 Shimmy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 06:25:07.895684 Shimmy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-21 06:24:58.000000 Shimmy-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.891684 Shimmy-1.2.1/Shimmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 06:24:58.000000 Shimmy-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:25:07.895684 Shimmy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-21 06:24:58.000000 Shimmy-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.891684 Shimmy-1.2.1/shimmy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/atari_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/bsuite_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/dm_control_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/dm_control_multiagent_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/dm_lab_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/meltingpot_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/openai_gym_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/openspiel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.895684 Shimmy-1.2.1/shimmy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/dm_control_multiagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/envs_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/meltingpot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.895684 Shimmy-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_atari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_bsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_dm_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_dm_control_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_meltingpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_openspiel.py
```

### Comparing `Shimmy-1.2.0/PKG-INFO` & `Shimmy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 1.2.0
+Version: 1.2.1
 Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Shimmy-1.2.0/README.md` & `Shimmy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/Shimmy.egg-info/PKG-INFO` & `Shimmy-1.2.1/Shimmy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Shimmy
-Version: 1.2.0
+Version: 1.2.1
 Summary: An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.
 Home-page: https://github.com/Farama-Foundation/Shimmy
 Author: Farama Foundation
 Author-email: contact@farama.org
 Keywords: Reinforcement Learning,game,RL,AI
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `Shimmy-1.2.0/Shimmy.egg-info/SOURCES.txt` & `Shimmy-1.2.1/Shimmy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/Shimmy.egg-info/requires.txt` & `Shimmy-1.2.1/Shimmy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/pyproject.toml` & `Shimmy-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/setup.py` & `Shimmy-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/__init__.py` & `Shimmy-1.2.1/shimmy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "DmLabCompatibilityV0",
     "GymV21CompatibilityV0",
     "GymV26CompatibilityV0",
     "MeltingPotCompatibilityV0",
 ]
 
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 
 try:
     import sys
 
     from farama_notifications import notifications
```

### Comparing `Shimmy-1.2.0/shimmy/atari_env.py` & `Shimmy-1.2.1/shimmy/atari_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/bsuite_compatibility.py` & `Shimmy-1.2.1/shimmy/bsuite_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/dm_control_compatibility.py` & `Shimmy-1.2.1/shimmy/dm_control_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/dm_control_multiagent_compatibility.py` & `Shimmy-1.2.1/shimmy/dm_control_multiagent_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/dm_lab_compatibility.py` & `Shimmy-1.2.1/shimmy/dm_lab_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/meltingpot_compatibility.py` & `Shimmy-1.2.1/shimmy/meltingpot_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/openai_gym_compatibility.py` & `Shimmy-1.2.1/shimmy/openai_gym_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/openspiel_compatibility.py` & `Shimmy-1.2.1/shimmy/openspiel_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/registration.py` & `Shimmy-1.2.1/shimmy/registration.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/utils/dm_control_multiagent.py` & `Shimmy-1.2.1/shimmy/utils/dm_control_multiagent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/utils/dm_env.py` & `Shimmy-1.2.1/shimmy/utils/dm_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/utils/dm_lab.py` & `Shimmy-1.2.1/shimmy/utils/dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/utils/envs_configs.py` & `Shimmy-1.2.1/shimmy/utils/envs_configs.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/shimmy/utils/meltingpot.py` & `Shimmy-1.2.1/shimmy/utils/meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_atari.py` & `Shimmy-1.2.1/tests/test_atari.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_bsuite.py` & `Shimmy-1.2.1/tests/test_bsuite.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_dm_control.py` & `Shimmy-1.2.1/tests/test_dm_control.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_dm_control_multi_agent.py` & `Shimmy-1.2.1/tests/test_dm_control_multi_agent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_dm_lab.py` & `Shimmy-1.2.1/tests/test_dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_gym.py` & `Shimmy-1.2.1/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_meltingpot.py` & `Shimmy-1.2.1/tests/test_meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.0/tests/test_openspiel.py` & `Shimmy-1.2.1/tests/test_openspiel.py`

 * *Files identical despite different names*

