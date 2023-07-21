# Comparing `tmp/hiera-transformer-0.1.1.tar.gz` & `tmp/hiera-transformer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiera-transformer-0.1.1.tar", last modified: Tue Jun 13 01:13:30 2023, max compression
+gzip compressed data, was "hiera-transformer-0.1.2.tar", last modified: Fri Jul 21 04:22:06 2023, max compression
```

## Comparing `hiera-transformer-0.1.1.tar` & `hiera-transformer-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:13:30.878605 hiera-transformer-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-06-13 01:13:30.878605 hiera-transformer-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10852 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:13:30.878605 hiera-transformer-0.1.1/hiera/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/hiera/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/hiera/benchmarking.py
--rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/hiera/hiera.py
--rw-r--r--   0 runner    (1001) docker     (123)    10425 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/hiera/hiera_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)    10719 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/hiera/hiera_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 01:13:30.878605 hiera-transformer-0.1.1/hiera_transformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-06-13 01:13:30.000000 hiera-transformer-0.1.1/hiera_transformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-13 01:13:30.000000 hiera-transformer-0.1.1/hiera_transformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 01:13:30.000000 hiera-transformer-0.1.1/hiera_transformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 01:13:30.000000 hiera-transformer-0.1.1/hiera_transformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 01:13:30.000000 hiera-transformer-0.1.1/hiera_transformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 01:13:30.878605 hiera-transformer-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-13 01:13:14.000000 hiera-transformer-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:22:06.572847 hiera-transformer-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-21 04:22:06.572847 hiera-transformer-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:22:06.572847 hiera-transformer-0.1.2/hiera/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/hiera/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/hiera/benchmarking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18527 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/hiera/hiera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/hiera/hiera_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/hiera/hiera_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 04:22:06.572847 hiera-transformer-0.1.2/hiera_transformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-21 04:22:06.000000 hiera-transformer-0.1.2/hiera_transformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-21 04:22:06.000000 hiera-transformer-0.1.2/hiera_transformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 04:22:06.000000 hiera-transformer-0.1.2/hiera_transformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-21 04:22:06.000000 hiera-transformer-0.1.2/hiera_transformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 04:22:06.000000 hiera-transformer-0.1.2/hiera_transformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 04:22:06.572847 hiera-transformer-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-21 04:21:54.000000 hiera-transformer-0.1.2/setup.py
```

### Comparing `hiera-transformer-0.1.1/LICENSE` & `hiera-transformer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hiera-transformer-0.1.1/PKG-INFO` & `hiera-transformer-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiera-transformer
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fast, powerful, and simple hierarchical vision transformer
 Home-page: https://github.com/facebookresearch/hiera
 Author: Chaitanya Ryali, Daniel Bolya
 License: CC BY-NC 4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -69,57 +69,59 @@
 cd hiera
 python setup.py build develop
 ```
 
 
 ## Model Zoo
 
-Here we provide model checkpoints for Hiera. Each model listed is accessible on [torch hub](https://pytorch.org/docs/stable/hub.html), e.g.:
+Here we provide model checkpoints for Hiera. Each model listed is accessible on [torch hub](https://pytorch.org/docs/stable/hub.html) even without the `hiera-transformer` package installed, e.g. the following initializes a base model pretrained and finetuned on ImageNet-1k:
 ```py
 model = torch.hub.load("facebookresearch/hiera", model="hiera_base_224", pretrained=True, checkpoint="mae_in1k_ft_in1k")
 ```
-For model names and corresponding checkpoint names see below.
 
-**Note:** the speeds listed here were benchmarked _without_ PyTorch's optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html). If using PyTorch 2.0 or above, your inference speed will probably be faster than what's listed here.
+If you want a model with MAE pretraining only, you can replace the checkpoint with `"mae_in1k"`. Additionally, if you'd like to load the MAE decoder as well (e.g., to continue pretraining), add `mae_` the the start of the model name, e.g.:
+```py
+model = torch.hub.load("facebookresearch/hiera", model="mae_hiera_base_224", pretrained=True, checkpoint="mae_in1k")
+```
+**Note:** Our MAE models were trained with a _normalized pixel loss_. That means that the patches were normalized before the network had to predict them. If you want to visualize the predictions, you'll have to unnormalize them using the visible patches (which might work but wouldn't be perfect) or unnormalize them using the ground truth. For model more names and corresponding checkpoint names see below.
 
-#### Coming Soon
-As of now, base finetuned models are available. The rest are coming soon.
 
+**Note:** the speeds listed here were benchmarked _without_ PyTorch's optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html). If using PyTorch 2.0 or above, your inference speed will probably be faster than what's listed here.
 ### Image Models
 | Model    | Model Name            | Pretrained Models<br>(IN-1K MAE) | Finetuned Models<br>(IN-1K Supervised) | IN-1K<br>Top-1 (%) | A100 fp16<br>Speed (im/s) |
 |----------|-----------------------|----------------------------------|----------------------------------------|:------------------:|:-------------------------:|
-| Hiera-T  | `hiera_tiny_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth)       |       82.8         |            2758           |
-| Hiera-S  | `hiera_small_224`     | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth)      |       83.8         |            2211           |
-| Hiera-B  | `hiera_base_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth)       |       84.5         |            1556           |
-| Hiera-B+ | `hiera_base_plus_224` | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth)  |       85.2         |            1247           |
-| Hiera-L  | `hiera_large_224`     | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth)      |       86.1         |            531            |
-| Hiera-H  | `hiera_huge_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth)       |       86.9         |            274            |
+| Hiera-T  | `hiera_tiny_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_tiny_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth)       |       82.8         |            2758           |
+| Hiera-S  | `hiera_small_224`     | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_small_224.pth)       | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth)      |       83.8         |            2211           |
+| Hiera-B  | `hiera_base_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth)       |       84.5         |            1556           |
+| Hiera-B+ | `hiera_base_plus_224` | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_224.pth)   | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth)  |       85.2         |            1247           |
+| Hiera-L  | `hiera_large_224`     | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_224.pth)       | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth)      |       86.1         |            531            |
+| Hiera-H  | `hiera_huge_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth)       |       86.9         |            274            |
 
 Each model inputs a 224x224 image.
 ### Video Models
 | Model    | Model Name               | Pretrained Models<br>(K400 MAE) | Finetuned Models<br>(K400) | K400 (3x5 views)<br>Top-1 (%) | A100 fp16<br>Speed (clip/s) |
 |----------|--------------------------|---------------------------------|----------------------------|:-----------------------------:|:---------------------------:|
-| Hiera-B  | `hiera_base_16x224`      | Coming Soon                     | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth)      |              84.0             |            133.6            |
-| Hiera-B+ | `hiera_base_plus_16x224` | Coming Soon                     | Coming Soon |              85.0             |             84.1            |
-| Hiera-L  | `hiera_large_16x224`     | Coming Soon                     | Coming Soon |              87.3             |             40.8            |
-| Hiera-H  | `hiera_huge_16x224`      | Coming Soon                     | Coming Soon |              87.8             |             20.9            |
+| Hiera-B  | `hiera_base_16x224`      | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_16x224.pth)       | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth)      |              84.0             |            133.6            |
+| Hiera-B+ | `hiera_base_plus_16x224` | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_16x224.pth)  | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_16x224.pth) |              85.0             |             84.1            |
+| Hiera-L  | `hiera_large_16x224`     | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_16x224.pth)      | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_large_16x224.pth)     |              87.3             |             40.8            |
+| Hiera-H  | `hiera_huge_16x224`      | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_16x224.pth)       | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_huge_16x224.pth)      |              87.8             |             20.9            |
 
 Each model inputs 16 224x224 frames with a temporal stride of 4.
 
 
 ## Usage
 
 This repo implements the code to run Hiera models for inference. This repository is still in progress. Here's what we currently have available and what we have planned:
 
  - [x] Image Inference
     - [x] MAE implementation
  - [x] Video Inference
-    - [ ] MAE implementation
+    - [x] MAE implementation
+ - [x] Full Model Zoo
  - [ ] Training scripts
- - [ ] Full Model Zoo
 
 
 See [examples](https://github.com/facebookresearch/hiera/tree/main/examples) for examples of how to use Hiera.
 
 ### Inference
 
 See [examples/inference](https://github.com/facebookresearch/hiera/blob/main/examples/inference.ipynb) for an example of how to prepare the data for inference.
@@ -136,14 +138,28 @@
 Video inference works the same way, just use a `16x224` model instead.
 
 **Note**: for efficiency, Hiera re-orders its tokens at the start of the network (see the `Roll` and `Unroll` modules in `hiera_utils.py`). Thus, tokens _aren't in spatial order_ by default. If you'd like to use intermediate feature maps for a downstream task, pass the `return_intermediates` flag when running the model:
 ```py
 output, intermediates = model(x, return_intermediates=True)
 ```
 
+#### MAE Inference
+By default, the models do not include the MAE decoder. If you would like to use the decoder or compute MAE loss, you can instantiate an mae version by running:
+```py
+import hiera
+model = hiera.mae_hiera_base_224(pretrained=True, checkpoint="mae_in1k")
+```
+Then when you run inference on the model, it will return a 4-tuple of `(loss, predictions, labels, mask)` where predictions and labels are for the _deleted tokens_ only. The returned mask will be `True` if the token is visible and `False` if it's deleted. You can change the masking ratio by passing it during inference:
+```py
+loss, preds, labels, mask = model(x, mask_ratio=0.6)
+```
+The default mask ratio is `0.6` for images, but you should pass in `0.9` for video. See the paper for details.
+
+**Note:** We use _normalized pixel targets_ for MAE pretraining, meaning the patches are each individually normalized before the model model has to predict them. Thus, you have to unnormalize them using the ground truth before visualizing them. See `get_pixel_label_2d` in `hiera_mae.py` for details.
+
 ### Benchmarking
 We provide a script for easy benchmarking. See [examples/benchmark](https://github.com/facebookresearch/hiera/blob/main/examples/benchmark.ipynb) to see how to use it.
 
 #### Scaled Dot Product Attention
 PyTorch 2.0 introduced optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html), which can speed up transformers quite a bit. We didn't use this in our original benchmarking, but since it's a free speed-up this repo will automatically use it if available. To get its benefits, make sure your torch version is 2.0 or above.
 
 ### Training
```

### Comparing `hiera-transformer-0.1.1/README.md` & `hiera-transformer-0.1.2/hiera_transformer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: hiera-transformer
+Version: 0.1.2
+Summary: A fast, powerful, and simple hierarchical vision transformer
+Home-page: https://github.com/facebookresearch/hiera
+Author: Chaitanya Ryali, Daniel Bolya
+License: CC BY-NC 4.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Hiera: A Hierarchical Vision Transformer without the Bells-and-Whistles
 
 This is the official implementation for our ICML 2023 Oral paper:  
 **[Hiera: A Hierarchical Vision Transformer without the Bells-and-Whistles][arxiv-link]**  
 [Chaitanya Ryali](https://scholar.google.com/citations?user=4LWx24UAAAAJ)\*,
 [Yuan-Ting Hu](https://scholar.google.com/citations?user=aMpbemkAAAAJ)\*,
 [Daniel Bolya](https://scholar.google.com/citations?hl=en&user=K3ht_ZUAAAAJ)\*,
@@ -59,57 +69,59 @@
 cd hiera
 python setup.py build develop
 ```
 
 
 ## Model Zoo
 
-Here we provide model checkpoints for Hiera. Each model listed is accessible on [torch hub](https://pytorch.org/docs/stable/hub.html), e.g.:
+Here we provide model checkpoints for Hiera. Each model listed is accessible on [torch hub](https://pytorch.org/docs/stable/hub.html) even without the `hiera-transformer` package installed, e.g. the following initializes a base model pretrained and finetuned on ImageNet-1k:
 ```py
 model = torch.hub.load("facebookresearch/hiera", model="hiera_base_224", pretrained=True, checkpoint="mae_in1k_ft_in1k")
 ```
-For model names and corresponding checkpoint names see below.
 
-**Note:** the speeds listed here were benchmarked _without_ PyTorch's optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html). If using PyTorch 2.0 or above, your inference speed will probably be faster than what's listed here.
+If you want a model with MAE pretraining only, you can replace the checkpoint with `"mae_in1k"`. Additionally, if you'd like to load the MAE decoder as well (e.g., to continue pretraining), add `mae_` the the start of the model name, e.g.:
+```py
+model = torch.hub.load("facebookresearch/hiera", model="mae_hiera_base_224", pretrained=True, checkpoint="mae_in1k")
+```
+**Note:** Our MAE models were trained with a _normalized pixel loss_. That means that the patches were normalized before the network had to predict them. If you want to visualize the predictions, you'll have to unnormalize them using the visible patches (which might work but wouldn't be perfect) or unnormalize them using the ground truth. For model more names and corresponding checkpoint names see below.
 
-#### Coming Soon
-As of now, base finetuned models are available. The rest are coming soon.
 
+**Note:** the speeds listed here were benchmarked _without_ PyTorch's optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html). If using PyTorch 2.0 or above, your inference speed will probably be faster than what's listed here.
 ### Image Models
 | Model    | Model Name            | Pretrained Models<br>(IN-1K MAE) | Finetuned Models<br>(IN-1K Supervised) | IN-1K<br>Top-1 (%) | A100 fp16<br>Speed (im/s) |
 |----------|-----------------------|----------------------------------|----------------------------------------|:------------------:|:-------------------------:|
-| Hiera-T  | `hiera_tiny_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth)       |       82.8         |            2758           |
-| Hiera-S  | `hiera_small_224`     | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth)      |       83.8         |            2211           |
-| Hiera-B  | `hiera_base_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth)       |       84.5         |            1556           |
-| Hiera-B+ | `hiera_base_plus_224` | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth)  |       85.2         |            1247           |
-| Hiera-L  | `hiera_large_224`     | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth)      |       86.1         |            531            |
-| Hiera-H  | `hiera_huge_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth)       |       86.9         |            274            |
+| Hiera-T  | `hiera_tiny_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_tiny_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth)       |       82.8         |            2758           |
+| Hiera-S  | `hiera_small_224`     | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_small_224.pth)       | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth)      |       83.8         |            2211           |
+| Hiera-B  | `hiera_base_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth)       |       84.5         |            1556           |
+| Hiera-B+ | `hiera_base_plus_224` | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_224.pth)   | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth)  |       85.2         |            1247           |
+| Hiera-L  | `hiera_large_224`     | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_224.pth)       | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth)      |       86.1         |            531            |
+| Hiera-H  | `hiera_huge_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth)       |       86.9         |            274            |
 
 Each model inputs a 224x224 image.
 ### Video Models
 | Model    | Model Name               | Pretrained Models<br>(K400 MAE) | Finetuned Models<br>(K400) | K400 (3x5 views)<br>Top-1 (%) | A100 fp16<br>Speed (clip/s) |
 |----------|--------------------------|---------------------------------|----------------------------|:-----------------------------:|:---------------------------:|
-| Hiera-B  | `hiera_base_16x224`      | Coming Soon                     | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth)      |              84.0             |            133.6            |
-| Hiera-B+ | `hiera_base_plus_16x224` | Coming Soon                     | Coming Soon |              85.0             |             84.1            |
-| Hiera-L  | `hiera_large_16x224`     | Coming Soon                     | Coming Soon |              87.3             |             40.8            |
-| Hiera-H  | `hiera_huge_16x224`      | Coming Soon                     | Coming Soon |              87.8             |             20.9            |
+| Hiera-B  | `hiera_base_16x224`      | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_16x224.pth)       | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth)      |              84.0             |            133.6            |
+| Hiera-B+ | `hiera_base_plus_16x224` | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_16x224.pth)  | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_16x224.pth) |              85.0             |             84.1            |
+| Hiera-L  | `hiera_large_16x224`     | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_16x224.pth)      | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_large_16x224.pth)     |              87.3             |             40.8            |
+| Hiera-H  | `hiera_huge_16x224`      | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_16x224.pth)       | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_huge_16x224.pth)      |              87.8             |             20.9            |
 
 Each model inputs 16 224x224 frames with a temporal stride of 4.
 
 
 ## Usage
 
 This repo implements the code to run Hiera models for inference. This repository is still in progress. Here's what we currently have available and what we have planned:
 
  - [x] Image Inference
     - [x] MAE implementation
  - [x] Video Inference
-    - [ ] MAE implementation
+    - [x] MAE implementation
+ - [x] Full Model Zoo
  - [ ] Training scripts
- - [ ] Full Model Zoo
 
 
 See [examples](https://github.com/facebookresearch/hiera/tree/main/examples) for examples of how to use Hiera.
 
 ### Inference
 
 See [examples/inference](https://github.com/facebookresearch/hiera/blob/main/examples/inference.ipynb) for an example of how to prepare the data for inference.
@@ -126,14 +138,28 @@
 Video inference works the same way, just use a `16x224` model instead.
 
 **Note**: for efficiency, Hiera re-orders its tokens at the start of the network (see the `Roll` and `Unroll` modules in `hiera_utils.py`). Thus, tokens _aren't in spatial order_ by default. If you'd like to use intermediate feature maps for a downstream task, pass the `return_intermediates` flag when running the model:
 ```py
 output, intermediates = model(x, return_intermediates=True)
 ```
 
+#### MAE Inference
+By default, the models do not include the MAE decoder. If you would like to use the decoder or compute MAE loss, you can instantiate an mae version by running:
+```py
+import hiera
+model = hiera.mae_hiera_base_224(pretrained=True, checkpoint="mae_in1k")
+```
+Then when you run inference on the model, it will return a 4-tuple of `(loss, predictions, labels, mask)` where predictions and labels are for the _deleted tokens_ only. The returned mask will be `True` if the token is visible and `False` if it's deleted. You can change the masking ratio by passing it during inference:
+```py
+loss, preds, labels, mask = model(x, mask_ratio=0.6)
+```
+The default mask ratio is `0.6` for images, but you should pass in `0.9` for video. See the paper for details.
+
+**Note:** We use _normalized pixel targets_ for MAE pretraining, meaning the patches are each individually normalized before the model model has to predict them. Thus, you have to unnormalize them using the ground truth before visualizing them. See `get_pixel_label_2d` in `hiera_mae.py` for details.
+
 ### Benchmarking
 We provide a script for easy benchmarking. See [examples/benchmark](https://github.com/facebookresearch/hiera/blob/main/examples/benchmark.ipynb) to see how to use it.
 
 #### Scaled Dot Product Attention
 PyTorch 2.0 introduced optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html), which can speed up transformers quite a bit. We didn't use this in our original benchmarking, but since it's a free speed-up this repo will automatically use it if available. To get its benefits, make sure your torch version is 2.0 or above.
 
 ### Training
```

### Comparing `hiera-transformer-0.1.1/hiera/__init__.py` & `hiera-transformer-0.1.2/hiera/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,9 +30,14 @@
     mae_hiera_tiny_224,
     mae_hiera_small_224,
     mae_hiera_base_224,
     mae_hiera_base_plus_224,
     mae_hiera_large_224,
     mae_hiera_huge_224,
 
+    mae_hiera_base_16x224,
+    mae_hiera_base_plus_16x224,
+    mae_hiera_large_16x224,
+    mae_hiera_huge_16x224,
+
     MaskedAutoencoderHiera,
 )
```

### Comparing `hiera-transformer-0.1.1/hiera/benchmarking.py` & `hiera-transformer-0.1.2/hiera/benchmarking.py`

 * *Files identical despite different names*

### Comparing `hiera-transformer-0.1.1/hiera/hiera.py` & `hiera-transformer-0.1.2/hiera/hiera.py`

 * *Files 13% similar despite different names*

```diff
@@ -229,14 +229,15 @@
         head_dropout: float = 0.0,
         head_init_scale: float = 0.001,
         sep_pos_embed: bool = False,
     ):
         super().__init__()
 
         depth = sum(stages)
+        self.patch_stride = patch_stride
         self.tokens_spatial_shape = [i // s for i, s in zip(input_size, patch_stride)]
         num_tokens = math.prod(self.tokens_spatial_shape)
         flat_mu_size = math.prod(mask_unit_size)
         flat_q_stride = math.prod(q_stride)
 
         assert q_pool < len(stages)
         self.q_pool, self.q_stride = q_pool, q_stride
@@ -434,58 +435,65 @@
         return x
 
 
 # Image models
 
 @pretrained_model({
     "mae_in1k_ft_in1k": "https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth",
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_tiny_224.pth",
 }, default="mae_in1k_ft_in1k")
 def hiera_tiny_224(**kwdargs):
     return Hiera(embed_dim=96, num_heads=1, stages=(1, 2, 7, 2), **kwdargs)
 
 
 @pretrained_model({
     "mae_in1k_ft_in1k": "https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth",
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_small_224.pth",
 }, default="mae_in1k_ft_in1k")
 def hiera_small_224(**kwdargs):
     return Hiera(embed_dim=96, num_heads=1, stages=(1, 2, 11, 2), **kwdargs)
 
 
 @pretrained_model({
     "mae_in1k_ft_in1k": "https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth",
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_224.pth",
 }, default="mae_in1k_ft_in1k")
 def hiera_base_224(**kwdargs):
     return Hiera(embed_dim=96, num_heads=1, stages=(2, 3, 16, 3), **kwdargs)
 
 
 @pretrained_model({
     "mae_in1k_ft_in1k": "https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth",
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_224.pth",
 }, default="mae_in1k_ft_in1k")
 def hiera_base_plus_224(**kwdargs):
     return Hiera(embed_dim=112, num_heads=2, stages=(2, 3, 16, 3), **kwdargs)
 
 
 @pretrained_model({
     "mae_in1k_ft_in1k": "https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth",
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_224.pth",
 }, default="mae_in1k_ft_in1k")
 def hiera_large_224(**kwdargs):
     return Hiera(embed_dim=144, num_heads=2, stages=(2, 6, 36, 4), **kwdargs)
 
 
 @pretrained_model({
     "mae_in1k_ft_in1k": "https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth",
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_224.pth",
 }, default="mae_in1k_ft_in1k")
 def hiera_huge_224(**kwdargs):
     return Hiera(embed_dim=256, num_heads=4, stages=(2, 6, 36, 4), **kwdargs)
 
 
 # Video models
 
 @pretrained_model({
     "mae_k400_ft_k400": "https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth",
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_16x224.pth",
 }, default="mae_k400_ft_k400")
 def hiera_base_16x224(num_classes: int = 400, **kwdargs):
     return Hiera(
         num_classes=num_classes,  # K400 has 400 classes
         input_size=(16, 224, 224),
         q_stride=(1, 2, 2),
         mask_unit_size=(1, 8, 8),
@@ -493,26 +501,35 @@
         patch_stride=(2, 4, 4),
         patch_padding=(1, 3, 3),
         sep_pos_embed=True,
         **kwdargs
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_k400_ft_k400": "https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_16x224.pth",
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_16x224.pth",
+}, default="mae_k400_ft_k400")
 def hiera_base_plus_16x224(**kwdargs):
     return hiera_base_16x224(
         embed_dim=112, num_heads=2, stages=(2, 3, 16, 3), **kwdargs
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_k400_ft_k400": "https://dl.fbaipublicfiles.com/hiera/hiera_large_16x224.pth",
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_16x224.pth",
+}, default="mae_k400_ft_k400")
 def hiera_large_16x224(**kwdargs):
     return hiera_base_16x224(
         embed_dim=144, num_heads=2, stages=(2, 6, 36, 4), **kwdargs
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_k400_ft_k400": "https://dl.fbaipublicfiles.com/hiera/hiera_huge_16x224.pth",
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_16x224.pth",
+}, default="mae_k400_ft_k400")
 def hiera_huge_16x224(**kwdargs):
     return hiera_base_16x224(
         embed_dim=256, num_heads=4, stages=(2, 6, 36, 4), **kwdargs
     )
```

### Comparing `hiera-transformer-0.1.1/hiera/hiera_mae.py` & `hiera-transformer-0.1.2/hiera/hiera_mae.py`

 * *Files 18% similar despite different names*

```diff
@@ -157,14 +157,36 @@
         if norm:
             mean = label.mean(dim=-1, keepdim=True)
             var = label.var(dim=-1, keepdim=True)
             label = (label - mean) / (var + 1.0e-6) ** 0.5
 
         return label
 
+    def get_pixel_label_3d(
+        self, input_vid: torch.Tensor, mask: torch.Tensor, norm: bool = True
+    ) -> torch.Tensor:
+        # mask (boolean tensor): True must correspond to *masked*
+
+        # We use time strided loss, only take the first frame from each token
+        input_vid = input_vid[:, :, ::self.patch_stride[0], :, :]
+
+        size = self.pred_stride
+        label = input_vid.unfold(3, size, size).unfold(4, size, size)
+        label = label.permute(0, 2, 3, 4, 5, 6, 1)  # Different from 2d, mistake during training lol
+        label = label.flatten(1, 3).flatten(2)
+        label = label[mask]
+
+        if norm:
+            mean = label.mean(dim=-1, keepdim=True)
+            var = label.var(dim=-1, keepdim=True)
+            label = (label - mean) / (var + 1.0e-6) ** 0.5
+
+        return label
+
+
     def forward_encoder(
         self, x: torch.Tensor, mask_ratio: float, mask: Optional[torch.Tensor] = None
     ) -> Tuple[torch.Tensor, torch.Tensor]:
 
         if mask is None:
             mask = self.get_random_mask(x, mask_ratio)  # [B, #MUs_all]
 
@@ -238,14 +260,16 @@
 
         x: e.g. [B, 3, H, W]
         pred: [B * num_pred_tokens, num_pixels_in_pred_patch * in_chans]
         label: [B * num_pred_tokens, num_pixels_in_pred_patch * in_chans]
         """
         if len(self.q_stride) == 2:
             label = self.get_pixel_label_2d(x, mask)
+        elif len(self.q_stride) == 3:
+            label = self.get_pixel_label_3d(x, mask)
         else:
             raise NotImplementedError
 
         pred = pred[mask]
         loss = (pred - label) ** 2
 
         return loss.mean(), pred, label
@@ -266,47 +290,109 @@
         return *self.forward_loss(x, pred, ~pred_mask), mask
 
 
 
 
 # Image Models
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_tiny_224.pth",
+}, default="mae_in1k")
 def mae_hiera_tiny_224(**kwargs):
     return MaskedAutoencoderHiera(
         embed_dim=96, num_heads=1, stages=(1, 2, 7, 2), q_pool=2, **kwargs,
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_small_224.pth",
+}, default="mae_in1k")
 def mae_hiera_small_224(**kwargs):
     return MaskedAutoencoderHiera(
         embed_dim=96, num_heads=1, stages=(1, 2, 11, 2), q_pool=2, **kwargs,
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_224.pth",
+}, default="mae_in1k")
 def mae_hiera_base_224(**kwargs):
     return MaskedAutoencoderHiera(
         embed_dim=96, num_heads=1, stages=(2, 3, 16, 3), q_pool=2, **kwargs,
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_224.pth",
+}, default="mae_in1k")
 def mae_hiera_base_plus_224(**kwargs):
     return MaskedAutoencoderHiera(
         embed_dim=112, num_heads=2, stages=(2, 3, 16, 3), q_pool=2, **kwargs,
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_224.pth",
+}, default="mae_in1k")
 def mae_hiera_large_224(**kwargs):
     return MaskedAutoencoderHiera(
         embed_dim=144, num_heads=2, stages=(2, 6, 36, 4), q_pool=2, **kwargs,
     )
 
 
-@pretrained_model(None)
+@pretrained_model({
+    "mae_in1k": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_224.pth",
+}, default="mae_in1k")
 def mae_hiera_huge_224(**kwargs):
     return MaskedAutoencoderHiera(
         embed_dim=256, num_heads=4, stages=(2, 6, 36, 4), q_pool=2, **kwargs,
     )
+
+
+
+# Video Models
+
+@pretrained_model({
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_16x224.pth",
+}, default="mae_k400")
+def mae_hiera_base_16x224(num_classes: int = 400, **kwdargs):
+    return MaskedAutoencoderHiera(
+        num_classes=num_classes,  # K400 has 400 classes
+        input_size=(16, 224, 224),
+        q_stride=(1, 2, 2),
+        mask_unit_size=(1, 8, 8),
+        patch_kernel=(3, 7, 7),
+        patch_stride=(2, 4, 4),
+        patch_padding=(1, 3, 3),
+        sep_pos_embed=True,
+        q_pool=2,
+        **kwdargs
+    )
+
+
+@pretrained_model({
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_16x224.pth",
+}, default="mae_k400")
+@pretrained_model(None)
+def mae_hiera_base_plus_16x224(**kwdargs):
+    return mae_hiera_base_16x224(
+        embed_dim=112, num_heads=2, stages=(2, 3, 16, 3), **kwdargs
+    )
+
+
+@pretrained_model({
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_16x224.pth",
+}, default="mae_k400")
+@pretrained_model(None)
+def mae_hiera_large_16x224(**kwdargs):
+    return mae_hiera_base_16x224(
+        embed_dim=144, num_heads=2, stages=(2, 6, 36, 4), **kwdargs
+    )
+
+
+@pretrained_model({
+    "mae_k400": "https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_16x224.pth",
+}, default="mae_k400")
+def mae_hiera_huge_16x224(**kwdargs):
+    return mae_hiera_base_16x224(
+        embed_dim=256, num_heads=4, stages=(2, 6, 36, 4), **kwdargs
+    )
```

### Comparing `hiera-transformer-0.1.1/hiera/hiera_utils.py` & `hiera-transformer-0.1.2/hiera/hiera_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,18 @@
                     # If the user specified a different number of classes, remove the projection weights or else we'll error out
                     elif kwdargs["num_classes"] != state_dict["model_state"]["head.projection.weight"].shape[0]:
                         del state_dict["model_state"]["head.projection.weight"]
                         del state_dict["model_state"]["head.projection.bias"]
 
             model = model_func(**kwdargs)
             if pretrained:
+                # Disable being strict when trying to load a encoder-decoder model into an encoder-only model
+                if "decoder_pos_embed" in state_dict["model_state"] and not hasattr(model, "decoder_pos_embed"):
+                    strict = False
+
                 model.load_state_dict(state_dict["model_state"], strict=strict)
             
             return model
 
         return model_def
     
     return inner
```

### Comparing `hiera-transformer-0.1.1/hiera_transformer.egg-info/PKG-INFO` & `hiera-transformer-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: hiera-transformer
-Version: 0.1.1
-Summary: A fast, powerful, and simple hierarchical vision transformer
-Home-page: https://github.com/facebookresearch/hiera
-Author: Chaitanya Ryali, Daniel Bolya
-License: CC BY-NC 4.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Hiera: A Hierarchical Vision Transformer without the Bells-and-Whistles
 
 This is the official implementation for our ICML 2023 Oral paper:  
 **[Hiera: A Hierarchical Vision Transformer without the Bells-and-Whistles][arxiv-link]**  
 [Chaitanya Ryali](https://scholar.google.com/citations?user=4LWx24UAAAAJ)\*,
 [Yuan-Ting Hu](https://scholar.google.com/citations?user=aMpbemkAAAAJ)\*,
 [Daniel Bolya](https://scholar.google.com/citations?hl=en&user=K3ht_ZUAAAAJ)\*,
@@ -69,57 +59,59 @@
 cd hiera
 python setup.py build develop
 ```
 
 
 ## Model Zoo
 
-Here we provide model checkpoints for Hiera. Each model listed is accessible on [torch hub](https://pytorch.org/docs/stable/hub.html), e.g.:
+Here we provide model checkpoints for Hiera. Each model listed is accessible on [torch hub](https://pytorch.org/docs/stable/hub.html) even without the `hiera-transformer` package installed, e.g. the following initializes a base model pretrained and finetuned on ImageNet-1k:
 ```py
 model = torch.hub.load("facebookresearch/hiera", model="hiera_base_224", pretrained=True, checkpoint="mae_in1k_ft_in1k")
 ```
-For model names and corresponding checkpoint names see below.
 
-**Note:** the speeds listed here were benchmarked _without_ PyTorch's optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html). If using PyTorch 2.0 or above, your inference speed will probably be faster than what's listed here.
+If you want a model with MAE pretraining only, you can replace the checkpoint with `"mae_in1k"`. Additionally, if you'd like to load the MAE decoder as well (e.g., to continue pretraining), add `mae_` the the start of the model name, e.g.:
+```py
+model = torch.hub.load("facebookresearch/hiera", model="mae_hiera_base_224", pretrained=True, checkpoint="mae_in1k")
+```
+**Note:** Our MAE models were trained with a _normalized pixel loss_. That means that the patches were normalized before the network had to predict them. If you want to visualize the predictions, you'll have to unnormalize them using the visible patches (which might work but wouldn't be perfect) or unnormalize them using the ground truth. For model more names and corresponding checkpoint names see below.
 
-#### Coming Soon
-As of now, base finetuned models are available. The rest are coming soon.
 
+**Note:** the speeds listed here were benchmarked _without_ PyTorch's optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html). If using PyTorch 2.0 or above, your inference speed will probably be faster than what's listed here.
 ### Image Models
 | Model    | Model Name            | Pretrained Models<br>(IN-1K MAE) | Finetuned Models<br>(IN-1K Supervised) | IN-1K<br>Top-1 (%) | A100 fp16<br>Speed (im/s) |
 |----------|-----------------------|----------------------------------|----------------------------------------|:------------------:|:-------------------------:|
-| Hiera-T  | `hiera_tiny_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth)       |       82.8         |            2758           |
-| Hiera-S  | `hiera_small_224`     | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth)      |       83.8         |            2211           |
-| Hiera-B  | `hiera_base_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth)       |       84.5         |            1556           |
-| Hiera-B+ | `hiera_base_plus_224` | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth)  |       85.2         |            1247           |
-| Hiera-L  | `hiera_large_224`     | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth)      |       86.1         |            531            |
-| Hiera-H  | `hiera_huge_224`      | Coming Soon         | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth)       |       86.9         |            274            |
+| Hiera-T  | `hiera_tiny_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_tiny_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_tiny_224.pth)       |       82.8         |            2758           |
+| Hiera-S  | `hiera_small_224`     | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_small_224.pth)       | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_small_224.pth)      |       83.8         |            2211           |
+| Hiera-B  | `hiera_base_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_224.pth)       |       84.5         |            1556           |
+| Hiera-B+ | `hiera_base_plus_224` | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_224.pth)   | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_224.pth)  |       85.2         |            1247           |
+| Hiera-L  | `hiera_large_224`     | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_224.pth)       | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_large_224.pth)      |       86.1         |            531            |
+| Hiera-H  | `hiera_huge_224`      | [mae_in1k](https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_224.pth)        | [mae_in1k_ft_in1k](https://dl.fbaipublicfiles.com/hiera/hiera_huge_224.pth)       |       86.9         |            274            |
 
 Each model inputs a 224x224 image.
 ### Video Models
 | Model    | Model Name               | Pretrained Models<br>(K400 MAE) | Finetuned Models<br>(K400) | K400 (3x5 views)<br>Top-1 (%) | A100 fp16<br>Speed (clip/s) |
 |----------|--------------------------|---------------------------------|----------------------------|:-----------------------------:|:---------------------------:|
-| Hiera-B  | `hiera_base_16x224`      | Coming Soon                     | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth)      |              84.0             |            133.6            |
-| Hiera-B+ | `hiera_base_plus_16x224` | Coming Soon                     | Coming Soon |              85.0             |             84.1            |
-| Hiera-L  | `hiera_large_16x224`     | Coming Soon                     | Coming Soon |              87.3             |             40.8            |
-| Hiera-H  | `hiera_huge_16x224`      | Coming Soon                     | Coming Soon |              87.8             |             20.9            |
+| Hiera-B  | `hiera_base_16x224`      | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_16x224.pth)       | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_16x224.pth)      |              84.0             |            133.6            |
+| Hiera-B+ | `hiera_base_plus_16x224` | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_base_plus_16x224.pth)  | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_base_plus_16x224.pth) |              85.0             |             84.1            |
+| Hiera-L  | `hiera_large_16x224`     | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_large_16x224.pth)      | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_large_16x224.pth)     |              87.3             |             40.8            |
+| Hiera-H  | `hiera_huge_16x224`      | [mae_k400](https://dl.fbaipublicfiles.com/hiera/mae_hiera_huge_16x224.pth)       | [mae_k400_ft_k400](https://dl.fbaipublicfiles.com/hiera/hiera_huge_16x224.pth)      |              87.8             |             20.9            |
 
 Each model inputs 16 224x224 frames with a temporal stride of 4.
 
 
 ## Usage
 
 This repo implements the code to run Hiera models for inference. This repository is still in progress. Here's what we currently have available and what we have planned:
 
  - [x] Image Inference
     - [x] MAE implementation
  - [x] Video Inference
-    - [ ] MAE implementation
+    - [x] MAE implementation
+ - [x] Full Model Zoo
  - [ ] Training scripts
- - [ ] Full Model Zoo
 
 
 See [examples](https://github.com/facebookresearch/hiera/tree/main/examples) for examples of how to use Hiera.
 
 ### Inference
 
 See [examples/inference](https://github.com/facebookresearch/hiera/blob/main/examples/inference.ipynb) for an example of how to prepare the data for inference.
@@ -136,14 +128,28 @@
 Video inference works the same way, just use a `16x224` model instead.
 
 **Note**: for efficiency, Hiera re-orders its tokens at the start of the network (see the `Roll` and `Unroll` modules in `hiera_utils.py`). Thus, tokens _aren't in spatial order_ by default. If you'd like to use intermediate feature maps for a downstream task, pass the `return_intermediates` flag when running the model:
 ```py
 output, intermediates = model(x, return_intermediates=True)
 ```
 
+#### MAE Inference
+By default, the models do not include the MAE decoder. If you would like to use the decoder or compute MAE loss, you can instantiate an mae version by running:
+```py
+import hiera
+model = hiera.mae_hiera_base_224(pretrained=True, checkpoint="mae_in1k")
+```
+Then when you run inference on the model, it will return a 4-tuple of `(loss, predictions, labels, mask)` where predictions and labels are for the _deleted tokens_ only. The returned mask will be `True` if the token is visible and `False` if it's deleted. You can change the masking ratio by passing it during inference:
+```py
+loss, preds, labels, mask = model(x, mask_ratio=0.6)
+```
+The default mask ratio is `0.6` for images, but you should pass in `0.9` for video. See the paper for details.
+
+**Note:** We use _normalized pixel targets_ for MAE pretraining, meaning the patches are each individually normalized before the model model has to predict them. Thus, you have to unnormalize them using the ground truth before visualizing them. See `get_pixel_label_2d` in `hiera_mae.py` for details.
+
 ### Benchmarking
 We provide a script for easy benchmarking. See [examples/benchmark](https://github.com/facebookresearch/hiera/blob/main/examples/benchmark.ipynb) to see how to use it.
 
 #### Scaled Dot Product Attention
 PyTorch 2.0 introduced optimized [scaled dot product attention](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html), which can speed up transformers quite a bit. We didn't use this in our original benchmarking, but since it's a free speed-up this repo will automatically use it if available. To get its benefits, make sure your torch version is 2.0 or above.
 
 ### Training
```

### Comparing `hiera-transformer-0.1.1/setup.py` & `hiera-transformer-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # LICENSE file in the root directory of this source tree.
 # --------------------------------------------------------
 
 from setuptools import find_packages, setup
 
 setup(
     name="hiera-transformer",
-    version="0.1.1",
+    version="0.1.2",
     author="Chaitanya Ryali, Daniel Bolya",
     url="https://github.com/facebookresearch/hiera",
     description="A fast, powerful, and simple hierarchical vision transformer",
     install_requires=["torch>=1.8.1", "timm>=0.4.12", "tqdm"],
     packages=find_packages(exclude=("examples", "build")),
     license = 'CC BY-NC 4.0',
     long_description=open("README.md", "r", encoding="utf-8").read(),
```

