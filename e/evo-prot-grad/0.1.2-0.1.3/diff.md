# Comparing `tmp/evo_prot_grad-0.1.2.tar.gz` & `tmp/evo_prot_grad-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_prot_grad-0.1.2.tar", last modified: Tue Jul 18 04:26:27 2023, max compression
+gzip compressed data, was "evo_prot_grad-0.1.3.tar", last modified: Fri Jul 21 02:13:05 2023, max compression
```

## Comparing `evo_prot_grad-0.1.2.tar` & `evo_prot_grad-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.020910 evo_prot_grad-0.1.2/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5007 2023-07-18 04:26:27.020617 evo_prot_grad-0.1.2/PKG-INFO
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     4278 2023-07-18 03:07:17.000000 evo_prot_grad-0.1.2/README.md
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.010586 evo_prot_grad-0.1.2/evo_prot_grad/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2343 2023-07-17 23:30:29.000000 evo_prot_grad-0.1.2/evo_prot_grad/__init__.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.015182 evo_prot_grad-0.1.2/evo_prot_grad/common/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-15 22:00:24.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2028 2023-07-02 17:16:56.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/embeddings.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    14982 2023-07-18 03:43:54.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/sampler.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2751 2023-07-17 13:44:18.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/tokenizers.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2636 2023-07-06 22:37:51.000000 evo_prot_grad-0.1.2/evo_prot_grad/common/utils.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.017848 evo_prot_grad-0.1.2/evo_prot_grad/experts/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-21 13:33:11.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    10623 2023-07-17 14:44:58.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/base_experts.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2986 2023-07-17 14:45:12.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/bert_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3015 2023-07-17 13:49:07.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/causallm_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2944 2023-07-17 13:48:59.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/esm_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3292 2023-07-17 14:45:29.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/evcouplings_expert.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1490 2023-07-17 13:41:13.000000 evo_prot_grad-0.1.2/evo_prot_grad/experts/onehot_downstream_regression_expert.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.018995 evo_prot_grad-0.1.2/evo_prot_grad/models/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      108 2023-06-21 12:05:07.000000 evo_prot_grad-0.1.2/evo_prot_grad/models/__init__.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1939 2023-07-02 21:00:15.000000 evo_prot_grad-0.1.2/evo_prot_grad/models/downstream_cnn.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    11712 2023-07-18 04:21:56.000000 evo_prot_grad-0.1.2/evo_prot_grad/models/potts.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.012778 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5007 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/PKG-INFO
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      847 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/SOURCES.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        1 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/dependency_links.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       28 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/requires.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       14 2023-07-18 04:26:26.000000 evo_prot_grad-0.1.2/evo_prot_grad.egg-info/top_level.txt
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       38 2023-07-18 04:26:27.021018 evo_prot_grad-0.1.2/setup.cfg
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1403 2023-07-18 04:25:50.000000 evo_prot_grad-0.1.2/setup.py
-drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-18 04:26:27.020137 evo_prot_grad-0.1.2/test/
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1611 2023-07-17 14:11:23.000000 evo_prot_grad-0.1.2/test/test_experts.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5099 2023-07-06 23:52:27.000000 evo_prot_grad-0.1.2/test/test_sampler.py
--rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3812 2023-07-17 14:14:09.000000 evo_prot_grad-0.1.2/test/test_utils.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.215789 evo_prot_grad-0.1.3/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5109 2023-07-21 02:13:05.215480 evo_prot_grad-0.1.3/PKG-INFO
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     4380 2023-07-18 04:32:27.000000 evo_prot_grad-0.1.3/README.md
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.205463 evo_prot_grad-0.1.3/evo_prot_grad/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2343 2023-07-17 23:30:29.000000 evo_prot_grad-0.1.3/evo_prot_grad/__init__.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.209530 evo_prot_grad-0.1.3/evo_prot_grad/common/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-15 22:00:24.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2028 2023-07-02 17:16:56.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/embeddings.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    15061 2023-07-21 02:08:17.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/sampler.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2751 2023-07-17 13:44:18.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/tokenizers.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3029 2023-07-20 23:46:27.000000 evo_prot_grad-0.1.3/evo_prot_grad/common/utils.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.212284 evo_prot_grad-0.1.3/evo_prot_grad/experts/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-06-21 13:33:11.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    10623 2023-07-17 14:44:58.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/base_experts.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2986 2023-07-17 14:45:12.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/bert_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3015 2023-07-17 13:49:07.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/causallm_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     2944 2023-07-17 13:48:59.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/esm_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3292 2023-07-17 14:45:29.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/evcouplings_expert.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1490 2023-07-17 13:41:13.000000 evo_prot_grad-0.1.3/evo_prot_grad/experts/onehot_downstream_regression_expert.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.213370 evo_prot_grad-0.1.3/evo_prot_grad/models/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      108 2023-06-21 12:05:07.000000 evo_prot_grad-0.1.3/evo_prot_grad/models/__init__.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1939 2023-07-02 21:00:15.000000 evo_prot_grad-0.1.3/evo_prot_grad/models/downstream_cnn.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)    11712 2023-07-18 04:21:56.000000 evo_prot_grad-0.1.3/evo_prot_grad/models/potts.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.207702 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5109 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/PKG-INFO
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)      847 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/SOURCES.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        1 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/dependency_links.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       28 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/requires.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       14 2023-07-21 02:13:05.000000 evo_prot_grad-0.1.3/evo_prot_grad.egg-info/top_level.txt
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)       38 2023-07-21 02:13:05.215929 evo_prot_grad-0.1.3/setup.cfg
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1403 2023-07-21 02:11:39.000000 evo_prot_grad-0.1.3/setup.py
+drwxr-xr-x   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)        0 2023-07-21 02:13:05.215008 evo_prot_grad-0.1.3/test/
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     1611 2023-07-17 14:11:23.000000 evo_prot_grad-0.1.3/test/test_experts.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     5099 2023-07-06 23:52:27.000000 evo_prot_grad-0.1.3/test/test_sampler.py
+-rw-r--r--   0 pemami   (1410084004) NREL_NT\Domain Users (18434217)     3812 2023-07-17 14:14:09.000000 evo_prot_grad-0.1.3/test/test_utils.py
```

### Comparing `evo_prot_grad-0.1.2/PKG-INFO` & `evo_prot_grad-0.1.3/evo_prot_grad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: evo_prot_grad
-Version: 0.1.2
+Name: evo-prot-grad
+Version: 0.1.3
 Summary: Directed evolution of proteins with fast gradient-based discrete MCMC.
 Home-page: https://github.nrel.gov/NREL/EvoProtGrad/
 Author: Patrick Emami
 Author-email: Patrick.Emami@nrel.gov
 License: BSD 3-Clause
 Keywords: protein engineering,directed evolution,huggingface,protein language models,mcmc
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # EvoProtGrad
 
+[![PyPI version](https://badge.fury.io/py/evo-prot-grad.svg)](https://badge.fury.io/py/evo-prot-grad)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 A Python package for directed **evo**lution on a **pro**tein sequence with **grad**ient-based discrete Markov chain monte carlo (MCMC). Users are able to compose their custom protein models that map sequence to function with various pretrained models, including protein language models (PLMs), to guide and constrain search. The library is designed to natively integrate with 🤗 HuggingFace and supports PLMs from the [transformers](https://huggingface.co/docs/transformers/index) library.
 
 The underlying search technique is based on a variant of discrete MCMC that uses gradients of a *differentiable* compositional target function to rapidly explore a protein's fitness landscape in sequence space. 
 We allow users to compose their own custom target function for MCMC by leveraging the Product of Experts MCMC paradigm.
 Each model is an "expert" that contributes its own knowledge about the protein's fitness landscape to the overall target function.
```

### Comparing `evo_prot_grad-0.1.2/README.md` & `evo_prot_grad-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # EvoProtGrad
 
+[![PyPI version](https://badge.fury.io/py/evo-prot-grad.svg)](https://badge.fury.io/py/evo-prot-grad)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 A Python package for directed **evo**lution on a **pro**tein sequence with **grad**ient-based discrete Markov chain monte carlo (MCMC). Users are able to compose their custom protein models that map sequence to function with various pretrained models, including protein language models (PLMs), to guide and constrain search. The library is designed to natively integrate with 🤗 HuggingFace and supports PLMs from the [transformers](https://huggingface.co/docs/transformers/index) library.
 
 The underlying search technique is based on a variant of discrete MCMC that uses gradients of a *differentiable* compositional target function to rapidly explore a protein's fitness landscape in sequence space. 
 We allow users to compose their own custom target function for MCMC by leveraging the Product of Experts MCMC paradigm.
 Each model is an "expert" that contributes its own knowledge about the protein's fitness landscape to the overall target function.
```

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/__init__.py` & `evo_prot_grad-0.1.3/evo_prot_grad/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/common/embeddings.py` & `evo_prot_grad-0.1.3/evo_prot_grad/common/embeddings.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/common/sampler.py` & `evo_prot_grad-0.1.3/evo_prot_grad/common/sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,24 +268,24 @@
                 accepted = (log_acc.exp() >= torch.rand_like(log_acc)).float().view(-1, *([1] * x_rank))
                 cur_chains_oh = y * accepted + (1.0 - accepted) * cur_chains_oh
 
             # Current chain state book-keeping    
             self.chains_oh = cur_chains_oh
             self.chains = self.canonical_chain_tokenizer.decode(cur_chains_oh)
             # History book-keeping
-            self.chains_oh_history += [cur_chains_oh]
+            self.chains_oh_history += [cur_chains_oh.clone()]
             PoE = proposed_PoE * accepted.squeeze() + PoE * (1. - accepted.squeeze())
-            self.PoE_history += [PoE]
+            self.PoE_history += [PoE.clone()]
             
             if self.verbose:
                 x_strs = self.canonical_chain_tokenizer.decode(cur_chains_oh)
-                print(f'step {i} acceptance rate: ', log_acc.exp().item())
+                print(f'step {i} acceptance rate: {log_acc.exp().item():.4f}')
                 for idx,variant in enumerate(x_strs):
-                    print(f'>variant {idx}, PoE {PoE[idx]}')
-                    print(variant)
+                    print(f'>chain {idx}, Product of Experts score: {PoE[idx]:.4f}')
+                    utils.print_variant_in_color(variant, self.wtseq)
 
             if self.max_mutations > 0:
                 # Once a chain reaches the max mutations, reset it to WT            
                 dist = utils.mut_distance(cur_chains_oh, self.wt_oh)
                 mask_flag = (dist >= self.max_mutations).bool()
                 mask_flag = mask_flag.reshape(self.parallel_chains)
                 cur_chains_oh[mask_flag] = self.wt_oh
```

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/common/tokenizers.py` & `evo_prot_grad-0.1.3/evo_prot_grad/common/tokenizers.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/common/utils.py` & `evo_prot_grad-0.1.3/evo_prot_grad/common/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -74,8 +74,19 @@
     """Set random seed for reproducibility.
     Args:
         seed (int): The seed to set.
     """
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     np.random.seed(seed)
-    random.seed(seed)
+    random.seed(seed)
+
+def print_variant_in_color(seq: str, wt: str, ignore_gaps: bool = True) -> None:
+    """Print a variant in color."""
+    for j in range(len(wt)):
+        if seq[j] != wt[j]:
+            if ignore_gaps and (seq[j] == '-' or seq[j] == 'X'):
+                continue
+            print(f'\033[91m{seq[j]}', end='')
+        else:
+            print(f'\033[0m{seq[j]}', end='')
+    print('\033[0m')
```

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/experts/base_experts.py` & `evo_prot_grad-0.1.3/evo_prot_grad/experts/base_experts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/experts/bert_expert.py` & `evo_prot_grad-0.1.3/evo_prot_grad/experts/bert_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/experts/causallm_expert.py` & `evo_prot_grad-0.1.3/evo_prot_grad/experts/causallm_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/experts/esm_expert.py` & `evo_prot_grad-0.1.3/evo_prot_grad/experts/esm_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/experts/evcouplings_expert.py` & `evo_prot_grad-0.1.3/evo_prot_grad/experts/evcouplings_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/experts/onehot_downstream_regression_expert.py` & `evo_prot_grad-0.1.3/evo_prot_grad/experts/onehot_downstream_regression_expert.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/models/downstream_cnn.py` & `evo_prot_grad-0.1.3/evo_prot_grad/models/downstream_cnn.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad/models/potts.py` & `evo_prot_grad-0.1.3/evo_prot_grad/models/potts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad.egg-info/PKG-INFO` & `evo_prot_grad-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: evo-prot-grad
-Version: 0.1.2
+Name: evo_prot_grad
+Version: 0.1.3
 Summary: Directed evolution of proteins with fast gradient-based discrete MCMC.
 Home-page: https://github.nrel.gov/NREL/EvoProtGrad/
 Author: Patrick Emami
 Author-email: Patrick.Emami@nrel.gov
 License: BSD 3-Clause
 Keywords: protein engineering,directed evolution,huggingface,protein language models,mcmc
 Classifier: Development Status :: 3 - Alpha
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # EvoProtGrad
 
+[![PyPI version](https://badge.fury.io/py/evo-prot-grad.svg)](https://badge.fury.io/py/evo-prot-grad)
 [![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 A Python package for directed **evo**lution on a **pro**tein sequence with **grad**ient-based discrete Markov chain monte carlo (MCMC). Users are able to compose their custom protein models that map sequence to function with various pretrained models, including protein language models (PLMs), to guide and constrain search. The library is designed to natively integrate with 🤗 HuggingFace and supports PLMs from the [transformers](https://huggingface.co/docs/transformers/index) library.
 
 The underlying search technique is based on a variant of discrete MCMC that uses gradients of a *differentiable* compositional target function to rapidly explore a protein's fitness landscape in sequence space. 
 We allow users to compose their own custom target function for MCMC by leveraging the Product of Experts MCMC paradigm.
 Each model is an "expert" that contributes its own knowledge about the protein's fitness landscape to the overall target function.
```

### Comparing `evo_prot_grad-0.1.2/evo_prot_grad.egg-info/SOURCES.txt` & `evo_prot_grad-0.1.3/evo_prot_grad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/setup.py` & `evo_prot_grad-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt', 'r') as f:
     requirements = f.read().splitlines()
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(name='evo_prot_grad',
-      version='0.1.2',
+      version='0.1.3',
       description='Directed evolution of proteins with fast gradient-based discrete MCMC.',
       author='Patrick Emami',
       author_email='Patrick.Emami@nrel.gov',
       url='https://github.nrel.gov/NREL/EvoProtGrad/',
       python_requires='>=3.8',
       install_requires=requirements,
       long_description=readme,
```

### Comparing `evo_prot_grad-0.1.2/test/test_experts.py` & `evo_prot_grad-0.1.3/test/test_experts.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/test/test_sampler.py` & `evo_prot_grad-0.1.3/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `evo_prot_grad-0.1.2/test/test_utils.py` & `evo_prot_grad-0.1.3/test/test_utils.py`

 * *Files identical despite different names*

