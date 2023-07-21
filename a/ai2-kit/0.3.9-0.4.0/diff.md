# Comparing `tmp/ai2_kit-0.3.9.tar.gz` & `tmp/ai2_kit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.3.9.tar", max compression
+gzip compressed data, was "ai2_kit-0.4.0.tar", max compression
```

## Comparing `ai2_kit-0.3.9.tar` & `ai2_kit-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,79 @@
--rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.3.9/LICENSE
--rw-r--r--   0        0        0     1962 2023-06-28 08:45:40.481907 ai2_kit-0.3.9/README.md
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/algorithm/__init__.py
--rw-r--r--   0        0        0    12100 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/algorithm/proton_transfer.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0     1854 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     5465 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/cmd.py
--rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     7939 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/executor.py
--rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.3.9/ai2_kit/core/future.py
--rw-r--r--   0        0        0     1991 2023-06-28 09:20:35.201482 ai2_kit-0.3.9/ai2_kit/core/job.py
--rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/core/log.py
--rw-r--r--   0        0        0     9449 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2572 2023-06-28 06:44:38.463386 ai2_kit-0.3.9/ai2_kit/core/resource_manager.py
--rw-r--r--   0        0        0     2358 2023-06-19 08:54:25.567391 ai2_kit-0.3.9/ai2_kit/core/script.py
--rw-r--r--   0        0        0     4195 2023-06-28 08:04:13.892405 ai2_kit-0.3.9/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/dflow/__init__.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0     1734 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/domain/cll.py
--rw-r--r--   0        0        0      381 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     8210 2023-06-28 08:04:13.892405 ai2_kit-0.3.9/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     4424 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/data_helper.py
--rw-r--r--   0        0        0     7169 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    16845 2023-06-28 08:04:13.892405 ai2_kit-0.3.9/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     3039 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      183 2023-06-28 03:52:57.155461 ai2_kit-0.3.9/ai2_kit/domain/updater.py
--rw-r--r--   0        0        0     9346 2023-06-28 02:30:53.156473 ai2_kit-0.3.9/ai2_kit/domain/vasp.py
--rw-r--r--   0        0        0     1588 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/tool/__init__.py
--rw-r--r--   0        0        0     1039 2023-06-28 08:16:01.942257 ai2_kit-0.3.9/ai2_kit/tool/ase.py
--rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.3.9/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     9230 2023-06-28 03:52:57.155461 ai2_kit-0.3.9/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     9117 2023-06-28 01:16:35.067371 ai2_kit-0.3.9/ai2_kit/workflow/fep_mlp.py
--rw-r--r--   0        0        0      843 2023-06-28 09:21:11.211476 ai2_kit-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     2989 1970-01-01 00:00:00.000000 ai2_kit-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1962 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.057371 ai2_kit-0.4.0/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0      144 2023-06-15 02:12:13.145370 ai2_kit-0.4.0/ai2_kit/algorithm/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     9573 2023-06-15 02:12:13.155370 ai2_kit-0.4.0/ai2_kit/algorithm/__pycache__/proton_transfer.cpython-39.pyc
+-rw-r--r--   0        0        0    14221 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0      139 2023-02-14 03:43:41.260120 ai2_kit-0.4.0/ai2_kit/core/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2243 2023-07-20 03:31:49.016223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/artifact.cpython-39.pyc
+-rw-r--r--   0        0        0     5928 2023-07-20 03:31:48.996223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/checkpoint.cpython-39.pyc
+-rw-r--r--   0        0        0      512 2023-06-15 07:55:24.192005 ai2_kit-0.4.0/ai2_kit/core/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     7307 2023-02-14 03:43:41.330120 ai2_kit-0.4.0/ai2_kit/core/__pycache__/connector.cpython-39.pyc
+-rw-r--r--   0        0        0     9582 2023-07-20 03:31:48.646223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/executor.cpython-39.pyc
+-rw-r--r--   0        0        0      894 2023-06-29 05:30:14.695752 ai2_kit-0.4.0/ai2_kit/core/__pycache__/future.cpython-39.pyc
+-rw-r--r--   0        0        0     2847 2023-07-20 03:31:48.996223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/job.cpython-39.pyc
+-rw-r--r--   0        0        0      436 2023-06-29 05:30:14.695752 ai2_kit-0.4.0/ai2_kit/core/__pycache__/log.cpython-39.pyc
+-rw-r--r--   0        0        0    10069 2023-07-20 07:05:10.973356 ai2_kit-0.4.0/ai2_kit/core/__pycache__/queue_system.cpython-39.pyc
+-rw-r--r--   0        0        0     3063 2023-07-20 03:31:49.026223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/resource_manager.cpython-39.pyc
+-rw-r--r--   0        0        0     2611 2023-07-20 03:31:49.026223 ai2_kit-0.4.0/ai2_kit/core/__pycache__/script.cpython-39.pyc
+-rw-r--r--   0        0        0     6829 2023-07-19 08:28:35.806120 ai2_kit-0.4.0/ai2_kit/core/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     1854 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     5745 2023-07-10 01:27:05.779682 ai2_kit-0.4.0/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-28 01:16:35.057371 ai2_kit-0.4.0/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7939 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0      365 2023-06-28 01:16:35.057371 ai2_kit-0.4.0/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     1991 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      298 2023-06-28 01:16:35.067371 ai2_kit-0.4.0/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     9587 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2572 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2363 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     5050 2023-07-18 07:59:30.544857 ai2_kit-0.4.0/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.4.0/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0      110 2023-06-15 07:55:24.202005 ai2_kit-0.4.0/ai2_kit/dflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0      141 2023-02-14 03:43:41.670121 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     4374 2023-07-19 08:29:57.336102 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/asap.cpython-39.pyc
+-rw-r--r--   0        0        0     2517 2023-06-29 05:30:14.805753 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/cll.cpython-39.pyc
+-rw-r--r--   0        0        0     3221 2023-02-23 07:10:20.489990 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0        0        0     1430 2023-07-19 08:30:00.906101 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/constant.cpython-39.pyc
+-rw-r--r--   0        0        0     5609 2023-07-21 01:23:26.304847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/cp2k.cpython-39.pyc
+-rw-r--r--   0        0        0     5983 2023-07-21 01:23:26.104847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0        0        0     6200 2023-06-27 02:27:16.171507 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/data_helper.cpython-39.pyc
+-rw-r--r--   0        0        0     6358 2023-07-21 01:23:26.094847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/deepmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2519 2023-07-20 03:31:49.026223 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/iface.cpython-39.pyc
+-rw-r--r--   0        0        0    12264 2023-07-21 01:23:26.164847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/lammps.cpython-39.pyc
+-rw-r--r--   0        0        0     9313 2023-07-21 01:23:26.174847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/lasp.cpython-39.pyc
+-rw-r--r--   0        0        0     3599 2023-07-21 01:23:26.174847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/selector.cpython-39.pyc
+-rw-r--r--   0        0        0      538 2023-07-21 01:23:26.544847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/updater.cpython-39.pyc
+-rw-r--r--   0        0        0     3360 2023-07-20 03:31:49.356223 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/util.cpython-39.pyc
+-rw-r--r--   0        0        0     6463 2023-07-21 01:23:26.304847 ai2_kit-0.4.0/ai2_kit/domain/__pycache__/vasp.cpython-39.pyc
+-rw-r--r--   0        0        0     5276 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/asap.py
+-rw-r--r--   0        0        0     1650 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     6585 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     6679 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/data.py
+-rw-r--r--   0        0        0     7895 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0     1121 2023-07-06 07:55:32.160324 ai2_kit-0.4.0/ai2_kit/domain/iface.py
+-rw-r--r--   0        0        0    17292 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     9028 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/lasp.py
+-rw-r--r--   0        0        0     3778 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      186 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0     6882 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/domain/util.py
+-rw-r--r--   0        0        0     7678 2023-07-21 01:27:23.144801 ai2_kit-0.4.0/ai2_kit/domain/vasp.py
+-rw-r--r--   0        0        0     1900 2023-07-06 07:55:32.150324 ai2_kit-0.4.0/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-28 01:16:35.067371 ai2_kit-0.4.0/ai2_kit/tool/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-28 08:15:51.392260 ai2_kit-0.4.0/ai2_kit/tool/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1616 2023-06-28 08:15:51.392260 ai2_kit-0.4.0/ai2_kit/tool/__pycache__/ase.cpython-39.pyc
+-rw-r--r--   0        0        0     1039 2023-07-07 01:23:16.068582 ai2_kit-0.4.0/ai2_kit/tool/ase.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.4.0/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-14 03:43:41.260120 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7915 2023-07-21 01:23:25.924847 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/cll_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0     5996 2023-06-15 08:55:37.729603 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/ec_fep.cpython-39.pyc
+-rw-r--r--   0        0        0     5966 2023-02-14 03:43:41.260120 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/fep.cpython-39.pyc
+-rw-r--r--   0        0        0     6336 2023-07-20 03:31:49.786223 ai2_kit-0.4.0/ai2_kit/workflow/__pycache__/fep_mlp.cpython-39.pyc
+-rw-r--r--   0        0        0    10027 2023-07-21 01:27:23.154801 ai2_kit-0.4.0/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     9073 2023-07-21 01:27:23.154801 ai2_kit-0.4.0/ai2_kit/workflow/fep_mlp.py
+-rw-r--r--   0        0        0      953 2023-07-21 01:28:07.314792 ai2_kit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3094 1970-01-01 00:00:00.000000 ai2_kit-0.4.0/PKG-INFO
```

### Comparing `ai2_kit-0.3.9/LICENSE` & `ai2_kit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/README.md` & `ai2_kit-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # ai<sup>2</sup>-kit
 
 [![PyPI version](https://badge.fury.io/py/ai2-kit.svg)](https://badge.fury.io/py/ai2-kit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ai2-kit)](https://pypi.org/project/ai2-kit/)
 
-A toolkit featured ***a**rtificial **i**ntelligence × **a**b **i**nitio* for computational chemistry research.
+A toolkit featured _**a**rtificial **i**ntelligence × **a**b **i**nitio_ for computational chemistry research.
 
 *Please be advised that `ai2-kit` is still under heavy development and you should expect things to change often. We encourage people to play and explore with `ai2-kit`, and stay tuned with us for more features to come.*
 
 
 ## Feature Highlights
 * Collection of tools to facilitate the development of automated workflows for computational chemistry research.
 * Utilities to execute and manage jobs in local or remote HPC job scheduler.
```

### Comparing `ai2_kit-0.3.9/ai2_kit/algorithm/proton_transfer.py` & `ai2_kit-0.4.0/ai2_kit/algorithm/proton_transfer.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 from functools import partial
 
 from dataclasses import dataclass
 from typing import List, Tuple, NamedTuple
 
 import fire
 import numpy as np
+from numpy import mean
+import matplotlib.pyplot as plt
 
 import json
 import os
 import io
 
 # TODO: use array instead of list for better performance when possible
 # TODO: use numba to speed up the calculation
 
+
 class AnalysisResult(NamedTuple):
     indicator_position: Tuple[float, float, float]
     transfers: List[Tuple[int, int]]
 
 
 @dataclass
 class SystemInfo:  # Information about the system
@@ -192,15 +195,15 @@
         parameter,
     )
 
     with Pool(processes=core_num) as pool:
         pool.map(partial(system.analysis, out_dir=out_dir), initial_donors)
 
 
-def visualize_transfer(analysis_result: str, input_traj: str,output_traj: str, initial_donor: int, cell: list):
+def visualize_transfer(analysis_result: str, input_traj: str, output_traj: str, initial_donor: int, cell: list):
     stc_list = ai.read(input_traj, index=":")
     donor = initial_donor
     with open(os.path.join(analysis_result, f'{initial_donor}.jsonl'), mode='r') as reader:
         for i, line in enumerate(reader):
             line = json.loads(line)
             stc_list[i][donor].symbol = 'N'
             stc_list[i].set_cell(cell)
@@ -215,26 +218,64 @@
 
 def analysis_transfer_paths(analysis_result: str, initial_donor: int):
     donor = initial_donor
     print("transfer_paths")
     fmt = "{:^40}\t{:^8}"
     content = fmt.format("transfer_path_index", "Snapshot")
     print(f"{content}")
-    with open(os.path.join(analysis_result, f'{initial_donor}.jsonl'), mode='r') as reader:
+    with open(os.path.join(analysis_result, f'{initial_donor}.jsonl'), mode='r') as reader, \
+            open(os.path.join(analysis_result, f'{initial_donor}_proton_infos.jsonl'), mode='wb') as writer:
         for i, line in enumerate(reader):
             line = json.loads(line)
             if line[1]:
                 for j, event in enumerate(line[1]):
                     acceptor = event[0]
                     proton = event[1]
                     content = f"{donor}({proton})->"
                     donor = acceptor
+                writer.write((json.dumps((proton, i)) + '\n').encode('utf-8'))
                 content = content + f"{acceptor}"
                 content = fmt.format(f"{content}", f"{i}")
                 print(content)
+        if proton:
+            writer.write((json.dumps((proton, i+1)) + '\n').encode('utf-8'))
+
+
+
+def calculate_distances(analysis_result: str, input_traj: str, upper_index: List[int], lower_index: List[int], initial_donor: int, interval: int = 1):
+    stc_list = ai.read(input_traj, index=":")
+    upper_pos = [stc_list[0][i].position[2] for i in upper_index]
+    lower_pos = [stc_list[0][i].position[2] for i in lower_index]
+    upper_interface = mean(upper_pos)
+    lower_interface = mean(lower_pos)
+    start = 0
+    with open(os.path.join(analysis_result, f'{initial_donor}_proton_infos.jsonl'), mode='rb') as reader, \
+            open(os.path.join(analysis_result, f'{initial_donor}_proton_distance_to_interface.jsonl'), mode='wb') as writer:
+        for i, line in enumerate(reader):
+            proton_info = json.loads(line)
+            end = proton_info[1]
+            for j in range(start, end, interval):
+                distance = min(abs(stc_list[j][proton_info[0]].position[2] - upper_interface),
+                               abs(stc_list[j][proton_info[0]].position[2] - lower_interface))
+                writer.write((json.dumps(distance) + '\n').encode('utf-8'))
+            start = end
+
+
+def show_distance_change(analysis_result: str, initial_donor: int):
+    y = []
+    with open(os.path.join(analysis_result, f'{initial_donor}_proton_distance_to_interface.jsonl'), mode='rb') as reader:
+        for i, line in enumerate(reader):
+            y.append(json.loads(line))
+    if y:
+        x = np.arange(len(y))
+        plt.plot(x, y)
+        plt.xlabel("Time")
+        plt.ylabel("Distance")
+        plt.title("Proton distance to interface")
+        plt.savefig(os.path.join(analysis_result, f'{initial_donor}_proton_distance_to_interface.png'))
 
 
 def detect_type_change(analysis_result: str, atom_types: dict, donors: list):
     type_change_event = []
     type_list = []
     type_change_name = []
     for i in range(len(atom_types)):
@@ -295,9 +336,11 @@
 
 
 if __name__ == '__main__':
     fire.Fire({
         "analyze": proton_transfer_detection,
         "visualize": visualize_transfer,
         "show-transfer-paths": analysis_transfer_paths,
-        "show-type-change": detect_type_change
+        "show-type-change": detect_type_change,
+        "calculate-distances": calculate_distances,
+        "show-distance-change": show_distance_change
     })
```

### Comparing `ai2_kit-0.3.9/ai2_kit/core/artifact.py` & `ai2_kit-0.4.0/ai2_kit/core/artifact.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/ai2_kit/core/checkpoint.py` & `ai2_kit-0.4.0/ai2_kit/core/checkpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import TypeVar, Union, Callable, NamedTuple, Optional
 from threading import Lock
 import functools
 import cloudpickle
 import os
 import inspect
+import fnmatch
 
 from .log import get_logger
 from .util import to_awaitable
 
 logger = get_logger(__name__)
 
 _lock = Lock()
@@ -161,28 +162,34 @@
     def __init__(self) -> None:
         ...
 
     def load(self, file):
         set_checkpoint_file(file)
         return self
 
-    def ls(self):
+    def ls(self, verbose=False):
         '''list all the checkpoint entries in the checkpoint file'''
         assert _checkpoint_data is not None
         for i, (key, value) in enumerate(_checkpoint_data.items()):
-            print('\n'.join([
-                '=' * 80,
-                f'Key:        \t{key}',
-                f'Call Site:  \t{value["info"]["call_site"]}',
-                f'Function:   \t{value["info"]["fn_name"]}',
-            ]))
-        print('=' * 80)
+            if verbose:
+                print('\n'.join([
+                    '=' * 80,
+                    f'Key:        \t{key}',
+                    f'Call Site:  \t{value["info"]["call_site"]}',
+                    f'Function:   \t{value["info"]["fn_name"]}',
+                ]))
+            else:
+                print(key)
 
-    def rm(self, prefix: str):
-        """remove checkpoint entries with the given prefix"""
+    def rm(self, glob_pattern: str, yes=False):
+        """remove checkpoint entries with the given pattern"""
         assert _checkpoint_data is not None
 
         for key in list(_checkpoint_data.keys()):
-            if key.startswith(prefix):
-                logger.info(f"Remove checkpoint: {key}")
-                del _checkpoint_data[key]
+            if fnmatch.fnmatch(key, glob_pattern):
+                if yes:
+                    del _checkpoint_data[key]
+                else:
+                    print(f"Delete checkpoint {key}? [y/n]")
+                    if input().lower() == 'y':
+                        del _checkpoint_data[key]
         _dump_checkpoint()
```

### Comparing `ai2_kit-0.3.9/ai2_kit/core/connector.py` & `ai2_kit-0.4.0/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/ai2_kit/core/executor.py` & `ai2_kit-0.4.0/ai2_kit/core/executor.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/ai2_kit/core/job.py` & `ai2_kit-0.4.0/ai2_kit/core/job.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/ai2_kit/core/queue_system.py` & `ai2_kit-0.4.0/ai2_kit/core/queue_system.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,16 +265,18 @@
 
     def resubmit(self):
         if not self.done():
             raise RuntimeError('Cannot resubmit an unfinished job!')
 
         # delete checkpoint on resubmit
         if self._checkpoint_key is not None:
+            logger.info(f'Delete checkpoint due to resubmit {self._checkpoint_key}')
             del_checkpoint(self._checkpoint_key)
 
+        logger.info(f'Resubmit job: {self._job_id}')
         return self._queue_system.submit(
             script=self._script,
             cwd=self._cwd,
             name=self._name,
             checkpoint_key=self._checkpoint_key,
             success_indicator=self._success_indicator,
         )
```

### Comparing `ai2_kit-0.3.9/ai2_kit/core/resource_manager.py` & `ai2_kit-0.4.0/ai2_kit/core/resource_manager.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/ai2_kit/core/script.py` & `ai2_kit-0.4.0/ai2_kit/core/script.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             rendered_step = '\n'.join([
                 rendered_step,
                 exit_on_error_statment()
             ])
 
         if self.checkpoint:
             checkpoint = shlex.quote(self.checkpoint + '.checkpoint')
-            msg = shlex.quote(f"pass {checkpoint}")
+            msg = shlex.quote(f"hit {checkpoint}, skip")
 
             rendered_step = '\n'.join([
                 f'if [ -f {checkpoint} ]; then echo {msg}; else',
                 rendered_step,
                 f'touch {checkpoint}; fi  # create checkpoint on success',
             ])
```

### Comparing `ai2_kit-0.3.9/ai2_kit/core/util.py` & `ai2_kit-0.4.0/ai2_kit/core/util.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,30 @@
 from ruamel.yaml import YAML
 from pathlib import Path
 from typing import Tuple, List, TypeVar
 from dataclasses import field
-from cp2k_input_tools.parser import CP2KInputParserSimplified
 
 import shortuuid
 import hashlib
 import base64
 import copy
 import os
-import io
+import random
 
 from .log import get_logger
 
 logger = get_logger(__name__)
 
 EMPTY = object()
 
+
 def default_mutable_field(obj):
     return field(default_factory=lambda: copy.copy(obj))
 
-def __merge_dict():
-    """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
-    def merge_dict(lo: dict, ro: dict, path=None):
-        """
-        merge two dict, the left dict will be overridden
 
-        this method won't merge list
-        """
-        if path is None:
-            path = []
-
-        for key, value in ro.items():
-            if key in lo:
-                current_path = path + [ str(key) ]
-                if isinstance(lo[key], dict) and isinstance(value, dict):
-                    merge_dict(lo[key], value, current_path)
-                else:
-                    print('.'.join(current_path) + ' has been overridden')
-                    lo[key] = value
-            else:
-                lo[key] = value
-        return lo
-    return merge_dict
-merge_dict = __merge_dict()
-
-
-# TODO: support http(s) url
 def load_yaml_file(path: Path):
     yaml = YAML(typ='safe')
     JoinTag.register(yaml)
     ReadTag.register(yaml)
     return yaml.load(path)
 
 
@@ -63,63 +37,44 @@
 
 
 def s_uuid():
     """short uuid"""
     return shortuuid.uuid()
 
 
-# TODO: this should be moved out from core module
-def parse_cp2k_input(text: str):
-    parser = CP2KInputParserSimplified(key_trafo=str.upper)
-    return parser.parse(io.StringIO(text))
-
-
-def dict_nested_get(d: dict, keys: List[str], default=EMPTY):
-    """get value from nested dict"""
-    for key in keys:
-        if key not in d and default is not EMPTY:
-            return default
-        d = d[key]
-    return d
-
-
-def dict_nested_set(d: dict, keys: List[str], value):
-    """set value to nested dict"""
-    for key in keys[:-1]:
-        d = d[key]
-    d[keys[-1]] = value
-
-
 def sort_unique_str_list(l: List[str]) -> List[str]:
     """remove duplicate str and sort"""
     return list(sorted(set(l)))
 
 
 T = TypeVar('T')
+
+
 def flatten(l: List[List[T]]) -> List[T]:
     return [item for sublist in l for item in sublist]
 
 
 def format_env_string(s: str) -> str:
     return s.format(**os.environ)
 
 
-def split_list(l: List[T], n: int) -> List[List[T]]:
+def list_split(l: List[T], n: int) -> List[List[T]]:
     """split list into n chunks"""
     # ref: https://stackoverflow.com/questions/2130016/splitting-a-list-into-n-parts-of-approximately-equal-length
     k, m = divmod(len(l), n)
-    return [l[i*k+min(i, m) : (i+1)*k+min(i+1, m)] for i in range(n)]
+    return [l[i*k+min(i, m): (i+1)*k+min(i+1, m)] for i in range(n)]
 
 
 def short_hash(s: str) -> str:
     """short hash string"""
     digest = hashlib.sha1(s.encode('utf-8')).digest()
     # use urlsafe encode to avoid '/' in the string, as it will cause problem in file path
     return base64.urlsafe_b64encode(digest).decode('utf-8')[:-2]
 
+
 async def to_awaitable(value: T) -> T:
     return value
 
 
 class JoinTag:
     """a tag to join strings in a list"""
 
@@ -156,7 +111,87 @@
     def to_yaml(cls, dumper, data):
         # do nothing
         return dumper.represent_sequence(cls.yaml_tag, data)
 
     @classmethod
     def register(cls, yaml: YAML):
         yaml.register_class(cls)
+
+
+def __export_remote_functions():
+    """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
+
+    def merge_dict(lo: dict, ro: dict, path=None):
+        """
+        Merge two dict, the left dict will be overridden.
+        Note: list will be replaced instead of merged.
+        """
+        if path is None:
+            path = []
+        for key, value in ro.items():
+            if key in lo:
+                current_path = path + [str(key)]
+                if isinstance(lo[key], dict) and isinstance(value, dict):
+                    merge_dict(lo[key], value, current_path)
+                else:
+                    print('.'.join(current_path) + ' has been overridden')
+                    lo[key] = value
+            else:
+                lo[key] = value
+        return lo
+
+    def dict_nested_get(d: dict, keys: List[str], default=EMPTY):
+        """get value from nested dict"""
+        for key in keys:
+            if key not in d and default is not EMPTY:
+                return default
+            d = d[key]
+        return d
+
+    def dict_nested_set(d: dict, keys: List[str], value):
+        """set value to nested dict"""
+        for key in keys[:-1]:
+            d = d[key]
+        d[keys[-1]] = value
+
+    def list_even_sample(l, size):
+        if size <= 0 or size > len(l):
+            return l
+        # calculate the sample interval
+        interval = len(l) / size
+        return [l[int(i * interval)] for i in range(size)]
+
+    def list_random_sample(l, size, seed = None):
+        if seed is None:
+            seed = len(l)
+        random.seed(seed)
+        return random.sample(l, size)
+
+    def list_sample(l, size, method='even', **kwargs):
+        if method == 'even':
+            return list_even_sample(l, size)
+        elif method == 'random':
+            return list_random_sample(l, size, **kwargs)
+        elif method == 'truncate':
+            return l[:size]
+        else:
+            raise ValueError(f'Unknown sample method {method}')
+
+    # export functions
+    return (
+        merge_dict,
+        dict_nested_get,
+        dict_nested_set,
+        list_even_sample,
+        list_random_sample,
+        list_sample,
+    )
+
+
+(
+    merge_dict,
+    dict_nested_get,
+    dict_nested_set,
+    list_even_sample,
+    list_random_sample,
+    list_sample,
+) = __export_remote_functions()
```

### Comparing `ai2_kit-0.3.9/ai2_kit/domain/cll.py` & `ai2_kit-0.4.0/ai2_kit/domain/iface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,47 @@
+# This is a class to defined common interface
+
 from abc import abstractmethod, ABC
 from ai2_kit.core.artifact import Artifact, ArtifactMap
-from ai2_kit.core.future import IFuture
 from ai2_kit.core.resource_manager import ResourceManager
-from typing import List, Callable, Any
+from typing import List
 from dataclasses import dataclass
 
+
 @dataclass
 class BaseCllContext:
     path_prefix: str
     resource_manager: ResourceManager
 
-######################
-# CLL Labeling Tasks #
-######################
-
 
 class ICllLabelOutput(ABC):
-
     @abstractmethod
     def get_labeled_system_dataset(self) -> List[Artifact]:
         ...
 
-CllLabelTaskType = Callable[[Any, BaseCllContext], IFuture[ICllLabelOutput]]
-
-######################
-# CLL Training Tasks #
-######################
-
 class ICllTrainOutput(ABC):
-
     @abstractmethod
     def get_mlp_models(self) -> List[Artifact]:
         ...
 
     @abstractmethod
     def get_training_dataset(self) -> List[Artifact]:
         ...
 
-
-CllTrainTaskType = Callable[[Any, BaseCllContext], IFuture[ICllTrainOutput]]
-
-######################
-# CLL Explore Tasks #
-######################
-
 class ICllExploreOutput(ABC):
-
     @abstractmethod
     def get_model_devi_dataset(self) -> List[Artifact]:
         ...
 
-CllExploreTaskType = Callable[[Any, BaseCllContext], IFuture[ICllExploreOutput]]
-
-######################
-# CLL Select Task    #
-######################
-
 class ICllSelectorOutput(ABC):
-
     @abstractmethod
     def get_model_devi_dataset(self) -> List[Artifact]:
         ...
 
     @abstractmethod
     def get_passing_rate(self) -> float:
         ...
 
-CllSelectorTaskType = Callable[[Any, BaseCllContext], IFuture[ICllSelectorOutput]]
-
 
 def init_artifacts(artifacts: ArtifactMap):
     for key, artifact in artifacts.items():
         artifact.attrs.setdefault('ancestor', key)
```

### Comparing `ai2_kit-0.3.9/ai2_kit/domain/cp2k.py` & `ai2_kit-0.4.0/ai2_kit/domain/lasp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,249 @@
+from ai2_kit.core.script import BashTemplate, BashStep, BashScript
 from ai2_kit.core.artifact import Artifact, ArtifactDict
-from ai2_kit.core.script import BashScript, BashStep, BashTemplate
-from ai2_kit.core.job import gather_jobs
-from ai2_kit.core.util import merge_dict, parse_cp2k_input, dict_nested_get, dict_nested_set, split_list
 from ai2_kit.core.log import get_logger
+from ai2_kit.core.job import gather_jobs
+from ai2_kit.core.util import list_split, merge_dict
 
-from typing import List, Union, Tuple
+from typing import List, Optional
 from pydantic import BaseModel
 from dataclasses import dataclass
 
+import numpy as np
+import ase.io
 import copy
 import os
+import re
+
+from .iface import BaseCllContext, ICllExploreOutput
+from .constant import DEFAULT_LASP_IN, DEFAULT_LAMMPS_TEMPLATE_FOR_DP_SSW, MODEL_DEVI_OUT
+from .data import artifacts_to_ase_atoms, DataFormat
 
-from .data_helper import LammpsOutputHelper, XyzHelper, Cp2kOutputHelper, ase_atoms_to_cp2k_input_data
-from .cll import ICllLabelOutput, BaseCllContext
 
 logger = get_logger(__name__)
 
-class GenericCp2kInputConfig(BaseModel):
-    init_system_files: List[str] = []
-    limit: int = 50
-    input_template: Union[dict, str]
+
+class CllLaspInputConfig(BaseModel):
+    class Potential(BaseModel):
+        class LammpsPotential(BaseModel):
+            input_template: str = DEFAULT_LAMMPS_TEMPLATE_FOR_DP_SSW
+
+        lammps: Optional[LammpsPotential] = None  # currently only lammps is supported
+
+    input_template: dict
     """
-    Input template for cp2k. Could be a dict or content of a cp2k input file.
+    Input template for LASP
+    """
+    potential: Potential
 
-    Note:
-    If you are using files in input templates, it is recommended to use artifact name instead of literal path.
-    String starts with '@' will be treated as artifact name.
-    For examples, FORCE_EVAL/DFT/BASIS_SET_FILE_NAME = @cp2k/basic_set.
-    You can still use literal path, but it is not recommended.
+    system_files: List[str]
+    """
+    Initial system files to explore
     """
 
-class GenericCp2kContextConfig(BaseModel):
+
+class CllLaspContextConfig(BaseModel):
+    lasp_cmd: str = 'lasp'
     script_template: BashTemplate
-    cp2k_cmd: str = 'cp2k'
     concurrency: int = 5
 
+
 @dataclass
-class GenericCp2kInput:
-    config: GenericCp2kInputConfig
-    system_files: List[Artifact]
+class CllLaspInput:
+    config: CllLaspInputConfig
     type_map: List[str]
-    initiated: bool = False
+    mass_map: List[float]
+    models: List[Artifact]
 
 
 @dataclass
-class GenericCp2kContext(BaseCllContext):
-    config: GenericCp2kContextConfig
+class CllLaspContext(BaseCllContext):
+    config: CllLaspContextConfig
 
 
 @dataclass
-class GenericCp2kOutput(ICllLabelOutput):
-    cp2k_outputs: List[Artifact]
+class CllLaspOutput(ICllExploreOutput):
+    output_dirs: List[Artifact]
 
-    def get_labeled_system_dataset(self):
-        return self.cp2k_outputs
+    def get_model_devi_dataset(self) -> List[Artifact]:
+        return self.output_dirs
 
 
-async def generic_cp2k(input: GenericCp2kInput, ctx: GenericCp2kContext) -> GenericCp2kOutput:
+async def cll_lasp(input: CllLaspInput, ctx: CllLaspContext):
     executor = ctx.resource_manager.default_executor
 
-    # For the first round
-    if not input.initiated:
-        input.system_files += ctx.resource_manager.get_artifacts(input.config.init_system_files)
-
     # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
-    [tasks_dir] = executor.setup_workspace(work_dir, ['tasks'])
+    tasks_dir, = executor.setup_workspace(work_dir, ['tasks'])
 
-    # prepare input template
-    if isinstance(input.config.input_template, str):
-        input_template = parse_cp2k_input(input.config.input_template)
-    else:
-        input_template = copy.deepcopy(input.config.input_template)
+    # resolve artifacts
+    systems = ctx.resource_manager.resolve_artifacts(input.config.system_files)
 
-    fields_with_artifact = [
-        ['FORCE_EVAL', 'DFT', 'BASIS_SET_FILE_NAME'],
-        ['FORCE_EVAL', 'DFT', 'POTENTIAL_FILE_NAME'],
-        ['FORCE_EVAL', 'DFT', 'XC', 'VDW_POTENTIAL', 'PAIR_POTENTIAL', 'PARAMETER', 'PARAMETER_FILE_NAME' ],
-    ]
-    for field_path in fields_with_artifact:
-        try :
-            field_value = dict_nested_get(input_template, field_path)
-            if isinstance(field_value, str) and field_value.startswith('@'):
-                logger.info(f'resolve artifact {field_value}')
-                dict_nested_set(
-                    input_template,
-                    field_path,
-                    ctx.resource_manager.resolve_artifact(field_value[1:])[0].url
-                )
-        except KeyError:
-            pass
-
-    # resolve data files
-    lammps_dump_files: List[Artifact] = []
-    xyz_files: List[Artifact] = []
-
-    # TODO: support POSCAR in the future
-    # TODO: refactor the way of handling different file formats
-    system_files = ctx.resource_manager.resolve_artifacts(input.system_files)
-    for system_file in system_files:
-        if LammpsOutputHelper.is_match(system_file):
-            lammps_out = LammpsOutputHelper(system_file)
-            lammps_dump_files.extend(lammps_out.get_passed_dump_files())
-        elif XyzHelper.is_match(system_file):
-            xyz_files.append(system_file)
-        else:
-            raise ValueError(f'unsupported format {system_file.url}: {system_file.format}')
-
-    # create task dirs and prepare input files
-    cp2k_task_dirs = []
-    if lammps_dump_files or xyz_files:
-        cp2k_task_dirs = executor.run_python_fn(make_cp2k_task_dirs)(
-            lammps_dump_files=[a.to_dict() for a in lammps_dump_files],
-            xyz_files=[a.to_dict() for a in xyz_files],
-            type_map=input.type_map,
-            base_dir=tasks_dir,
-            input_template=input_template,
-            limit=input.config.limit,
-        )
+    # setup configuration
+    lasp_in_data = merge_dict(copy.deepcopy(DEFAULT_LASP_IN), input.config.input_template)
+    lasp_in_data['explore_type'] = 'ssw'
+    lasp_in_data['SSW.output'] = 'T'
+
+    lammps_input_template = None
+    if input.config.potential.lammps is not None:
+        lasp_in_data['potential'] = 'lammps'
+        lammps_input_template = input.config.potential.lammps.input_template
     else:
-        logger.warn('no available candidates, skip')
-        return GenericCp2kOutput(cp2k_outputs=[])
+        raise ValueError('At least one potential should be specified.')
 
-    # build commands
+    # make task dirs
+    task_dirs = executor.run_python_fn(make_lasp_task_dirs)(
+        systems=[a.to_dict() for a in systems],
+        type_map=input.type_map, mass_map=input.mass_map,
+        lasp_in_data=lasp_in_data,
+        dp_models=[m.url for m in input.models],
+        lammps_input_template=lammps_input_template,
+        base_dir=tasks_dir,
+    )
+
+    # generate steps
+    lasp_cmd = f'{ctx.config.lasp_cmd} 1 >> lasp.out >> lasp.err'
     steps = []
-    for cp2k_task_dir in cp2k_task_dirs:
-        steps.append(BashStep(
-            cwd=cp2k_task_dir['url'],
-            cmd=[ctx.config.cp2k_cmd, '-i input.inp 1>> output 2>> output'],
-            checkpoint='cp2k',
-        ))
+    for task_dir in task_dirs :
+        steps.append(BashStep(cwd=task_dir['url'], cmd=lasp_cmd, checkpoint='lasp'))
 
-    # submit tasks and wait for completion
+    # submit jobs by the number of concurrency
     jobs = []
-    for i, steps_group in enumerate(split_list(steps, ctx.config.concurrency)):
+    for i, steps_group in enumerate(list_split(steps, ctx.config.concurrency)):
         if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
             steps=steps_group,
         )
         job = executor.submit(script.render(), cwd=tasks_dir,
-                              checkpoint_key=f'submit-job/cp2k/{i}:{tasks_dir}')
+                              checkpoint_key=f'queue-job/lasp/{i}:{tasks_dir}')
         jobs.append(job)
-    jobs = await gather_jobs(jobs, max_tries=2)
+    await gather_jobs(jobs, max_tries=2)
 
-    cp2k_outputs = [Artifact.of(
-        url=a['url'],
-        format=Cp2kOutputHelper.format,
-        executor=executor.name,
-        attrs=a['attrs'],
-    ) for a in cp2k_task_dirs]
+    # process outputs
+    executor.run_python_fn(process_lasp_outputs)(task_dirs=[a['url'] for a in task_dirs])
 
-    return GenericCp2kOutput(cp2k_outputs=cp2k_outputs)
+    output_dirs = [
+        Artifact.of(
+            url=task_dir['url'],
+            executor=executor.name,
+            format=DataFormat.LASP_LAMMPS_OUT_DIR,
+            attrs={ **task_dir['attrs'],  'traj_file': 'traj.xyz'},
+        ) for task_dir in task_dirs]  # type: ignore
+    return CllLaspOutput(output_dirs=output_dirs)
 
 
-def __make_cp2k_task_dirs():
-    def make_cp2k_task_dirs(lammps_dump_files: List[ArtifactDict],
-                            xyz_files: List[ArtifactDict],
-                            type_map: List[str],
-                            input_template: dict,
+def __export_remote_functions():
+
+    from string import Template
+
+    class LammpsInputTemplate(Template):
+        delimiter = '$$'
+
+    def make_lasp_task_dirs(systems: List[ArtifactDict],
+                            lasp_in_data: dict,
                             base_dir: str,
-                            limit: int = 0,
-                            input_file_name: str = 'input.inp',
+                            type_map: List[str],
+                            mass_map: List[float],
+                            dp_models: List[str],
+                            lammps_input_template: Optional[str],
                             ) -> List[ArtifactDict]:
-        """Generate CP2K input files from LAMMPS dump files or XYZ files."""
-        from cp2k_input_tools import DEFAULT_CP2K_INPUT_XML
-        from cp2k_input_tools.generator import CP2KInputGenerator
-
-        import ase.io
-        from ase import Atoms
-
-        cp2k_generator = CP2KInputGenerator(DEFAULT_CP2K_INPUT_XML)
-        task_dirs = []
-        atoms_list: List[Tuple[ArtifactDict, Atoms]] = []
-
-        # read atoms
-        for dump_file in lammps_dump_files:
-            atoms_list += [
-                (dump_file, atoms)
-                for atoms in ase.io.read(dump_file['url'], ':', format='lammps-dump-text', order=False, specorder=type_map)
-            ]  # type: ignore
-        for xyz_file in xyz_files:
-            atoms_list += [
-                (xyz_file, atoms)
-                for atoms in ase.io.read(xyz_file['url'], ':', format='extxyz')
-            ]  # type: ignore
-
-        if limit > 0:
-            atoms_list = atoms_list[:limit]
-
-        for i, (file, atoms) in enumerate(atoms_list):
-            # create task dir
-            task_dir = os.path.join(base_dir, f'{str(i).zfill(6)}')
+        input_data = artifacts_to_ase_atoms(systems, type_map=type_map)
+
+        i, task_dirs = 0, []
+        for artifact,  atoms in input_data:
+            # create task_dir
+            task_dir = os.path.join(base_dir, f'task_{i:06}' )
             os.makedirs(task_dir, exist_ok=True)
+            # create lasp.in
+            lasp_in_text =  '\n'.join([f'{k:32} {v}' for k, v in lasp_in_data.items()])
+            with open(os.path.join(task_dir, 'lasp.in'), 'w', encoding='utf-8') as f:
+                f.write(lasp_in_text)
+            # create lasp.str
+            ase.io.write(os.path.join(task_dir, 'lasp.str'), atoms, format='dmol-arc')
+            if lammps_input_template is not None:
+                # create lammps.data
+                data_file = os.path.join(task_dir, 'lammps.data')
+                ase.io.write(data_file, atoms, format='lammps-data', specorder=type_map)  # type: ignore
+                # create lammps input: in.simple, PS: Its LASP to blame for the name
+                read_data_section = '\n'.join([
+                    f"read_data {data_file}",
+                    *(f"mass {i+1} {m}" for i, m in enumerate(mass_map))
+                ])
+                force_field_section = '\n'.join([
+                    f"pair_style deepmd {' '.join(dp_models)} out_file {MODEL_DEVI_OUT}",
+                    f"pair_coeff * *"
+                ])
+                lammps_input = LammpsInputTemplate(lammps_input_template).substitute(
+                    read_data_section=read_data_section,
+                    force_field_section=force_field_section,
+                )
+                lammps_input_file = os.path.join(task_dir, 'in.simple')
+                with open(lammps_input_file, 'w', encoding='utf-8') as f:
+                    f.write(lammps_input)
+            else:
+                raise ValueError('At least one potential should be specified.')
+            task_dirs.append({'url': task_dir, 'attrs': artifact['attrs']})
+            i += 1
+        return task_dirs
 
-            # create input file
-            input_data = copy.deepcopy(input_template)
-            coords, cell = ase_atoms_to_cp2k_input_data(atoms)
-            merge_dict(input_data, {
-                'FORCE_EVAL': {
-                    'SUBSYS': {
-                        'COORD': {
-                            '*': coords
-                        },
-                        'CELL': {
-                            'A': cell[0],
-                            'B': cell[1],
-                            'C': cell[2],
-                        }
-                    }
-                }
-            })
-            input_text = '\n'.join(cp2k_generator.line_iter(input_data))
-            with open(os.path.join(task_dir, input_file_name), 'w') as f:
-                f.write(input_text)
-
-            # inherit attrs from input file
-            # TODO: inherit only ancestor key should be enough
-            task_dirs.append({
-                'url': task_dir,
-                'attrs': file['attrs'],
-            })
 
-        return task_dirs
+    def process_lasp_output(task_dir: str, file_name='traj.xyz'):
+        """
+        Align lasp output with model_devi records.
+
+        As allstr.arc contains all the structures generated by LASP,
+        we need to use the result of lasp.out for alignment.
+
+        The following code is copy from ChecMate, may need to be refactored
+        """
+        all_str_file = os.path.join(task_dir, 'allstr.arc')
+        lasp_out_file = os.path.join(task_dir, 'lasp.out')
+        all_strs = ase.io.read(all_str_file, ':', format='dmol-arc')
+
+        with open(all_str_file, "r") as f:
+            all_qs = list((round(float(line[:73].strip().split()[-2]),6) for line in f.readlines() if "Energy" in line))
+        with open(lasp_out_file, "r") as f:
+            lines = f.readlines()
+            traj_qs = list((round(float(line[:73].strip().split()[2]),6) for line in lines if "Energy,force" in line))
+            traj_es = list((round(float(line[:73].strip().split()[1]),6) for line in lines if "Energy,force" in line))
+
+        traj_strs = []
+        for i, q in enumerate(all_qs):
+            # FIXME: using fuzzy match to align data may have problem in some corner cases
+            if len(traj_qs) > 0 and np.isclose(q, traj_qs[0], rtol=0, atol=0.0001):
+                all_strs[i].info['ssw_energy'] = traj_es[len(traj_strs)]  # type: ignore
+                traj_strs.append(all_strs[i])
+                traj_qs.pop(0)
+        # write trajectory to file
+        ase.io.write(os.path.join(task_dir, file_name), traj_strs, format='extxyz')
+        # edit model_devi.out
+        model_devi_file = os.path.join(task_dir, MODEL_DEVI_OUT)
+        lines = []
+        with open(model_devi_file, "r") as f:
+            for i, line in enumerate(f):
+                if i > 0:
+                    # replace step 0 with step i so that it can be aligned with traj.xyz
+                    line = re.sub(r'^\s+\d+', f'{i-1:>12} ', line)   #
+                lines.append(line)
+        with open(model_devi_file, "w") as f:
+            f.writelines(lines)
+
+    def process_lasp_outputs(task_dirs: List[str], workers: int = 4):
+        import joblib
+        joblib.Parallel(n_jobs=workers)(
+            joblib.delayed(process_lasp_output)(task_dir)
+            for task_dir in task_dirs
+        )
+
+
+    return (
+        make_lasp_task_dirs,
+        process_lasp_outputs,
+    )
+
 
-    return make_cp2k_task_dirs
-make_cp2k_task_dirs = __make_cp2k_task_dirs()
+(
+    make_lasp_task_dirs,
+    process_lasp_outputs,
+) = __export_remote_functions()
```

### Comparing `ai2_kit-0.3.9/ai2_kit/domain/deepmd.py` & `ai2_kit-0.4.0/ai2_kit/domain/deepmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,116 @@
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.script import BashTemplate
 from ai2_kit.core.script import BashScript, BashStep
 from ai2_kit.core.job import JobFuture, gather_jobs
 from ai2_kit.core.log import get_logger
+from ai2_kit.core.util import dict_nested_get
 
 from pydantic import BaseModel
 from typing import List
 from dataclasses import dataclass
 import os
 import copy
 import random
 import sys
 import json
 
-from .cll import ICllTrainOutput, BaseCllContext
-from .data_helper import Cp2kOutputHelper, DeepmdNpyHelper, convert_to_deepmd_npy
+from .iface import ICllTrainOutput, BaseCllContext
+from .data import DataFormat, get_data_format, convert_to_deepmd_npy
+
 from .constant import (
     DP_CHECKPOINT_FILE,
     DP_DISP_FILE,
     DP_PROFILING_FILE,
     DP_INPUT_FILE,
     DP_FROZEN_MODEL,
     DP_ORIGINAL_MODEL
 )
 
 logger = get_logger(__name__)
 
 
-class GenericDeepmdInputConfig(BaseModel):
+class CllDeepmdInputConfig(BaseModel):
     model_num: int = 4
     init_dataset: List[str]
     input_template: dict
     compress_model: bool = False
 
-class GenericDeepmdContextConfig(BaseModel):
+class CllDeepmdContextConfig(BaseModel):
     script_template: BashTemplate
     dp_cmd: str = 'dp'
 
 
 @dataclass
-class GenericDeepmdInput:
-    config: GenericDeepmdInputConfig
+class CllDeepmdInput:
+    config: CllDeepmdInputConfig
     type_map: List[str]
     old_dataset: List[Artifact]  # training data used by previous iteration
     new_dataset: List[Artifact]  # training data used by current iteration
-    initiated: bool = False
+    initiated: bool = False  # FIXME: this seems to be a bad design idea
 
     def update_training_dataset(self, dataset: List[Artifact]):
         self.old_dataset += self.new_dataset
         self.new_dataset = dataset
 
 
 @dataclass
-class GenericDeepmdContext(BaseCllContext):
-    config: GenericDeepmdContextConfig
+class CllDeepmdContext(BaseCllContext):
+    config: CllDeepmdContextConfig
 
 
 @dataclass
 class GenericDeepmdOutput(ICllTrainOutput):
     outputs: List[Artifact]
-    input: GenericDeepmdInput
+    input: CllDeepmdInput
 
     def get_mlp_models(self) -> List[Artifact]:
         return [a.join(DP_FROZEN_MODEL) for a in self.outputs]
 
     def get_training_dataset(self) -> List[Artifact]:
         return self.input.new_dataset + self.input.old_dataset
 
 
-async def generic_deepmd(input: GenericDeepmdInput, ctx: GenericDeepmdContext):
+async def cll_deepmd(input: CllDeepmdInput, ctx: CllDeepmdContext):
     executor = ctx.resource_manager.default_executor
 
     # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
     [converted_data_dir, tasks_dir] = executor.setup_workspace(
         work_dir, ['converted_input_data', 'tasks'])
 
     # initialization
     if not input.initiated:
         input.new_dataset += ctx.resource_manager.resolve_artifacts(
             input.config.init_dataset)
 
     # convert data type if necessary, only needed for new data as old data is already converted
-    new_deepmd_npy_data: List[Artifact] = []
-    cp2k_output_data: List[Artifact] = []
+    deepmd_npy_data: List[Artifact] = []
+    data_to_be_converted: List[Artifact] = []
 
-    # TODO: refactor data type conversion
     for artifact in input.new_dataset:
-        if not artifact.format or DeepmdNpyHelper.is_match(artifact):
-            # treated as deepmd npy data if format is not specified
-            new_deepmd_npy_data.append(artifact)
-        elif Cp2kOutputHelper.is_match(artifact):
-            cp2k_output_data.append(artifact)
+        data = artifact.to_dict()
+        format = get_data_format(data)  # type: ignore
+        if format == DataFormat.DEEPMD_NPY or not format:
+            deepmd_npy_data.append(artifact)
         else:
-            raise ValueError(f'unsupported data type: {artifact.format}')
+            data_to_be_converted.append(artifact)
 
     # convert data to deepmd/npy format
-    # TODO: support more data type
     converted_data_dirs = executor.run_python_fn(convert_to_deepmd_npy)(
-        cp2k_outputs=[a.to_dict() for a in cp2k_output_data],
+        dataset=[a.to_dict() for a in data_to_be_converted],
         base_dir=converted_data_dir,
         type_map=input.type_map,
     )
-    new_deepmd_npy_data += [Artifact.of(
-        url=url, format=DeepmdNpyHelper.format,
-    ) for url in converted_data_dirs]
 
-    input.new_dataset = new_deepmd_npy_data
+    deepmd_npy_data += [Artifact.of(
+        url=a['url'], format=a['format'], attrs=a['attrs']
+    ) for a in converted_data_dirs]
+
+    input.new_dataset = deepmd_npy_data
 
     jobs: List[JobFuture] = []
     output_dirs = []
 
     # train multiple models at the same time
     for i in range(input.config.model_num):
         # each model should be trained in its own task_dir
@@ -140,16 +140,21 @@
                 d['seed'] = _random_seed()
         else:
             discriptor['seed'] = _random_seed()
         dp_input['model']['fitting_net']['seed'] = _random_seed()
         dp_input['training']['seed'] = _random_seed()
 
         # set training data
-        systems = [a.url for a in input.old_dataset + input.new_dataset]
-        training['systems'] = systems
+        VALIDATION_DATA_KEY = 'validation_data'
+        train_systems = [a.url for a in input.old_dataset + input.new_dataset
+                         if not dict_nested_get(a.attrs, ['deepmd', VALIDATION_DATA_KEY], False)]
+        validation_systems = [a.url for a in input.old_dataset + input.new_dataset
+                            if dict_nested_get(a.attrs, ['deepmd', VALIDATION_DATA_KEY], False)]
+
+        training['systems'] = train_systems
         set_prefix: str = training.setdefault(
             'set_prefix', 'set')  # respect user input
         auto_prob_str = "prob_sys_size"
         training.setdefault('batch_size', 'auto')
         training['auto_prob_style'] = auto_prob_str
 
         # v2 training data
@@ -157,14 +162,24 @@
             'systems': training['systems'],
             'set_prefix': training['set_prefix'],
             'auto_prob_style': training['auto_prob_style'],
             'batch_size': training['batch_size'],
         }
         training['training_data'] = training_data
 
+        # ignore validation section if no data is provided, or else dp will throw error
+        # OSError: [Errno cannot find valid a data system] Please check your setting for data systems
+        if len(validation_systems) > 0:
+            validation_data = {
+                'systems': validation_systems,
+                'set_prefix': training['set_prefix'],
+                'batch_size': training['batch_size'],
+            }
+            training['validation_data'] = validation_data
+
         # other params
         dp_input['model']['type_map'] = input.type_map
 
         # write config to executor
         dp_input_text = json.dumps(dp_input, indent=2)
         dp_input_path = os.path.join(task_dir, DP_INPUT_FILE)
         executor.dump_text(dp_input_text, dp_input_path)
@@ -190,22 +205,23 @@
         dp_train_script = BashScript(
             template=ctx.config.script_template,
             steps=steps # type: ignore
         )
         output_dirs.append(task_dir)
 
         # submit job
-        job = executor.submit(dp_train_script.render(), cwd=task_dir, checkpoint_key=f'submit-job/dp-train/{i}:{task_dir}')
+        job = executor.submit(dp_train_script.render(), cwd=task_dir, checkpoint_key=f'queue-job:dp-train:{task_dir}:{i}')
         jobs.append(job)
 
     await gather_jobs(jobs, max_tries=2)
 
     return GenericDeepmdOutput(
         input=input,
         outputs=[Artifact.of(
             url=url,
+            format=DataFormat.DEEPMD_OUTPUT_DIR,
         ) for url in output_dirs]
     )
 
 
 def _random_seed():
     return random.randrange(sys.maxsize) % (1 << 32)
```

### Comparing `ai2_kit-0.3.9/ai2_kit/domain/lammps.py` & `ai2_kit-0.4.0/ai2_kit/domain/lammps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 from ai2_kit.core.script import BashTemplate, BashStep, BashScript
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.job import gather_jobs
-from ai2_kit.core.util import split_list, dict_nested_get
+from ai2_kit.core.util import list_split, dict_nested_get
 
-from typing import List, Literal, Optional, Union, Mapping, Sequence, Any
+from typing import List, Literal, Optional, Mapping, Sequence, Any
 from pydantic import BaseModel
 from dataclasses import dataclass
 from string import Template
 from allpairspy import AllPairs
 import os
 import itertools
 import random
 
 
-from .cll import BaseCllContext, ICllExploreOutput
+from .iface import BaseCllContext, ICllExploreOutput
 from .constant import (
     MODEL_DEVI_OUT,
     MODEL_DEVI_NEU_OUT,
     MODEL_DEVI_RED_OUT,
     LAMMPS_TRAJ_DIR,
     LAMMPS_TRAJ_SUFFIX,
 )
-from .data_helper import LammpsOutputHelper, PoscarHelper, convert_to_lammps_input_data
+from .data import convert_to_lammps_input_data, DataFormat
 
 logger = get_logger(__name__)
 
 
 class ExploreVariants(BaseModel):
     temp: List[float]
     """Temperatures variants."""
-
     pres: List[float]
     """Pressures variants."""
-
     others: Mapping[str, Sequence[Any]] = dict()
     """
     Other variants to be combined with.
     The key is the name of the variant, and the value is the list of values.
     For example, if you want to combine the variant 'LAMBDA' with values [0.0, 0.5, 1.0],
     you can set the others field to {'LAMBDA': [0.0, 0.5, 1.0]}.
     And in LAMMPS input template, you can use the variable ${LAMBDA} and v_LAMBDA to access the value.
     """
 
 
-class GenericLammpsInputConfig(BaseModel):
-
+class CllLammpsInputConfig(BaseModel):
     explore_vars: ExploreVariants
     """Variants to be explored."""
 
     n_wise: int = 0
     """The way of combining variants.
     0 means cartesian product, 2 means 2-wise, etc.
     If n_wise is less than 2 or greater than total fields,
     the full combination will be used.
     It is strongly recommended to use n_wise when the full combination is too large.
     """
-
     system_files: List[str]
     """Artifacts of initial system data."""
-
     plumed_config: Optional[str]
     """Plumed config file content."""
+    plumed_config_file: Optional[str]
+    """Plumed config file path."""
 
-    no_pbc: bool = False
+    # ensemble specific params
     tau_t: float = 0.1
     tau_p: float = 0.5
+    time_const: float = 0.1
+    ensemble: Literal['nvt', 'nvt-i', 'nvt-a', 'nvt-iso', 'nvt-aniso', 'npt', 'npt-t', 'npt-tri', 'nve', 'csvr']
+
+    no_pbc: bool = False
     timestep: float = 0.0005
     sample_freq: int
     nsteps: int
-    ensemble: Literal['nvt', 'nvt-i', 'nvt-a', 'nvt-iso', 'nvt-aniso', 'npt', 'npt-t', 'npt-tri', 'nve']
+
     """Ensemble to be used.
     nvt means constant volume and temperature.
     nvt-i means constant volume and temperature, with isotropic scaling.
     nvt-a means constant volume and temperature, with anisotropic scaling.
     nvt-iso means constant volume and temperature, with isotropic scaling.
     npt means constant pressure and temperature.
     npt-t means constant pressure and temperature, with isotropic scaling.
@@ -88,76 +89,66 @@
     post_init_section: str = ''
     post_read_data_section: str = ''
     post_force_field_section: str = ''
     post_md_section: str = ''
     post_run_section: str = ''
 
 
-class GenericLammpsContextConfig(BaseModel):
+class CllLammpsContextConfig(BaseModel):
     script_template: BashTemplate
     lammps_cmd: str = 'lmp'
     concurrency: int = 5
 
 
 @dataclass
-class GenericLammpsInput:
+class CllLammpsInput:
 
     @dataclass
     class MdOptions:
         models: List[Artifact]
 
     @dataclass
     class FepOptions:
         red_models: List[Artifact]
         neu_models: List[Artifact]
 
-    config: GenericLammpsInputConfig
+    config: CllLammpsInputConfig
     type_map: List[str]
     mass_map: List[float]
 
     # The following options are mutex
     md_options: Optional[MdOptions] = None
     fep_options: Optional[FepOptions] = None
 
 
 @dataclass
-class GenericLammpsContext(BaseCllContext):
-    config: GenericLammpsContextConfig
+class CllLammpsContext(BaseCllContext):
+    config: CllLammpsContextConfig
 
 
 @dataclass
 class GenericLammpsOutput(ICllExploreOutput):
     model_devi_outputs: List[Artifact]
 
     def get_model_devi_dataset(self) -> List[Artifact]:
         return self.model_devi_outputs
 
 
-async def generic_lammps(input: GenericLammpsInput, ctx: GenericLammpsContext):
+async def cll_lammps(input: CllLammpsInput, ctx: CllLammpsContext):
     executor = ctx.resource_manager.default_executor
 
     # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
     input_data_dir, tasks_dir = executor.setup_workspace(work_dir, ['input_data', 'tasks'])
-
     systems = ctx.resource_manager.resolve_artifacts(input.config.system_files)
 
-    # prepare lammps input data
-    # TODO: refactor the way of handling different types of input
-    # TODO: handle more data format, for example, cp2k output
-    poscar_files: List[Artifact] = []
-
-    for system_file in systems:
-        if PoscarHelper.is_match(system_file):
-            poscar_files.append(system_file)
-        else:
-            raise ValueError(f'unsupported system file type: {system_file}')
-
+    # TODO: the whole process to generate task dirs should be run remotely
+    # Reference: lasp.py
     input_data_files: List[ArtifactDict] = executor.run_python_fn(convert_to_lammps_input_data)(
-        poscar_files=[a.to_dict() for a in poscar_files],
+        systems=[a.to_dict() for a in systems],
         base_dir=input_data_dir,
         type_map=input.type_map,
     )
 
     combination_fields: List[str] = [
         'data_file',
         'temp',
@@ -204,52 +195,51 @@
             force_field_section = make_fep_force_field_section(
                 neu_models=[a.url for a in input.fep_options.neu_models],
                 red_models=[a.url for a in input.fep_options.red_models],
             )
         else:
             raise ValueError('one and only one of md_options or fep_options must be set')
 
-        plumed_file = None
-        # plumed_config could be overrided by the attrs of data_file
+        # Config plumed if either plumed_config_file or plumed_config is set.
+        # The plumed config can be set in both workflow config and input data file.
+        # The config in input data file has higher priority.
+        plumed_config_file = dict_nested_get(data_file, ['attrs', 'lammps', 'plumed_config_file'],
+                                             input.config.plumed_config_file)
         plumed_config = dict_nested_get(data_file, ['attrs', 'lammps', 'plumed_config'],
                                         input.config.plumed_config)
-
-        if plumed_config and isinstance(plumed_config, str):
-            plumed_file = 'plumed.input'
-            plumed_file_path = os.path.join(lammps_task_dir, plumed_file)
+        if plumed_config_file is None and isinstance(plumed_config, str):
+            plumed_config_file = 'plumed.input'
+            plumed_file_path = os.path.join(lammps_task_dir, plumed_config_file)
             logger.info(f'found plumed config, generate {plumed_file_path}')
             executor.dump_text(plumed_config, plumed_file_path)
 
         template = input.config.input_template or  DEFAULT_LAMMPS_INPUT_TEMPLATE
-
         input_text = make_lammps_input(data_file=data_file['url'],
                                        nsteps=input.config.nsteps,
                                        timestep=input.config.timestep,
                                        trj_freq=input.config.sample_freq,
                                        temp=temp,
                                        pres=pres,
                                        tau_t=input.config.tau_t,
                                        tau_p=input.config.tau_p,
+                                       time_const=input.config.time_const,
                                        ensemble=input.config.ensemble,
                                        mass_map=input.mass_map,
                                        others_dict=others_dict,
-
                                        force_field_section=force_field_section,
-
                                        template=template,
                                        post_variables_section=input.config.post_variables_section,
                                        post_init_section=input.config.post_init_section,
                                        post_read_data_section=input.config.post_read_data_section,
                                        post_force_field_section=input.config.post_force_field_section,
                                        post_md_section=input.config.post_md_section,
                                        post_run_section=input.config.post_run_section,
-                                       plumed_file=plumed_file,
+                                       plumed_config_file=plumed_config_file,  # type: ignore
                                        no_pbc=False,
-                                       rand_start=1_000_000,
-                                       )
+                                       rand_start=1_000_000)
         input_file_path = os.path.join(lammps_task_dir, lammps_input_file_name)
         logger.info(f'generate lammps config {input_file_path}')
 
         executor.dump_text(input_text, input_file_path)
         lammps_task_dirs.append({'url': lammps_task_dir, 'attrs': data_file['attrs']})  # type: ignore
 
     # build scripts and submit
@@ -260,32 +250,32 @@
     # generate steps
     steps = []
     for lammps_task_dir in lammps_task_dirs:
         steps.append(BashStep(cwd=lammps_task_dir['url'], cmd=cmd, checkpoint='lammps'))
 
     # submit jobs by the number of concurrency
     jobs = []
-    for i, steps_group in enumerate(split_list(steps, ctx.config.concurrency)):
+    for i, steps_group in enumerate(list_split(steps, ctx.config.concurrency)):
         if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
             steps=steps_group,
         )
         job = executor.submit(script.render(), cwd=tasks_dir,
-                              checkpoint_key=f'submit-job/lammps/{i}:{tasks_dir}')
+                              checkpoint_key=f'queue-job/lammps/{i}:{tasks_dir}')
         jobs.append(job)
 
     await gather_jobs(jobs, max_tries=2)
 
     outputs = [
         Artifact.of(
             url=task_dir['url'],
             executor=executor.name,
-            format=LammpsOutputHelper.format,
+            format=DataFormat.LAMMPS_OUTPUT_DIR,
             attrs=task_dir['attrs'],
         ) for task_dir in lammps_task_dirs]  # type: ignore
 
     return GenericLammpsOutput(model_devi_outputs=outputs)
 
 
 def make_md_force_field_section(models: List[str]):
@@ -331,15 +321,16 @@
                       post_init_section: str,
                       post_read_data_section: str,
                       post_force_field_section: str,
                       post_md_section: str,
                       post_run_section: str,
 
                       force_field_section: List[str],
-                      plumed_file: Optional[str] = None,
+                      plumed_config_file: Optional[str] = None,
+                      time_const = 0.1,
                       no_pbc=False,
                       rand_start=1_000_000,
                       ):
 
     # FIXME: I am not sure if it is a good idea to fix it automatically
     # maybe we should consider raise an error here
     if not ensemble.startswith('npt'):
@@ -350,14 +341,15 @@
         'variable NSTEPS      equal %d' % nsteps,
         'variable THERMO_FREQ equal %d' % trj_freq,
         'variable DUMP_FREQ   equal %d' % trj_freq,
         'variable TEMP        equal %f' % temp,
         'variable PRES        equal %f' % pres,
         'variable TAU_T       equal %f' % tau_t,
         'variable TAU_P       equal %f' % tau_p,
+        'variable TIME_CONST  equal %f' % time_const,
         '',
         '# custom variables (if any)',
     ]
 
     for k, v in others_dict.items():
         variables.append(f'variable {k} equal {v}')
 
@@ -382,19 +374,22 @@
         md_section.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} aniso ${PRES} ${PRES} ${TAU_P}')
     elif ensemble in ('npt-t', 'npt-tri',):
         md_section.append('fix 1 all npt temp ${TEMP} ${TEMP} ${TAU_T} tri ${PRES} ${PRES} ${TAU_P}')
     elif ensemble in ('nvt',):
         md_section.append('fix 1 all nvt temp ${TEMP} ${TEMP} ${TAU_T}')
     elif ensemble in ('nve',):
         md_section.append('fix 1 all nve')
+    elif ensemble in ('csvr',):
+        md_section.append('fix 1 all nve')
+        md_section.append('fix 2 all temp/csvr ${TEMP} ${TEMP} ${TIME_CONST} %d' % (random.randrange(rand_start - 1) + 1))
     else:
         raise ValueError('unknown ensemble: ' + ensemble)
 
-    if plumed_file:
-        md_section.append(f'fix dpgen_plm all plumed plumedfile {plumed_file} outfile plumed.out')
+    if plumed_config_file:
+        md_section.append(f'fix dpgen_plm all plumed plumedfile {plumed_config_file} outfile plumed.out')
 
     if no_pbc:
         md_section.extend([
             'velocity all zero linear',
             'fix      fm all momentum 1 linear 1 1 1',
         ])
```

### Comparing `ai2_kit-0.3.9/ai2_kit/domain/selector.py` & `ai2_kit-0.4.0/ai2_kit/domain/selector.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,65 +2,72 @@
 from ai2_kit.core.log import get_logger
 
 from typing import List
 from io import StringIO
 from pydantic import BaseModel
 from dataclasses import dataclass
 import pandas as pd
+import os
+from tabulate import tabulate
 
-from .data_helper import LammpsOutputHelper
-from .cll import ICllSelectorOutput, BaseCllContext
+from .data import get_data_format, DataFormat
+from .iface import ICllSelectorOutput, BaseCllContext
+from .constant import LAMMPS_DUMPS_CLASSIFIED
 
 logger = get_logger(__name__)
 
-class ThresholdSelectorInputConfig(BaseModel):
+class CllModelDeviSelectorInputConfig(BaseModel):
     f_trust_lo: float
     f_trust_hi: float
 
-
 @dataclass
-class ThresholdSelectorContext(BaseCllContext):
+class CllModelDevSelectorContext(BaseCllContext):
     ...
 
-
 @dataclass
-class ThresholdSelectorOutput(ICllSelectorOutput):
+class CllModelDeviSelectorOutput(ICllSelectorOutput):
     model_devi_data: List[Artifact]
     passing_rate: float
 
     def get_model_devi_dataset(self):
         return self.model_devi_data
 
     def get_passing_rate(self) -> float:
         return self.passing_rate
 
 @dataclass
-class ThresholdSelectorInput:
-    config: ThresholdSelectorInputConfig
+class CllModelDeviSelectorInput:
+    config: CllModelDeviSelectorInputConfig
     model_devi_data: List[Artifact]
     model_devi_out_filename: str
 
     def set_model_devi_dataset(self, data: List[Artifact]):
         self.model_devi_data = data
 
-async def threshold_selector(input: ThresholdSelectorInput, ctx: ThresholdSelectorContext):
+async def cll_model_devi_selector(input: CllModelDeviSelectorInput, ctx: CllModelDevSelectorContext):
     executor = ctx.resource_manager.default_executor
+    work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
+    executor.mkdir(work_dir)
 
     f_trust_lo = input.config.f_trust_lo
     f_trust_hi = input.config.f_trust_hi
-    col_force = 'avg_devi_f'
+    col_force = 'max_devi_f'
     logger.info('criteria: %f <= %s < %f ', f_trust_lo, col_force, f_trust_hi)
 
     total_count = 0
     passed_count = 0
 
-    # TODO: support output of different software
+    table = []
+
     for candidate in input.model_devi_data:
-        if LammpsOutputHelper.is_match(candidate):
-            model_devi_out_file = LammpsOutputHelper(candidate).get_model_devi_file(input.model_devi_out_filename).url
+        data_format = get_data_format(candidate.to_dict())  # type: ignore
+        if data_format == DataFormat.LAMMPS_OUTPUT_DIR:
+            model_devi_out_file = candidate.join(input.model_devi_out_filename).url
+        elif data_format == DataFormat.LASP_LAMMPS_OUT_DIR:
+            model_devi_out_file = candidate.join(input.model_devi_out_filename).url
         else:
             raise ValueError('unknown model_devi_data types')
 
         logger.info('start to analysis file: %s', model_devi_out_file)
         text = executor.load_text(model_devi_out_file)
 
         df = pd.read_csv(StringIO(text.lstrip('#')), delim_whitespace=True)
@@ -69,21 +76,31 @@
         # 0        0    0.006793    0.000672    0.003490    0.143317    0.005612    0.026106
         # 1      100    0.006987    0.000550    0.003952    0.128178    0.006042    0.022608
 
         passed_df   = df[df[col_force] < f_trust_lo]
         selected_df = df[(df[col_force] >= f_trust_lo) & (df[col_force] < f_trust_hi)]
         rejected_df = df[df[col_force] >= f_trust_hi]
 
-        logger.info('result: total: %d, passed: %d, selected: %d, rejected: %d', len(df), len(passed_df), len(selected_df), len(rejected_df))
+        classified_result = {
+            'all': df.step.tolist(),
+            'passed': passed_df.step.tolist(),
+            'selected': selected_df.step.tolist(),
+            'rejected': rejected_df.step.tolist(),
+        }
 
-        candidate.attrs['all'] = df.step.tolist()
-        candidate.attrs['passed']   = passed_df.step.tolist()
-        candidate.attrs['selected'] = selected_df.step.tolist()
-        candidate.attrs['rejected'] = rejected_df.step.tolist()
+        candidate.attrs[LAMMPS_DUMPS_CLASSIFIED] = classified_result
 
+        passing_rate = len(passed_df) / len(df)
         total_count += len(df)
         passed_count += len(passed_df)
 
-    return ThresholdSelectorOutput(
+        table.append([os.path.relpath(model_devi_out_file, work_dir), len(df), len(passed_df), len(selected_df), len(rejected_df), passing_rate])
+
+    headers = ['file', 'total', 'pass', 'candidate', 'reject', 'pass%']
+    stats_report = tabulate(table, headers=headers, tablefmt='tsv')
+    logger.info('stats report: \n%s', stats_report)
+
+    executor.dump_text(stats_report, os.path.join(work_dir, 'stats.tsv'))
+    return CllModelDeviSelectorOutput(
         model_devi_data=input.model_devi_data,
         passing_rate=passed_count / total_count,
     )
```

### Comparing `ai2_kit-0.3.9/ai2_kit/domain/vasp.py` & `ai2_kit-0.4.0/ai2_kit/domain/vasp.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,220 +1,179 @@
 from ai2_kit.core.artifact import Artifact, ArtifactDict
 from ai2_kit.core.script import BashScript, BashStep, BashTemplate
 from ai2_kit.core.job import gather_jobs
-from ai2_kit.core.util import merge_dict, dict_nested_get, dict_nested_set, split_list
+from ai2_kit.core.util import dict_nested_get, list_split, list_sample
 from ai2_kit.core.log import get_logger
 
-from typing import List, Union
+from typing import List, Union, Literal
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 from typing import List, Union, Optional, Tuple
 from pymatgen.io.vasp.inputs import Incar, Kpoints
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 import copy
 import os
 
-from .data_helper import LammpsOutputHelper, XyzHelper, VaspOutputHelper
-from .cll import ICllLabelOutput, BaseCllContext
+from .data import DataFormat, artifacts_to_ase_atoms
+from .iface import ICllLabelOutput, BaseCllContext
 
 logger = get_logger(__name__)
 
-class GenericVaspInputConfig(BaseModel):
+class CllVaspInputConfig(BaseModel):
     init_system_files: List[str] = []
-    limit: int = 50
     input_template: Union[dict, str]
     potcar_source: Union[dict, list]
-    kpoints_template: Optional[str] = None
+    kpoints_template: Optional[Union[dict, str]] = None
     """
     Input template for VASP. Could be a dict or content of a VASP input file.
-
-    Note:
-    If you are using files in input templates, it is recommended to use artifact name instead of literal path.
-    String starts with '@' will be treated as artifact name.
-    For examples, input_template = @vasp/INCAR.
-    You can still use literal path, but it is not recommended.
     """
+    limit: int = 50
+    limit_method: Literal["even", "random", "truncate"] = "even"
 
-class GenericVaspContextConfig(BaseModel):
+class CllVaspContextConfig(BaseModel):
     script_template: BashTemplate
     vasp_cmd: str = 'vasp_std'
     concurrency: int = 5
 
 @dataclass
-class GenericVaspInput:
-    config: GenericVaspInputConfig
+class CllVaspInput:
+    config: CllVaspInputConfig
     system_files: List[Artifact]
     type_map: List[str]
     initiated: bool = False
 
 
 @dataclass
-class GenericVaspContext(BaseCllContext):
-    config: GenericVaspContextConfig
+class CllVaspContext(BaseCllContext):
+    config: CllVaspContextConfig
 
 
 @dataclass
 class GenericVaspOutput(ICllLabelOutput):
     vasp_outputs: List[Artifact]
 
     def get_labeled_system_dataset(self):
         return self.vasp_outputs
 
 
-async def generic_vasp(input: GenericVaspInput, ctx: GenericVaspContext) -> GenericVaspOutput:
+async def cll_vasp(input: CllVaspInput, ctx: CllVaspContext) -> GenericVaspOutput:
     executor = ctx.resource_manager.default_executor
 
     # For the first round
     if not input.initiated:
         input.system_files += ctx.resource_manager.get_artifacts(input.config.init_system_files)
 
+    if len(input.system_files) == 0:
+        return GenericVaspOutput(vasp_outputs=[])
+
     # setup workspace
     work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
     [tasks_dir] = executor.setup_workspace(work_dir, ['tasks'])
 
     # prepare input template
     if isinstance(input.config.input_template, str):
         input_template = input.config.input_template
-        if input_template.startswith('@'):
-            input_template = \
-                ctx.resource_manager.resolve_artifact(input_template[1:])[0].url
         input_template = Incar.from_file(input_template).as_dict()
     else:
         input_template = copy.deepcopy(input.config.input_template)
 
     # prepare potcar
     if isinstance(input.config.potcar_source, dict):
         potcar_source = input.config.potcar_source
-    else:
+    elif isinstance(input.config.potcar_source, list):
         # default: use same sequence as type_map
         if len(input.config.potcar_source) >= len(input.type_map):
             potcar_source = {
                 k: v for k, v in zip(input.type_map, input.config.potcar_source)
             }
         else:
             raise ValueError('potcar_source should not be shorter than type_map')
-        
-    for k, v in potcar_source.items():
-        if v.startswith('@'):
-            potcar_source[k] = \
-                ctx.resource_manager.resolve_artifact(v[1:])[0].url
+    else:
+        # TODO: support generate POTCAR from given path of potential.
+        raise ValueError('potcar_source should be either dict or list')
 
     # prepare kpoints
     kpoints_template = input.config.kpoints_template
-    if kpoints_template:
-        if kpoints_template.startswith('@'):
-            logger.info(f'resolve artifact {kpoints_template}')
-            kpoints_template = \
-                ctx.resource_manager.resolve_artifact(kpoints_template[1:])[0].url
+    if isinstance(kpoints_template, str):
         kpoints_template = Kpoints.from_file(kpoints_template).as_dict()
+    elif isinstance(kpoints_template, dict):
+        kpoints_template = copy.deepcopy(kpoints_template)
     else:
         kpoints_template = None
 
-    # resolve data files
-    lammps_dump_files: List[Artifact] = []
-    xyz_files: List[Artifact] = []
-
-    # TODO: support POSCAR in the future
-    # TODO: refactor the way of handling different file formats
     system_files = ctx.resource_manager.resolve_artifacts(input.system_files)
-    for system_file in system_files:
-        if LammpsOutputHelper.is_match(system_file):
-            lammps_out = LammpsOutputHelper(system_file)
-            lammps_dump_files.extend(lammps_out.get_passed_dump_files())
-        elif XyzHelper.is_match(system_file):
-            xyz_files.append(system_file)
-        else:
-            raise ValueError(f'unsupported format {system_file.url}: {system_file.format}')
 
     # create task dirs and prepare input files
-    vasp_task_dirs = []
-    if lammps_dump_files or xyz_files:
-        vasp_task_dirs = executor.run_python_fn(make_vasp_task_dirs)(
-            lammps_dump_files=[a.to_dict() for a in lammps_dump_files],
-            xyz_files=[a.to_dict() for a in xyz_files],
-            type_map=input.type_map,
-            base_dir=tasks_dir,
-            input_template=input_template,
-            potcar_source=potcar_source,
-            kpoints_template=kpoints_template,
-            limit=input.config.limit,
-        )
-    else:
-        logger.warn('no available candidates, skip')
-        return GenericVaspOutput(vasp_outputs=[])
+    vasp_task_dirs = executor.run_python_fn(make_vasp_task_dirs)(
+        system_files=[a.to_dict() for a in system_files],
+        type_map=input.type_map,
+        base_dir=tasks_dir,
+        input_template=input_template,
+        potcar_source=potcar_source,
+        kpoints_template=kpoints_template,
+        limit=input.config.limit,
+    )
 
     # build commands
     steps = []
     for vasp_task_dir in vasp_task_dirs:
         steps.append(BashStep(
             cwd=vasp_task_dir['url'],
             cmd=[ctx.config.vasp_cmd, ' 1>> output 2>> output'],
             checkpoint='vasp',
         ))
 
-    # run tasks
+    # submit tasks and wait for completion
     jobs = []
-    for i, steps_group in enumerate(split_list(steps, ctx.config.concurrency)):
+    for i, steps_group in enumerate(list_split(steps, ctx.config.concurrency)):
         if not steps_group:
             continue
         script = BashScript(
             template=ctx.config.script_template,
-            steps=steps,
+            steps=steps_group,
         )
         job = executor.submit(script.render(), cwd=tasks_dir,
-                              checkpoint_key=f'submit-job/vasp/{i}:{tasks_dir}')
+                              checkpoint_key=f'queue-job:vasp:{tasks_dir}:{i}')
         jobs.append(job)
     jobs = await gather_jobs(jobs, max_tries=2)
 
     vasp_outputs = [Artifact.of(
         url=a['url'],
-        format=VaspOutputHelper.format,
+        format=DataFormat.VASP_OUTPUT_DIR,
         executor=executor.name,
         attrs=a['attrs'],
     ) for a in vasp_task_dirs]
 
     return GenericVaspOutput(vasp_outputs=vasp_outputs)
 
 
-def __make_vasp_task_dirs():
-    def make_vasp_task_dirs(lammps_dump_files: List[ArtifactDict],
-                            xyz_files: List[ArtifactDict],
+def __export_remote_functions():
+    def make_vasp_task_dirs(system_files: List[ArtifactDict],
                             type_map: List[str],
                             input_template: dict,
                             potcar_source: dict,
                             base_dir: str,
                             kpoints_template: Optional[dict] = None,
-                            limit: int = 0
+                            limit: int = 0,
+                            sample_method: Literal["even", "random", "truncate"] = "even"
                             ) -> List[ArtifactDict]:
         """Generate VASP input files from LAMMPS dump files or XYZ files."""
 
         import ase.io
         from ase import Atoms
         from ase.io.vasp import _symbol_count_from_symbols
 
         task_dirs = []
-        atoms_list: List[Tuple[ArtifactDict, Atoms]] = []
-
-        # read atoms
-        for dump_file in lammps_dump_files:
-            atoms_list += [
-                (dump_file, atoms)
-                for atoms in ase.io.read(dump_file['url'], ':', format='lammps-dump-text', order=False, specorder=type_map)
-            ]  # type: ignore
-        for xyz_file in xyz_files:
-            atoms_list += [
-                (xyz_file, atoms)
-                for atoms in ase.io.read(xyz_file['url'], ':', format='extxyz')
-            ]  # type: ignore
+        atoms_list: List[Tuple[ArtifactDict, Atoms]] = artifacts_to_ase_atoms(system_files, type_map)
 
         if limit > 0:
-            atoms_list = atoms_list[:limit]
+            atoms_list = list_sample(atoms_list, limit, method=sample_method)
 
         for i, (file, atoms) in enumerate(atoms_list):
             # create task dir
             task_dir = os.path.join(base_dir, f'{str(i).zfill(6)}')
             os.makedirs(task_dir, exist_ok=True)
 
             # create input file
@@ -227,26 +186,26 @@
 
             # create POSCAR
             elements_all = atoms.get_chemical_symbols()
             elements = [
                 item[0] for item in _symbol_count_from_symbols(elements_all)
             ]
             ase.io.write(
-                os.path.join(task_dir, 'POSCAR'), atoms, format='vasp5'
+                os.path.join(task_dir, 'POSCAR'), atoms, format='vasp'
             )
 
             # create POTCAR
             with open(os.path.join(task_dir, 'POTCAR'), 'w') as out_file:
                 for element in elements:
                     with open(potcar_source[element], 'r') as in_file:
                         out_file.write(in_file.read())
 
             # create KPOINTS
             kpoints_template = dict_nested_get(
-                file, ['attrs', 'vasp', 'kpoints_template'] # type: ignore
+                file, ['attrs', 'vasp', 'kpoints_template'], None # type: ignore
             )
             if kpoints_template:
                 kpoints = Kpoints.from_dict(kpoints_template)
                 kpoints.write_file(os.path.join(task_dir, 'KPOINTS'))
 
             # inherit attrs from input file
             # TODO: inherit only ancestor key should be enough
@@ -254,8 +213,8 @@
                 'url': task_dir,
                 'attrs': file['attrs'],
             })
 
         return task_dirs
 
     return make_vasp_task_dirs
-make_vasp_task_dirs = __make_vasp_task_dirs()
+make_vasp_task_dirs = __export_remote_functions()
```

### Comparing `ai2_kit-0.3.9/ai2_kit/main.py` & `ai2_kit-0.4.0/ai2_kit/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,24 @@
         return proton_transfer.analysis_transfer_paths
 
     @property
     def show_type_change(self):
         from ai2_kit.algorithm import proton_transfer
         return proton_transfer.detect_type_change
 
+    @property
+    def calculate_distances(self):
+        from ai2_kit.algorithm import proton_transfer
+        return proton_transfer.calculate_distances
+
+    @property
+    def show_distance_change(self):
+        from ai2_kit.algorithm import proton_transfer
+        return proton_transfer.show_distance_change
+
 
 class WorkflowGroup:
     @property
     def cll_mlp_training(self):
         from ai2_kit.workflow.cll_mlp import run_workflow
         return run_workflow
```

### Comparing `ai2_kit-0.3.9/ai2_kit/tool/ase.py` & `ai2_kit-0.4.0/ai2_kit/tool/ase.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.3.9/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.4.0/ai2_kit/workflow/cll_mlp.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from ai2_kit.core.artifact import ArtifactMap
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.util import load_yaml_files, merge_dict
 from ai2_kit.core.resource_manager import ResourceManager
 from ai2_kit.core.checkpoint import set_checkpoint_file, apply_checkpoint
 from ai2_kit.domain import (
     deepmd,
+    iface,
     lammps,
+    lasp,
     selector,
     cp2k,
     vasp,
     constant as const,
     updater,
-    cll,
 )
 
 from pydantic import BaseModel
 from typing import Dict, List, Optional, Any
 from fire import Fire
 
 import asyncio
@@ -26,22 +27,23 @@
 
 logger = get_logger(__name__)
 
 
 class CllWorkflowExecutorConfig(BaseExecutorConfig):
     class Context(BaseModel):
         class Train(BaseModel):
-            deepmd: deepmd.GenericDeepmdContextConfig
+            deepmd: deepmd.CllDeepmdContextConfig
 
         class Explore(BaseModel):
-            lammps: lammps.GenericLammpsContextConfig
+            lammps: Optional[lammps.CllLammpsContextConfig]
+            lasp: Optional[lasp.CllLaspContextConfig]
 
         class Label(BaseModel):
-            cp2k: Optional[cp2k.GenericCp2kContextConfig]
-            vasp: Optional[vasp.GenericVaspContextConfig]
+            cp2k: Optional[cp2k.CllCp2kContextConfig]
+            vasp: Optional[vasp.CllVaspContextConfig]
 
         train: Train
         explore: Explore
         label: Label
 
     context: Context
 
@@ -49,28 +51,29 @@
 class WorkflowConfig(BaseModel):
     class General(BaseModel):
         type_map: List[str]
         mass_map: List[float]
         max_iters: int = 10
 
     class Label(BaseModel):
-        cp2k: Optional[cp2k.GenericCp2kInputConfig]
-        vasp: Optional[vasp.GenericVaspInputConfig]
+        cp2k: Optional[cp2k.CllCp2kInputConfig]
+        vasp: Optional[vasp.CllVaspInputConfig]
 
     class Train(BaseModel):
-        deepmd: deepmd.GenericDeepmdInputConfig
+        deepmd: deepmd.CllDeepmdInputConfig
 
     class Explore(BaseModel):
-        lammps: lammps.GenericLammpsInputConfig
+        lammps: Optional[lammps.CllLammpsInputConfig]
+        lasp: Optional[lasp.CllLaspInputConfig]
 
     class Select(BaseModel):
-        by_threshold: selector.ThresholdSelectorInputConfig
+        model_devi: selector.CllModelDeviSelectorInputConfig
 
     class Update(BaseModel):
-        walkthrough: updater.WalkthroughUpdaterInputConfig
+        walkthrough: updater.CllWalkthroughUpdaterInputConfig
 
     general: General
     train: Train
     explore: Explore
     select: Select
     label: Label
     update: Update
@@ -80,47 +83,47 @@
 
     executors: Dict[str, CllWorkflowExecutorConfig]
     artifacts: ArtifactMap
     workflow: Any  # Keep it raw here, it should be parsed later in iteration
 
 
 def run_workflow(*config_files, executor: Optional[str] = None,
-                 path_prefix: Optional[str] = None, checkpoint_file: Optional[str] = None):
+                 path_prefix: Optional[str] = None, checkpoint: Optional[str] = None):
     """
     Run Closed-Loop Learning (CLL) workflow to train Machine Learning Potential (MLP) models.
     """
-    if checkpoint_file is not None:
-        set_checkpoint_file(checkpoint_file)
+    if checkpoint is not None:
+        set_checkpoint_file(checkpoint)
 
     config_data = load_yaml_files(*config_files)
     config = CllWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
-    cll.init_artifacts(config.artifacts)
+    iface.init_artifacts(config.artifacts)
     resource_manager = ResourceManager(
         executor_configs=config.executors,
         artifacts=config.artifacts,
         default_executor=executor,
     )
     return asyncio.run(cll_mlp_training_workflow(config, resource_manager, executor, path_prefix))
 
 
 async def cll_mlp_training_workflow(config: CllWorkflowConfig, resource_manager: ResourceManager, executor: str, path_prefix: str):
     context_config = config.executors[executor].context
     raw_workflow_config = copy.deepcopy(config.workflow)
 
     # output of each step
-    label_output: Optional[cll.ICllLabelOutput] = None
-    selector_output: Optional[cll.ICllSelectorOutput] = None
-    train_output: Optional[cll.ICllTrainOutput] = None
-    explore_output: Optional[cll.ICllExploreOutput] = None
+    label_output: Optional[iface.ICllLabelOutput] = None
+    selector_output: Optional[iface.ICllSelectorOutput] = None
+    train_output: Optional[iface.ICllTrainOutput] = None
+    explore_output: Optional[iface.ICllExploreOutput] = None
 
     # cursor of update table
     update_cursor = 0
 
     # Start iteration
     for i in itertools.count(0):
 
@@ -136,97 +139,117 @@
 
         # decide path prefix for each iteration
         iter_path_prefix = os.path.join(path_prefix, f'iters-{i:03d}')
         # prefix of checkpoint
         cp_prefix = f'iters-{i:03d}'
 
         # label
-        if workflow_config.label.cp2k:
-            cp2k_input = cp2k.GenericCp2kInput(
+        if workflow_config.label.cp2k and context_config.label.cp2k:
+            cp2k_input = cp2k.CllCp2kInput(
                 config=workflow_config.label.cp2k,
                 type_map=type_map,
                 system_files=[] if selector_output is None else selector_output.get_model_devi_dataset(),
                 initiated=i > 0,
             )
-            if context_config.label.cp2k is None:
-                raise ValueError('label > cp2k should not be empty')
-            cp2k_context = cp2k.GenericCp2kContext(
+            cp2k_context = cp2k.CllCp2kContext(
                 config=context_config.label.cp2k,
                 path_prefix=os.path.join(iter_path_prefix, 'label-cp2k'),
                 resource_manager=resource_manager,
             )
-            label_output = await apply_checkpoint(f'{cp_prefix}/label-cp2k')(cp2k.generic_cp2k)(cp2k_input, cp2k_context)
-        elif workflow_config.label.vasp:
-            vasp_input = vasp.GenericVaspInput(
+            label_output = await apply_checkpoint(f'{cp_prefix}/label-cp2k')(cp2k.cll_cp2k)(cp2k_input, cp2k_context)
+
+        elif workflow_config.label.vasp and context_config.label.vasp:
+            vasp_input = vasp.CllVaspInput(
                 config=workflow_config.label.vasp,
                 type_map=type_map,
                 system_files=[] if selector_output is None else selector_output.get_model_devi_dataset(),
                 initiated=i > 0,
             )
-            if context_config.label.vasp is None:
-                raise ValueError('label > vasp should not be empty')
-            vasp_context = vasp.GenericVaspContext(
+            vasp_context = vasp.CllVaspContext(
                 config=context_config.label.vasp,
                 path_prefix=os.path.join(iter_path_prefix, 'label-vasp'),
                 resource_manager=resource_manager,
             )
-            label_output = await apply_checkpoint(f'{cp_prefix}/label-vasp')(vasp.generic_vasp)(vasp_input, vasp_context)
+            label_output = await apply_checkpoint(f'{cp_prefix}/label-vasp')(vasp.cll_vasp)(vasp_input, vasp_context)
+
         else:
             raise ValueError('No label method is specified')
 
+        # return if no new data is generated
+        if i > 0 and len(label_output.get_labeled_system_dataset()) == 0:
+            logger.info("No new data is generated, stop iteration.")
+            break
+
         # train
         if workflow_config.train.deepmd:
-            deepmd_input = deepmd.GenericDeepmdInput(
+            deepmd_input = deepmd.CllDeepmdInput(
                 config=workflow_config.train.deepmd,
                 type_map=type_map,
                 old_dataset=[] if train_output is None else train_output.get_training_dataset(),
                 new_dataset=label_output.get_labeled_system_dataset(),
                 initiated=i > 0,
             )
-            deepmd_context = deepmd.GenericDeepmdContext(
+            deepmd_context = deepmd.CllDeepmdContext(
                 path_prefix=os.path.join(iter_path_prefix, 'train-deepmd'),
                 config=context_config.train.deepmd,
                 resource_manager=resource_manager,
             )
-            train_output = await apply_checkpoint(f'{cp_prefix}/train-deepmd')(deepmd.generic_deepmd)(deepmd_input, deepmd_context)
+            train_output = await apply_checkpoint(f'{cp_prefix}/train-deepmd')(deepmd.cll_deepmd)(deepmd_input, deepmd_context)
+
         else:
             raise ValueError('No train method is specified')
 
         # explore
-        if workflow_config.explore.lammps:
-            md_options = lammps.GenericLammpsInput.MdOptions(
+        if workflow_config.explore.lammps and context_config.explore.lammps:
+            md_options = lammps.CllLammpsInput.MdOptions(
                 models=train_output.get_mlp_models(),
             )
-            lammps_input = lammps.GenericLammpsInput(
+            lammps_input = lammps.CllLammpsInput(
                 config=workflow_config.explore.lammps,
                 type_map=type_map,
                 mass_map=mass_map,
                 md_options=md_options,
             )
-            lammps_context = lammps.GenericLammpsContext(
+            lammps_context = lammps.CllLammpsContext(
                 path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
                 config=context_config.explore.lammps,
                 resource_manager=resource_manager,
             )
-            explore_output = await apply_checkpoint(f'{cp_prefix}/explore-lammps')(lammps.generic_lammps)(lammps_input, lammps_context)
+            explore_output = await apply_checkpoint(f'{cp_prefix}/explore-lammps')(lammps.cll_lammps)(lammps_input, lammps_context)
+
+        elif workflow_config.explore.lasp and context_config.explore.lasp:
+            lasp_input = lasp.CllLaspInput(
+                config=workflow_config.explore.lasp,
+                type_map=type_map,
+                mass_map=mass_map,
+                models=train_output.get_mlp_models(),
+            )
+            lasp_context = lasp.CllLaspContext(
+                config=context_config.explore.lasp,
+                path_prefix=os.path.join(iter_path_prefix, 'explore-lasp'),
+                resource_manager=resource_manager,
+            )
+            explore_output = await apply_checkpoint(f'{cp_prefix}/explore-lasp')(lasp.cll_lasp)(lasp_input, lasp_context)
+
         else:
             raise ValueError('No explore method is specified')
 
         # select
-        if workflow_config.select.by_threshold:
-            selector_input = selector.ThresholdSelectorInput(
-                config=workflow_config.select.by_threshold,
+        if workflow_config.select.model_devi:
+            selector_input = selector.CllModelDeviSelectorInput(
+                config=workflow_config.select.model_devi,
                 model_devi_data=explore_output.get_model_devi_dataset(),
                 model_devi_out_filename=const.MODEL_DEVI_OUT,
             )
-            selector_context = selector.ThresholdSelectorContext(
+            selector_context = selector.CllModelDevSelectorContext(
                 path_prefix=os.path.join(iter_path_prefix, 'selector-threshold'),
                 resource_manager=resource_manager,
             )
-            selector_output = await apply_checkpoint(f'{cp_prefix}/selector-threshold')(selector.threshold_selector)(selector_input, selector_context)
+            selector_output = await apply_checkpoint(f'{cp_prefix}/selector-threshold')(selector.cll_model_devi_selector)(selector_input, selector_context)
+
         else:
             raise ValueError('No select method is specified')
 
         # Update
         update_config = workflow_config.update.walkthrough
 
         # nothing to update because the table is empty
```

### Comparing `ai2_kit-0.3.9/ai2_kit/workflow/fep_mlp.py` & `ai2_kit-0.4.0/ai2_kit/workflow/fep_mlp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from ai2_kit.core.executor import BaseExecutorConfig
 from ai2_kit.core.artifact import ArtifactMap
 from ai2_kit.core.log import get_logger
 from ai2_kit.core.util import load_yaml_files
 from ai2_kit.core.resource_manager import ResourceManager
 from ai2_kit.domain import (
     deepmd,
+    iface,
     lammps,
     selector,
     cp2k,
     constant as const,
     updater,
-    cll,
 )
 from ai2_kit.core.checkpoint import set_checkpoint_file, apply_checkpoint
 
 from pydantic import BaseModel
 from typing import Dict, List, Optional, Any
 from fire import Fire
 
@@ -25,39 +25,39 @@
 
 logger = get_logger(__name__)
 
 
 class FepExecutorConfig(BaseExecutorConfig):
     class Context(BaseModel):
 
-        deepmd: deepmd.GenericDeepmdContextConfig
-        lammps: lammps.GenericLammpsContextConfig
-        cp2k: cp2k.GenericCp2kContextConfig
+        deepmd: deepmd.CllDeepmdContextConfig
+        lammps: lammps.CllLammpsContextConfig
+        cp2k: cp2k.CllCp2kContextConfig
 
     context: Context
 
 
 class WorkflowConfig(BaseModel):
     class General(BaseModel):
         type_map: List[str]
         mass_map: List[float]
         max_iters: int = 10
 
     class Branch(BaseModel):
-        deepmd: deepmd.GenericDeepmdInputConfig
-        cp2k: cp2k.GenericCp2kInputConfig
-        threshold: selector.ThresholdSelectorInputConfig
+        deepmd: deepmd.CllDeepmdInputConfig
+        cp2k: cp2k.CllCp2kInputConfig
+        threshold: selector.CllModelDeviSelectorInputConfig
 
     class Update(BaseModel):
-        walkthrough: updater.WalkthroughUpdaterInputConfig
+        walkthrough: updater.CllWalkthroughUpdaterInputConfig
 
     general: General
     neu: Branch
     red: Branch
-    lammps: lammps.GenericLammpsInputConfig
+    lammps: lammps.CllLammpsInputConfig
     update: Update
 
 
 class FepWorkflowConfig(BaseModel):
     executors: Dict[str, FepExecutorConfig]
     artifacts: ArtifactMap
     workflow: Any
@@ -75,38 +75,38 @@
     config = FepWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
-    cll.init_artifacts(config.artifacts)
+    iface.init_artifacts(config.artifacts)
     resource_manager = ResourceManager(
         executor_configs=config.executors,
         artifacts=config.artifacts,
         default_executor=executor,
     )
     return asyncio.run(cll_mlp_training_workflow(config, resource_manager, executor, path_prefix))
 
 
 async def cll_mlp_training_workflow(config: FepWorkflowConfig, resource_manager: ResourceManager, executor: str, path_prefix: str):
     context_config = config.executors[executor].context
     raw_workflow_config = copy.deepcopy(config.workflow)
 
     # output of each step
-    neu_label_output: Optional[cll.ICllLabelOutput] = None
-    red_label_output: Optional[cll.ICllLabelOutput] = None
+    neu_label_output: Optional[iface.ICllLabelOutput] = None
+    red_label_output: Optional[iface.ICllLabelOutput] = None
 
-    neu_selector_output: Optional[cll.ICllSelectorOutput] = None
-    red_selector_output: Optional[cll.ICllSelectorOutput] = None
+    neu_selector_output: Optional[iface.ICllSelectorOutput] = None
+    red_selector_output: Optional[iface.ICllSelectorOutput] = None
 
-    neu_train_output: Optional[cll.ICllTrainOutput] = None
-    red_train_output: Optional[cll.ICllTrainOutput] = None
+    neu_train_output: Optional[iface.ICllTrainOutput] = None
+    red_train_output: Optional[iface.ICllTrainOutput] = None
 
-    explore_output: Optional[cll.ICllExploreOutput] = None
+    explore_output: Optional[iface.ICllExploreOutput] = None
 
     # cursor of update table
     update_cursor = 0
     # Start iteration
     for i in itertools.count(0):
 
         # parse workflow config
@@ -121,116 +121,116 @@
 
         # decide path prefix for each iteration
         iter_path_prefix = os.path.join(path_prefix, f'iters-{i:03d}')
         # prefix of checkpoint
         cp_prefix = f'iters-{i:03d}'
 
         # label: cp2k
-        red_cp2k_input = cp2k.GenericCp2kInput(
+        red_cp2k_input = cp2k.CllCp2kInput(
             config=workflow_config.red.cp2k,
             type_map=type_map,
             system_files=[] if red_selector_output is None else red_selector_output.get_model_devi_dataset(),
             initiated=i > 0,
         )
-        red_cpk2_context = cp2k.GenericCp2kContext(
+        red_cpk2_context = cp2k.CllCp2kContext(
             config=context_config.cp2k,
             path_prefix=os.path.join(iter_path_prefix, 'red-label-cp2k'),
             resource_manager=resource_manager,
         )
 
-        neu_cp2k_input = cp2k.GenericCp2kInput(
+        neu_cp2k_input = cp2k.CllCp2kInput(
             config=workflow_config.neu.cp2k,
             type_map=type_map,
             system_files=[] if neu_selector_output is None else neu_selector_output.get_model_devi_dataset(),
             initiated=i > 0,
         )
-        neu_cp2k_context = cp2k.GenericCp2kContext(
+        neu_cp2k_context = cp2k.CllCp2kContext(
             config=context_config.cp2k,
             path_prefix=os.path.join(iter_path_prefix, 'neu-label-cp2k'),
             resource_manager=resource_manager,
         )
 
         red_label_output, neu_label_output = await asyncio.gather(
-            apply_checkpoint(f'{cp_prefix}/cp2k/red')(cp2k.generic_cp2k)(red_cp2k_input, red_cpk2_context),
-            apply_checkpoint(f'{cp_prefix}/cp2k/neu')(cp2k.generic_cp2k)(neu_cp2k_input, neu_cp2k_context),
+            apply_checkpoint(f'{cp_prefix}/cp2k/red')(cp2k.cll_cp2k)(red_cp2k_input, red_cpk2_context),
+            apply_checkpoint(f'{cp_prefix}/cp2k/neu')(cp2k.cll_cp2k)(neu_cp2k_input, neu_cp2k_context),
         )
 
         # Train
-        red_deepmd_input = deepmd.GenericDeepmdInput(
+        red_deepmd_input = deepmd.CllDeepmdInput(
             config=workflow_config.red.deepmd,
             type_map=type_map,
             old_dataset=[] if red_train_output is None else red_train_output.get_training_dataset(),
             new_dataset=red_label_output.get_labeled_system_dataset(),
             initiated=i > 0,
         )
-        red_deepmd_context = deepmd.GenericDeepmdContext(
+        red_deepmd_context = deepmd.CllDeepmdContext(
             path_prefix=os.path.join(iter_path_prefix, 'red-train-deepmd'),
             config=context_config.deepmd,
             resource_manager=resource_manager,
         )
-        neu_deepmd_input = deepmd.GenericDeepmdInput(
+        neu_deepmd_input = deepmd.CllDeepmdInput(
             config=workflow_config.neu.deepmd,
             type_map=type_map,
             old_dataset=[] if neu_train_output is None else neu_train_output.get_training_dataset(),
             new_dataset=neu_label_output.get_labeled_system_dataset(),
             initiated=i > 0,
         )
-        neu_deepmd_context = deepmd.GenericDeepmdContext(
+        neu_deepmd_context = deepmd.CllDeepmdContext(
             path_prefix=os.path.join(iter_path_prefix, 'neu-train-deepmd'),
             config=context_config.deepmd,
             resource_manager=resource_manager,
         )
 
         red_train_output, neu_train_output = await asyncio.gather(
-            apply_checkpoint(f'{cp_prefix}/deepmd/red')(deepmd.generic_deepmd)(red_deepmd_input, red_deepmd_context),
-            apply_checkpoint(f'{cp_prefix}/deepmd/neu')(deepmd.generic_deepmd)(neu_deepmd_input, neu_deepmd_context),
+            apply_checkpoint(f'{cp_prefix}/deepmd/red')(deepmd.cll_deepmd)(red_deepmd_input, red_deepmd_context),
+            apply_checkpoint(f'{cp_prefix}/deepmd/neu')(deepmd.cll_deepmd)(neu_deepmd_input, neu_deepmd_context),
         )
 
         # explore
-        lammps_input = lammps.GenericLammpsInput(
+        lammps_input = lammps.CllLammpsInput(
             config=workflow_config.lammps,
             type_map=type_map,
             mass_map=mass_map,
-            fep_options=lammps.GenericLammpsInput.FepOptions(
+            fep_options=lammps.CllLammpsInput.FepOptions(
                 neu_models=neu_train_output.get_mlp_models(),
                 red_models=red_train_output.get_mlp_models(),
             ),
         )
-        lammps_context = lammps.GenericLammpsContext(
+        lammps_context = lammps.CllLammpsContext(
             path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
             config=context_config.lammps,
             resource_manager=resource_manager,
         )
-        explore_output = await apply_checkpoint(f'{cp_prefix}/lammps')(lammps.generic_lammps)(lammps_input, lammps_context)
+        explore_output = await apply_checkpoint(f'{cp_prefix}/lammps')(lammps.cll_lammps)(lammps_input, lammps_context)
 
         # select
-        red_selector_input = selector.ThresholdSelectorInput(
+        red_selector_input = selector.CllModelDeviSelectorInput(
             config=workflow_config.red.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
             model_devi_out_filename=const.MODEL_DEVI_RED_OUT,
         )
-        red_selector_context = selector.ThresholdSelectorContext(
+        red_selector_context = selector.CllModelDevSelectorContext(
             path_prefix=os.path.join(
                 iter_path_prefix, 'red-selector-threshold'),
             resource_manager=resource_manager,
         )
 
-        neu_selector_input = selector.ThresholdSelectorInput(
+        neu_selector_input = selector.CllModelDeviSelectorInput(
             config=workflow_config.neu.threshold,
             model_devi_data=explore_output.get_model_devi_dataset(),
             model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
         )
-        neu_selector_context = selector.ThresholdSelectorContext(
+        neu_selector_context = selector.CllModelDevSelectorContext(
             path_prefix=os.path.join(iter_path_prefix, 'neu-selector-threshold'),
             resource_manager=resource_manager,
         )
 
         red_selector_output, neu_selector_output = await asyncio.gather(
-            apply_checkpoint(f'{cp_prefix}/selector/red')(selector.threshold_selector)(red_selector_input, red_selector_context),
-            apply_checkpoint(f'{cp_prefix}/selector/neu')(selector.threshold_selector)(neu_selector_input, neu_selector_context),
+            apply_checkpoint(f'{cp_prefix}/selector/red')(selector.cll_model_devi_selector)(red_selector_input, red_selector_context),
+            apply_checkpoint(f'{cp_prefix}/selector/neu')(selector.cll_model_devi_selector)(neu_selector_input, neu_selector_context),
         )
 
         # Update
         update_config = workflow_config.update.walkthrough
 
         # nothing to update because the table is empty
         if not update_config.table:
```

### Comparing `ai2_kit-0.3.9/pyproject.toml` & `ai2_kit-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.3.9"
+version = "0.4.0"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -13,31 +13,37 @@
 pydantic = "^1.10.2"
 invoke = "^1.7.3"
 ruamel-yaml = "^0.17.21"
 cloudpickle = "^2.2.0"
 shortuuid = "^1.0.11"
 dpdata = "^0.2.13"
 pandas = "^1.5.3"
-cp2k-input-tools = "^0.8.2"
 ase = "^3.22.1"
 pymatgen = "^2023.2.22"
 mdanalysis = "^2.4.3"
 allpairspy = "^2.5.0"
+tabulate = "^0.9.0"
+asaplib = "^0.0.2"
+joblib = "^1.2.0"
+dscribe = "1.2.2"
 
 
 [[tool.poetry.source]]
 name = "ustc"
 url = "https://pypi.mirrors.ustc.edu.cn/simple/"
 default = true
 secondary = false
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.0"
 pytest = "^7.2.0"
 
+[tool.poetry.group.doc.dependencies]
+jupyter-book = "^0.15.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ai2-kit= "ai2_kit.main:main"
```

### Comparing `ai2_kit-0.3.9/PKG-INFO` & `ai2_kit-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: ai2-kit
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Author: weihong.xu
 Author-email: xuweihong.cn@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: allpairspy (>=2.5.0,<3.0.0)
+Requires-Dist: asaplib (>=0.0.2,<0.0.3)
 Requires-Dist: ase (>=3.22.1,<4.0.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
-Requires-Dist: cp2k-input-tools (>=0.8.2,<0.9.0)
 Requires-Dist: dpdata (>=0.2.13,<0.3.0)
+Requires-Dist: dscribe (==1.2.2)
 Requires-Dist: fabric (>=2.7.1,<3.0.0)
 Requires-Dist: fire (>=0.5.0,<0.6.0)
 Requires-Dist: invoke (>=1.7.3,<2.0.0)
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: mdanalysis (>=2.4.3,<3.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: pymatgen (>=2023.2.22,<2024.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: shortuuid (>=1.0.11,<2.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # ai<sup>2</sup>-kit
 
 [![PyPI version](https://badge.fury.io/py/ai2-kit.svg)](https://badge.fury.io/py/ai2-kit)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ai2-kit)](https://pypi.org/project/ai2-kit/)
 
-A toolkit featured ***a**rtificial **i**ntelligence × **a**b **i**nitio* for computational chemistry research.
+A toolkit featured _**a**rtificial **i**ntelligence × **a**b **i**nitio_ for computational chemistry research.
 
 *Please be advised that `ai2-kit` is still under heavy development and you should expect things to change often. We encourage people to play and explore with `ai2-kit`, and stay tuned with us for more features to come.*
 
 
 ## Feature Highlights
 * Collection of tools to facilitate the development of automated workflows for computational chemistry research.
 * Utilities to execute and manage jobs in local or remote HPC job scheduler.
```

