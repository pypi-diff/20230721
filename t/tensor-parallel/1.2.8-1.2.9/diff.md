# Comparing `tmp/tensor_parallel-1.2.8.tar.gz` & `tmp/tensor_parallel-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.2.8.tar", last modified: Fri Jun 23 13:23:29 2023, max compression
+gzip compressed data, was "tensor_parallel-1.2.9.tar", last modified: Fri Jul 21 16:02:23 2023, max compression
```

## Comparing `tensor_parallel-1.2.8.tar` & `tensor_parallel-1.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.771500 tensor_parallel-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.779501 tensor_parallel-1.2.8/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.779501 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 13:23:29.000000 tensor_parallel-1.2.8/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 13:23:29.783501 tensor_parallel-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-06-23 13:23:19.000000 tensor_parallel-1.2.8/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:23.288169 tensor_parallel-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-21 16:02:23.288169 tensor_parallel-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-21 16:02:23.288169 tensor_parallel-1.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:23.280168 tensor_parallel-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:23.284169 tensor_parallel-1.2.9/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22037 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11969 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:23.288169 tensor_parallel-1.2.9/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-21 16:02:23.000000 tensor_parallel-1.2.9/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-21 16:02:23.000000 tensor_parallel-1.2.9/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 16:02:23.000000 tensor_parallel-1.2.9/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-21 16:02:23.000000 tensor_parallel-1.2.9/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 16:02:23.000000 tensor_parallel-1.2.9/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 16:02:23.288169 tensor_parallel-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-21 16:02:10.000000 tensor_parallel-1.2.9/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.2.8/LICENCE` & `tensor_parallel-1.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/PKG-INFO` & `tensor_parallel-1.2.9/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tensor_parallel
-Version: 1.2.8
+Name: tensor-parallel
+Version: 1.2.9
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 
 # tensor_parallel
 [![PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)](https://pypi.org/project/tensor-parallel/)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/tensor_parallel/actions)
 
 <p align="center">
-    🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/">Try new 20B LLMs demo in Kaggle</a></b>
+    🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int4-llm/">Try new 40B LLMs demo in Kaggle</a></b>
 </p>
 
 Run large PyTorch models on multiple GPUs in one line of code with potentially linear speedup.
 
 ```python
 import transformers
 import tensor_parallel as tp
@@ -67,22 +67,22 @@
 
 
 Simply wrap your PyTorch model with `tp.tensor_parallel` and use it normally.
 For best memory efficiency, call `tp.tensor_parallel` while the model is still on CPU.  
 
 Here are a few use cases:
 - [`examples/training_flan-t5-xl.ipynb`](./examples/training_flan-t5-xl.ipynb) - fine-tune full FLAN-T5 model on text summarization
-- [`tensor_parallel int8 LLM`](https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/) - inferencing a large language model with LLM.8bit + tensor_parallel
+- [`tensor_parallel int8 LLM`](https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/) - adapter-tuning a large language model with LLM.8bit + tensor_parallel
 - __TBA__ - defining custom parallelism strategy
 
 
 Advanced parameters to `tensor_parallel`:
 - `device_ids: List[device]` - which devices to use; defaults to all available GPUs
 - `output_device: device` - model outputs will have this device
-- `tensor_parallel_config: tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./tensor_parallel/slicing_configs.py)
+- `tensor_parallel_config: tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./src/tensor_parallel/slicing_configs.py)
 - `distributed: bool` - if True, use torch.distributed backend instead of threading (requires `torchrun`)
 - `sharded: bool` - if True, find all trainable parameters that weren't split by Tensor Parallelism and split them using [ZeRO-3 algorithm](https://deepspeed.readthedocs.io/en/latest/zero3.html).
    - weights will be split between GPUs and re-assembled before each forward pass
    - TL;DR use this when training to avoid duplicate parameters (enabled by default!) 
    - `sharded_param_names: List[str]` - parameter names that should be sharded this way, default = found automatically
 
   
@@ -137,19 +137,19 @@
     tensor_parallel_config=model.tensor_parallel_config,
     world_size=len(model.devices),
 )
 
 # Dispatch the partial state_dict (load_state_dict doesn't work with meta so here I use accelerate)
 device_map = tp.infer_sharded_device_map(model)
 for param_name, param in state_dict.items():
-  module_name = param_name
-  while len(module_name) > 0 and module_name not in device_map:
-      module_name = ".".join(module_name.split(".")[:-1])
-  param_device = device_map[module_name]
-  accelerate.utils.set_module_tensor_to_device(model, param_name, param_device, value=param)
+    module_name = param_name
+    while len(module_name) > 0 and module_name not in device_map:
+        module_name = ".".join(module_name.split(".")[:-1])
+    param_device = device_map[module_name]
+    accelerate.utils.set_module_tensor_to_device(model, param_name, param_device, value=param)
 ```
 
 With this no more than one part of the model needs to be loaded into memory at once. 
   
 ## FAQ
 
 - __Q:__ I don't have a multi-GPU server. Can I use tensor_parallel in Google Colab?
@@ -169,26 +169,24 @@
 
 
 Why use `tensor_parallel` ...
 - v.s. [DeepSpeed](https://github.com/microsoft/DeepSpeed) and [FairScale](https://github.com/facebookresearch/fairscale/)
   - DeepSpeed has many parallelization strategies, but requires careful configuration
   - tensor_parallel has one strategy that works with 1 line of code
   - tensor_parallel works in a jupyter notebook
-- v.s. [MegatronLM](https://github.com/NVIDIA/Megatron-LM)?
+- v.s. [MegatronLM](https://github.com/NVIDIA/Megatron-LM)
   - MegatronLM has _great_ tensor parallelism for one model architecture
   - tensor_parallel has _good_ parallelism for any architecture
   - tensor_parallel is way easier to install
-- v.s. [parallelformers](https://github.com/tunib-ai/parallelformers)?
-  - parallelformers implements a fixed [list of architectures](https://github.com/tunib-ai/parallelformers/tree/main/parallelformers/transformers)
-  - tensor_parallel works for any architecture automatically 
+- v.s. [parallelformers](https://github.com/tunib-ai/parallelformers) 
   - parallelformers is inference-only, tensor_parallel supports training
 - v.s. [`alpa`](https://github.com/alpa-projects/alpa)
   - alpa is a powerful tool for automatic distributed training / inference in JAX
   - tensor_parallel works with PyTorch
-- v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/model_doc/gpt2#transformers.GPT2Model.parallelize)?
+- v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/model_doc/gpt2#transformers.GPT2Model.parallelize)
   - both are easy to use, both fit large models
   - in parallelize, one GPU works at a time
   - in tensor_parallel, GPUs work in parallel
 
 In short, use `tensor_parallel` for quick prototyping on a single machine.
 Use DeepSpeed+Megatron or alpa for million-dollar training runs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.8 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.9 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -17,15 +17,15 @@
 text/markdown Provides-Extra: dev License-File: LICENCE # tensor_parallel [!
 [PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)]
 (https://pypi.org/project/tensor-parallel/) [![Black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI
 status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-
 tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/
 tensor_parallel/actions)
-                     ð  Try_new_20B_LLMs_demo_in_Kaggle
+                     ð  Try_new_40B_LLMs_demo_in_Kaggle
 Run large PyTorch models on multiple GPUs in one line of code with potentially
 linear speedup. ```python import transformers import tensor_parallel as tp
 tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
 model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") #
 use opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:
 1"]) # <- each GPU has half the weights inputs = tokenizer("A cat sat",
 return_tensors="pt")["input_ids"].to("cuda:0") outputs = model.generate(inputs,
@@ -35,20 +35,20 @@
 (recommended): ``` pip install tensor_parallel ``` Bleeding edge version: ```
 pip install https://github.com/BlackSamorez/tensor_parallel/archive/main.zip
 ``` ## Usage Simply wrap your PyTorch model with `tp.tensor_parallel` and use
 it normally. For best memory efficiency, call `tp.tensor_parallel` while the
 model is still on CPU. Here are a few use cases: - [`examples/training_flan-t5-
 xl.ipynb`](./examples/training_flan-t5-xl.ipynb) - fine-tune full FLAN-T5 model
 on text summarization - [`tensor_parallel int8 LLM`](https://www.kaggle.com/
-code/blacksamorez/tensor-parallel-int8-llm/) - inferencing a large language
+code/blacksamorez/tensor-parallel-int8-llm/) - adapter-tuning a large language
 model with LLM.8bit + tensor_parallel - __TBA__ - defining custom parallelism
 strategy Advanced parameters to `tensor_parallel`: - `device_ids: List[device]`
 - which devices to use; defaults to all available GPUs - `output_device:
 device` - model outputs will have this device - `tensor_parallel_config:
-tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./
+tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./src/
 tensor_parallel/slicing_configs.py) - `distributed: bool` - if True, use
 torch.distributed backend instead of threading (requires `torchrun`) -
 `sharded: bool` - if True, find all trainable parameters that weren't split by
 Tensor Parallelism and split them using [ZeRO-3 algorithm](https://
 deepspeed.readthedocs.io/en/latest/zero3.html). - weights will be split between
 GPUs and re-assembled before each forward pass - TL;DR use this when training
 to avoid duplicate parameters (enabled by default!) - `sharded_param_names:
@@ -95,27 +95,24 @@
 FullyShardedDataParallel and ZeRO? - __A:__ ZeRO is better if you can fit a
 large batch, TensorParallel is better for small batches Why use
 `tensor_parallel` ... - v.s. [DeepSpeed](https://github.com/microsoft/
 DeepSpeed) and [FairScale](https://github.com/facebookresearch/fairscale/) -
 DeepSpeed has many parallelization strategies, but requires careful
 configuration - tensor_parallel has one strategy that works with 1 line of code
 - tensor_parallel works in a jupyter notebook - v.s. [MegatronLM](https://
-github.com/NVIDIA/Megatron-LM)? - MegatronLM has _great_ tensor parallelism for
+github.com/NVIDIA/Megatron-LM) - MegatronLM has _great_ tensor parallelism for
 one model architecture - tensor_parallel has _good_ parallelism for any
 architecture - tensor_parallel is way easier to install - v.s.
-[parallelformers](https://github.com/tunib-ai/parallelformers)? -
-parallelformers implements a fixed [list of architectures](https://github.com/
-tunib-ai/parallelformers/tree/main/parallelformers/transformers) -
-tensor_parallel works for any architecture automatically - parallelformers is
-inference-only, tensor_parallel supports training - v.s. [`alpa`](https://
-github.com/alpa-projects/alpa) - alpa is a powerful tool for automatic
-distributed training / inference in JAX - tensor_parallel works with PyTorch -
-v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/
-model_doc/gpt2#transformers.GPT2Model.parallelize)? - both are easy to use,
-both fit large models - in parallelize, one GPU works at a time - in
+[parallelformers](https://github.com/tunib-ai/parallelformers) -
+parallelformers is inference-only, tensor_parallel supports training - v.s.
+[`alpa`](https://github.com/alpa-projects/alpa) - alpa is a powerful tool for
+automatic distributed training / inference in JAX - tensor_parallel works with
+PyTorch - v.s. [`Model.parallelize()`](https://huggingface.co/docs/
+transformers/model_doc/gpt2#transformers.GPT2Model.parallelize) - both are easy
+to use, both fit large models - in parallelize, one GPU works at a time - in
 tensor_parallel, GPUs work in parallel In short, use `tensor_parallel` for
 quick prototyping on a single machine. Use DeepSpeed+Megatron or alpa for
 million-dollar training runs. ## Troubleshooting If you experience NCCL errors,
 or random hanging, you may have some code errors that are not displayed
 properly. To debug these errors, we recommend restarting with `export
 TENSOR_PARALLEL_USE_NATIVE=1` or on a single device. If you found a bug or
 encountered a problem, please report it to [our issue tracker](https://
```

### Comparing `tensor_parallel-1.2.8/README.md` & `tensor_parallel-1.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # tensor_parallel
 [![PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)](https://pypi.org/project/tensor-parallel/)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/tensor_parallel/actions)
 
 <p align="center">
-    🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/">Try new 20B LLMs demo in Kaggle</a></b>
+    🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int4-llm/">Try new 40B LLMs demo in Kaggle</a></b>
 </p>
 
 Run large PyTorch models on multiple GPUs in one line of code with potentially linear speedup.
 
 ```python
 import transformers
 import tensor_parallel as tp
@@ -39,22 +39,22 @@
 
 
 Simply wrap your PyTorch model with `tp.tensor_parallel` and use it normally.
 For best memory efficiency, call `tp.tensor_parallel` while the model is still on CPU.  
 
 Here are a few use cases:
 - [`examples/training_flan-t5-xl.ipynb`](./examples/training_flan-t5-xl.ipynb) - fine-tune full FLAN-T5 model on text summarization
-- [`tensor_parallel int8 LLM`](https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/) - inferencing a large language model with LLM.8bit + tensor_parallel
+- [`tensor_parallel int8 LLM`](https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/) - adapter-tuning a large language model with LLM.8bit + tensor_parallel
 - __TBA__ - defining custom parallelism strategy
 
 
 Advanced parameters to `tensor_parallel`:
 - `device_ids: List[device]` - which devices to use; defaults to all available GPUs
 - `output_device: device` - model outputs will have this device
-- `tensor_parallel_config: tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./tensor_parallel/slicing_configs.py)
+- `tensor_parallel_config: tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./src/tensor_parallel/slicing_configs.py)
 - `distributed: bool` - if True, use torch.distributed backend instead of threading (requires `torchrun`)
 - `sharded: bool` - if True, find all trainable parameters that weren't split by Tensor Parallelism and split them using [ZeRO-3 algorithm](https://deepspeed.readthedocs.io/en/latest/zero3.html).
    - weights will be split between GPUs and re-assembled before each forward pass
    - TL;DR use this when training to avoid duplicate parameters (enabled by default!) 
    - `sharded_param_names: List[str]` - parameter names that should be sharded this way, default = found automatically
 
   
@@ -109,19 +109,19 @@
     tensor_parallel_config=model.tensor_parallel_config,
     world_size=len(model.devices),
 )
 
 # Dispatch the partial state_dict (load_state_dict doesn't work with meta so here I use accelerate)
 device_map = tp.infer_sharded_device_map(model)
 for param_name, param in state_dict.items():
-  module_name = param_name
-  while len(module_name) > 0 and module_name not in device_map:
-      module_name = ".".join(module_name.split(".")[:-1])
-  param_device = device_map[module_name]
-  accelerate.utils.set_module_tensor_to_device(model, param_name, param_device, value=param)
+    module_name = param_name
+    while len(module_name) > 0 and module_name not in device_map:
+        module_name = ".".join(module_name.split(".")[:-1])
+    param_device = device_map[module_name]
+    accelerate.utils.set_module_tensor_to_device(model, param_name, param_device, value=param)
 ```
 
 With this no more than one part of the model needs to be loaded into memory at once. 
   
 ## FAQ
 
 - __Q:__ I don't have a multi-GPU server. Can I use tensor_parallel in Google Colab?
@@ -141,26 +141,24 @@
 
 
 Why use `tensor_parallel` ...
 - v.s. [DeepSpeed](https://github.com/microsoft/DeepSpeed) and [FairScale](https://github.com/facebookresearch/fairscale/)
   - DeepSpeed has many parallelization strategies, but requires careful configuration
   - tensor_parallel has one strategy that works with 1 line of code
   - tensor_parallel works in a jupyter notebook
-- v.s. [MegatronLM](https://github.com/NVIDIA/Megatron-LM)?
+- v.s. [MegatronLM](https://github.com/NVIDIA/Megatron-LM)
   - MegatronLM has _great_ tensor parallelism for one model architecture
   - tensor_parallel has _good_ parallelism for any architecture
   - tensor_parallel is way easier to install
-- v.s. [parallelformers](https://github.com/tunib-ai/parallelformers)?
-  - parallelformers implements a fixed [list of architectures](https://github.com/tunib-ai/parallelformers/tree/main/parallelformers/transformers)
-  - tensor_parallel works for any architecture automatically 
+- v.s. [parallelformers](https://github.com/tunib-ai/parallelformers) 
   - parallelformers is inference-only, tensor_parallel supports training
 - v.s. [`alpa`](https://github.com/alpa-projects/alpa)
   - alpa is a powerful tool for automatic distributed training / inference in JAX
   - tensor_parallel works with PyTorch
-- v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/model_doc/gpt2#transformers.GPT2Model.parallelize)?
+- v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/model_doc/gpt2#transformers.GPT2Model.parallelize)
   - both are easy to use, both fit large models
   - in parallelize, one GPU works at a time
   - in tensor_parallel, GPUs work in parallel
 
 In short, use `tensor_parallel` for quick prototyping on a single machine.
 Use DeepSpeed+Megatron or alpa for million-dollar training runs.
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # tensor_parallel [![PyPI version](https://img.shields.io/pypi/v/tensor-
 parallel.svg?color=blue)](https://pypi.org/project/tensor-parallel/) [![Black]
 (https://img.shields.io/badge/code%20style-black-000000.svg)](https://
 github.com/psf/black) [![CI status](https://github.com/BlackSamorez/
 tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https:
 //github.com/BlackSamorez/tensor_parallel/actions)
-                     ð  Try_new_20B_LLMs_demo_in_Kaggle
+                     ð  Try_new_40B_LLMs_demo_in_Kaggle
 Run large PyTorch models on multiple GPUs in one line of code with potentially
 linear speedup. ```python import transformers import tensor_parallel as tp
 tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
 model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") #
 use opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:
 1"]) # <- each GPU has half the weights inputs = tokenizer("A cat sat",
 return_tensors="pt")["input_ids"].to("cuda:0") outputs = model.generate(inputs,
@@ -18,20 +18,20 @@
 (recommended): ``` pip install tensor_parallel ``` Bleeding edge version: ```
 pip install https://github.com/BlackSamorez/tensor_parallel/archive/main.zip
 ``` ## Usage Simply wrap your PyTorch model with `tp.tensor_parallel` and use
 it normally. For best memory efficiency, call `tp.tensor_parallel` while the
 model is still on CPU. Here are a few use cases: - [`examples/training_flan-t5-
 xl.ipynb`](./examples/training_flan-t5-xl.ipynb) - fine-tune full FLAN-T5 model
 on text summarization - [`tensor_parallel int8 LLM`](https://www.kaggle.com/
-code/blacksamorez/tensor-parallel-int8-llm/) - inferencing a large language
+code/blacksamorez/tensor-parallel-int8-llm/) - adapter-tuning a large language
 model with LLM.8bit + tensor_parallel - __TBA__ - defining custom parallelism
 strategy Advanced parameters to `tensor_parallel`: - `device_ids: List[device]`
 - which devices to use; defaults to all available GPUs - `output_device:
 device` - model outputs will have this device - `tensor_parallel_config:
-tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./
+tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./src/
 tensor_parallel/slicing_configs.py) - `distributed: bool` - if True, use
 torch.distributed backend instead of threading (requires `torchrun`) -
 `sharded: bool` - if True, find all trainable parameters that weren't split by
 Tensor Parallelism and split them using [ZeRO-3 algorithm](https://
 deepspeed.readthedocs.io/en/latest/zero3.html). - weights will be split between
 GPUs and re-assembled before each forward pass - TL;DR use this when training
 to avoid duplicate parameters (enabled by default!) - `sharded_param_names:
@@ -78,27 +78,24 @@
 FullyShardedDataParallel and ZeRO? - __A:__ ZeRO is better if you can fit a
 large batch, TensorParallel is better for small batches Why use
 `tensor_parallel` ... - v.s. [DeepSpeed](https://github.com/microsoft/
 DeepSpeed) and [FairScale](https://github.com/facebookresearch/fairscale/) -
 DeepSpeed has many parallelization strategies, but requires careful
 configuration - tensor_parallel has one strategy that works with 1 line of code
 - tensor_parallel works in a jupyter notebook - v.s. [MegatronLM](https://
-github.com/NVIDIA/Megatron-LM)? - MegatronLM has _great_ tensor parallelism for
+github.com/NVIDIA/Megatron-LM) - MegatronLM has _great_ tensor parallelism for
 one model architecture - tensor_parallel has _good_ parallelism for any
 architecture - tensor_parallel is way easier to install - v.s.
-[parallelformers](https://github.com/tunib-ai/parallelformers)? -
-parallelformers implements a fixed [list of architectures](https://github.com/
-tunib-ai/parallelformers/tree/main/parallelformers/transformers) -
-tensor_parallel works for any architecture automatically - parallelformers is
-inference-only, tensor_parallel supports training - v.s. [`alpa`](https://
-github.com/alpa-projects/alpa) - alpa is a powerful tool for automatic
-distributed training / inference in JAX - tensor_parallel works with PyTorch -
-v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/
-model_doc/gpt2#transformers.GPT2Model.parallelize)? - both are easy to use,
-both fit large models - in parallelize, one GPU works at a time - in
+[parallelformers](https://github.com/tunib-ai/parallelformers) -
+parallelformers is inference-only, tensor_parallel supports training - v.s.
+[`alpa`](https://github.com/alpa-projects/alpa) - alpa is a powerful tool for
+automatic distributed training / inference in JAX - tensor_parallel works with
+PyTorch - v.s. [`Model.parallelize()`](https://huggingface.co/docs/
+transformers/model_doc/gpt2#transformers.GPT2Model.parallelize) - both are easy
+to use, both fit large models - in parallelize, one GPU works at a time - in
 tensor_parallel, GPUs work in parallel In short, use `tensor_parallel` for
 quick prototyping on a single machine. Use DeepSpeed+Megatron or alpa for
 million-dollar training runs. ## Troubleshooting If you experience NCCL errors,
 or random hanging, you may have some code errors that are not displayed
 properly. To debug these errors, we recommend restarting with `export
 TENSOR_PARALLEL_USE_NATIVE=1` or on a single device. If you found a bug or
 encountered a problem, please report it to [our issue tracker](https://
```

### Comparing `tensor_parallel-1.2.8/setup.cfg` & `tensor_parallel-1.2.9/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.2.8
+version = 1.2.9
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls = 
@@ -36,19 +36,19 @@
 	transformers>=4.20.1
 
 [options.extras_require]
 dev = 
 	pytest==6.2.5
 	pytest-forked
 	pytest-asyncio==0.16.0
-	accelerate==0.15.0
+	accelerate==0.20.3
 	black==22.3.0
 	isort==5.10.1
 	psutil
-	peft>=0.3.0
+	peft==0.3.0
 	einops==0.6.1
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build =
```

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/__init__.py` & `tensor_parallel-1.2.9/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.2.9/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.2.9/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/communications.py` & `tensor_parallel-1.2.9/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/config.py` & `tensor_parallel-1.2.9/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.2.9/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.2.9/src/tensor_parallel/dispatch.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/factory.py` & `tensor_parallel-1.2.9/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.2.9/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.2.9/src/tensor_parallel/pretrained_model.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/shard.py` & `tensor_parallel-1.2.9/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/sharding.py` & `tensor_parallel-1.2.9/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.2.9/src/tensor_parallel/slicing_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,28 +342,39 @@
 
 
 def get_llama_config(model_config: PretrainedConfig, devices: Sequence[torch.device]) -> Config:
     # We can't use LlamaConfig since it requires pre-release `transformers``
     assert model_config.model_type == "llama", f"Trying to pass {model_config.model_type} as llama config"
 
     world_size = len(devices)
-    num_heads = model_config.num_attention_heads
     head_dim = model_config.hidden_size // model_config.num_attention_heads
+    try:
+        num_kv = model_config.num_key_value_heads
+        q_per_kv = model_config.num_attention_heads // model_config.num_key_value_heads
+        new_modeling = True
+    except AttributeError:
+        num_kv = model_config.num_attention_heads
+        q_per_kv = 1
+        new_modeling = False
 
     gather_kv_across_ranks = CollectiveOperation(
         world_size=world_size, func=lambda *kvs: gather_kv(*kvs, world_size=world_size)
     )  # this operation ensures that we get attention cache for all heads on each device
 
-    return Config(
+    config = Config(
         state_rules={
             # LlamaAttention
-            r".*self_attn\.q_proj\.weight$": SplitInChunks(world_size=world_size, dim=0, chunk_size=head_dim),
+            r".*self_attn\.q_proj\.weight$": SplitInChunks(
+                world_size=world_size, dim=0, chunk_size=q_per_kv * head_dim
+            ),
             r".*self_attn\.k_proj\.weight$": SplitInChunks(world_size=world_size, dim=0, chunk_size=head_dim),
             r".*self_attn\.v_proj\.weight$": SplitInChunks(world_size=world_size, dim=0, chunk_size=head_dim),
-            r".*self_attn\.o_proj\.weight$": SplitInChunks(world_size=world_size, dim=1, chunk_size=head_dim),
+            r".*self_attn\.o_proj\.weight$": SplitInChunks(
+                world_size=world_size, dim=1, chunk_size=q_per_kv * head_dim
+            ),
             # LlamaFeedForward
             r".*mlp\.gate_proj\.weight$": Split(world_size=world_size, dim=0),
             r".*mlp\.down_proj\.weight$": Split(world_size=world_size, dim=1),
             r".*mlp\.up_proj\.weight$": Split(world_size=world_size, dim=0),
             # LlamaModel
             r".*embed_tokens.weight$": Split(world_size=world_size, dim=1),
             r".*lm_head\.weight$": Split(world_size=world_size, dim=0),
@@ -375,20 +386,26 @@
             r".*self_attn$": {0: "sum", 2: gather_kv_across_ranks},
             r".*mlp$": {0: "sum"},
             r".*embed_tokens$": {0: "gather -1"},
             r".*lm_head$": {0: "gather -1"},
         },
         attr_rules={
             r".*self_attn$": {
-                "hidden_size": partial(split_inner_dim, num_heads=num_heads, world_size=world_size),
-                "num_heads": partial(split_num_heads, world_size=world_size),
+                "hidden_size": partial(split_inner_dim, num_heads=num_kv, world_size=world_size),
+                "num_heads": lambda n, rank: q_per_kv
+                * split_num_heads(n // q_per_kv, rank=rank, world_size=world_size),
             }
         },
     )
 
+    if new_modeling:
+        config.attr_rules[r".*self_attn$"]["num_key_value_heads"] = partial(split_num_heads, world_size=world_size)
+
+    return config
+
 
 def get_refined_web_config(model_config: PretrainedConfig, devices: Sequence[torch.device]) -> Config:
     # We can't use `RWConfig`` since it's custom code
     assert model_config.model_type == "RefinedWeb", f"Trying to pass {model_config.model_type} as RefinedWeb config"
     assert not model_config.bias and not model_config.alibi, f"Running Falcon with biases or alibi is not supported"
 
     world_size = len(devices)
```

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.2.9/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.2.9/src/tensor_parallel/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/utils.py` & `tensor_parallel-1.2.9/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.2.9/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tensor-parallel
-Version: 1.2.8
+Name: tensor_parallel
+Version: 1.2.9
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 
 # tensor_parallel
 [![PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)](https://pypi.org/project/tensor-parallel/)
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![CI status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/tensor_parallel/actions)
 
 <p align="center">
-    🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/">Try new 20B LLMs demo in Kaggle</a></b>
+    🚀 &nbsp;<b><a href="https://www.kaggle.com/code/blacksamorez/tensor-parallel-int4-llm/">Try new 40B LLMs demo in Kaggle</a></b>
 </p>
 
 Run large PyTorch models on multiple GPUs in one line of code with potentially linear speedup.
 
 ```python
 import transformers
 import tensor_parallel as tp
@@ -67,22 +67,22 @@
 
 
 Simply wrap your PyTorch model with `tp.tensor_parallel` and use it normally.
 For best memory efficiency, call `tp.tensor_parallel` while the model is still on CPU.  
 
 Here are a few use cases:
 - [`examples/training_flan-t5-xl.ipynb`](./examples/training_flan-t5-xl.ipynb) - fine-tune full FLAN-T5 model on text summarization
-- [`tensor_parallel int8 LLM`](https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/) - inferencing a large language model with LLM.8bit + tensor_parallel
+- [`tensor_parallel int8 LLM`](https://www.kaggle.com/code/blacksamorez/tensor-parallel-int8-llm/) - adapter-tuning a large language model with LLM.8bit + tensor_parallel
 - __TBA__ - defining custom parallelism strategy
 
 
 Advanced parameters to `tensor_parallel`:
 - `device_ids: List[device]` - which devices to use; defaults to all available GPUs
 - `output_device: device` - model outputs will have this device
-- `tensor_parallel_config: tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./tensor_parallel/slicing_configs.py)
+- `tensor_parallel_config: tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./src/tensor_parallel/slicing_configs.py)
 - `distributed: bool` - if True, use torch.distributed backend instead of threading (requires `torchrun`)
 - `sharded: bool` - if True, find all trainable parameters that weren't split by Tensor Parallelism and split them using [ZeRO-3 algorithm](https://deepspeed.readthedocs.io/en/latest/zero3.html).
    - weights will be split between GPUs and re-assembled before each forward pass
    - TL;DR use this when training to avoid duplicate parameters (enabled by default!) 
    - `sharded_param_names: List[str]` - parameter names that should be sharded this way, default = found automatically
 
   
@@ -137,19 +137,19 @@
     tensor_parallel_config=model.tensor_parallel_config,
     world_size=len(model.devices),
 )
 
 # Dispatch the partial state_dict (load_state_dict doesn't work with meta so here I use accelerate)
 device_map = tp.infer_sharded_device_map(model)
 for param_name, param in state_dict.items():
-  module_name = param_name
-  while len(module_name) > 0 and module_name not in device_map:
-      module_name = ".".join(module_name.split(".")[:-1])
-  param_device = device_map[module_name]
-  accelerate.utils.set_module_tensor_to_device(model, param_name, param_device, value=param)
+    module_name = param_name
+    while len(module_name) > 0 and module_name not in device_map:
+        module_name = ".".join(module_name.split(".")[:-1])
+    param_device = device_map[module_name]
+    accelerate.utils.set_module_tensor_to_device(model, param_name, param_device, value=param)
 ```
 
 With this no more than one part of the model needs to be loaded into memory at once. 
   
 ## FAQ
 
 - __Q:__ I don't have a multi-GPU server. Can I use tensor_parallel in Google Colab?
@@ -169,26 +169,24 @@
 
 
 Why use `tensor_parallel` ...
 - v.s. [DeepSpeed](https://github.com/microsoft/DeepSpeed) and [FairScale](https://github.com/facebookresearch/fairscale/)
   - DeepSpeed has many parallelization strategies, but requires careful configuration
   - tensor_parallel has one strategy that works with 1 line of code
   - tensor_parallel works in a jupyter notebook
-- v.s. [MegatronLM](https://github.com/NVIDIA/Megatron-LM)?
+- v.s. [MegatronLM](https://github.com/NVIDIA/Megatron-LM)
   - MegatronLM has _great_ tensor parallelism for one model architecture
   - tensor_parallel has _good_ parallelism for any architecture
   - tensor_parallel is way easier to install
-- v.s. [parallelformers](https://github.com/tunib-ai/parallelformers)?
-  - parallelformers implements a fixed [list of architectures](https://github.com/tunib-ai/parallelformers/tree/main/parallelformers/transformers)
-  - tensor_parallel works for any architecture automatically 
+- v.s. [parallelformers](https://github.com/tunib-ai/parallelformers) 
   - parallelformers is inference-only, tensor_parallel supports training
 - v.s. [`alpa`](https://github.com/alpa-projects/alpa)
   - alpa is a powerful tool for automatic distributed training / inference in JAX
   - tensor_parallel works with PyTorch
-- v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/model_doc/gpt2#transformers.GPT2Model.parallelize)?
+- v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/model_doc/gpt2#transformers.GPT2Model.parallelize)
   - both are easy to use, both fit large models
   - in parallelize, one GPU works at a time
   - in tensor_parallel, GPUs work in parallel
 
 In short, use `tensor_parallel` for quick prototyping on a single machine.
 Use DeepSpeed+Megatron or alpa for million-dollar training runs.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.2.8 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.2.9 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
@@ -17,15 +17,15 @@
 text/markdown Provides-Extra: dev License-File: LICENCE # tensor_parallel [!
 [PyPI version](https://img.shields.io/pypi/v/tensor-parallel.svg?color=blue)]
 (https://pypi.org/project/tensor-parallel/) [![Black](https://img.shields.io/
 badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CI
 status](https://github.com/BlackSamorez/tensor_parallel/actions/workflows/run-
 tests.yaml/badge.svg?branch=main)](https://github.com/BlackSamorez/
 tensor_parallel/actions)
-                     ð  Try_new_20B_LLMs_demo_in_Kaggle
+                     ð  Try_new_40B_LLMs_demo_in_Kaggle
 Run large PyTorch models on multiple GPUs in one line of code with potentially
 linear speedup. ```python import transformers import tensor_parallel as tp
 tokenizer = transformers.AutoTokenizer.from_pretrained("facebook/opt-13b")
 model = transformers.AutoModelForCausalLM.from_pretrained("facebook/opt-13b") #
 use opt-125m for testing model = tp.tensor_parallel(model, ["cuda:0", "cuda:
 1"]) # <- each GPU has half the weights inputs = tokenizer("A cat sat",
 return_tensors="pt")["input_ids"].to("cuda:0") outputs = model.generate(inputs,
@@ -35,20 +35,20 @@
 (recommended): ``` pip install tensor_parallel ``` Bleeding edge version: ```
 pip install https://github.com/BlackSamorez/tensor_parallel/archive/main.zip
 ``` ## Usage Simply wrap your PyTorch model with `tp.tensor_parallel` and use
 it normally. For best memory efficiency, call `tp.tensor_parallel` while the
 model is still on CPU. Here are a few use cases: - [`examples/training_flan-t5-
 xl.ipynb`](./examples/training_flan-t5-xl.ipynb) - fine-tune full FLAN-T5 model
 on text summarization - [`tensor_parallel int8 LLM`](https://www.kaggle.com/
-code/blacksamorez/tensor-parallel-int8-llm/) - inferencing a large language
+code/blacksamorez/tensor-parallel-int8-llm/) - adapter-tuning a large language
 model with LLM.8bit + tensor_parallel - __TBA__ - defining custom parallelism
 strategy Advanced parameters to `tensor_parallel`: - `device_ids: List[device]`
 - which devices to use; defaults to all available GPUs - `output_device:
 device` - model outputs will have this device - `tensor_parallel_config:
-tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./
+tp.Config` - use custom parallelism strategy, see [`slicing_configs.py`](./src/
 tensor_parallel/slicing_configs.py) - `distributed: bool` - if True, use
 torch.distributed backend instead of threading (requires `torchrun`) -
 `sharded: bool` - if True, find all trainable parameters that weren't split by
 Tensor Parallelism and split them using [ZeRO-3 algorithm](https://
 deepspeed.readthedocs.io/en/latest/zero3.html). - weights will be split between
 GPUs and re-assembled before each forward pass - TL;DR use this when training
 to avoid duplicate parameters (enabled by default!) - `sharded_param_names:
@@ -95,27 +95,24 @@
 FullyShardedDataParallel and ZeRO? - __A:__ ZeRO is better if you can fit a
 large batch, TensorParallel is better for small batches Why use
 `tensor_parallel` ... - v.s. [DeepSpeed](https://github.com/microsoft/
 DeepSpeed) and [FairScale](https://github.com/facebookresearch/fairscale/) -
 DeepSpeed has many parallelization strategies, but requires careful
 configuration - tensor_parallel has one strategy that works with 1 line of code
 - tensor_parallel works in a jupyter notebook - v.s. [MegatronLM](https://
-github.com/NVIDIA/Megatron-LM)? - MegatronLM has _great_ tensor parallelism for
+github.com/NVIDIA/Megatron-LM) - MegatronLM has _great_ tensor parallelism for
 one model architecture - tensor_parallel has _good_ parallelism for any
 architecture - tensor_parallel is way easier to install - v.s.
-[parallelformers](https://github.com/tunib-ai/parallelformers)? -
-parallelformers implements a fixed [list of architectures](https://github.com/
-tunib-ai/parallelformers/tree/main/parallelformers/transformers) -
-tensor_parallel works for any architecture automatically - parallelformers is
-inference-only, tensor_parallel supports training - v.s. [`alpa`](https://
-github.com/alpa-projects/alpa) - alpa is a powerful tool for automatic
-distributed training / inference in JAX - tensor_parallel works with PyTorch -
-v.s. [`Model.parallelize()`](https://huggingface.co/docs/transformers/
-model_doc/gpt2#transformers.GPT2Model.parallelize)? - both are easy to use,
-both fit large models - in parallelize, one GPU works at a time - in
+[parallelformers](https://github.com/tunib-ai/parallelformers) -
+parallelformers is inference-only, tensor_parallel supports training - v.s.
+[`alpa`](https://github.com/alpa-projects/alpa) - alpa is a powerful tool for
+automatic distributed training / inference in JAX - tensor_parallel works with
+PyTorch - v.s. [`Model.parallelize()`](https://huggingface.co/docs/
+transformers/model_doc/gpt2#transformers.GPT2Model.parallelize) - both are easy
+to use, both fit large models - in parallelize, one GPU works at a time - in
 tensor_parallel, GPUs work in parallel In short, use `tensor_parallel` for
 quick prototyping on a single machine. Use DeepSpeed+Megatron or alpa for
 million-dollar training runs. ## Troubleshooting If you experience NCCL errors,
 or random hanging, you may have some code errors that are not displayed
 properly. To debug these errors, we recommend restarting with `export
 TENSOR_PARALLEL_USE_NATIVE=1` or on a single device. If you found a bug or
 encountered a problem, please report it to [our issue tracker](https://
```

### Comparing `tensor_parallel-1.2.8/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.2.9/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/tests/test_basic.py` & `tensor_parallel-1.2.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/tests/test_factory.py` & `tensor_parallel-1.2.9/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/tests/test_integration.py` & `tensor_parallel-1.2.9/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/tests/test_saving.py` & `tensor_parallel-1.2.9/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.2.8/tests/test_transformers.py` & `tensor_parallel-1.2.9/tests/test_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,46 +68,50 @@
         tensor_parallel_configs.append(find_predefined_tensor_parallel_config(model.config, devices))
 
     assert all_equal(
         map(lambda x: x.attr_rules.keys(), tensor_parallel_configs)
     )  # basically asserting that all of those have the same config
 
 
+def prepare_model(model_name, use_lora):
+    if model_name == "BlackSamorez/falcon-40b-tiny-testing" and torch.__version__ < "2.0":
+        pytest.skip(f"Not testing {model_name} with torch=={torch.__version__}")
+    if model_name == "BlackSamorez/llama-2-tiny-testing" and transformers.__version__ < "4.31":
+        pytest.skip(f"Not testing {model_name} with transformers=={transformers.__version__}")
+
+    try:
+        model = AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True, trust_remote_code=True).float()
+    except KeyError as err:
+        pytest.skip(f"Could not create model {model_name} with error {err}")
+    if use_lora:
+        if model_name == "gpt2":
+            pytest.skip("Not testing LoRA for gpt2")
+        model = add_lora(model, model_name)
+    return model
+
+
 @pytest.mark.parametrize("use_lora", [False, True])
 @pytest.mark.parametrize("use_config", [False, True])
 @pytest.mark.parametrize("devices", [("cpu",) * 2, ("cpu",) * 3])
 @pytest.mark.parametrize(
     "model_name",
     [
         "bigscience/bloom-560m",
         "gpt2",
         "trl-internal-testing/tiny-random-GPTNeoXForCausalLM",
         "Salesforce/codegen-350M-mono",
         "Bingsu/llama-190m-arch",
+        "BlackSamorez/llama-2-tiny-testing",
         "BlackSamorez/falcon-40b-tiny-testing",
     ],
 )
 def test_forward_gpt2_like(use_lora, use_config, devices, model_name):
     torch.manual_seed(0)
 
-    if model_name == "BlackSamorez/falcon-40b-tiny-testing" and torch.__version__ < "2.0":
-        pytest.skip(f"Not testing {model_name} with torch=={torch.__version__}")
-
-    try:
-        model = (
-            AutoModelForCausalLM.from_pretrained(model_name, low_cpu_mem_usage=True, trust_remote_code=True)
-            .float()
-            .to(devices[0])
-        )
-    except KeyError as err:
-        pytest.skip(f"Could not create model {model_name} with error {err}")
-    if use_lora:
-        if model_name == "gpt2":
-            pytest.skip("Not testing LoRA for gpt2")
-        model = add_lora(model, model_name)
+    model = prepare_model(model_name, use_lora)
 
     inp1 = torch.randint(1, 1000, size=(2, 3), device=devices[0])
     inp2 = torch.randint(1, 1000, size=(2, 1), device=devices[0])
     inp3 = torch.randint(1, 1000, size=(2, 2), device=devices[0])
 
     out1_ref = model(inp1, use_cache=True, output_hidden_states=True)
     out2_ref = model(inp2, use_cache=True, past_key_values=out1_ref.past_key_values)
```

