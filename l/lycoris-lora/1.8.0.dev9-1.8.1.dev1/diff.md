# Comparing `tmp/lycoris_lora-1.8.0.dev9.tar.gz` & `tmp/lycoris_lora-1.8.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.0.dev9.tar", last modified: Wed Jul 12 02:43:32 2023, max compression
+gzip compressed data, was "lycoris_lora-1.8.1.dev1.tar", last modified: Fri Jul 21 03:00:03 2023, max compression
```

## Comparing `lycoris_lora-1.8.0.dev9.tar` & `lycoris_lora-1.8.1.dev1.tar`

### file list

```diff
@@ -1,47 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.050250 lycoris_lora-1.8.0.dev9/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev9/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.0.dev9/Algo.md
--rw-rw-rw-   0        0        0      977 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.0.dev9/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev9/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-07-12 02:43:32.049749 lycoris_lora-1.8.0.dev9/PKG-INFO
--rw-rw-rw-   0        0        0     7677 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.034749 lycoris_lora-1.8.0.dev9/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev9/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.0.dev9/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.0.dev9/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.0.dev9/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.0.dev9/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.0.dev9/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.0.dev9/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.0.dev9/experiments/time_test.py
--rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.0.dev9/experiments/weakre_speed.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.035748 lycoris_lora-1.8.0.dev9/lycoris/
--rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.037248 lycoris_lora-1.8.0.dev9/lycoris/kohya/
--rw-rw-rw-   0        0        0    24690 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    48868 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/kohya/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/kohya/kohya_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.041248 lycoris_lora-1.8.0.dev9/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     4762 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0    10763 2023-07-06 08:19:32.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4117 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0     2103 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0     5542 2023-07-12 02:38:34.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0     9888 2023-07-12 02:43:19.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    10896 2023-07-08 09:14:16.000000 lycoris_lora-1.8.0.dev9/lycoris/modules/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-06-05 03:39:30.000000 lycoris_lora-1.8.0.dev9/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.048248 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-07-12 02:43:31.000000 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2023-07-12 02:43:31.000000 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 02:43:31.000000 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-12 02:43:31.000000 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-12 02:43:31.000000 lycoris_lora-1.8.0.dev9/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       58 2023-07-02 13:30:53.000000 lycoris_lora-1.8.0.dev9/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 02:43:32.050250 lycoris_lora-1.8.0.dev9/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-07-12 02:43:28.000000 lycoris_lora-1.8.0.dev9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 02:43:32.049249 lycoris_lora-1.8.0.dev9/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-1.8.0.dev9/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-1.8.0.dev9/tools/merge.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.494421 lycoris_lora-1.8.1.dev1/
+-rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.1.dev1/Algo.md
+-rw-rw-rw-   0        0        0     1111 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.1.dev1/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.1.dev1/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-07-21 03:00:03.493921 lycoris_lora-1.8.1.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     7451 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.469420 lycoris_lora-1.8.1.dev1/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.1.dev1/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.1.dev1/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/experiments/compare_norm.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.1.dev1/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.1.dev1/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.1.dev1/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/experiments/loha_svd.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.1.dev1/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.1.dev1/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.1.dev1/experiments/time_test.py
+-rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.1.dev1/experiments/weakre_speed.py
+-rw-rw-rw-   0        0        0     4116 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/hyperdream_gen_weight.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.470420 lycoris_lora-1.8.1.dev1/lycoris/
+-rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2514 2023-07-21 02:47:27.000000 lycoris_lora-1.8.1.dev1/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.471920 lycoris_lora-1.8.1.dev1/lycoris/kohya/
+-rw-rw-rw-   0        0        0    38215 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    48868 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/kohya/kohya_model_utils.py
+-rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/kohya/kohya_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.476420 lycoris_lora-1.8.1.dev1/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     7334 2023-07-21 02:47:27.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/attention.py
+-rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4117 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/hyperlycoris.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.477421 lycoris_lora-1.8.1.dev1/lycoris/modules/hypernet/
+-rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/hypernet/__init__.py
+-rw-rw-rw-   0        0        0     8229 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/hypernet/generater.py
+-rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    10342 2023-07-21 02:47:27.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    10065 2023-07-21 02:47:27.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    12646 2023-07-21 02:59:08.000000 lycoris_lora-1.8.1.dev1/lycoris/modules/lokr.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.478422 lycoris_lora-1.8.1.dev1/lycoris/utils/
+-rw-rw-rw-   0        0        0    21031 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/lycoris/utils/xformers_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.491920 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-07-21 03:00:03.000000 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2023-07-21 03:00:03.000000 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 03:00:03.000000 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-07-21 03:00:03.000000 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-21 03:00:03.000000 lycoris_lora-1.8.1.dev1/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-21 03:00:03.494421 lycoris_lora-1.8.1.dev1/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-07-21 02:59:27.000000 lycoris_lora-1.8.1.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 03:00:03.493422 lycoris_lora-1.8.1.dev1/tools/
+-rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-1.8.1.dev1/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2293 2023-06-05 03:39:47.000000 lycoris_lora-1.8.1.dev1/tools/merge.py
+-rw-rw-rw-   0        0        0    55333 2023-07-19 08:00:19.000000 lycoris_lora-1.8.1.dev1/train_hyperdream.py
```

### Comparing `lycoris_lora-1.8.0.dev9/.gitignore` & `lycoris_lora-1.8.1.dev1/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # test
 test_model/
+huggingface/
+*.safetensors
+*.pt
+*.ckpt
+logs/
+output/
 
 # Editors
 .vscode/
 .idea/
 
 # Vagrant
 .vagrant/
```

### Comparing `lycoris_lora-1.8.0.dev9/Algo.md` & `lycoris_lora-1.8.1.dev1/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/Change.md` & `lycoris_lora-1.8.1.dev1/Change.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Change Log
 
+## 2023/07/19 update to 1.8.0
+* reimplement weight init method
+* implement HyperDreamBooth into LyCORIS
+* better file structure
+
 ## 2023/06/28 update to 1.7.1
 * **rearrange the version format, previous 0.1.7 should be 1.7.0**
 * fix the bug in scale weight norm
 
 ## 2023/06/26 Update to 0.1.7
 * Add support for rank_dropout and module_dropout on LoCon/LoHa/LoKr
 * Add support for scale_weight_norms on LoCon/LoHa/LoKr
```

### Comparing `lycoris_lora-1.8.0.dev9/Demo.md` & `lycoris_lora-1.8.1.dev1/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/LICENSE.md` & `lycoris_lora-1.8.1.dev1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/README.md` & `lycoris_lora-1.8.1.dev1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -134,22 +134,19 @@
 ## Example and Comparing for different algo
 see [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) and [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md)
 
 
 ## Change Log
 For full log, please see [Change.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Change.md)
 
-### 2023/06/28 update to 1.7.1
-* **rearrange the version format, previous 0.1.7 should be 1.7.0**
-* fix the bug in scale weight norm
+## 2023/07/19 update to 1.8.0
+* reimplement weight init method
+* implement HyperDreamBooth into LyCORIS
+* better file structure
 
-### 2023/06/26 Update for 0.1.7
-* Add support for rank_dropout and module_dropout on LoCon/LoHa/LoKr
-* Add support for scale_weight_norms on LoCon/LoHa/LoKr
-* Will support SDXL on 0.1.8 (you can follow the dev branch)
 
 ## Todo list
 - [ ] Module and Document for using LyCORIS in any other model, Not only SD.
 - [x] Proposition3 in [FedPara](https://arxiv.org/abs/2108.06098)
   * also need custom backward to save the vram
 - [ ] Low rank + sparse representation
   - [x] For extraction
```

### Comparing `lycoris_lora-1.8.0.dev9/experiments/better_conv.py` & `lycoris_lora-1.8.1.dev1/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/better_conv_extract.py` & `lycoris_lora-1.8.1.dev1/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/concept_neuron.py` & `lycoris_lora-1.8.1.dev1/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/locon_extract_test.py` & `lycoris_lora-1.8.1.dev1/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/locon_merge_test.py` & `lycoris_lora-1.8.1.dev1/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/singular_value_test.py` & `lycoris_lora-1.8.1.dev1/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/sparse_bias_test.py` & `lycoris_lora-1.8.1.dev1/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/experiments/time_test.py` & `lycoris_lora-1.8.1.dev1/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/kohya/__init__.py` & `lycoris_lora-1.8.1.dev1/lycoris/kohya/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 # https://github.com/kohya-ss/sd-scripts/blob/main/networks/lora.py
 
 import math
 from warnings import warn
 import os
 from typing import List
 import torch
+import torch.utils.checkpoint as checkpoint
 
 from .kohya_utils import *
 from ..modules.locon import LoConModule
 from ..modules.loha import LohaModule
 from ..modules.ia3 import IA3Module
 from ..modules.lokr import LokrModule
 from ..modules.dylora import DyLoraModule
 from ..modules.glora import GLoRAModule
+from ..modules.hypernet import ImgWeightGenerator
 
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
         network_dim = 4                     # default
     conv_dim = int(kwargs.get('conv_dim', network_dim) or network_dim)
     conv_alpha = float(kwargs.get('conv_alpha', network_alpha) or network_alpha)
@@ -74,17 +76,56 @@
             use_cp=use_cp,
             network_module=network_module,
             decompose_both=kwargs.get('decompose_both', False),
             factor=kwargs.get('factor', -1),
             block_size = block_size
         )
     
+    if algo=='dylora':
+        #dylora didn't support scale weight norm yet
+        delattr(network, 'apply_max_norm_regularization')
+    
     return network
 
 
+def create_hypernetwork(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
+    if network_dim is None:
+        network_dim = 4
+    dropout = float(kwargs.get('dropout', 0.) or 0.)
+    rank_dropout = float(kwargs.get("rank_dropout", 0.) or 0.)
+    module_dropout = float(kwargs.get("module_dropout", 0.) or 0.)
+    algo = (kwargs.get('algo', 'lora') or 'lora').lower()
+    use_cp = (not kwargs.get('disable_conv_cp', True)
+              or kwargs.get('use_conv_cp', False))
+    block_size = int(kwargs.get('block_size', 4) or 4)
+    down_dim = int(kwargs.get('down_dim', 128) or 128)
+    up_dim = int(kwargs.get('up_dim', 64) or 64)
+    delta_iters = int(kwargs.get('delta_iters', 5) or 5)
+    decoder_blocks = int(kwargs.get('decoder_blocks', 4) or 4)
+    network_module = {
+        'lora': LoConModule,
+        'locon': LoConModule,
+    }[algo]
+    
+    print(f'Using rank adaptation algo: {algo}')
+    
+    return HyperDreamNetwork(
+        text_encoder, unet, 
+        multiplier=multiplier, 
+        lora_dim=network_dim, alpha=network_alpha,
+        use_cp=use_cp,
+        dropout=dropout, rank_dropout=rank_dropout, module_dropout=module_dropout,
+        network_module=network_module,
+        down_dim=down_dim, up_dim=up_dim, delta_iters=delta_iters, decoder_blocks=decoder_blocks,
+        decompose_both=kwargs.get('decompose_both', False),
+        factor=kwargs.get('factor', -1),
+        block_size = block_size
+    )
+
+
 class LycorisNetwork(torch.nn.Module):
     '''
     LoRA + LoCon
     '''
     # Ignore proj_in or proj_out, their channels is only a few.
     UNET_TARGET_REPLACE_MODULE = [
         "Transformer2DModel", 
@@ -402,14 +443,288 @@
                 scaled, norm = lora.apply_max_norm(max_norm_value, device)
                 norms.append(norm)
                 scaled += int(scaled)
         
         return scaled, sum(norms)/len(norms), max(norms)
 
 
+class HyperDreamNetwork(torch.nn.Module):
+    '''
+    HyperDreamBooth hypernetwork part
+    only train Attention right now
+    '''
+    UNET_TARGET_REPLACE_MODULE = [
+        "Attention", 
+    ]
+    UNET_TARGET_REPLACE_NAME = []
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention"]
+    LORA_PREFIX_UNET = 'lora_unet'
+    LORA_PREFIX_TEXT_ENCODER = 'lora_te'
+
+    def __init__(
+        self, 
+        text_encoder, unet, 
+        multiplier=1.0, 
+        lora_dim=4, alpha=1,
+        use_cp = False,
+        dropout = 0, rank_dropout = 0, module_dropout = 0,
+        network_module = LoConModule,
+        down_dim = 100, up_dim = 50, delta_iters = 5, decoder_blocks = 4,
+        **kwargs,
+    ) -> None:
+        super().__init__()
+        self.gradient_ckpt = False
+        self.multiplier = multiplier
+        self.lora_dim = lora_dim
+        self.alpha = alpha
+        
+        if 1 >= dropout >= 0:
+            print(f'Use Dropout value: {dropout}')
+        if network_module != LoConModule:
+            print('HyperDreamBooth only support LoRA at this time')
+            raise NotImplementedError
+        if lora_dim*(down_dim+up_dim) > 4096:
+            print('weight elements > 4096 (dim * (down_dim + up_dim)) is not recommended!')
+        
+        self.dropout = dropout
+        self.rank_dropout = rank_dropout
+        self.module_dropout = module_dropout
+        
+        # create module instances
+        def create_modules(
+            prefix, 
+            root_module: torch.nn.Module, 
+            target_replace_modules,
+            target_replace_names = []
+        ) -> List[network_module]:
+            print('Create LyCORIS Module')
+            loras = []
+            for name, module in root_module.named_modules():
+                if module.__class__.__name__ in target_replace_modules:
+                    for child_name, child_module in module.named_modules():
+                        lora_name = prefix + '.' + name + '.' + child_name
+                        lora_name = lora_name.replace('.', '_')
+                        if child_module.__class__.__name__ == 'Linear' and lora_dim>0:
+                            lora = network_module(
+                                lora_name, child_module, self.multiplier, 
+                                self.lora_dim, self.alpha, 
+                                self.dropout, self.rank_dropout, self.module_dropout, 
+                                use_cp,
+                                **kwargs
+                            )
+                        elif child_module.__class__.__name__ == 'Conv2d':
+                            k_size, *_ = child_module.kernel_size
+                            if k_size==1 and lora_dim>0:
+                                lora = network_module(
+                                    lora_name, child_module, self.multiplier, 
+                                    self.lora_dim, self.alpha, 
+                                    self.dropout, self.rank_dropout, self.module_dropout, 
+                                    use_cp,
+                                    **kwargs
+                                )
+                            else:
+                                continue
+                        else:
+                            continue
+                        loras.append(lora)
+                elif name in target_replace_names:
+                    lora_name = prefix + '.' + name
+                    lora_name = lora_name.replace('.', '_')
+                    if module.__class__.__name__ == 'Linear' and lora_dim>0:
+                        lora = network_module(
+                            lora_name, module, self.multiplier, 
+                            self.lora_dim, self.alpha, 
+                            self.dropout, self.rank_dropout, self.module_dropout, 
+                            use_cp,
+                            **kwargs
+                        )
+                    elif module.__class__.__name__ == 'Conv2d':
+                        k_size, *_ = module.kernel_size
+                        if k_size==1 and lora_dim>0:
+                            lora = network_module(
+                                lora_name, module, self.multiplier, 
+                                self.lora_dim, self.alpha, 
+                                self.dropout, self.rank_dropout, self.module_dropout, 
+                                use_cp,
+                                **kwargs
+                            )
+                        else:
+                            continue
+                    else:
+                        continue
+                    loras.append(lora)
+            return loras
+
+        if isinstance(text_encoder, list):
+            text_encoders = text_encoder
+            use_index = True
+        else:
+            text_encoders = [text_encoder]
+            use_index = False
+
+        self.text_encoder_loras = []
+        for i, te in enumerate(text_encoders):
+            self.text_encoder_loras.extend(create_modules(
+                LycorisNetwork.LORA_PREFIX_TEXT_ENCODER + (f'{i+1}' if use_index else ''),
+                te, 
+                LycorisNetwork.TEXT_ENCODER_TARGET_REPLACE_MODULE
+            ))
+        print(f"create LyCORIS for Text Encoder: {len(self.text_encoder_loras)} modules.")
+
+        self.unet_loras = create_modules(LycorisNetwork.LORA_PREFIX_UNET, unet, LycorisNetwork.UNET_TARGET_REPLACE_MODULE)
+        print(f"create LyCORIS for U-Net: {len(self.unet_loras)} modules.")
+        
+        self.loras: list[LoConModule] = self.text_encoder_loras + self.unet_loras
+        self.weight_generater = ImgWeightGenerator(
+            weight_dim=(down_dim+up_dim)*lora_dim,
+            weight_num=len(self.loras),
+            sample_iters=delta_iters,
+            decoder_blocks=decoder_blocks,
+        )
+        self.split = (down_dim* lora_dim, up_dim  * lora_dim)
+        self.lora_dim = lora_dim
+
+        self.weights_sd = None
+
+        # assertion
+        names = set()
+        for lora in self.text_encoder_loras + self.unet_loras:
+            assert lora.lora_name not in names, f"duplicated lora name: {lora.lora_name}"
+            names.add(lora.lora_name)
+        
+        self.checkpoint = torch.nn.Parameter(torch.tensor(0.0))
+        
+        with torch.no_grad():
+            self.update_reference(torch.randn(1, 3, *self.weight_generater.ref_size))
+        
+        # for lora in self.loras:
+        #     assert torch.all(lora.data[0]==0)
+
+    def gen_weight(self, ref_img, iter=None):
+        weights = self.weight_generater(ref_img, iter)
+        weights = weights + self.checkpoint
+        return [i.split(self.split, dim=-1) for i in weights.split(1, dim=1)]
+
+    def update_reference(self, ref_img, iter=None):
+        # use idx for aux weight seed
+        if self.gradient_ckpt and self.training:
+            weights_list = checkpoint.checkpoint(self.gen_weight, ref_img, iter)
+        else:
+            weights_list = self.gen_weight(ref_img, iter)
+        for idx, (lora, weight) in enumerate(zip(self.loras, weights_list)):
+            assert lora.multiplier > 0, f"multiplier must be positive: {lora.multiplier}"
+            # weight: [batch, 1, weight_dim]
+            # if weight.dim()==3:
+            #     weight = weight.squeeze(1)
+            lora.update_weights(*weight, idx)
+
+    def set_multiplier(self, multiplier):
+        self.multiplier = multiplier
+        for lora in self.text_encoder_loras + self.unet_loras:
+            lora.multiplier = self.multiplier
+    
+    def load_weights(self, file):
+        if os.path.splitext(file)[1] == '.safetensors':
+            from safetensors.torch import load_file, safe_open
+            self.weights_sd = load_file(file)
+        else:
+            self.weights_sd = torch.load(file, map_location='cpu')
+
+    def apply_to(self, text_encoder, unet, apply_text_encoder=None, apply_unet=None):
+        if self.weights_sd:
+            weights_has_text_encoder = weights_has_unet = False
+            for key in self.weights_sd.keys():
+                if key.startswith(LycorisNetwork.LORA_PREFIX_TEXT_ENCODER):
+                    weights_has_text_encoder = True
+                elif key.startswith(LycorisNetwork.LORA_PREFIX_UNET):
+                    weights_has_unet = True
+
+            if apply_text_encoder is None:
+                apply_text_encoder = weights_has_text_encoder
+            else:
+                assert apply_text_encoder == weights_has_text_encoder, f"text encoder weights: {weights_has_text_encoder} but text encoder flag: {apply_text_encoder} / 重みとText Encoderのフラグが矛盾しています"
+
+            if apply_unet is None:
+                apply_unet = weights_has_unet
+            else:
+                assert apply_unet == weights_has_unet, f"u-net weights: {weights_has_unet} but u-net flag: {apply_unet} / 重みとU-Netのフラグが矛盾しています"
+        else:
+            assert apply_text_encoder is not None and apply_unet is not None, f"internal error: flag not set"
+
+        if apply_text_encoder:
+            print("enable LyCORIS for text encoder")
+        else:
+            self.text_encoder_loras = []
+
+        if apply_unet:
+            print("enable LyCORIS for U-Net")
+        else:
+            self.unet_loras = []
+
+        for lora in self.text_encoder_loras + self.unet_loras:
+            lora.apply_to(is_hypernet=True)
+
+    def enable_gradient_checkpointing(self):
+        self.gradient_ckpt = True
+
+    def prepare_optimizer_params(self, text_encoder_lr, unet_lr, learning_rate):
+        self.requires_grad_(True)
+        all_params = []
+        all_params.append({
+            'params': (
+                [p for p in self.weight_generater.decoder_model.parameters()]
+                + [p for p in self.weight_generater.pos_emb_proj.parameters()]
+                + [p for p in self.weight_generater.feature_proj.parameters()]
+                + ([p for p in self.weight_generater.encoder_model.parameters()] 
+                   if self.weight_generater.train_encoder else [])
+            ), 
+            'lr': learning_rate
+        })
+        return all_params
+
+    def prepare_grad_etc(self, text_encoder, unet):
+        self.requires_grad_(True)
+
+    def on_epoch_start(self, text_encoder, unet):
+        self.train()
+
+    def get_trainable_params(self):
+        return self.parameters()
+
+    def save_weights(self, file, dtype, metadata):
+        if metadata is not None and len(metadata) == 0:
+            metadata = None
+
+        state_dict = self.weight_generater.state_dict()
+        if not self.weight_generater.train_encoder:
+            for k in self.weight_generater.encoder_model.state_dict().keys():
+                state_dict.pop(f'encoder_model.{k}')
+        state_dict = {f'weight_generater.{i}': v for i, v in state_dict.items()}
+
+        if dtype is not None:
+            for key in list(state_dict.keys()):
+                v = state_dict[key]
+                v = v.detach().clone().to("cpu").to(dtype)
+                state_dict[key] = v
+
+        if os.path.splitext(file)[1] == '.safetensors':
+            from safetensors.torch import save_file
+
+            # Precalculate model hashes to save time on indexing
+            if metadata is None:
+                metadata = {}
+            model_hash, legacy_hash = precalculate_safetensors_hashes(state_dict, metadata)
+            metadata["sshs_model_hash"] = model_hash
+            metadata["sshs_legacy_hash"] = legacy_hash
+
+            save_file(state_dict, file, metadata)
+        else:
+            torch.save(state_dict, file)
+
+
 class IA3Network(torch.nn.Module):
     '''
     IA3 network
     '''
     # Ignore proj_in or proj_out, their channels is only a few.
     UNET_TARGET_REPLACE_MODULE = []
     UNET_TARGET_REPLACE_NAME = ["to_k", "to_v", "ff.net.2"]
```

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/kohya/kohya_model_utils.py` & `lycoris_lora-1.8.1.dev1/lycoris/kohya/kohya_model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/kohya/kohya_utils.py` & `lycoris_lora-1.8.1.dev1/lycoris/kohya/kohya_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/modules/dylora.py` & `lycoris_lora-1.8.1.dev1/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/modules/glokr.py` & `lycoris_lora-1.8.1.dev1/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/modules/glora.py` & `lycoris_lora-1.8.1.dev1/lycoris/modules/glora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/modules/ia3.py` & `lycoris_lora-1.8.1.dev1/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/modules/loha.py` & `lycoris_lora-1.8.1.dev1/lycoris/modules/loha.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,14 +162,18 @@
         torch.nn.init.normal_(self.hada_w1_a, std=0.1)
         torch.nn.init.normal_(self.hada_w2_b, std=1)
         torch.nn.init.normal_(self.hada_w2_a, std=0.1)
 
         self.multiplier = multiplier
         self.org_module = [org_module] # remove in applying
         self.grad_ckpt = False
+        self.register_load_state_dict_post_hook(self.load_weight_hook)
+    
+    def load_weight_hook(self):
+        self.scalar = nn.Parameter(torch.ones_like(self.scalar))
 
     def apply_to(self):
         self.org_module[0].forward = self.forward
 
     def get_weight(self, orig_weight=None):
         if self.cp:
             weight = make_weight_cp(
```

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/modules/lokr.py` & `lycoris_lora-1.8.1.dev1/lycoris/modules/lokr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+from collections import OrderedDict
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 # 4, build custom backward function
 #  - 
@@ -17,20 +18,20 @@
     secon value is a value for weight.
     
     Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
     
     examples)
     factor
         -1               2                4               8               16               ...
-    127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
-    128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
-    250 -> 125, 2   250 -> 125, 2    250 -> 125, 2   250 -> 125, 2   250 -> 125, 2
-    360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
-    512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
-    1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
+    127 -> 1, 127   127 -> 1, 127    127 -> 1, 127   127 -> 1, 127   127 -> 1, 127
+    128 -> 8, 16    128 -> 2, 64     128 -> 4, 32    128 -> 8, 16    128 -> 8, 16
+    250 -> 10, 25   250 -> 2, 125    250 -> 2, 125   250 -> 5, 50    250 -> 10, 25
+    360 -> 8, 45    360 -> 2, 180    360 -> 4, 90    360 -> 8, 45    360 -> 12, 30
+    512 -> 16, 32   512 -> 2, 256    512 -> 4, 128   512 -> 8, 64    512 -> 16, 32
+    1024 -> 32, 32  1024 -> 2, 512   1024 -> 4, 256  1024 -> 8, 128  1024 -> 16, 64
     '''
     
     if factor > 0 and (dimension % factor) == 0:
         m = factor
         n = dimension // factor
         return m, n
     if factor == -1:
@@ -170,21 +171,22 @@
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         if self.use_w2 and self.use_w1:
             #use scale = 1
             alpha = lora_dim
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
+        self.scalar = nn.Parameter(torch.tensor(0.0))
         if self.use_w2:
             torch.nn.init.constant_(self.lokr_w2, 0)
         else:
             if self.cp:
                 torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
             torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
-            torch.nn.init.constant_(self.lokr_w2_b, 0)
+            torch.nn.init.kaiming_uniform_(self.lokr_w2_b, a=math.sqrt(5))
         
         if self.use_w1:
             torch.nn.init.kaiming_uniform_(self.lokr_w1, a=math.sqrt(5))
         else:
             torch.nn.init.kaiming_uniform_(self.lokr_w1_a, a=math.sqrt(5))
             torch.nn.init.kaiming_uniform_(self.lokr_w1_b, a=math.sqrt(5))
 
@@ -194,14 +196,18 @@
             self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
             (self.lokr_w2 if self.use_w2 
              else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
              else self.lokr_w2_a@self.lokr_w2_b),
             torch.tensor(self.multiplier * self.scale)
         )
         assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
+        self.register_load_state_dict_post_hook(self.load_weight_hook)
+    
+    def load_weight_hook(self):
+        self.scalar = nn.Parameter(torch.ones_like(self.scalar))
 
     # Same as locon.py
     def apply_to(self):
         self.org_forward = self.org_module[0].forward
         self.org_module[0].forward = self.forward
     
     def get_weight(self, orig_weight = None):
@@ -214,14 +220,49 @@
         )
         if orig_weight is not None:
             weight = weight.reshape(orig_weight.shape)
         if self.training and self.rank_dropout:
             drop = torch.rand(weight.size(0)) < self.rank_dropout
             weight *= drop.view(-1, [1]*len(weight.shape[1:])).to(weight.device)
         return weight
+    
+    def state_dict(self, *args, destination=None, prefix='', keep_vars=False):
+        # TODO: Remove `args` and the parsing logic when BC allows.
+        if len(args) > 0:
+            if destination is None:
+                destination = args[0]
+            if len(args) > 1 and prefix == '':
+                prefix = args[1]
+            if len(args) > 2 and keep_vars is False:
+                keep_vars = args[2]
+            # DeprecationWarning is ignored by default
+
+        if destination is None:
+            destination = OrderedDict()
+            destination._metadata = OrderedDict()
+
+        local_metadata = dict(version=self._version)
+        if hasattr(destination, "_metadata"):
+            destination._metadata[prefix[:-1]] = local_metadata
+
+        destination[f'{prefix}alpha'] = self.alpha
+        if self.use_w1:
+            destination[f'{prefix}lokr_w1'] = self.lokr_w1 * self.scalar
+        else:
+            destination[f'{prefix}lokr_w1_a'] = self.lokr_w1_a * self.scalar
+            destination[f'{prefix}lokr_w1_b'] = self.lokr_w1_b
+        
+        if self.use_2:
+            destination[f'{prefix}lokr_w2'] = self.lokr_w2
+        else:
+            destination[f'{prefix}lokr_w2_a'] = self.lokr_w2_a
+            destination[f'{prefix}lokr_w2_b'] = self.lokr_w2_b
+            if self.cp:
+                destination[f'{prefix}lokr_t2'] = self.lokr_t2
+        return destination
 
     @torch.no_grad()
     def apply_max_norm(self, max_norm, device=None):
         orig_norm = self.get_weight().norm()
         norm = torch.clamp(orig_norm, max_norm/2)
         desired = torch.clamp(norm, max=max_norm)
         ratio = desired.cpu()/norm.cpu()
@@ -251,15 +292,15 @@
                 return self.op(
                     x,
                     self.org_module[0].weight.data,
                     None if self.org_module[0].bias is None else self.org_module[0].bias.data
                 )
         weight = (
             self.org_module[0].weight.data 
-            + self.get_weight(self.org_module[0].weight.data) * self.multiplier
+            + self.get_weight(self.org_module[0].weight.data) * self.scalar * self.multiplier
         )
         bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
         return self.op(
             x, 
             weight.view(self.shape),
             bias,
             **self.extra_args
```

### Comparing `lycoris_lora-1.8.0.dev9/lycoris/utils.py` & `lycoris_lora-1.8.1.dev1/lycoris/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 import torch.nn.functional as F
 
 import torch.linalg as linalg
 
 from tqdm import tqdm
 
 
+def default(val, d):
+    return val if val is not None else d
+
+
 def make_sparse(t: torch.Tensor, sparsity=0.95):
     abs_t = torch.abs(t)
     np_array = abs_t.detach().cpu().numpy()
     quan = float(np.quantile(np_array, sparsity))
     sparse_t = t.masked_fill(abs_t < quan, 0)
     return sparse_t
```

### Comparing `lycoris_lora-1.8.0.dev9/setup.py` & `lycoris_lora-1.8.1.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.0.dev9',
+    version='1.8.1.dev1',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-1.8.0.dev9/tools/extract_locon.py` & `lycoris_lora-1.8.1.dev1/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.0.dev9/tools/merge.py` & `lycoris_lora-1.8.1.dev1/tools/merge.py`

 * *Files identical despite different names*

