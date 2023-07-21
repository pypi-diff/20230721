# Comparing `tmp/ddbox-0.1.0.tar.gz` & `tmp/ddbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddbox-0.1.0.tar", max compression
+gzip compressed data, was "ddbox-0.1.1.tar", max compression
```

## Comparing `ddbox-0.1.0.tar` & `ddbox-0.1.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
--rw-r--r--   0        0        0        0 2023-07-21 18:14:30.198837 ddbox-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-02 16:40:01.000000 ddbox-0.1.0/ddbox/__init__.py
--rw-r--r--   0        0        0     6148 2023-07-21 12:57:54.261925 ddbox-0.1.0/ddbox/bin/.DS_Store
--rw-r--r--   0        0        0  4089576 2023-07-21 12:57:33.278474 ddbox-0.1.0/ddbox/bin/vina_1.2.5_linux_x86_64
--rwxr-xr-x   0        0        0  1297344 2023-07-21 12:57:33.571825 ddbox-0.1.0/ddbox/bin/vina_1.2.5_mac_x86_64
--rw-r--r--   0        0        0      195 2023-07-21 17:33:12.086871 ddbox-0.1.0/ddbox/configs.py
--rw-r--r--   0        0        0      707 2023-07-21 18:26:42.676148 ddbox-0.1.0/ddbox/data/torch.py
--rw-r--r--   0        0        0        0 2023-07-21 17:42:23.416142 ddbox-0.1.0/ddbox/data/utils/__init__.py
--rw-r--r--   0        0        0     4041 2023-07-21 18:26:43.637242 ddbox-0.1.0/ddbox/data/utils/loaders.py
--rw-r--r--   0        0        0      320 2023-05-27 09:00:08.000000 ddbox-0.1.0/ddbox/datasets/smallworld.py
--rw-r--r--   0        0        0      495 2023-05-27 08:58:38.000000 ddbox-0.1.0/ddbox/datasets/zinc.py
--rw-r--r--   0        0        0        0 2023-07-21 15:41:03.059597 ddbox-0.1.0/ddbox/docking/utils/__init__.py
--rw-r--r--   0        0        0     4048 2023-07-21 18:26:43.606148 ddbox-0.1.0/ddbox/docking/utils/vina.py
--rw-r--r--   0        0        0     1485 2023-07-21 18:26:42.663565 ddbox-0.1.0/ddbox/docking/vina.py
--rw-r--r--   0        0        0     6148 2023-07-21 11:44:43.785208 ddbox-0.1.0/ddbox/metrics/.DS_Store
--rw-r--r--   0        0        0        0 2023-06-05 17:27:37.000000 ddbox-0.1.0/ddbox/metrics/SA_Score/__init__.py
--rw-r--r--   0        0        0  3848394 2023-06-05 17:33:36.000000 ddbox-0.1.0/ddbox/metrics/SA_Score/fpscores.pkl.gz
--rw-r--r--   0        0        0     5815 2023-06-07 15:48:53.000000 ddbox-0.1.0/ddbox/metrics/SA_Score/sascorer.py
--rw-r--r--   0        0        0      262 2023-06-17 07:00:52.000000 ddbox-0.1.0/ddbox/metrics/__init__.py
--rw-r--r--   0        0        0        0 2023-07-21 11:44:48.652936 ddbox-0.1.0/ddbox/metrics/benchmarks/__init__.py
--rw-r--r--   0        0        0     3267 2023-07-21 11:44:48.653147 ddbox-0.1.0/ddbox/metrics/benchmarks/moses.py
--rw-r--r--   0        0        0      739 2023-06-04 17:35:43.000000 ddbox-0.1.0/ddbox/metrics/data/mcf.csv
--rw-r--r--   0        0        0   207419 2023-06-07 15:48:53.000000 ddbox-0.1.0/ddbox/metrics/data/wehi_pains.csv
--rw-r--r--   0        0        0     2096 2023-07-21 18:26:42.682662 ddbox-0.1.0/ddbox/metrics/distribution_difference.py
--rw-r--r--   0        0        0      415 2023-07-21 18:26:42.668963 ddbox-0.1.0/ddbox/metrics/fcd.py
--rw-r--r--   0        0        0     1636 2023-07-21 18:26:42.678205 ddbox-0.1.0/ddbox/metrics/fraction_passes.py
--rw-r--r--   0        0        0      630 2023-07-21 18:26:42.683229 ddbox-0.1.0/ddbox/metrics/fraction_unique.py
--rw-r--r--   0        0        0      458 2023-06-11 15:03:10.000000 ddbox-0.1.0/ddbox/metrics/fraction_valid.py
--rw-r--r--   0        0        0      906 2023-07-21 18:26:42.679502 ddbox-0.1.0/ddbox/metrics/fragment.py
--rw-r--r--   0        0        0      638 2023-07-21 18:26:42.662217 ddbox-0.1.0/ddbox/metrics/intdiv.py
--rw-r--r--   0        0        0        0 2023-06-17 06:53:06.000000 ddbox-0.1.0/ddbox/metrics/novelty.py
--rw-r--r--   0        0        0     1171 2023-07-21 18:26:42.667781 ddbox-0.1.0/ddbox/metrics/scaffold.py
--rw-r--r--   0        0        0      434 2023-07-21 18:26:42.668394 ddbox-0.1.0/ddbox/metrics/snn.py
--rw-r--r--   0        0        0     3468 2023-06-07 15:48:54.000000 ddbox-0.1.0/ddbox/metrics/utils.py
--rw-r--r--   0        0        0       76 2023-07-21 18:26:42.680031 ddbox-0.1.0/ddbox/molecule/__init__.py
--rw-r--r--   0        0        0     4445 2023-07-21 18:26:42.671450 ddbox-0.1.0/ddbox/molecule/descriptors.py
--rw-r--r--   0        0        0    10805 2023-07-21 18:26:43.660690 ddbox-0.1.0/ddbox/molecule/objects.py
--rw-r--r--   0        0        0       66 2023-06-11 15:02:40.000000 ddbox-0.1.0/ddbox/registries.py
--rw-r--r--   0        0        0     1265 2023-07-21 18:26:43.685212 ddbox-0.1.0/ddbox/utils.py
--rw-r--r--   0        0        0      822 2023-07-21 18:22:00.974968 ddbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 ddbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 18:14:30.198837 ddbox-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-02 16:40:01.000000 ddbox-0.1.1/ddbox/__init__.py
+-rw-r--r--   0        0        0     6148 2023-07-21 12:57:54.261925 ddbox-0.1.1/ddbox/bin/.DS_Store
+-rw-r--r--   0        0        0  4089576 2023-07-21 12:57:33.278474 ddbox-0.1.1/ddbox/bin/vina_1.2.5_linux_x86_64
+-rwxr-xr-x   0        0        0  1297344 2023-07-21 12:57:33.571825 ddbox-0.1.1/ddbox/bin/vina_1.2.5_mac_x86_64
+-rw-r--r--   0        0        0      279 2023-07-21 18:49:24.527234 ddbox-0.1.1/ddbox/configs.py
+-rw-r--r--   0        0        0      707 2023-07-21 18:26:42.676148 ddbox-0.1.1/ddbox/data/torch.py
+-rw-r--r--   0        0        0        0 2023-07-21 17:42:23.416142 ddbox-0.1.1/ddbox/data/utils/__init__.py
+-rw-r--r--   0        0        0     4041 2023-07-21 18:26:43.637242 ddbox-0.1.1/ddbox/data/utils/loaders.py
+-rw-r--r--   0        0        0      320 2023-05-27 09:00:08.000000 ddbox-0.1.1/ddbox/datasets/smallworld.py
+-rw-r--r--   0        0        0      495 2023-05-27 08:58:38.000000 ddbox-0.1.1/ddbox/datasets/zinc.py
+-rw-r--r--   0        0        0        0 2023-07-21 18:52:46.441179 ddbox-0.1.1/ddbox/docking/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 15:41:03.059597 ddbox-0.1.1/ddbox/docking/utils/__init__.py
+-rw-r--r--   0        0        0     4048 2023-07-21 18:26:43.606148 ddbox-0.1.1/ddbox/docking/utils/vina.py
+-rw-r--r--   0        0        0     1409 2023-07-21 18:52:26.381364 ddbox-0.1.1/ddbox/docking/vina.py
+-rw-r--r--   0        0        0     6148 2023-07-21 11:44:43.785208 ddbox-0.1.1/ddbox/metrics/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-05 17:27:37.000000 ddbox-0.1.1/ddbox/metrics/SA_Score/__init__.py
+-rw-r--r--   0        0        0  3848394 2023-06-05 17:33:36.000000 ddbox-0.1.1/ddbox/metrics/SA_Score/fpscores.pkl.gz
+-rw-r--r--   0        0        0     5815 2023-06-07 15:48:53.000000 ddbox-0.1.1/ddbox/metrics/SA_Score/sascorer.py
+-rw-r--r--   0        0        0      262 2023-06-17 07:00:52.000000 ddbox-0.1.1/ddbox/metrics/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-21 11:44:48.652936 ddbox-0.1.1/ddbox/metrics/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3267 2023-07-21 11:44:48.653147 ddbox-0.1.1/ddbox/metrics/benchmarks/moses.py
+-rw-r--r--   0        0        0      739 2023-06-04 17:35:43.000000 ddbox-0.1.1/ddbox/metrics/data/mcf.csv
+-rw-r--r--   0        0        0   207419 2023-06-07 15:48:53.000000 ddbox-0.1.1/ddbox/metrics/data/wehi_pains.csv
+-rw-r--r--   0        0        0     2096 2023-07-21 18:26:42.682662 ddbox-0.1.1/ddbox/metrics/distribution_difference.py
+-rw-r--r--   0        0        0      415 2023-07-21 18:26:42.668963 ddbox-0.1.1/ddbox/metrics/fcd.py
+-rw-r--r--   0        0        0     1636 2023-07-21 18:26:42.678205 ddbox-0.1.1/ddbox/metrics/fraction_passes.py
+-rw-r--r--   0        0        0      630 2023-07-21 18:26:42.683229 ddbox-0.1.1/ddbox/metrics/fraction_unique.py
+-rw-r--r--   0        0        0      458 2023-06-11 15:03:10.000000 ddbox-0.1.1/ddbox/metrics/fraction_valid.py
+-rw-r--r--   0        0        0      906 2023-07-21 18:26:42.679502 ddbox-0.1.1/ddbox/metrics/fragment.py
+-rw-r--r--   0        0        0      638 2023-07-21 18:26:42.662217 ddbox-0.1.1/ddbox/metrics/intdiv.py
+-rw-r--r--   0        0        0        0 2023-06-17 06:53:06.000000 ddbox-0.1.1/ddbox/metrics/novelty.py
+-rw-r--r--   0        0        0     1171 2023-07-21 18:26:42.667781 ddbox-0.1.1/ddbox/metrics/scaffold.py
+-rw-r--r--   0        0        0      434 2023-07-21 18:26:42.668394 ddbox-0.1.1/ddbox/metrics/snn.py
+-rw-r--r--   0        0        0     3468 2023-06-07 15:48:54.000000 ddbox-0.1.1/ddbox/metrics/utils.py
+-rw-r--r--   0        0        0       76 2023-07-21 18:26:42.680031 ddbox-0.1.1/ddbox/molecule/__init__.py
+-rw-r--r--   0        0        0     4445 2023-07-21 18:26:42.671450 ddbox-0.1.1/ddbox/molecule/descriptors.py
+-rw-r--r--   0        0        0    10805 2023-07-21 18:26:43.660690 ddbox-0.1.1/ddbox/molecule/objects.py
+-rw-r--r--   0        0        0       66 2023-06-11 15:02:40.000000 ddbox-0.1.1/ddbox/registries.py
+-rw-r--r--   0        0        0     1265 2023-07-21 18:26:43.685212 ddbox-0.1.1/ddbox/utils.py
+-rw-r--r--   0        0        0      822 2023-07-21 18:54:43.187444 ddbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1330 1970-01-01 00:00:00.000000 ddbox-0.1.1/PKG-INFO
```

### Comparing `ddbox-0.1.0/ddbox/bin/.DS_Store` & `ddbox-0.1.1/ddbox/bin/.DS_Store`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/bin/vina_1.2.5_linux_x86_64` & `ddbox-0.1.1/ddbox/bin/vina_1.2.5_linux_x86_64`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/bin/vina_1.2.5_mac_x86_64` & `ddbox-0.1.1/ddbox/bin/vina_1.2.5_mac_x86_64`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/data/torch.py` & `ddbox-0.1.1/ddbox/data/torch.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/data/utils/loaders.py` & `ddbox-0.1.1/ddbox/data/utils/loaders.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/docking/utils/vina.py` & `ddbox-0.1.1/ddbox/docking/utils/vina.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/docking/vina.py` & `ddbox-0.1.1/ddbox/docking/vina.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 import logging
-import os
-import platform
 from subprocess import PIPE, Popen
-from typing import List, Tuple
+from typing import Tuple
 
 from ddbox.docking.utils.vina import (
     download_if_needed,
     get_config_filepath,
     get_pdbqt_file_from_smiles,
     get_pdbqt_filepath,
     get_vina_filepath,
 )
-from ddbox.utils import get_random_uuid_hex
 
 logger = logging.getLogger(__name__)
 
 
 def vina_docking(receptor_id: str, ligand_smiles: str, center: Tuple[float, float, float] | None = None, size: Tuple[float, float, float] | None = None):
     download_if_needed(receptor_id)
```

### Comparing `ddbox-0.1.0/ddbox/metrics/.DS_Store` & `ddbox-0.1.1/ddbox/metrics/.DS_Store`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/SA_Score/fpscores.pkl.gz` & `ddbox-0.1.1/ddbox/metrics/SA_Score/fpscores.pkl.gz`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/SA_Score/sascorer.py` & `ddbox-0.1.1/ddbox/metrics/SA_Score/sascorer.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/benchmarks/moses.py` & `ddbox-0.1.1/ddbox/metrics/benchmarks/moses.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/data/mcf.csv` & `ddbox-0.1.1/ddbox/metrics/data/mcf.csv`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/data/wehi_pains.csv` & `ddbox-0.1.1/ddbox/metrics/data/wehi_pains.csv`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/distribution_difference.py` & `ddbox-0.1.1/ddbox/metrics/distribution_difference.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/fraction_passes.py` & `ddbox-0.1.1/ddbox/metrics/fraction_passes.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/fraction_unique.py` & `ddbox-0.1.1/ddbox/metrics/fraction_unique.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/fragment.py` & `ddbox-0.1.1/ddbox/metrics/fragment.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/intdiv.py` & `ddbox-0.1.1/ddbox/metrics/intdiv.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/scaffold.py` & `ddbox-0.1.1/ddbox/metrics/scaffold.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/metrics/utils.py` & `ddbox-0.1.1/ddbox/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/molecule/descriptors.py` & `ddbox-0.1.1/ddbox/molecule/descriptors.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/molecule/objects.py` & `ddbox-0.1.1/ddbox/molecule/objects.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/ddbox/utils.py` & `ddbox-0.1.1/ddbox/utils.py`

 * *Files identical despite different names*

### Comparing `ddbox-0.1.0/pyproject.toml` & `ddbox-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ddbox"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Azamat <unawares15@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 urllib3 = "1.26.15"
```

### Comparing `ddbox-0.1.0/PKG-INFO` & `ddbox-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Azamat
 Author-email: unawares15@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

