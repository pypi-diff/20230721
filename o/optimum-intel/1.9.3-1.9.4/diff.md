# Comparing `tmp/optimum-intel-1.9.3.tar.gz` & `tmp/optimum-intel-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-intel-1.9.3.tar", last modified: Fri Jun 30 16:19:34 2023, max compression
+gzip compressed data, was "optimum-intel-1.9.4.tar", last modified: Thu Jul 20 22:41:58 2023, max compression
```

## Comparing `optimum-intel-1.9.3.tar` & `optimum-intel-1.9.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.346316 optimum-intel-1.9.3/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.346316 optimum-intel-1.9.3/optimum/commands/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/commands/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/commands/neural_compressor/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/commands/neural_compressor/quantize.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/commands/register/register_inc.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/generation/
--rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/generation/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/generation/modeling.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.356316 optimum-intel-1.9.3/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3801 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    28880 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    39154 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-06-30 15:23:44.000000 optimum-intel-1.9.3/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15386 2023-06-30 15:34:13.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18209 2023-06-30 15:34:13.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    17272 2023-06-30 15:36:28.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    28923 2023-06-30 15:34:13.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18209 2023-06-30 15:36:28.000000 optimum-intel-1.9.3/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    14186 2023-06-30 15:38:45.000000 optimum-intel-1.9.3/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-06-30 15:23:44.000000 optimum-intel-1.9.3/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-06-30 15:23:44.000000 optimum-intel-1.9.3/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     9057 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/optimum/intel/utils/modeling_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-30 15:47:07.000000 optimum-intel-1.9.3/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-30 15:50:15.000000 optimum-intel-1.9.3/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-30 16:19:34.000000 optimum-intel-1.9.3/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-30 16:19:34.366316 optimum-intel-1.9.3/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-06-30 15:19:57.000000 optimum-intel-1.9.3/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.664207 optimum-intel-1.9.4/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-07-20 22:41:58.664207 optimum-intel-1.9.4/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9062 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.634207 optimum-intel-1.9.4/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.634207 optimum-intel-1.9.4/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.634207 optimum-intel-1.9.4/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.634207 optimum-intel-1.9.4/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.644207 optimum-intel-1.9.4/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6726 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.644207 optimum-intel-1.9.4/optimum/intel/generation/
+-rw-r--r--   0 ella      (1000) ella      (1000)      659 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/generation/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17914 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/generation/modeling.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.644207 optimum-intel-1.9.4/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     6317 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.644207 optimum-intel-1.9.4/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1213 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3801 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2759 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28880 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    39154 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10837 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4386 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.654207 optimum-intel-1.9.4/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1662 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3097 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    21678 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15386 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18209 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    17272 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    28923 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18209 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    14506 2023-07-20 22:38:47.000000 optimum-intel-1.9.4/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    37677 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.654207 optimum-intel-1.9.4/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1468 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1042 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     9057 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3553 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/optimum/intel/utils/modeling_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-07-20 22:40:02.000000 optimum-intel-1.9.4/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-07-20 22:41:58.664207 optimum-intel-1.9.4/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    10309 2023-07-20 22:41:57.000000 optimum-intel-1.9.4/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     2012 2023-07-20 22:41:58.000000 optimum-intel-1.9.4/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-07-20 22:41:57.000000 optimum-intel-1.9.4/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-07-20 22:41:58.000000 optimum-intel-1.9.4/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-07-20 22:41:57.000000 optimum-intel-1.9.4/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      441 2023-07-20 22:41:58.000000 optimum-intel-1.9.4/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-07-20 22:41:58.000000 optimum-intel-1.9.4/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-07-20 22:37:13.000000 optimum-intel-1.9.4/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-07-20 22:41:58.664207 optimum-intel-1.9.4/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2671 2023-07-20 22:38:41.000000 optimum-intel-1.9.4/setup.py
```

### Comparing `optimum-intel-1.9.3/LICENSE` & `optimum-intel-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/MANIFEST.in` & `optimum-intel-1.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/PKG-INFO` & `optimum-intel-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.3
+Version: 1.9.4
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.3/README.md` & `optimum-intel-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/commands/neural_compressor/base.py` & `optimum-intel-1.9.4/optimum/commands/neural_compressor/base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/commands/neural_compressor/quantize.py` & `optimum-intel-1.9.4/optimum/commands/neural_compressor/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/commands/register/register_inc.py` & `optimum-intel-1.9.4/optimum/commands/register/register_inc.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/__init__.py` & `optimum-intel-1.9.4/optimum/intel/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/generation/__init__.py` & `optimum-intel-1.9.4/optimum/intel/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/generation/modeling.py` & `optimum-intel-1.9.4/optimum/intel/generation/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/ipex/inference.py` & `optimum-intel-1.9.4/optimum/intel/ipex/inference.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/__init__.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/configuration.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/modeling_diffusion.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.9.4/optimum/intel/neural_compressor/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/__init__.py` & `optimum-intel-1.9.4/optimum/intel/openvino/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/configuration.py` & `optimum-intel-1.9.4/optimum/intel/openvino/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/modeling.py` & `optimum-intel-1.9.4/optimum/intel/openvino/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.9.4/optimum/intel/openvino/modeling_base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.9.4/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/modeling_decoder.py` & `optimum-intel-1.9.4/optimum/intel/openvino/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.9.4/optimum/intel/openvino/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/modeling_seq2seq.py` & `optimum-intel-1.9.4/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/quantization.py` & `optimum-intel-1.9.4/optimum/intel/openvino/quantization.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional, Tuple, Union
 
 import nncf
 import openvino
 import torch
 import transformers
+from accelerate.data_loader import DataLoaderStateMixin
 from datasets import Dataset, load_dataset
 from huggingface_hub import HfApi
 from nncf import NNCFConfig
 from nncf.torch import create_compressed_model, register_default_init_args
 from nncf.torch.dynamic_graph.io_handling import wrap_nncf_model_inputs_with_objwalk
 from nncf.torch.initialization import PTInitializingDataLoader
 from nncf.torch.nncf_network import NNCFNetwork
@@ -56,14 +57,21 @@
 logger = logging.getLogger(__name__)
 
 
 class OVDataLoader(PTInitializingDataLoader):
     def get_inputs(self, dataloader_output) -> Tuple[Tuple, Dict]:
         return (), dataloader_output
 
+    @property
+    def batch_size(self):
+        batch_size = self._data_loader.batch_size
+        if batch_size is None and isinstance(self._data_loader, DataLoaderStateMixin):
+            batch_size = self._data_loader.total_batch_size
+        return batch_size
+
 
 class OVQuantizer(OptimumQuantizer):
     """
     Handle the NNCF quantization process.
     """
 
     def __init__(self, model: transformers.PreTrainedModel, task: Optional[str] = None, seed: int = 42, **kwargs):
```

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/trainer.py` & `optimum-intel-1.9.4/optimum/intel/openvino/trainer.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/training_args.py` & `optimum-intel-1.9.4/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/openvino/utils.py` & `optimum-intel-1.9.4/optimum/intel/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/__init__.py` & `optimum-intel-1.9.4/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/constant.py` & `optimum-intel-1.9.4/optimum/intel/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.9.4/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py` & `optimum-intel-1.9.4/optimum/intel/utils/dummy_neural_compressor_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.9.4/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.9.4/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.9.4/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.9.4/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/import_utils.py` & `optimum-intel-1.9.4/optimum/intel/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/utils/modeling_utils.py` & `optimum-intel-1.9.4/optimum/intel/utils/modeling_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/optimum/intel/version.py` & `optimum-intel-1.9.4/optimum/intel/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.9.3"
+__version__ = "1.9.4"
```

### Comparing `optimum-intel-1.9.3/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.9.4/optimum_intel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.9.3
+Version: 1.9.4
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.9.3/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.9.4/optimum_intel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/pyproject.toml` & `optimum-intel-1.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/setup.cfg` & `optimum-intel-1.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.9.3/setup.py` & `optimum-intel-1.9.4/setup.py`

 * *Files identical despite different names*

