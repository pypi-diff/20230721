# Comparing `tmp/bojaxns-1.0.0.tar.gz` & `tmp/bojaxns-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bojaxns-1.0.0.tar", last modified: Thu Jul 20 23:17:57 2023, max compression
+gzip compressed data, was "bojaxns-1.0.1.tar", last modified: Thu Jul 20 23:49:52 2023, max compression
```

## Comparing `bojaxns-1.0.0.tar` & `bojaxns-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:17:57.638634 bojaxns-1.0.0/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-06-20 14:43:21.000000 bojaxns-1.0.0/LICENSE
--rw-rw-r--   0 albert    (1000) albert    (1000)     2082 2023-07-20 23:17:57.638634 bojaxns-1.0.0/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)     1631 2023-07-20 22:52:41.000000 bojaxns-1.0.0/README.md
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:17:57.634634 bojaxns-1.0.0/bojax/
--rw-rw-r--   0 albert    (1000) albert    (1000)      189 2023-07-20 16:10:25.000000 bojaxns-1.0.0/bojax/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-06-29 23:24:48.000000 bojaxns-1.0.0/bojax/base.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2218 2023-06-07 17:50:36.000000 bojaxns-1.0.0/bojax/basic.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3278 2023-07-20 22:11:27.000000 bojaxns-1.0.0/bojax/experiment.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:17:57.634634 bojaxns-1.0.0/bojax/gaussian_process_formulation/
--rw-rw-r--   0 albert    (1000) albert    (1000)       68 2023-06-29 23:24:48.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    10670 2023-07-20 16:10:25.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)    15663 2023-07-20 12:35:56.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/distribution_math.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9084 2023-06-29 23:40:14.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/multi_step_lookahead.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:17:57.638634 bojaxns-1.0.0/bojax/gaussian_process_formulation/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-20 16:10:25.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     4898 2023-07-20 22:11:27.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/tests/test_bayesian_optimiser.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5935 2023-07-20 16:10:25.000000 bojaxns-1.0.0/bojax/gaussian_process_formulation/tests/test_distribution_maths.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     5067 2023-07-20 12:35:56.000000 bojaxns-1.0.0/bojax/parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     9495 2023-07-20 12:35:56.000000 bojaxns-1.0.0/bojax/service.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:17:57.638634 bojaxns-1.0.0/bojax/tests/
--rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 bojaxns-1.0.0/bojax/tests/__init__.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2175 2023-06-21 15:30:00.000000 bojaxns-1.0.0/bojax/tests/test_experiment.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     3504 2023-07-20 16:10:25.000000 bojaxns-1.0.0/bojax/tests/test_parameter_space.py
--rw-rw-r--   0 albert    (1000) albert    (1000)      620 2023-07-20 12:35:56.000000 bojaxns-1.0.0/bojax/tests/test_utils.py
--rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-20 22:11:27.000000 bojaxns-1.0.0/bojax/utils.py
-drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:17:57.638634 bojaxns-1.0.0/bojaxns.egg-info/
--rw-rw-r--   0 albert    (1000) albert    (1000)     2082 2023-07-20 23:17:57.000000 bojaxns-1.0.0/bojaxns.egg-info/PKG-INFO
--rw-rw-r--   0 albert    (1000) albert    (1000)      858 2023-07-20 23:17:57.000000 bojaxns-1.0.0/bojaxns.egg-info/SOURCES.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-20 23:17:57.000000 bojaxns-1.0.0/bojaxns.egg-info/dependency_links.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)        6 2023-07-20 23:17:57.000000 bojaxns-1.0.0/bojaxns.egg-info/top_level.txt
--rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-04-19 01:15:53.000000 bojaxns-1.0.0/pyproject.toml
--rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-20 23:17:57.638634 bojaxns-1.0.0/setup.cfg
--rwxrwxr-x   0 albert    (1000) albert    (1000)      997 2023-07-20 23:17:46.000000 bojaxns-1.0.0/setup.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2553 2023-06-20 14:43:21.000000 bojaxns-1.0.1/LICENSE
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2106 2023-07-20 23:49:52.601389 bojaxns-1.0.1/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)     1655 2023-07-20 23:32:59.000000 bojaxns-1.0.1/README.md
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/
+-rw-rw-r--   0 albert    (1000) albert    (1000)      199 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5038 2023-06-29 23:24:48.000000 bojaxns-1.0.1/bojaxns/base.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2218 2023-06-07 17:50:36.000000 bojaxns-1.0.1/bojaxns/basic.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3282 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/experiment.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/
+-rw-rw-r--   0 albert    (1000) albert    (1000)       70 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    10678 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)    15665 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/distribution_math.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9088 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/multi_step_lookahead.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-20 16:10:25.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     4904 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5939 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     5069 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     9503 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/service.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns/tests/
+-rw-rw-r--   0 albert    (1000) albert    (1000)        0 2022-10-13 02:52:05.000000 bojaxns-1.0.1/bojaxns/tests/__init__.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2181 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/tests/test_experiment.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     3508 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/tests/test_parameter_space.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)      622 2023-07-20 23:19:20.000000 bojaxns-1.0.1/bojaxns/tests/test_utils.py
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2986 2023-07-20 22:11:27.000000 bojaxns-1.0.1/bojaxns/utils.py
+drwxrwxr-x   0 albert    (1000) albert    (1000)        0 2023-07-20 23:49:52.601389 bojaxns-1.0.1/bojaxns.egg-info/
+-rw-rw-r--   0 albert    (1000) albert    (1000)     2106 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/PKG-INFO
+-rw-rw-r--   0 albert    (1000) albert    (1000)      894 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/SOURCES.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        1 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/dependency_links.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)        8 2023-07-20 23:49:52.000000 bojaxns-1.0.1/bojaxns.egg-info/top_level.txt
+-rw-rw-r--   0 albert    (1000) albert    (1000)      103 2023-04-19 01:15:53.000000 bojaxns-1.0.1/pyproject.toml
+-rw-rw-r--   0 albert    (1000) albert    (1000)       38 2023-07-20 23:49:52.601389 bojaxns-1.0.1/setup.cfg
+-rwxrwxr-x   0 albert    (1000) albert    (1000)      997 2023-07-20 23:49:43.000000 bojaxns-1.0.1/setup.py
```

### Comparing `bojaxns-1.0.0/LICENSE` & `bojaxns-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.0/PKG-INFO` & `bojaxns-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojax
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Python](https://img.shields.io/pypi/pyversions/bojax.svg)](https://badge.fury.io/py/bojax)
-[![PyPI](https://badge.fury.io/py/bojax.svg)](https://badge.fury.io/py/bojax)
+[![Python](https://img.shields.io/pypi/pyversions/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
+[![PyPI](https://badge.fury.io/py/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
 
 Main
 Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
 Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ## Mission: _To make advanced Bayesian Optimisation easy._
 
 # What is it?
 
-Bojax is:
+Bojaxns is:
 
 1) a Bayesian Optimisation package for easily performing advanced non-myopic Bayesian optimisation.
 2) using [JAXNS](https://github.com/JoshuaAlbert/jaxns) under the hood to marginalise over multiple models.
 3) using multi-step lookahead to plan out your next step.
 4) available for academic use and non-commercial use (without permission) read the license.
 
 # Documentation
 
 For examples, check out the [documentation](https://bojax.readthedocs.io/) (still in progress).
 
 # Install
 
 **Notes:**
 
-1. Bojax requires >= Python 3.9.
+1. Bojaxns requires >= Python 3.9.
 2. It is always highly recommended to use a unique virtual environment for each project.
    To use `miniconda`, have it installed, and run
 
 ```bash
 # To create a new env, if necessary
-conda create -n bojax_py python=3.11
-conda activate bojax_py
+conda create -n bojaxns_py python=3.11
+conda activate bojaxns_py
 ```
 
 ## For end users
 
 Install directly from PyPi,
 
 ```bash
-pip install bojax
+pip install bojaxns
 ```
 
 ## For development
 
-Clone repo `git clone https://www.github.com/JoshuaAlbert/bojax.git`, and install:
+Clone repo `git clone https://www.github.com/JoshuaAlbert/bojaxns.git`, and install:
 
 ```bash
-cd jaxns
+cd bojaxns
 pip install -r requirements.txt
 pip install -r requirements-tests.txt
 pip install .
 ```
 # Change Log
 
-20 July, 2023 -- Bojax 1.0.0 released
+20 July, 2023 -- Bojaxns 1.0.0 released
```

### Comparing `bojaxns-1.0.0/README.md` & `bojaxns-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-[![Python](https://img.shields.io/pypi/pyversions/bojax.svg)](https://badge.fury.io/py/bojax)
-[![PyPI](https://badge.fury.io/py/bojax.svg)](https://badge.fury.io/py/bojax)
+[![Python](https://img.shields.io/pypi/pyversions/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
+[![PyPI](https://badge.fury.io/py/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
 
 Main
 Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
 Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ## Mission: _To make advanced Bayesian Optimisation easy._
 
 # What is it?
 
-Bojax is:
+Bojaxns is:
 
 1) a Bayesian Optimisation package for easily performing advanced non-myopic Bayesian optimisation.
 2) using [JAXNS](https://github.com/JoshuaAlbert/jaxns) under the hood to marginalise over multiple models.
 3) using multi-step lookahead to plan out your next step.
 4) available for academic use and non-commercial use (without permission) read the license.
 
 # Documentation
 
 For examples, check out the [documentation](https://bojax.readthedocs.io/) (still in progress).
 
 # Install
 
 **Notes:**
 
-1. Bojax requires >= Python 3.9.
+1. Bojaxns requires >= Python 3.9.
 2. It is always highly recommended to use a unique virtual environment for each project.
    To use `miniconda`, have it installed, and run
 
 ```bash
 # To create a new env, if necessary
-conda create -n bojax_py python=3.11
-conda activate bojax_py
+conda create -n bojaxns_py python=3.11
+conda activate bojaxns_py
 ```
 
 ## For end users
 
 Install directly from PyPi,
 
 ```bash
-pip install bojax
+pip install bojaxns
 ```
 
 ## For development
 
-Clone repo `git clone https://www.github.com/JoshuaAlbert/bojax.git`, and install:
+Clone repo `git clone https://www.github.com/JoshuaAlbert/bojaxns.git`, and install:
 
 ```bash
-cd jaxns
+cd bojaxns
 pip install -r requirements.txt
 pip install -r requirements-tests.txt
 pip install .
 ```
 # Change Log
 
-20 July, 2023 -- Bojax 1.0.0 released
+20 July, 2023 -- Bojaxns 1.0.0 released
```

### Comparing `bojaxns-1.0.0/bojax/base.py` & `bojaxns-1.0.1/bojaxns/base.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.0/bojax/basic.py` & `bojaxns-1.0.1/bojaxns/basic.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.0/bojax/experiment.py` & `bojaxns-1.0.1/bojaxns/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from typing import Literal, List, Dict, Union
 from uuid import uuid4
 
 from pydantic import BaseModel, Field, validator, conint, confloat
 
-from bojax.parameter_space import ParameterSpace
-from bojax.utils import current_utc, build_example
+from bojaxns.parameter_space import ParameterSpace
+from bojaxns.utils import current_utc, build_example
 
 __all__ = [
     'FloatValue',
     'IntValue',
     'Trial',
     'TrialUpdate',
     'OptimisationExperiment',
```

### Comparing `bojaxns-1.0.0/bojax/gaussian_process_formulation/bayesian_optimiser.py` & `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/bayesian_optimiser.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from etils.array_types import PRNGKey
 from jax import random, numpy as jnp, vmap
 from jax._src.lax.control_flow import scan
 from jaxns import Model, TerminationCondition, NestedSamplerResults, ApproximateNestedSampler, \
     UniformSampler, UniDimSliceSampler
 from jaxns.types import float_type
 
-from bojax.base import AbstractAcquisition, MarginalisedAcquisitionFunction, MarginalisationData
-from bojax.experiment import OptimisationExperiment
-from bojax.gaussian_process_formulation.distribution_math import GaussianProcessData, \
+from bojaxns.base import AbstractAcquisition, MarginalisedAcquisitionFunction, MarginalisationData
+from bojaxns.experiment import OptimisationExperiment
+from bojaxns.gaussian_process_formulation.distribution_math import GaussianProcessData, \
     GaussianProcessConditionalPredictiveFactory, ExpectedImprovementAcquisitionFactory, TopTwoAcquisitionFactory
-from bojax.gaussian_process_formulation.multi_step_lookahead import run_multi_lookahead, convert_tree_to_graph
+from bojaxns.gaussian_process_formulation.multi_step_lookahead import run_multi_lookahead, convert_tree_to_graph
 
 tfpb = tfp.bijectors
 
 
 class BayesianOptimiser:
     def __init__(self, experiment: OptimisationExperiment, num_parallel_solvers: int = 1, beta: float = 0.5,
                  S: int = 512):
```

### Comparing `bojaxns-1.0.0/bojax/gaussian_process_formulation/distribution_math.py` & `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/distribution_math.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from jax import numpy as jnp, tree_map
 from jax._src.scipy.linalg import solve_triangular
 from jaxns import PriorModelGen, Prior, Categorical
 from jaxns.prior import PriorModelType
 from jaxns.types import float_type
 from tensorflow_probability.substrates import jax as tfp
 
-from bojax.base import _assert_rank, _assert_same_leading_dim, ConditionalPredictive, ConditionalPredictiveFactory, \
+from bojaxns.base import _assert_rank, _assert_same_leading_dim, ConditionalPredictive, ConditionalPredictiveFactory, \
     AbstractAcquisition, AcquisitionFactory
 
 tfpd = tfp.distributions
 
 
 def log_normal(x, mean, cov):
     L = jnp.linalg.cholesky(cov)
```

### Comparing `bojaxns-1.0.0/bojax/gaussian_process_formulation/multi_step_lookahead.py` & `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/multi_step_lookahead.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import chex
 import jax
 import jax.numpy as jnp
 import mctx
 from jax import tree_map
 from mctx import PolicyOutput, GumbelMuZeroExtraData, RootFnOutput, RecurrentFn
 
-from bojax.base import MarginalisedConditionalPredictive, MarginalisationData, MarginalisedAcquisitionFunction
-from bojax.gaussian_process_formulation.distribution_math import GaussianProcessData, \
+from bojaxns.base import MarginalisedConditionalPredictive, MarginalisationData, MarginalisedAcquisitionFunction
+from bojaxns.gaussian_process_formulation.distribution_math import GaussianProcessData, \
     GaussianProcessConditionalPredictiveFactory, ExpectedImprovementAcquisitionFactory
 
 
 def convert_tree_to_graph(
         tree: mctx.Tree,
         action_labels: Optional[Sequence[str]] = None,
         batch_index: int = 0
```

### Comparing `bojaxns-1.0.0/bojax/gaussian_process_formulation/tests/test_bayesian_optimiser.py` & `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import List, Union
 from uuid import uuid4
 
 import pylab as plt
 from jax import random, numpy as jnp
 from pydantic import BaseModel, Field
 
-from bojax.experiment import NewExperimentRequest, Trial, TrialUpdate
-from bojax.parameter_space import ParameterSpace, Parameter, ContinuousPrior, IntegerPrior, CategoricalPrior
-from bojax.service import BayesianOptimisation
+from bojaxns.experiment import NewExperimentRequest, Trial, TrialUpdate
+from bojaxns.parameter_space import ParameterSpace, Parameter, ContinuousPrior, IntegerPrior, CategoricalPrior
+from bojaxns.service import BayesianOptimisation
 
 
 def test_bayesian_optimisation():
     num_steps = 11
 
     def objective(x):
         return -0.5 * jnp.sum(x ** 4 - 16 * x ** 2 + 5 * x)
```

### Comparing `bojaxns-1.0.0/bojax/gaussian_process_formulation/tests/test_distribution_maths.py` & `bojaxns-1.0.1/bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from functools import partial
 from time import monotonic_ns
 
 import jax
 from jax import numpy as jnp
 from tensorflow_probability.substrates import jax as tfp
 
-from bojax import GaussianProcessData
-from bojax.gaussian_process_formulation.distribution_math import GaussianProcessConditionalPredictive
+from bojaxns import GaussianProcessData
+from bojaxns.gaussian_process_formulation.distribution_math import GaussianProcessConditionalPredictive
 
 
 def test_broadcast_lengthscale():
     # Define your length scales.
     # For example, for a 3-dimensional feature vector:
     length_scale = jnp.asarray([1.0, 2.0, 3.0])
```

### Comparing `bojaxns-1.0.0/bojax/parameter_space.py` & `bojaxns-1.0.1/bojaxns/parameter_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tensorflow_probability.substrates.jax as tfp
 from jaxns import Prior, PriorModelGen
 from jaxns.prior import PriorModelType
 from jaxns.special_priors import Categorical
 from jaxns.types import float_type
 from pydantic import BaseModel, Field, validator, confloat
 
-from bojax.utils import build_example
+from bojaxns.utils import build_example
 
 tfpd = tfp.distributions
 
 __all__ = [
     'ContinuousPrior',
     'IntegerPrior',
     'CategoricalPrior',
```

### Comparing `bojaxns-1.0.0/bojax/service.py` & `bojaxns-1.0.1/bojaxns/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 import numpy as np
 import pylab as plt
 from jax import random, numpy as jnp
 from jax._src.random import PRNGKey
 from jaxns.prior import parse_prior, PriorModelType, transform
 from matplotlib import dates as mdates
 
-from bojax.experiment import OptimisationExperiment, NewExperimentRequest, Trial, FloatValue, \
+from bojaxns.experiment import OptimisationExperiment, NewExperimentRequest, Trial, FloatValue, \
     IntValue, TrialUpdate
-from bojax.gaussian_process_formulation.bayesian_optimiser import BayesianOptimiser
-from bojax.parameter_space import build_prior_model, ContinuousPrior, IntegerPrior, CategoricalPrior
-from bojax.utils import latin_hypercube
+from bojaxns.gaussian_process_formulation.bayesian_optimiser import BayesianOptimiser
+from bojaxns.parameter_space import build_prior_model, ContinuousPrior, IntegerPrior, CategoricalPrior
+from bojaxns.utils import latin_hypercube
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 __all__ = [
     'InvalidTrial',
     'BayesianOptimisation'
```

### Comparing `bojaxns-1.0.0/bojax/tests/test_experiment.py` & `bojaxns-1.0.1/bojaxns/tests/test_experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jax import numpy as jnp
 
-from bojax.experiment import Trial, FloatValue, IntValue, OptimisationExperiment, \
+from bojaxns.experiment import Trial, FloatValue, IntValue, OptimisationExperiment, \
     TrialUpdate
-from bojax.parameter_space import Parameter, IntegerPrior, CategoricalPrior, ParameterSpace, \
+from bojaxns.parameter_space import Parameter, IntegerPrior, CategoricalPrior, ParameterSpace, \
     ContinuousPrior
-from bojax.utils import current_utc
+from bojaxns.utils import current_utc
 
 
 def test_optimisation_experiment():
     param1 = Parameter(
         name='continuous',
         prior=ContinuousPrior(
             lower=0,
```

### Comparing `bojaxns-1.0.0/bojax/tests/test_parameter_space.py` & `bojaxns-1.0.1/bojaxns/tests/test_parameter_space.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from jax import vmap, random, numpy as jnp
 from jaxns.prior import transform, parse_prior
 from jaxns.types import float_type
 
-from bojax.parameter_space import IntegerPrior, CategoricalPrior, ParameterSpace, \
+from bojaxns.parameter_space import IntegerPrior, CategoricalPrior, ParameterSpace, \
     Parameter, build_prior_model, ContinuousPrior
-from bojax.utils import build_example
+from bojaxns.utils import build_example
 
 
 def test_serialisation():
     for m in [
         IntegerPrior,
         CategoricalPrior,
         ContinuousPrior
```

### Comparing `bojaxns-1.0.0/bojax/tests/test_utils.py` & `bojaxns-1.0.1/bojaxns/tests/test_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from jax import numpy as jnp
 
-from bojax.utils import latin_hypercube
+from bojaxns.utils import latin_hypercube
 
 
 def test_latin_hyper_cube():
     num_samples = 50
     ndim = 2
     samples = latin_hypercube(42, num_samples, ndim)
     s = jnp.sort(samples, axis=0) * num_samples
```

### Comparing `bojaxns-1.0.0/bojax/utils.py` & `bojaxns-1.0.1/bojaxns/utils.py`

 * *Files identical despite different names*

### Comparing `bojaxns-1.0.0/bojaxns.egg-info/PKG-INFO` & `bojaxns-1.0.1/bojaxns.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 Metadata-Version: 2.1
 Name: bojaxns
-Version: 1.0.0
+Version: 1.0.1
 Summary: Bayesian Optimisation with JAXNS
 Home-page: https://github.com/joshuaalbert/bojax
 Author: Joshua G. Albert
 Author-email: albert@strw.leidenuniv.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Python](https://img.shields.io/pypi/pyversions/bojax.svg)](https://badge.fury.io/py/bojax)
-[![PyPI](https://badge.fury.io/py/bojax.svg)](https://badge.fury.io/py/bojax)
+[![Python](https://img.shields.io/pypi/pyversions/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
+[![PyPI](https://badge.fury.io/py/bojaxns.svg)](https://badge.fury.io/py/bojaxns)
 
 Main
 Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=main)
 
 Develop
 Status: ![Workflow name](https://github.com/JoshuaAlbert/bojax/actions/workflows/unittests.yml/badge.svg?branch=develop)
 
 ## Mission: _To make advanced Bayesian Optimisation easy._
 
 # What is it?
 
-Bojax is:
+Bojaxns is:
 
 1) a Bayesian Optimisation package for easily performing advanced non-myopic Bayesian optimisation.
 2) using [JAXNS](https://github.com/JoshuaAlbert/jaxns) under the hood to marginalise over multiple models.
 3) using multi-step lookahead to plan out your next step.
 4) available for academic use and non-commercial use (without permission) read the license.
 
 # Documentation
 
 For examples, check out the [documentation](https://bojax.readthedocs.io/) (still in progress).
 
 # Install
 
 **Notes:**
 
-1. Bojax requires >= Python 3.9.
+1. Bojaxns requires >= Python 3.9.
 2. It is always highly recommended to use a unique virtual environment for each project.
    To use `miniconda`, have it installed, and run
 
 ```bash
 # To create a new env, if necessary
-conda create -n bojax_py python=3.11
-conda activate bojax_py
+conda create -n bojaxns_py python=3.11
+conda activate bojaxns_py
 ```
 
 ## For end users
 
 Install directly from PyPi,
 
 ```bash
-pip install bojax
+pip install bojaxns
 ```
 
 ## For development
 
-Clone repo `git clone https://www.github.com/JoshuaAlbert/bojax.git`, and install:
+Clone repo `git clone https://www.github.com/JoshuaAlbert/bojaxns.git`, and install:
 
 ```bash
-cd jaxns
+cd bojaxns
 pip install -r requirements.txt
 pip install -r requirements-tests.txt
 pip install .
 ```
 # Change Log
 
-20 July, 2023 -- Bojax 1.0.0 released
+20 July, 2023 -- Bojaxns 1.0.0 released
```

### Comparing `bojaxns-1.0.0/bojaxns.egg-info/SOURCES.txt` & `bojaxns-1.0.1/bojaxns.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-./bojax/__init__.py
-./bojax/base.py
-./bojax/basic.py
-./bojax/experiment.py
-./bojax/parameter_space.py
-./bojax/service.py
-./bojax/utils.py
-./bojax/gaussian_process_formulation/__init__.py
-./bojax/gaussian_process_formulation/bayesian_optimiser.py
-./bojax/gaussian_process_formulation/distribution_math.py
-./bojax/gaussian_process_formulation/multi_step_lookahead.py
-./bojax/gaussian_process_formulation/tests/__init__.py
-./bojax/gaussian_process_formulation/tests/test_bayesian_optimiser.py
-./bojax/gaussian_process_formulation/tests/test_distribution_maths.py
-./bojax/tests/__init__.py
-./bojax/tests/test_experiment.py
-./bojax/tests/test_parameter_space.py
-./bojax/tests/test_utils.py
+./bojaxns/__init__.py
+./bojaxns/base.py
+./bojaxns/basic.py
+./bojaxns/experiment.py
+./bojaxns/parameter_space.py
+./bojaxns/service.py
+./bojaxns/utils.py
 ./bojaxns.egg-info/PKG-INFO
 ./bojaxns.egg-info/SOURCES.txt
 ./bojaxns.egg-info/dependency_links.txt
-./bojaxns.egg-info/top_level.txt
+./bojaxns.egg-info/top_level.txt
+./bojaxns/gaussian_process_formulation/__init__.py
+./bojaxns/gaussian_process_formulation/bayesian_optimiser.py
+./bojaxns/gaussian_process_formulation/distribution_math.py
+./bojaxns/gaussian_process_formulation/multi_step_lookahead.py
+./bojaxns/gaussian_process_formulation/tests/__init__.py
+./bojaxns/gaussian_process_formulation/tests/test_bayesian_optimiser.py
+./bojaxns/gaussian_process_formulation/tests/test_distribution_maths.py
+./bojaxns/tests/__init__.py
+./bojaxns/tests/test_experiment.py
+./bojaxns/tests/test_parameter_space.py
+./bojaxns/tests/test_utils.py
```

### Comparing `bojaxns-1.0.0/setup.py` & `bojaxns-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #     for line in fh:
 #         setup_requires.append(line)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='bojaxns',
-      version='1.0.0',
+      version='1.0.1',
       description='Bayesian Optimisation with JAXNS',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/joshuaalbert/bojax",
       author='Joshua G. Albert',
       author_email='albert@strw.leidenuniv.nl',
       setup_requires=setup_requires,
```

