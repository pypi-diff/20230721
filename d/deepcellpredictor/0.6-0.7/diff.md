# Comparing `tmp/deepcellpredictor-0.6.tar.gz` & `tmp/deepcellpredictor-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcellpredictor-0.6.tar", last modified: Thu Jul 20 22:07:40 2023, max compression
+gzip compressed data, was "deepcellpredictor-0.7.tar", last modified: Thu Jul 20 22:16:56 2023, max compression
```

## Comparing `deepcellpredictor-0.6.tar` & `deepcellpredictor-0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:07:40.871257 deepcellpredictor-0.6/
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:07:40.867257 deepcellpredictor-0.6/DCP/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.6/DCP/ModelPlanner.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8286 2023-07-20 15:52:22.000000 deepcellpredictor-0.6/DCP/VAEtorch.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.6/DCP/__init__.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11581 2023-07-20 15:52:22.000000 deepcellpredictor-0.6/DCP/deep_predictor.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.6/DCP/flow.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.6/DCP/utils.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.6/LICENSE
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      442 2023-07-20 22:07:40.867257 deepcellpredictor-0.6/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.6/README.md
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:07:40.867257 deepcellpredictor-0.6/deepcellpredictor.egg-info/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      442 2023-07-20 22:07:40.000000 deepcellpredictor-0.6/deepcellpredictor.egg-info/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 22:07:40.000000 deepcellpredictor-0.6/deepcellpredictor.egg-info/SOURCES.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 22:07:40.000000 deepcellpredictor-0.6/deepcellpredictor.egg-info/dependency_links.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       84 2023-07-20 22:07:40.000000 deepcellpredictor-0.6/deepcellpredictor.egg-info/requires.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 22:07:40.000000 deepcellpredictor-0.6/deepcellpredictor.egg-info/top_level.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 22:07:40.871257 deepcellpredictor-0.6/setup.cfg
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      790 2023-07-20 22:07:07.000000 deepcellpredictor-0.6/setup.py
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:16:56.112755 deepcellpredictor-0.7/
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:16:56.112755 deepcellpredictor-0.7/DCP/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.7/DCP/ModelPlanner.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8286 2023-07-20 15:52:22.000000 deepcellpredictor-0.7/DCP/VAEtorch.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.7/DCP/__init__.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11629 2023-07-20 22:15:36.000000 deepcellpredictor-0.7/DCP/deep_predictor.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.7/DCP/flow.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.7/DCP/utils.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.7/LICENSE
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      442 2023-07-20 22:16:56.112755 deepcellpredictor-0.7/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.7/README.md
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 22:16:56.112755 deepcellpredictor-0.7/deepcellpredictor.egg-info/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      442 2023-07-20 22:16:55.000000 deepcellpredictor-0.7/deepcellpredictor.egg-info/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 22:16:56.000000 deepcellpredictor-0.7/deepcellpredictor.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 22:16:55.000000 deepcellpredictor-0.7/deepcellpredictor.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       84 2023-07-20 22:16:55.000000 deepcellpredictor-0.7/deepcellpredictor.egg-info/requires.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 22:16:56.000000 deepcellpredictor-0.7/deepcellpredictor.egg-info/top_level.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 22:16:56.112755 deepcellpredictor-0.7/setup.cfg
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      790 2023-07-20 22:16:39.000000 deepcellpredictor-0.7/setup.py
```

### Comparing `deepcellpredictor-0.6/DCP/ModelPlanner.py` & `deepcellpredictor-0.7/DCP/ModelPlanner.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.6/DCP/VAEtorch.py` & `deepcellpredictor-0.7/DCP/VAEtorch.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.6/DCP/deep_predictor.py` & `deepcellpredictor-0.7/DCP/deep_predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import math
 import torch
+import VAEtorch
+import flow
+import ModelPlanner
 from VAEtorch import *
 from pytorch_lightning import LightningDataModule, LightningModule
 from anndata import AnnData
 from ModelPlanner import Planner 
 from pytorch_lightning import Trainer
 from typing import List
 from flow import *
```

### Comparing `deepcellpredictor-0.6/DCP/flow.py` & `deepcellpredictor-0.7/DCP/flow.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.6/DCP/utils.py` & `deepcellpredictor-0.7/DCP/utils.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.6/LICENSE` & `deepcellpredictor-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.6/setup.py` & `deepcellpredictor-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.6'
+VERSION = '0.7'
 DESCRIPTION = "a transfer learning approach that explicitly models changes in transcriptional variance using a combination of variational autoencoders and normalizing flows"
 
 setup(
     name='deepcellpredictor',
     version=VERSION,
     description='transfer learning approach',
     long_description=DESCRIPTION,
```

