# Comparing `tmp/Shimmy-1.1.0.tar.gz` & `tmp/Shimmy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimmy-1.1.0.tar", last modified: Thu Jun 15 22:38:22 2023, max compression
+gzip compressed data, was "Shimmy-1.2.0.tar", last modified: Fri Jul 21 01:30:36 2023, max compression
```

## Comparing `Shimmy-1.1.0.tar` & `Shimmy-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.037121 Shimmy-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 22:38:22.037121 Shimmy-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-06-15 22:38:18.000000 Shimmy-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.033121 Shimmy-1.1.0/Shimmy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-15 22:38:22.000000 Shimmy-1.1.0/Shimmy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 22:38:18.000000 Shimmy-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 22:38:22.037121 Shimmy-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-15 22:38:18.000000 Shimmy-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.033121 Shimmy-1.1.0/shimmy/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/atari_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/bsuite_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/dm_control_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/dm_control_multiagent_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/dm_lab_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/meltingpot_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/openai_gym_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/openspiel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.037121 Shimmy-1.1.0/shimmy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/dm_control_multiagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/envs_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-15 22:38:18.000000 Shimmy-1.1.0/shimmy/utils/meltingpot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 22:38:22.037121 Shimmy-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_atari.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_bsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_dm_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_dm_control_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_meltingpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-06-15 22:38:18.000000 Shimmy-1.1.0/tests/test_openspiel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 01:30:36.896838 Shimmy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-21 01:30:27.000000 Shimmy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.892838 Shimmy-1.2.0/Shimmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 01:30:36.000000 Shimmy-1.2.0/Shimmy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 01:30:27.000000 Shimmy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:30:36.896838 Shimmy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-21 01:30:27.000000 Shimmy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/shimmy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/atari_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/bsuite_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/dm_control_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/dm_control_multiagent_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/dm_lab_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/meltingpot_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/openai_gym_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/openspiel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/shimmy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/dm_control_multiagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/envs_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 01:30:27.000000 Shimmy-1.2.0/shimmy/utils/meltingpot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:30:36.896838 Shimmy-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_atari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_bsuite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_dm_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_dm_control_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_meltingpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-21 01:30:27.000000 Shimmy-1.2.0/tests/test_openspiel.py
```

### Comparing `Shimmy-1.1.0/README.md` & `Shimmy-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8140744.svg)](https://doi.org/10.5281/zenodo.8140744)
+
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Shimmy/main/shimmy-text.png" width="500px"/>
 </p>
 
 Shimmy is an API conversion tool providing [Gymnasium](https://github.com/farama-Foundation/gymnasium) and [PettingZoo](https://github.com/farama-Foundation/pettingZoo/) bindings for popular external reinforcement learning environments.
 
 The documentation website is at [shimmy.farama.org](https://shimmy.farama.org/) and we have a public discord server (which we also use to coordinate development work) that you can join here: https://discord.gg/nhvKkYa6qX
@@ -11,15 +13,15 @@
 ### [OpenAI Gym](http://shimmy.farama.org/contents/gym/)
 - Bindings to convert [OpenAI Gym](https://github.com/openai/gym) environments to [Gymnasium](https://gymnasium.farama.org/).
 
 ### [Atari Environments for OpenAI Gym](http://shimmy.farama.org/contents/atari/)
 - Bindings to convert [ALE-py](https://github.com/mgbellemare/Arcade-Learning-Environment) Atari environments to [Gymnasium](https://gymnasium.farama.org/).
 
 ### [DeepMind Control](http://shimmy.farama.org/contents/dm_control/)
-- Bindings to convert [DM Control](https://github.com/deepmind/dm_control/) environments to [Gymnasium](https://gymnasium.farama.org/). 
+- Bindings to convert [DM Control](https://github.com/deepmind/dm_control/) environments to [Gymnasium](https://gymnasium.farama.org/).
 
 ### [DeepMind Control: Multi-Agent](http://shimmy.farama.org/contents/dm_multi/)
 - Bindings to convert [DM Control Soccer](https://github.com/deepmind/dm_control/blob/main/dm_control/locomotion/soccer/README.md) environments to [PettingZoo](https://pettingzoo.farama.org/).
 
 ### [DMLab](http://shimmy.farama.org/contents/dm_lab/)
 - Bindings to convert [DM Lab](https://github.com/deepmind/lab) environments to [PettingZoo](https://pettingzoo.farama.org/).
 
@@ -90,15 +92,21 @@
 
 Maintenance for this project is also contributed by the broader Farama team: [farama.org/team](https://farama.org/team).
 
 ## Citation
 
 If you use Shimmy in your research, please cite:
 ```
-@software{shimmy2022github,
-  author = {{Jun Jet Tai, Mark Towers, Elliot Tower} and Jordan Terry},
-  title = {Shimmy: Gymnasium and PettingZoo Wrappers for Commonly Used Environments},
-  url = {https://github.com/Farama-Foundation/Shimmy},
-  version = {1.0.0},
-  year = {2022},
+@software{jun_jet_tai_2023_8140744,
+  author       = {Jun Jet Tai and
+                  Mark Towers and
+                  Elliot Tower},
+  title        = {{Shimmy: Gymnasium and PettingZoo Wrappers for
+                   Commonly Used Environments}},
+  month        = jun,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v1.1.0},
+  doi          = {10.5281/zenodo.8140744},
+  url          = {https://doi.org/10.5281/zenodo.8140744}
 }
 ```
```

### Comparing `Shimmy-1.1.0/Shimmy.egg-info/SOURCES.txt` & `Shimmy-1.2.0/Shimmy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/Shimmy.egg-info/requires.txt` & `Shimmy-1.2.0/Shimmy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/pyproject.toml` & `Shimmy-1.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ]
 
 strict = [
 
 ]
 
 typeCheckingMode = "basic"
-pythonVersion = "3.7"
+pythonVersion = "3.8"
 pythonPlatform = "All"
 enableTypeIgnoreComments = true
 # This is required as the CI pre-commit does not download the module (i.e. numpy, pygame, box2d)
 #   Therefore, we have to ignore missing imports
 reportMissingImports = "none"
 # Some modules are missing type stubs, which is an issue when running pyright locally
 reportMissingTypeStubs = false
```

### Comparing `Shimmy-1.1.0/setup.py` & `Shimmy-1.2.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -65,21 +65,20 @@
     author_email="contact@farama.org",
     description="An API conversion tool providing Gymnasium and PettingZoo bindings for popular external reinforcement learning environments.",
     url="https://github.com/Farama-Foundation/Shimmy",
     license_files=("LICENSE.txt",),
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["Reinforcement Learning", "game", "RL", "AI"],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     packages=find_packages(),
     install_requires=["numpy>=1.18.0", "gymnasium>=0.27.0"],
     tests_require=extras["testing"],
     extras_require=extras,
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `Shimmy-1.1.0/shimmy/__init__.py` & `Shimmy-1.2.0/shimmy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "DmLabCompatibilityV0",
     "GymV21CompatibilityV0",
     "GymV26CompatibilityV0",
     "MeltingPotCompatibilityV0",
 ]
 
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 
 try:
     import sys
 
     from farama_notifications import notifications
```

### Comparing `Shimmy-1.1.0/shimmy/atari_env.py` & `Shimmy-1.2.0/shimmy/atari_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/bsuite_compatibility.py` & `Shimmy-1.2.0/shimmy/bsuite_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/dm_control_compatibility.py` & `Shimmy-1.2.0/shimmy/dm_control_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/dm_control_multiagent_compatibility.py` & `Shimmy-1.2.0/shimmy/dm_control_multiagent_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/dm_lab_compatibility.py` & `Shimmy-1.2.0/shimmy/dm_lab_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/meltingpot_compatibility.py` & `Shimmy-1.2.0/shimmy/meltingpot_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/openai_gym_compatibility.py` & `Shimmy-1.2.0/shimmy/openai_gym_compatibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Compatibility wrappers for OpenAI gym V21 and V26."""
 # pyright: reportGeneralTypeIssues=false, reportPrivateImportUsage=false
 from __future__ import annotations
 
 import sys
-from typing import Any
+from typing import Any, Protocol, runtime_checkable
 
 import gymnasium
 from gymnasium import error
 from gymnasium.core import ActType, ObsType
 from gymnasium.error import MissingArgument
 from gymnasium.logger import warn
 from gymnasium.spaces import (
@@ -21,20 +21,14 @@
     Text,
     Tuple,
 )
 from gymnasium.utils.step_api_compatibility import (
     convert_to_terminated_truncated_step_api,
 )
 
-if sys.version_info >= (3, 8):
-    from typing import Protocol, runtime_checkable
-else:
-    from typing_extensions import Protocol, runtime_checkable
-
-
 try:
     import gym
     import gym.wrappers
 except ImportError as e:
     GYM_IMPORT_ERROR = e
 else:
     GYM_IMPORT_ERROR = None
```

### Comparing `Shimmy-1.1.0/shimmy/openspiel_compatibility.py` & `Shimmy-1.2.0/shimmy/openspiel_compatibility.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+# pyright: reportGeneralTypeIssues=false
 """Wrapper to convert an OpenSpiel environment into a pettingzoo compatible environment."""
 from __future__ import annotations
 
-import functools
 import string
 from typing import Any, Dict, Optional
 
 import numpy as np
 import pettingzoo as pz
 import pyspiel
 from gymnasium import spaces
 from gymnasium.utils import EzPickle, seeding
-from pettingzoo.utils.env import AgentID, ObsType
+from pettingzoo.utils.env import AgentID
 
 
 class OpenSpielCompatibilityV0(pz.AECEnv, EzPickle):
     """This compatibility wrapper converts an OpenSpiel environment into a PettingZoo environment.
 
     OpenSpiel is a collection of environments and algorithms for research in general reinforcement learning
     and search/planning in games. OpenSpiel supports n-player (single- and multi- agent) zero-sum,
@@ -30,113 +30,138 @@
     }
 
     def __init__(
         self,
         env: pyspiel.Game | None = None,
         game_name: str | None = None,
         render_mode: str | None = None,
+        config: dict | None = None,
     ):
         """Wrapper to convert a OpenSpiel environment into a PettingZoo environment.
 
         Args:
             env (Optional[pyspiel.Game]): existing OpenSpiel environment to wrap
             game_name (Optional[str]): name of OpenSpiel game to load
             render_mode (Optional[str]): rendering mode
+            config (Optional[dict]): PySpiel config
         """
         EzPickle.__init__(self, env, game_name, render_mode)
         super().__init__()
 
+        self.config = config
+
         # Only one of game_name and env can be provided, the other should be None
         if env is None and game_name is None:
             raise ValueError(
                 "No environment provided. Use `env` to specify an existing environment, or load an environment with `game_name`."
             )
         elif env is not None and game_name is not None:
             raise ValueError(
                 "Two environments provided. Use `env` to specify an existing environment, or load an environment with `game_name`."
             )
         elif game_name is not None:
-            self._env = pyspiel.load_game(game_name)
+            if self.config is not None:
+                self._env = pyspiel.load_game(game_name, self.config)
+            else:
+                self._env = pyspiel.load_game(game_name)
         elif env is not None:
             self._env = env
 
         self.possible_agents = [
             "player_" + str(r) for r in range(self._env.num_players())
         ]
         self.agent_id_name_mapping = dict(
             zip(range(self._env.num_players()), self.possible_agents)
         )
         self.agent_name_id_mapping = dict(
             zip(self.possible_agents, range(self._env.num_players()))
         )
+        self.agent_ids = [self.agent_name_id_mapping[a] for a in self.possible_agents]
 
         self.game_type = self._env.get_type()
         self.game_name = self.game_type.short_name
 
+        self.observation_spaces = {}
+        self.action_spaces = {}
+
+        self._update_observation_spaces()
+        self._update_action_spaces()
+
         self.render_mode = render_mode
 
-    @functools.lru_cache(maxsize=None)
+    def _update_observation_spaces(self):
+        for agent in self.possible_agents:
+            if self.game_type.provides_observation_tensor:
+                self.observation_spaces[agent] = spaces.Box(
+                    low=-np.inf,
+                    high=np.inf,
+                    shape=self._env.observation_tensor_shape(),
+                    dtype=np.float64,
+                )
+            elif self.game_type.provides_information_state_tensor:
+                self.observation_spaces[agent] = spaces.Box(
+                    low=-np.inf,
+                    high=np.inf,
+                    shape=self._env.information_state_tensor_shape(),
+                    dtype=np.float64,
+                )
+            elif (
+                self.game_type.provides_information_state_string
+                or self.game_type.provides_observation_string
+            ):
+                self.observation_spaces[agent] = spaces.Text(
+                    min_length=0, max_length=2**16, charset=string.printable
+                )
+            else:
+                raise NotImplementedError(
+                    f"No information/observation tensor/string implemented for {self._env}."
+                )
+
+    def _update_action_spaces(self):
+        for agent in self.possible_agents:
+            try:
+                self.action_spaces[agent] = spaces.Discrete(
+                    self._env.num_distinct_actions()
+                )
+            except pyspiel.SpielError as e:
+                raise NotImplementedError(
+                    f"{str(e)[:-1]} for action space for {self._env}."
+                )
+
     def observation_space(self, agent: AgentID):
         """observation_space.
 
         We get the observation space from the underlying game.
         OpenSpiel possibly provides information and observation in several forms.
         This wrapper chooses which one to use depending on the following precedence:
         1. Observation Tensor
         2. Information Tensor
         3. Observation String
         4. Information String
 
         Args:
             agent (AgentID): agent
+        Returns:
+            space (gymnasium.spaces.Space): observation space for the specified agent
+
         """
-        if self.game_type.provides_observation_tensor:
-            return spaces.Box(
-                low=-np.inf,
-                high=np.inf,
-                shape=self._env.observation_tensor_shape(),
-                dtype=np.float64,
-            )
-        elif self.game_type.provides_information_state_tensor:
-            return spaces.Box(
-                low=-np.inf,
-                high=np.inf,
-                shape=self._env.information_state_tensor_shape(),
-                dtype=np.float64,
-            )
-        elif (
-            self.game_type.provides_information_state_string
-            or self.game_type.provides_observation_string
-        ):
-            return spaces.Text(
-                min_length=0, max_length=2**16, charset=string.printable
-            )
-        else:
-            raise NotImplementedError(
-                f"No information/observation tensor/string implemented for {self._env}."
-            )
+        return self.observation_spaces[agent]
 
-    @functools.lru_cache(maxsize=None)
     def action_space(self, agent: AgentID):
         """action_space.
 
         Get the action space from the underlying OpenSpiel game.
 
         Args:
             agent (AgentID): agent
 
         Returns:
-            space
+            space (gymnasium.spaces.Space): action space for the specified agent
         """
-        try:
-            return spaces.Discrete(self._env.num_distinct_actions())
-        except pyspiel.SpielError as e:
-            raise NotImplementedError(
-                f"{str(e)[:-1]} for action space for {self._env}."
-            )
+        return self.action_spaces[agent]
 
     def render(self):
         """render.
 
         Print the current game state.
         """
         if not hasattr(self, "game_state"):
@@ -149,15 +174,15 @@
     def observe(self, agent: AgentID) -> Any:
         """observe.
 
         Args:
             agent (AgentID): agent
 
         Returns:
-            observation
+            observation (Any)
         """
         return self.observations[agent]
 
     def close(self):
         """close."""
         pass
 
@@ -171,22 +196,32 @@
         Args:
             seed (Optional[int]): seed
             options (Optional[Dict]): options
         """
         # initialize np random the seed
         self.np_random, self.np_seed = seeding.np_random(seed)
 
+        self.game_name = self.game_type.short_name
+
         # seed argument is only valid for three games
         if self.game_name in ["deep_sea", "hanabi", "mfg_garnet"] and seed is not None:
-            self.game_name = self.game_type.short_name
-            self._env = pyspiel.load_game(self.game_name, {"seed": seed})
+            if self.config is not None:
+                reset_config = self.config.copy()
+                reset_config["seed"] = seed
+            else:
+                reset_config = {"seed": seed}
+            self._env = pyspiel.load_game(self.game_name, reset_config)
+        else:
+            if self.config is not None:
+                self._env = pyspiel.load_game(self.game_name, self.config)
+            else:
+                self._env = pyspiel.load_game(self.game_name)
 
         # all agents
         self.agents = self.possible_agents[:]
-        self.agent_ids = [self.agent_name_id_mapping[a] for a in self.agents]
 
         # boilerplate stuff
         self._cumulative_rewards = {a: 0.0 for a in self.agents}
         self.rewards = {a: 0.0 for a in self.agents}
         self.terminations = {a: False for a in self.agents}
         self.truncations = {a: False for a in self.agents}
         self.infos = {a: {} for a in self.agents}
@@ -194,14 +229,18 @@
         # get a new game state, game_length = number of game nodes
         self.game_length = 1
         self.game_state = self._env.new_initial_state()
 
         # holders in case of simultaneous actions
         self.simultaneous_actions = dict()
 
+        # make sure observation and action spaces are correct for this environment config
+        self._update_observation_spaces()
+        self._update_action_spaces()
+
         # step through chance nodes
         # then update obs and act masks
         # then choose next agent
         self._execute_chance_node()
         self._update_action_masks()
         self._update_observations()
         self._choose_next_agent()
@@ -299,45 +338,45 @@
     def _update_observations(self):
         """Updates all the observations inside the observations dictionary."""
         if self.game_state.is_terminal():
             return
 
         if self.game_type.provides_observation_tensor:
             self.observations = {
-                self.agents[a]: np.array(self.game_state.observation_tensor(a)).reshape(
-                    self.observation_space(self.agents[0]).shape
+                self.agents[i]: np.array(self.game_state.observation_tensor(i)).reshape(
+                    self.observation_space(self.agents[i]).shape
                 )
-                for a in self.agent_ids
+                for i in self.agent_ids
             }
         elif self.game_type.provides_information_state_tensor:
             self.observations = {
-                self.agents[a]: np.array(
-                    self.game_state.information_state_tensor(a)
-                ).reshape(self.observation_space(self.agents[0]).shape)
-                for a in self.agent_ids
+                self.agents[i]: np.array(
+                    self.game_state.information_state_tensor(i)
+                ).reshape(self.observation_space(self.agents[i]).shape)
+                for i in self.agent_ids
             }
         elif self.game_type.provides_observation_string:
             self.observations = {
-                self.agents[a]: self.game_state.observation_string(a)
-                for a in self.agent_ids
+                self.agents[i]: self.game_state.observation_string(i)
+                for i in self.agent_ids
             }
         elif self.game_type.provides_information_state_string:
             self.observations = {
-                self.agents[a]: self.game_state.information_state_string(a)
-                for a in self.agent_ids
+                self.agents[i]: self.game_state.information_state_string(i)
+                for i in self.agent_ids
             }
         else:
             raise NotImplementedError(
                 f"No information/observation tensor/string implemented for {self._env}."
             )
 
     def _update_action_masks(self):
         """Updates all the action masks inside the infos dictionary."""
         for agent_id, agent_name in zip(self.agent_ids, self.agents):
-            action_mask = np.zeros(self.action_space(agent_name).n, dtype=np.int8)
+            action_mask = np.zeros(self._env.num_distinct_actions(), dtype=np.int8)
             action_mask[self.game_state.legal_actions(agent_id)] = 1
 
             self.infos[agent_name] = {"action_mask": action_mask}
 
     def _update_rewards(self):
         """Updates all the _cumulative_rewards of the environment."""
         # retrieve rewards
@@ -394,14 +433,18 @@
             action (int): action
         """
         # reset the cumulative rewards for the current agent
         self._cumulative_rewards[self.agent_selection] = 0.0
 
         # handle the possibility of an end step
         if not self._end_routine():
+            # ensure observation and action spaces are up-to-date with the underlying environment
+            self._update_observation_spaces()
+            self._update_action_spaces()
+
             # step the environment
             self._execute_action_node(action)
             self._execute_chance_node()
             self._update_action_masks()
             self._update_observations()
             self._update_rewards()
             self._update_termination_truncation()
```

### Comparing `Shimmy-1.1.0/shimmy/registration.py` & `Shimmy-1.2.0/shimmy/registration.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/utils/dm_control_multiagent.py` & `Shimmy-1.2.0/shimmy/utils/dm_control_multiagent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/utils/dm_env.py` & `Shimmy-1.2.0/shimmy/utils/dm_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/utils/dm_lab.py` & `Shimmy-1.2.0/shimmy/utils/dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/utils/envs_configs.py` & `Shimmy-1.2.0/shimmy/utils/envs_configs.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/shimmy/utils/meltingpot.py` & `Shimmy-1.2.0/shimmy/utils/meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/tests/test_atari.py` & `Shimmy-1.2.0/tests/test_atari.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/tests/test_bsuite.py` & `Shimmy-1.2.0/tests/test_bsuite.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/tests/test_dm_control.py` & `Shimmy-1.2.0/tests/test_dm_control.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,19 +50,24 @@
         "A Box observation space has an unconventional shape (neither an image, nor a 1D vector). We recommend flattening the observation to have only a 1D vector or use a custom policy to properly process the data. Actual observation shape: (1, 6)",
         "A Box observation space has an unconventional shape (neither an image, nor a 1D vector). We recommend flattening the observation to have only a 1D vector or use a custom policy to properly process the data. Actual observation shape: (1, 4)",
         "A Box observation space has an unconventional shape (neither an image, nor a 1D vector). We recommend flattening the observation to have only a 1D vector or use a custom policy to properly process the data. Actual observation shape: (1, 9)",
         "A Box observation space has an unconventional shape (neither an image, nor a 1D vector). We recommend flattening the observation to have only a 1D vector or use a custom policy to properly process the data. Actual observation shape: (1, 5)",
         "It seems a Box observation space is an image but the `dtype` is not `np.uint8`, actual type: float64. If the Box observation space is not an image, we recommend flattening the observation to have only a 1D vector.",
         "It seems a Box observation space is an image but the upper and lower bounds are not in [0, 255]. Generally, CNN policies assume observations are within that range, so you may encounter an issue if the observation values are not.",
         "arrays to stack must be passed as a 'sequence' type such as list or tuple. Support for non-sequence iterables such as generators is deprecated as of NumPy 1.16 and will raise an error in the future.",
+        "Calling `env.close()` on the closed environment should be allowed, but it raised an exception: _data",
+        "Calling `env.close()` on the closed environment should be allowed, but it raised an exception: 'Physics' object has no attribute '_data'",
     ]
 ]
 CHECK_ENV_IGNORE_WARNINGS.append(
     'arrays to stack must be passed as a "sequence" type such as list or tuple. Support for non-sequence iterables such as generators is deprecated as of NumPy 1.16 and will raise an error in the future.',
 )
+CHECK_ENV_IGNORE_WARNINGS.append(
+    "Conversion of an array with ndim > 0 to a scalar is deprecated, and will error in future. Ensure you extract a single element from your array before performing this operation. (Deprecated NumPy 1.25.)"
+)
 
 
 @pytest.mark.parametrize("env_id", DM_CONTROL_ENV_IDS)
 def test_check_env(env_id):
     """Check that environment pass the gymnasium check_env."""
     env = gym.make(env_id, disable_env_checker=True)
 
@@ -206,14 +211,17 @@
     frame = env.render()
     assert isinstance(frame, np.ndarray)
     assert frame.shape == (height, width, 3), frame.shape
 
     env.close()
 
 
+@pytest.mark.skip(
+    reason="This test is currently broken due to an issue with DM control and Gymnasium v29."
+)
 @pytest.mark.parametrize(
     "wrapper_fn",
     (
         action_noise.Wrapper,
         lambda x: action_scale.Wrapper(x, minimum=0, maximum=1),
         mujoco_profiling.Wrapper,
         pixels.Wrapper,
```

### Comparing `Shimmy-1.1.0/tests/test_dm_control_multi_agent.py` & `Shimmy-1.2.0/tests/test_dm_control_multi_agent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/tests/test_dm_lab.py` & `Shimmy-1.2.0/tests/test_dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/tests/test_gym.py` & `Shimmy-1.2.0/tests/test_gym.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 CHECK_ENV_IGNORE_WARNINGS = [
     f"\x1b[33mWARN: {message}\x1b[0m"
     for message in [
         "This version of the mujoco environments depends on the mujoco-py bindings, which are no longer maintained and may stop working. Please upgrade to the v4 versions of the environments (which depend on the mujoco python bindings instead), unless you are trying to precisely replicate previous works).",
         "A Box observation space minimum value is -infinity. This is probably too low.",
         "A Box observation space maximum value is -infinity. This is probably too high.",
         "For Box action spaces, we recommend using a symmetric and normalized space (range=[-1, 1] or [0, 1]). See https://stable-baselines3.readthedocs.io/en/master/guide/rl_tips.html for more information.",
+        "The environment CartPole-v0 is out of date. You should consider upgrading to version `v1`.",
     ]
 ]
 CHECK_ENV_IGNORE_WARNINGS.append(
     "`np.bool8` is a deprecated alias for `np.bool_`.  (Deprecated NumPy 1.24)"
 )
 
 # We do not test Atari environment's here because we check all variants of Pong in test_envs.py (There are too many Atari environments)
```

### Comparing `Shimmy-1.1.0/tests/test_meltingpot.py` & `Shimmy-1.2.0/tests/test_meltingpot.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.1.0/tests/test_openspiel.py` & `Shimmy-1.2.0/tests/test_openspiel.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,33 +89,31 @@
     "tiny_bridge_4p",
     "tiny_hanabi",
     "trade_comm",
     "ultimate_tic_tac_toe",
     "universal_poker",
     "y",
     "mfg_dynamic_routing",
-]
-
-_SOMETIMES_FAILING_GAMES = [
     "backgammon",
     "solitaire",
 ]
 
-_FAILING_GAMES = [
+# See https://github.com/deepmind/open_spiel/blob/efa004d8c5f5088224e49fdc198c5d74b6b600d0/open_spiel/python/tests/pyspiel_test.py#L162
+_NON_DEFAULT_LOADABLE_GAMES = [
+    "add_noise",
     "efg_game",
-    "misere",
+    "nfg_game" "misere",
+    "turn_based_simultaneous_game",
     "normal_form_extensive_game",
     "repeated_game",
     "restricted_nash_response",
     "start_at",
-    "turn_based_simultaneous_game",
+    "zerosum",
 ]
 
-_UNKNOWN_BUGS_GAMES = ["nfg_game"]
-
 
 @pytest.mark.parametrize("game_name", _PASSING_GAMES)
 def test_passing_games(game_name):
     """Tests the conversion of all OpenSpiel environments using the OpenSpielCompatibility wrapper."""
     for _ in range(5):
         env = pyspiel.load_game(game_name)
         env = OpenSpielCompatibilityV0(env=env, render_mode=None)
@@ -127,19 +125,23 @@
         env.reset()
         for agent in env.agent_iter():
             observation, reward, termination, truncation, info = env.last()
             action = env.action_space(agent).sample(mask=info["action_mask"])
             env.step(action)
 
 
-@pytest.mark.parametrize("game_name", _FAILING_GAMES)
+@pytest.mark.parametrize("game_name", _NON_DEFAULT_LOADABLE_GAMES)
 def test_failing_games(game_name):
     """Ensures that failing OpenSpiel games are still failing."""
     with pytest.raises(pyspiel.SpielError):
-        test_passing_games(game_name)
+        if game_name == "nfg_game":
+            with pytest.raises(IndexError):
+                test_passing_games(game_name)
+        else:
+            test_passing_games(game_name)
 
 
 @pytest.mark.parametrize("game_name", _PASSING_GAMES)
 def test_loading_env(game_name):
     """Tests the loading of all OpenSpiel environments using the OpenSpielCompatibility wrapper."""
     env = OpenSpielCompatibilityV0(game_name=game_name, render_mode=None)
```

