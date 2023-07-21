# Comparing `tmp/hcpdiff-0.4.2.tar.gz` & `tmp/hcpdiff-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcpdiff-0.4.2.tar", last modified: Mon May 22 06:07:04 2023, max compression
+gzip compressed data, was "hcpdiff-0.5.4.tar", last modified: Thu Jul 20 09:52:58 2023, max compression
```

## Comparing `hcpdiff-0.4.2.tar` & `hcpdiff-0.5.4.tar`

### file list

```diff
@@ -1,110 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.665458 hcpdiff-0.4.2/cfgs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/deepspeed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/infer/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/change_vae.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/euler_a.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/img2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/img2img_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/offload_2GB.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/text2img.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/infer/text2img_DA++.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/plugins/plugin_controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/te_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/train/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/cfgs/train/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/CustomDiffusion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/DreamArtist++.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/DreamArtist.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/DreamBooth.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/Lion_optimizer.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/TextualInversion.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/controlnet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/fine-tuning.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/locon.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/lora_conventional.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/examples/min_snr.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/train_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/train/tuning_base.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/cfgs/unet_struct.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.669458 hcpdiff-0.4.2/hcpdiff/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/ckpt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/ckpt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_pkl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_safetensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/data/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/cond_pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7132 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/pair_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/base_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/cli_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/loss/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loss/min_snr_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/loss/mse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/models/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/cfg_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/controlnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/lora_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/text_emb_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/textencoder_ex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/models/tokenizer_ex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff/noise/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/noise/noise_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/noise/pyramid_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/hcpdiff/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/convert_caption_txt2json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/create_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/gen_from_ptlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/init_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/lora_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/tools/sd2diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28412 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_ac_single.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_colo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/train_deepspeed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/hcpdiff/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/caption_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/cfg_net_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/colo_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/ema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/img_size_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/hcpdiff/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.673458 hcpdiff-0.4.2/hcpdiff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 06:07:04.000000 hcpdiff-0.4.2/hcpdiff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/prompt_tuning_template/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/name.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/name_2pt_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/name_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/object.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/object_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/style.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/prompt_tuning_template/style_caption.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:07:04.677458 hcpdiff-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-22 06:06:40.000000 hcpdiff-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5944 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.504845 hcpdiff-0.5.4/cfgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/deepspeed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/cfgs/infer/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/change_vae.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/euler_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/img2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/img2img_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/inpaint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/load_unet_part.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/offload_2GB.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/save_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/text2img.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/text2img_DA++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/infer/text2img_anime.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/cfgs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/plugins/plugin_controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/te_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/cfgs/train/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/cfgs/train/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/dataset/base_dataset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/dataset/regularization_dataset.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/cfgs/train/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/CustomDiffusion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/DreamArtist++.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/DreamArtist.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/DreamBooth.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/Lion_optimizer.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/TextualInversion.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/add_logger_tensorboard_wandb.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/controlnet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/fine-tuning.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/locon.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/lora_anime.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/lora_conventional.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/examples/min_snr.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/train_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/train/tuning_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    45190 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/cfgs/unet_struct.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/hcpdiff/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/hcpdiff/ckpt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/ckpt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/ckpt_manager/ckpt_pkl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/ckpt_manager/ckpt_safetensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.512846 hcpdiff-0.5.4/hcpdiff/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/caption_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/cond_pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/pair_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.512846 hcpdiff-0.5.4/hcpdiff/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loggers/base_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loggers/cli_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loggers/wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loggers/webui_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.512846 hcpdiff-0.5.4/hcpdiff/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loss/min_snr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/loss/mse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.512846 hcpdiff-0.5.4/hcpdiff/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/cfg_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/lora_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/multi_textencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/text_emb_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/textencoder_ex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/models/tokenizer_ex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.512846 hcpdiff-0.5.4/hcpdiff/noise/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/noise/noise_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/noise/pyramid_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/hcpdiff/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/convert_caption_txt2json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/create_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/gen_from_ptlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/init_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/lora_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16420 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/tools/sd2diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29117 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/train_ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/train_ac_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/train_colo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/train_deepspeed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/hcpdiff/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/caption_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/cfg_net_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/colo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/ema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/img_size_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26880 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/pipe_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/hcpdiff/vis/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/vis/base_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/vis/disk_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/vis/webui_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10029 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/hcpdiff/visualizer_reloadable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.508846 hcpdiff-0.5.4/hcpdiff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-20 09:52:58.000000 hcpdiff-0.5.4/hcpdiff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-20 09:52:58.000000 hcpdiff-0.5.4/hcpdiff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:52:58.000000 hcpdiff-0.5.4/hcpdiff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 09:52:58.000000 hcpdiff-0.5.4/hcpdiff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-20 09:52:58.000000 hcpdiff-0.5.4/hcpdiff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 09:52:58.000000 hcpdiff-0.5.4/hcpdiff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/prompt_tuning_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/name.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/name_2pt_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/name_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/object.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/object_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/prompt_tuning_template/style_caption.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:52:58.516846 hcpdiff-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 09:52:45.000000 hcpdiff-0.5.4/setup.py
```

### Comparing `hcpdiff-0.4.2/LICENSE` & `hcpdiff-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/PKG-INFO` & `hcpdiff-0.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.4.2
+Version: 0.5.4
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -24,18 +24,18 @@
 [![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
 [![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
 
 [📘中文说明](./README_cn.md)
 
 ## Introduction
-HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
-It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
+HCP-Diffusion is a toolbox for Stable Diffusion models based on [🤗 Diffusers](https://github.com/huggingface/diffusers).
+It facilitates flexiable configurations and component support for training, in comparison with [webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) and [sd-scripts](https://github.com/kohya-ss/sd-scripts).
 
-This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
+This toolbox supports [**Colossal-AI**](https://github.com/hpcaitech/ColossalAI), which can significantly reduce GPU memory usage.
 
 HCP-Diffusion can unify existing training methods for text-to-image generation (e.g., Prompt-tuning, Textual Inversion, DreamArtist, Fine-tuning, DreamBooth, LoRA, ControlNet, etc) and model structures through a single ```.yaml``` configuration file.
 
 The toolbox has also implemented an upgraded version of DreamArtist with LoRA, named DreamArtist++, for one-shot text-to-image generation.
 Compared to DreamArtist, DreamArtist++ is more stable with higher image quality and generation controllability, and faster training speed.
 
 ## Features
@@ -47,20 +47,21 @@
 * DreamArtist and DreamArtist++
 * Aspect Ratio Bucket (ARB) with automatic clustering
 * Multiple datasets with multiple data sources
 * Image attention mask
 * Word attention multiplier
 * Custom words that occupy multiple words
 * Maximum sentence length expansion
-* colossal-AI
-* xformers for unet and text-encoder
+* [🤗 Accelerate](https://github.com/huggingface/accelerate)
+* [Colossal-AI](https://github.com/hpcaitech/ColossalAI)
+* [xFormers](https://github.com/facebookresearch/xformers) for UNet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
-* safetensors support
-* Controlnet (support train)
+* [Safetensors](https://github.com/huggingface/safetensors) support
+* [Controlnet](https://github.com/lllyasviel/ControlNet) (support training)
 * Min-SNR loss
 * Custom optimizer (Lion, DAdaptation, pytorch-optimizer, ...)
 * Custom lr scheduler
 
 ## Install
 
 Install with pip:
@@ -75,76 +76,86 @@
 git clone https://github.com/7eu7d7/HCP-Diffusion.git
 cd HCP-Diffusion
 pip install -e .
 # Modified based on this project or start a new project and make initialization
 ## hcpinit
 ```
 
+To use xFormers to reduce VRAM usage and accelerate training:
+```bash
+# use conda
+conda install xformers -c xformers
+
+# use pip
+pip install xformers>=0.0.17
+```
+
 ## User guidance
 
-Training:
+### Training
+
+Training scripts based on 🤗 Accelerate or Colossal-AI are provided.
++ For 🤗 Accelerate, you may need to [configure the environment](https://github.com/huggingface/accelerate/tree/main#launching-script) before launching the scripts.
++ For Colossal-AI, you can use [torchrun](https://pytorch.org/docs/stable/elastic/run.html) to launch the scripts.
+
 ```yaml
-# with accelerate
+# with Accelerate
 accelerate launch -m hcpdiff.train_ac --cfg cfgs/train/cfg_file.yaml
-# with accelerate and only one gpu
+# with Accelerate and only one GPU
 accelerate launch -m hcpdiff.train_ac_single --cfg cfgs/train/cfg_file.yaml
-# with colossal-AI
+# with Colossal-AI
 torchrun --nproc_per_node 1 -m hcpdiff.train_colo --cfg cfgs/train/cfg_file.yaml
 ```
 
-Inference:
+### Inference
 ```yaml
 python -m hcpdiff.visualizer --cfg cfgs/infer/cfg.yaml pretrained_model=pretrained_model_path \
         prompt='positive_prompt' \
         neg_prompt='negative_prompt' \
         seed=42
 ```
 
-The framework is based on diffusers. So it needs to convert the original stable diffusion model into a supported format using the [scripts provided by diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
+### Conversion of Stable Diffusion models
+The framework is based on 🤗 Diffusers. So it needs to convert the original Stable Diffusion model into a supported format using the [scripts provided by 🤗 Diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
 + Download the [config file](https://huggingface.co/runwayml/stable-diffusion-v1-5/blob/main/v1-inference.yaml)
 + Convert models based on config file
 
 ```bash
 python -m hcpdiff.tools.sd2diffusers \
     --checkpoint_path "path_to_stable_diffusion_model" \
     --original_config_file "path_to_config_file" \
     --dump_path "save_directory" \
-    [--extract_ema] # Extract ema model
+    [--extract_ema] # Extract EMA model
     [--from_safetensors] # Whether the original model is in safetensors format
     [--to_safetensors] # Whether to save to safetensors format
 ```
 
 Convert VAE:
 ```bash
 python -m hcpdiff.tools.sd2diffusers \
     --vae_pt_path "path_to_VAE_model" \
     --original_config_file "path_to_config_file" \
     --dump_path "save_directory"
     [--from_safetensors]
 ```
 
+### Tutorials
 + [Model Training Tutorial](doc/guide_train.md)
 + [DreamArtist++ Tutorial](doc/guide_DA.md)
 + [Model Inference Tutorial](doc/guide_infer.md)
 + [Configuration File Explanation](doc/guide_cfg.md)
 + [webui Model Conversion Tutorial](doc/guide_webui_lora.md)
 
-Use xformer to reduce VRAM usage and accelerate training:
-```bash
-# use conda
-conda install xformers -c xformers
+## Contributing
 
-# use pip
-pip install xfromers>=0.0.17
-```
+You are welcome to contribute more models and features to this toolbox!
 
 ## Team
 
 This toolbox is maintained by [HCP-Lab, SYSU](https://www.sysu-hcp.net/).
-More models and features are welcome to contribute to this toolbox.
 
 ## Citation
 
 ```
 @article{DBLP:journals/corr/abs-2211-11337,
   author    = {Ziyi Dong and
                Pengxu Wei and
```

### Comparing `hcpdiff-0.4.2/README.md` & `hcpdiff-0.5.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 [![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
 [![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
 
 [📘中文说明](./README_cn.md)
 
 ## Introduction
-HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
-It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
+HCP-Diffusion is a toolbox for Stable Diffusion models based on [🤗 Diffusers](https://github.com/huggingface/diffusers).
+It facilitates flexiable configurations and component support for training, in comparison with [webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) and [sd-scripts](https://github.com/kohya-ss/sd-scripts).
 
-This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
+This toolbox supports [**Colossal-AI**](https://github.com/hpcaitech/ColossalAI), which can significantly reduce GPU memory usage.
 
 HCP-Diffusion can unify existing training methods for text-to-image generation (e.g., Prompt-tuning, Textual Inversion, DreamArtist, Fine-tuning, DreamBooth, LoRA, ControlNet, etc) and model structures through a single ```.yaml``` configuration file.
 
 The toolbox has also implemented an upgraded version of DreamArtist with LoRA, named DreamArtist++, for one-shot text-to-image generation.
 Compared to DreamArtist, DreamArtist++ is more stable with higher image quality and generation controllability, and faster training speed.
 
 ## Features
@@ -28,20 +28,21 @@
 * DreamArtist and DreamArtist++
 * Aspect Ratio Bucket (ARB) with automatic clustering
 * Multiple datasets with multiple data sources
 * Image attention mask
 * Word attention multiplier
 * Custom words that occupy multiple words
 * Maximum sentence length expansion
-* colossal-AI
-* xformers for unet and text-encoder
+* [🤗 Accelerate](https://github.com/huggingface/accelerate)
+* [Colossal-AI](https://github.com/hpcaitech/ColossalAI)
+* [xFormers](https://github.com/facebookresearch/xformers) for UNet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
-* safetensors support
-* Controlnet (support train)
+* [Safetensors](https://github.com/huggingface/safetensors) support
+* [Controlnet](https://github.com/lllyasviel/ControlNet) (support training)
 * Min-SNR loss
 * Custom optimizer (Lion, DAdaptation, pytorch-optimizer, ...)
 * Custom lr scheduler
 
 ## Install
 
 Install with pip:
@@ -56,76 +57,86 @@
 git clone https://github.com/7eu7d7/HCP-Diffusion.git
 cd HCP-Diffusion
 pip install -e .
 # Modified based on this project or start a new project and make initialization
 ## hcpinit
 ```
 
+To use xFormers to reduce VRAM usage and accelerate training:
+```bash
+# use conda
+conda install xformers -c xformers
+
+# use pip
+pip install xformers>=0.0.17
+```
+
 ## User guidance
 
-Training:
+### Training
+
+Training scripts based on 🤗 Accelerate or Colossal-AI are provided.
++ For 🤗 Accelerate, you may need to [configure the environment](https://github.com/huggingface/accelerate/tree/main#launching-script) before launching the scripts.
++ For Colossal-AI, you can use [torchrun](https://pytorch.org/docs/stable/elastic/run.html) to launch the scripts.
+
 ```yaml
-# with accelerate
+# with Accelerate
 accelerate launch -m hcpdiff.train_ac --cfg cfgs/train/cfg_file.yaml
-# with accelerate and only one gpu
+# with Accelerate and only one GPU
 accelerate launch -m hcpdiff.train_ac_single --cfg cfgs/train/cfg_file.yaml
-# with colossal-AI
+# with Colossal-AI
 torchrun --nproc_per_node 1 -m hcpdiff.train_colo --cfg cfgs/train/cfg_file.yaml
 ```
 
-Inference:
+### Inference
 ```yaml
 python -m hcpdiff.visualizer --cfg cfgs/infer/cfg.yaml pretrained_model=pretrained_model_path \
         prompt='positive_prompt' \
         neg_prompt='negative_prompt' \
         seed=42
 ```
 
-The framework is based on diffusers. So it needs to convert the original stable diffusion model into a supported format using the [scripts provided by diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
+### Conversion of Stable Diffusion models
+The framework is based on 🤗 Diffusers. So it needs to convert the original Stable Diffusion model into a supported format using the [scripts provided by 🤗 Diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
 + Download the [config file](https://huggingface.co/runwayml/stable-diffusion-v1-5/blob/main/v1-inference.yaml)
 + Convert models based on config file
 
 ```bash
 python -m hcpdiff.tools.sd2diffusers \
     --checkpoint_path "path_to_stable_diffusion_model" \
     --original_config_file "path_to_config_file" \
     --dump_path "save_directory" \
-    [--extract_ema] # Extract ema model
+    [--extract_ema] # Extract EMA model
     [--from_safetensors] # Whether the original model is in safetensors format
     [--to_safetensors] # Whether to save to safetensors format
 ```
 
 Convert VAE:
 ```bash
 python -m hcpdiff.tools.sd2diffusers \
     --vae_pt_path "path_to_VAE_model" \
     --original_config_file "path_to_config_file" \
     --dump_path "save_directory"
     [--from_safetensors]
 ```
 
+### Tutorials
 + [Model Training Tutorial](doc/guide_train.md)
 + [DreamArtist++ Tutorial](doc/guide_DA.md)
 + [Model Inference Tutorial](doc/guide_infer.md)
 + [Configuration File Explanation](doc/guide_cfg.md)
 + [webui Model Conversion Tutorial](doc/guide_webui_lora.md)
 
-Use xformer to reduce VRAM usage and accelerate training:
-```bash
-# use conda
-conda install xformers -c xformers
+## Contributing
 
-# use pip
-pip install xfromers>=0.0.17
-```
+You are welcome to contribute more models and features to this toolbox!
 
 ## Team
 
 This toolbox is maintained by [HCP-Lab, SYSU](https://www.sysu-hcp.net/).
-More models and features are welcome to contribute to this toolbox.
 
 ## Citation
 
 ```
 @article{DBLP:journals/corr/abs-2211-11337,
   author    = {Ziyi Dong and
                Pengxu Wei and
@@ -135,8 +146,8 @@
   journal   = {CoRR},
   volume    = {abs/2211.11337},
   year      = {2022},
   doi       = {10.48550/arXiv.2211.11337},
   eprinttype = {arXiv},
   eprint    = {2211.11337},
 }
-```
+```
```

### Comparing `hcpdiff-0.4.2/cfgs/deepspeed.json` & `hcpdiff-0.5.4/cfgs/deepspeed.json`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/cfgs/infer/text2img.yaml` & `hcpdiff-0.5.4/cfgs/infer/text2img.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 # base_state*base_model_alpha + (lora_state[i]*lora_scale[i]*lora_alpha[i]) + (part_state[k]*part_alpha[k])
 
 pretrained_model: ''
 prompt: ''
 neg_prompt: 'lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry'
-out_dir: 'output/'
 emb_dir: 'embs/'
+out_dir: 'output/'
 N_repeats: 1
 clip_skip: 0
 bs: 4
 num: 1
 seed: null
 dtype: 'fp16'
 
 condition: null
 
+ex_input: {}
+
 save:
   save_cfg: True
   image_type: png
   quality: 95
 #  image_type: webp
 #  quality: 75
 
 offload: null
 #offload:
 #  max_VRAM: 8GiB
 #  max_RAM: 30GiB
 #  vae_cpu: False
 
+#vae_optimize: null
+vae_optimize:
+  tiling: True
+  slicing: False
+
+interface:
+  - _target_: hcpdiff.vis.DiskInterface
+    show_steps: 0
+    save_root: 'output/'
+
 infer_args:
   width: 512
   height: 512
   guidance_scale: 7.5
   num_inference_steps: 50
 
 new_components: {}
```

### Comparing `hcpdiff-0.4.2/cfgs/infer/text2img_DA++.yaml` & `hcpdiff-0.5.4/cfgs/infer/text2img_DA++.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/cfgs/te_struct.txt` & `hcpdiff-0.5.4/cfgs/te_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/cfgs/train/examples/CustomDiffusion.yaml` & `hcpdiff-0.5.4/cfgs/train/examples/controlnet.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,13 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
-
-unet:
-  -
-    lr: 1e-6
-    layers:
-      - 're:.*\.to_k$'
-      - 're:.*\.to_v$'
-
-## lora version of CustomDiffusion
-#lora_unet:
-#  -
-#    lr: 1e-4
-#    layers:
-#      - 're:.*\.to_k$'
-#      - 're:.*\.to_v$'
+_base_:
+  - cfgs/train/train_base.yaml
+  - cfgs/plugins/plugin_controlnet.yaml # include controlnet plugin
 
 tokenizer_pt:
-  train: # prompt tuning embeddings, needs to be created in advance
-    - { name: 'pt-dog1', lr: 0.003 }
+  train: null
 
 train:
   gradient_accumulation_steps: 1
   save_step: 100
 
   scheduler:
     name: 'constant_with_warmup'
@@ -32,58 +18,41 @@
   pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
   tokenizer_repeats: 1
   ema_unet: 0
   ema_text_encoder: 0
 
 data:
   dataset1:
+    _target_: hcpdiff.data.TextImageCondPairDataset
+    _partial_: True # Not directly instantiate the object here. There are other parameters to be added in the runtime.
     batch_size: 4
     cache_latents: True
+    att_mask_encode: False
     loss_weight: 1.0
 
     source:
       data_source1:
         img_root: 'imgs/'
+        cond_root: 'cond_imgs/'
         prompt_template: 'prompt_tuning_template/object.txt'
         caption_file: null # path to image captions (file_words)
-        tag_transforms:
-          transforms:
-            - _target_: hcpdiff.utils.caption_tools.TagShuffle
-            - _target_: hcpdiff.utils.caption_tools.TagDropout
-              p: 0.1
-            - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names:
-                pt1: sks
-                class: dog
-    bucket:
-      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-      num_bucket: 1
-
-  dataset_class:
-    _target_: hcpdiff.data.TextImagePairDataset
-    _partial_: True
-    batch_size: 1
-    cache_latents: True
-    att_mask_encode: False
-    loss_weight: 1.0
-
-    source:
-      data_source1:
-        img_root: 'imgs/db_class'
-        prompt_template: 'prompt_tuning_template/object.txt'
-        caption_file: null
         att_mask: null
-        bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
-        image_transforms: ${....dataset1.source.data_source1.image_transforms}
+        bg_color: [ 255, 255, 255 ] # RGB; for ARGB -> RGB
+
+        image_transforms:
+          _target_: torchvision.transforms.Compose # "_target_" for hydra.utils.instantiate
+          transforms:
+            - _target_: torchvision.transforms.ToTensor
+            - _target_: torchvision.transforms.Normalize
+              _args_: [ [ 0.5 ], [ 0.5 ] ]
         tag_transforms:
           _target_: torchvision.transforms.Compose
           transforms:
             - _target_: hcpdiff.utils.caption_tools.TagShuffle
             - _target_: hcpdiff.utils.caption_tools.TagDropout
               p: 0.1
             - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names:
-                class: dog
+              word_names: { }
     bucket:
-      _target_: hcpdiff.data.bucket.FixedBucket
-      target_size: [512, 512]
+      _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
+      target_area: ${times:512,512}
+      num_bucket: 5
```

### Comparing `hcpdiff-0.4.2/cfgs/train/examples/DreamArtist++.yaml` & `hcpdiff-0.5.4/cfgs/train/examples/DreamArtist++.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+_base_:
+  - cfgs/train/dataset/regularization_dataset.yaml
+  - cfgs/train/train_base.yaml
+  - cfgs/train/tuning_base.yaml
 
 unet: null
 
 lora_unet:
   - lr: 1e-4
     rank: 0.01875
     branch: p
@@ -80,59 +83,53 @@
 model:
   pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
   tokenizer_repeats: 1
   ema_unet: 0
   ema_text_encoder: 0
   clip_skip: 0
 
+# The dataset configuration inherits regularization_dataset.yaml
+# 数据集配置继承自 regularization_dataset.yaml， 只需修改部分参数
 data:
   dataset1:
     batch_size: 4
     cache_latents: True
-    loss_weight: 1.0
 
     source:
       data_source1:
         img_root: 'imgs/'
         prompt_template: 'prompt_tuning_template/object.txt'
         caption_file: null # path to image captions (file_words)
+        att_mask: null
+
+        word_names: --- # remove unused item
         tag_transforms:
-          transforms:
+          transforms: # without TagShuffle and TagDropout. | 去掉 TagShuffle 和 TagDropout.
             - _target_: hcpdiff.utils.caption_tools.TemplateFill
               word_names:
                 pt1: [pt-botdog1, pt-botdog1-neg]
     bucket:
       _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      target_area: ${times:512,512}
       num_bucket: 1
 
-
   # Add regularization to prevent image crashes
   # Regularization images is generated by model itself with prompt from dataset
   dataset_class:
-    _target_: hcpdiff.data.TextImagePairDataset
-    _partial_: True
     batch_size: 1
     cache_latents: True
-    att_mask_encode: False
     loss_weight: 1.0
 
     source:
       data_source1:
         img_root: 'imgs/v15'
         prompt_template: 'prompt_tuning_template/caption.txt'
-        caption_file: 'imgs/v15/image_captions.json'
+        caption_file:
+          _targe_: hcpdiff.data.JsonCaptionLoader
+          path: 'imgs/v15/image_captions.json'
         att_mask: null
-        bg_color: [255, 255, 255] # RGB; for ARGB -> RGB
-        image_transforms: ${....dataset1.source.data_source1.image_transforms}
-        tag_transforms:
-          _target_: torchvision.transforms.Compose
-          transforms:
-            - _target_: hcpdiff.utils.caption_tools.TagShuffle
-            - _target_: hcpdiff.utils.caption_tools.TagDropout
-              p: 0.1
-            - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names:
-                pt1: ['', '']
+
+        word_names:
+          pt1: ['', '']
     bucket:
       _target_: hcpdiff.data.bucket.FixedBucket
       target_size: [512, 512]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hcpdiff-0.4.2/cfgs/train/examples/DreamArtist.yaml` & `hcpdiff-0.5.4/cfgs/train/examples/DreamArtist.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+_base_:
+  - cfgs/train/dataset/base_dataset.yaml
+  - cfgs/train/train_base.yaml
+  - cfgs/train/tuning_base.yaml
 
 tokenizer_pt:
   train: # prompt tuning embeddings, needs to be created in advance
     - { name: 'pt-catgirl1', lr: 0.003 }
     - { name: 'pt-catgirl1-neg', lr: 0.003 }
 
 train:
@@ -29,19 +32,14 @@
     cache_latents: True
 
     source:
       data_source1:
         img_root: 'imgs/'
         prompt_template: 'prompt_tuning_template/object.txt'
         caption_file: null # path to image captions (file_words)
-        tag_transforms:
-          transforms:
-            - _target_: hcpdiff.utils.caption_tools.TagShuffle
-            - _target_: hcpdiff.utils.caption_tools.TagDropout
-              p: 0.1
-            - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names:
-                pt1: [pt-catgirl1, pt-catgirl1-neg] # A pair of word for positive and negative branches respectively.
+
+        word_names:
+          pt1: [ pt-catgirl1, pt-catgirl1-neg ] # A pair of word for positive and negative branches respectively.
     bucket:
       _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-      num_bucket: 5
+      target_area: ${times:512,512}
+      num_bucket: 1
```

### Comparing `hcpdiff-0.4.2/cfgs/train/examples/TextualInversion.yaml` & `hcpdiff-0.5.4/cfgs/train/examples/TextualInversion.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
+_base_:
+  - cfgs/train/dataset/base_dataset.yaml
+  - cfgs/train/train_base.yaml
+  - cfgs/train/tuning_base.yaml
 
 tokenizer_pt:
   train: # prompt tuning embeddings, needs to be created in advance
     - { name: 'pt-catgirl1', lr: 0.003 }
 
 train:
   gradient_accumulation_steps: 1
@@ -25,19 +28,14 @@
     cache_latents: True
 
     source:
       data_source1:
         img_root: 'imgs/'
         prompt_template: 'prompt_tuning_template/object.txt'
         caption_file: null # path to image captions (file_words)
-        tag_transforms:
-          transforms:
-            - _target_: hcpdiff.utils.caption_tools.TagShuffle
-            - _target_: hcpdiff.utils.caption_tools.TagDropout
-              p: 0.1
-            - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names:
-                pt1: pt-catgirl1
+
+        word_names:
+          pt1: pt-catgirl1
     bucket:
       _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-      num_bucket: 5
+      target_area: ${times:512,512}
+      num_bucket: 1
```

### Comparing `hcpdiff-0.4.2/cfgs/train/examples/controlnet.yaml` & `hcpdiff-0.5.4/cfgs/train/examples/CustomDiffusion.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,30 @@
 _base_:
+  - cfgs/train/dataset/regularization_dataset.yaml
   - cfgs/train/train_base.yaml
-  - cfgs/plugins/plugin_controlnet.yaml # include controlnet plugin
+  - cfgs/train/tuning_base.yaml
+
+unet:
+  -
+    lr: 1e-6
+    layers: # k,v of cross attention
+      - 're:.*attn2\.to_k$'
+      - 're:.*attn2\.to_v$'
+
+## lora version of CustomDiffusion
+#lora_unet:
+#  -
+#    lr: 1e-4
+#    layers:
+#      - 're:.*attn2\.to_k$'
+#      - 're:.*attn2\.to_v$'
 
 tokenizer_pt:
-  train: null
+  train: # prompt tuning embeddings, needs to be created in advance
+    - { name: 'pt-dog1', lr: 0.003 }
 
 train:
   gradient_accumulation_steps: 1
   save_step: 100
 
   scheduler:
     name: 'constant_with_warmup'
@@ -26,18 +43,32 @@
     cache_latents: True
 
     source:
       data_source1:
         img_root: 'imgs/'
         prompt_template: 'prompt_tuning_template/object.txt'
         caption_file: null # path to image captions (file_words)
-        tag_transforms:
-          transforms:
-            - _target_: hcpdiff.utils.caption_tools.TagShuffle
-            - _target_: hcpdiff.utils.caption_tools.TagDropout
-              p: 0.1
-            - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names: { }
+
+        word_names:
+          pt1: sks
+          class: dog
     bucket:
       _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
-      num_bucket: 5
+      target_area: ${times:512,512}
+      num_bucket: 1
+
+  dataset_class:
+    batch_size: 1
+    cache_latents: True
+    loss_weight: 1.0
+
+    source:
+      data_source1:
+        img_root: 'imgs/db_class'
+        prompt_template: 'prompt_tuning_template/object.txt'
+        caption_file: null
+
+        word_names:
+          class: dog
+    bucket:
+      _target_: hcpdiff.data.bucket.FixedBucket
+      target_size: [512, 512]
```

### Comparing `hcpdiff-0.4.2/cfgs/train/examples/locon.yaml` & `hcpdiff-0.5.4/cfgs/train/examples/fine-tuning.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,23 @@
-_base_: [cfgs/train/train_base.yaml, cfgs/train/tuning_base.yaml]
-
-lora_unet:
-  - # Linear
-    lr: 1e-4
-    rank: 8
-    layers:
-      - 're:.*\.attn.?$'
-      - 're:.*\.ff$'
-  - # Conv2d
-    lr: 1e-4
-    rank: 8
-    layers:
-      - 're:.*\.resnets$'
-      - 're:.*\.proj_in$'
-      - 're:.*\.proj_out$'
-      - 're:.*\.conv$'
-
-lora_text_encoder:
-  - lr: 1e-5
-    rank: 4
+_base_:
+  - cfgs/train/dataset/base_dataset.yaml
+  - cfgs/train/train_base.yaml
+  - cfgs/train/tuning_base.yaml
+
+unet:
+  -
+    lr: 1e-6
     layers:
-      - 're:.*self_attn$'
-      - 're:.*mlp$'
+      - '' # fine-tuning all layers in unet
+
+## fine-tuning text-encoder
+#text_encoder:
+#  - lr: 1e-6
+#    layers:
+#      - ''
 
 tokenizer_pt:
   train: null
 
 train:
   gradient_accumulation_steps: 1
   save_step: 100
@@ -37,28 +29,25 @@
 
 model:
   pretrained_model_name_or_path: 'runwayml/stable-diffusion-v1-5'
   tokenizer_repeats: 1
   ema_unet: 0
   ema_text_encoder: 0
 
+# The dataset configuration inherits base_dataset.yaml
+# 数据集配置继承自base_dataset.yaml， 只需修改部分参数
 data:
   dataset1:
     batch_size: 4
     cache_latents: True
 
     source:
       data_source1:
         img_root: 'imgs/'
         prompt_template: 'prompt_tuning_template/object.txt'
         caption_file: null # path to image captions (file_words)
-        tag_transforms:
-          transforms:
-            - _target_: hcpdiff.utils.caption_tools.TagShuffle
-            - _target_: hcpdiff.utils.caption_tools.TagDropout
-              p: 0.1
-            - _target_: hcpdiff.utils.caption_tools.TemplateFill
-              word_names: { }
+        att_mask: null
+
     bucket:
       _target_: hcpdiff.data.bucket.RatioBucket.from_files # aspect ratio bucket
-      target_area: {_target_: "builtins.eval", _args_: ['512*512']}
+      target_area: ${times:512,512}
       num_bucket: 5
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hcpdiff-0.4.2/cfgs/train/tuning_base.yaml` & `hcpdiff-0.5.4/cfgs/train/tuning_base.yaml`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/cfgs/unet_struct.txt` & `hcpdiff-0.5.4/cfgs/unet_struct.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_pkl.py` & `hcpdiff-0.5.4/hcpdiff/ckpt_manager/ckpt_pkl.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         self.save_dir = save_dir
         self.emb_dir = emb_dir
 
     def exclude_state(self, state, key):
         if key is None:
             return state
         else:
-            return {k: v for k, v in state.items() if key in k}
+            return {k: v for k, v in state.items() if key not in k}
 
     def save_model(self, model: nn.Module, name, step, model_ema=None, exclude_key=None):
         sd_model = {
             'base': self.exclude_state(LoraBlock.extract_trainable_state_without_lora(model), exclude_key),
         }
         if model_ema is not None:
             sd_ema, sd_ema_lora = split_state(model_ema.state_dict())
```

### Comparing `hcpdiff-0.4.2/hcpdiff/ckpt_manager/ckpt_safetensor.py` & `hcpdiff-0.5.4/hcpdiff/ckpt_manager/ckpt_safetensor.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/data/__init__.py` & `hcpdiff-0.5.4/hcpdiff/data/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .pair_dataset import TextImagePairDataset
 from .cond_pair_dataset import TextImageCondPairDataset
 from .bucket import BaseBucket, FixedBucket, RatioBucket
 from .utils import CycleData
-
+from .caption_loader import JsonCaptionLoader, TXTCaptionLoader
 
 class DataGroup:
     def __init__(self, loader_list, loss_weights):
         self.loader_list = loader_list
         self.loss_weights = loss_weights
 
     def __iter__(self):
```

### Comparing `hcpdiff-0.4.2/hcpdiff/data/bucket.py` & `hcpdiff-0.5.4/hcpdiff/data/bucket.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import cv2
 import numpy as np
 from loguru import logger
 from sklearn.cluster import KMeans
 
 from hcpdiff.utils.img_size_tool import types_support, get_image_size
 from hcpdiff.utils.utils import get_file_ext
-from .utils import resize_crop_fix
+from .utils import resize_crop_fix, pad_crop_fix
 
 class BaseBucket:
     def __getitem__(self, idx):
         '''
         :return: (file name of image), (target image size)
         '''
         raise NotImplementedError()
@@ -38,47 +38,50 @@
     def rest(self, epoch):
         pass
 
     def crop_resize(self, image, size, mask_interp=cv2.INTER_CUBIC):
         return image
 
 class FixedBucket(BaseBucket):
-    def __init__(self, target_size: Union[Tuple[int, int], int] = 512):
+    def __init__(self, target_size: Union[Tuple[int, int], int] = 512, **kwargs):
         self.target_size = (target_size, target_size) if isinstance(target_size, int) else target_size
 
     def build(self, bs: int, img_root_list: List[str]):
         self.img_root_list = img_root_list
-        self.file_names = [os.path.join(img_root, x) for img_root in img_root_list for x in os.listdir(img_root) if get_file_ext(x) in types_support]
+        self.file_names = []
+        for img_root, repeat in img_root_list:
+            imgs = [os.path.join(img_root, x) for x in os.listdir(img_root) if get_file_ext(x) in types_support]
+            self.file_names.extend(imgs*repeat)
 
     def crop_resize(self, image, size, mask_interp=cv2.INTER_CUBIC):
         return resize_crop_fix(image, size, mask_interp=mask_interp)
 
     def __getitem__(self, idx) -> Tuple[str, Tuple[int, int]]:
         return self.file_names[idx], self.target_size
 
     def __len__(self):
         return len(self.file_names)
 
 class RatioBucket(BaseBucket):
-    def __init__(self, taget_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, pre_build_arb: str = None):
+    def __init__(self, taget_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, pre_build_bucket: str = None):
         self.taget_area = taget_area
         self.step_size = step_size
         self.num_bucket = num_bucket
-        self.pre_build_arb = pre_build_arb
+        self.pre_build_bucket = pre_build_bucket
 
-    def load_arb(self, path):
+    def load_bucket(self, path):
         with open(path, 'rb') as f:
             data = pickle.load(f)
         self.buckets = data['buckets']
         self.size_buckets = data['size_buckets']
         self.file_names = data['file_names']
         self.idx_bucket_map = data['idx_bucket_map']
         self.data_len = data['data_len']
 
-    def save_arb(self, path):
+    def save_bucket(self, path):
         with open(path, 'wb') as f:
             pickle.dump({
                 'buckets':self.buckets,
                 'size_buckets':self.size_buckets,
                 'idx_bucket_map':self.idx_bucket_map,
                 'file_names':self.file_names,
                 'data_len':self.data_len,
@@ -99,15 +102,15 @@
                 data.append([w*h, np.log2(w/h), w, h])  # 对比例取对数，更符合人感知，宽高相反的可以对称分布。
         data = np.array(data)
 
         error_area = np.abs(data[:, 0]-self.taget_area)
         data_use = data[np.argsort(error_area)[:self.num_bucket*3], :]  # 取最小的num_bucket*3个
 
         # 聚类，选出指定个数的bucket
-        kmeans = KMeans(n_clusters=self.num_bucket, random_state=0).fit(data_use[:, 1].reshape(-1, 1))
+        kmeans = KMeans(n_clusters=self.num_bucket, random_state=3407).fit(data_use[:, 1].reshape(-1, 1))
         labels = kmeans.labels_
         self.buckets = []  # [bucket_id:[file_idx,...]]
         self.ratios_log = []
         self.size_buckets = []
         for i in range(self.num_bucket):
             map_idx = np.where(labels == i)[0]
             m_idx = map_idx[np.argmin(np.abs(data_use[labels == i, 1]-np.median(data_use[labels == i, 1])))]
@@ -133,15 +136,15 @@
         for i, file in enumerate(self.file_names):
             w, h = get_image_size(file)
             ratio = np.log2(w/h)
             ratio_list.append(ratio)
         ratio_list = np.array(ratio_list)
 
         # 聚类，选出指定个数的bucket
-        kmeans = KMeans(n_clusters=self.num_bucket, random_state=0).fit(ratio_list.reshape(-1, 1))
+        kmeans = KMeans(n_clusters=self.num_bucket, random_state=3407).fit(ratio_list.reshape(-1, 1))
         labels = kmeans.labels_
         self.ratios_log = kmeans.cluster_centers_.reshape(-1)
 
         ratios = 2**self.ratios_log
         h_all = np.sqrt(self.taget_area/ratios)
         w_all = h_all*ratios
 
@@ -158,69 +161,111 @@
             self.buckets.append(np.where(bnow)[0].tolist())
             self.idx_bucket_map[bnow] = bidx
         logger.info('buckets info: '+', '.join(f'size:{self.size_buckets[i]}, num:{len(b)}' for i, b in enumerate(self.buckets)))
 
     def build(self, bs: int, img_root_list: List[str]):
         '''
         :param bs: batch_size * n_gpus * accumulation_step
-        :param pre_build_arb:
+        :param img_root_list:
         '''
         self.img_root_list = img_root_list
-        if self.pre_build_arb and os.path.exists(self.pre_build_arb):
-            self.load_arb(self.pre_build_arb)
+        if self.pre_build_bucket and os.path.exists(self.pre_build_bucket):
+            self.load_bucket(self.pre_build_bucket)
             return
         else:
-            self.file_names = [os.path.join(img_root, x) for img_root in img_root_list for x in os.listdir(img_root)
-                if get_file_ext(x) in types_support]
+            self.file_names = []
+            for img_root, repeat in img_root_list:
+                imgs = [os.path.join(img_root, x) for x in os.listdir(img_root) if get_file_ext(x) in types_support]
+                self.file_names.extend(imgs*repeat)
         self._build()
 
         self.bs = bs
         rs = np.random.RandomState(42)
         # make len(bucket)%bs==0
         self.data_len = 0
         for bidx, bucket in enumerate(self.buckets):
             rest = len(bucket)%bs
             if rest>0:
                 bucket.extend(rs.choice(bucket, bs-rest))
             self.data_len += len(bucket)
             self.buckets[bidx] = np.array(bucket)
 
-        if self.pre_build_arb:
-            self.save_arb(self.pre_build_arb)
+        if self.pre_build_bucket:
+            self.save_bucket(self.pre_build_bucket)
 
     def rest(self, epoch):
         rs = np.random.RandomState(42+epoch)
         bucket_list = [x.copy() for x in self.buckets]
         # shuffle inter bucket
         for x in bucket_list:
             rs.shuffle(x)
 
         # shuffle of batches
         bucket_list = np.hstack(bucket_list).reshape(-1, self.bs).astype(int)
         rs.shuffle(bucket_list)
 
-        self.idx_arb = bucket_list.reshape(-1)
+        self.idx_bucket = bucket_list.reshape(-1)
 
     def crop_resize(self, image, size, mask_interp=cv2.INTER_CUBIC):
         return resize_crop_fix(image, size, mask_interp=mask_interp)
 
     def __getitem__(self, idx):
-        fidx = self.idx_arb[idx]
-        bidx = self.idx_bucket_map[fidx]
-        return self.file_names[fidx], self.size_buckets[bidx]
+        file_idx = self.idx_bucket[idx]
+        bucket_idx = self.idx_bucket_map[file_idx]
+        return self.file_names[file_idx], self.size_buckets[bucket_idx]
 
     def __len__(self):
         return self.data_len
 
     @classmethod
     def from_ratios(cls, target_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, ratio_max: float = 4,
-                    pre_build_arb: str = None):
-        arb = cls(target_area, step_size, num_bucket, pre_build_arb=pre_build_arb)
+                    pre_build_bucket: str = None, **kwargs):
+        arb = cls(target_area, step_size, num_bucket, pre_build_bucket=pre_build_bucket)
         arb.ratio_max = ratio_max
         arb._build = arb.build_buckets_from_ratios
         return arb
 
     @classmethod
-    def from_files(cls, target_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, pre_build_arb: str = None):
-        arb = RatioBucket(target_area, step_size, num_bucket, pre_build_arb=pre_build_arb)
+    def from_files(cls, target_area: int = 640*640, step_size: int = 8, num_bucket: int = 10, pre_build_bucket: str = None, **kwargs):
+        arb = cls(target_area, step_size, num_bucket, pre_build_bucket=pre_build_bucket)
         arb._build = arb.build_buckets_from_images
         return arb
+
+class SizeBucket(RatioBucket):
+    def __init__(self, step_size: int = 8, num_bucket: int = 10, pre_build_bucket: str = None):
+        super().__init__(step_size=step_size, num_bucket=num_bucket, pre_build_bucket=pre_build_bucket)
+
+    def build_buckets_from_images(self):
+        '''
+        根据图像尺寸聚类，不会resize图像，只有剪裁和填充操作。
+        '''
+        logger.info('build buckets from images size')
+        size_list = []
+        for i, file in enumerate(self.file_names):
+            w, h = get_image_size(file)
+            size_list.append([w, h])
+        size_list = np.array(size_list)
+
+        # 聚类，选出指定个数的bucket
+        kmeans = KMeans(n_clusters=self.num_bucket, random_state=3407).fit(size_list)
+        labels = kmeans.labels_
+        size_buckets = kmeans.cluster_centers_
+
+        # SD需要边长是8的倍数
+        self.size_buckets = (np.round(size_buckets/self.step_size)*self.step_size).astype(int)
+
+        self.buckets = []  # [bucket_id:[file_idx,...]]
+        self.idx_bucket_map = np.empty(len(self.file_names), dtype=int)
+        for bidx in range(self.num_bucket):
+            bnow = labels == bidx
+            self.buckets.append(np.where(bnow)[0].tolist())
+            self.idx_bucket_map[bnow] = bidx
+        logger.info('buckets info: '+', '.join(f'size:{self.size_buckets[i]}, num:{len(b)}' for i, b in enumerate(self.buckets)))
+
+    def crop_resize(self, image, size):
+        return pad_crop_fix(image, size)
+
+    @classmethod
+    def from_files(cls, step_size: int = 8, num_bucket: int = 10, pre_build_bucket: str = None, **kwargs):
+        arb = cls(step_size, num_bucket, pre_build_bucket=pre_build_bucket)
+        arb._build = arb.build_buckets_from_images
+        return arb
```

### Comparing `hcpdiff-0.4.2/hcpdiff/data/cond_pair_dataset.py` & `hcpdiff-0.5.4/hcpdiff/data/cond_pair_dataset.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/data/pair_dataset.py` & `hcpdiff-0.5.4/hcpdiff/data/pair_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,28 @@
     :Name:        text-image pair dataset
     :Author:      Dong Ziyi
     :Affiliation: HCP Lab, SYSU
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
 
-import json
 import os.path
 from argparse import Namespace
 
 import cv2
 import torch
-import yaml
 from PIL import Image
 from torch.utils.data import Dataset
 from tqdm.auto import tqdm
 
 from hcpdiff.utils.caption_tools import *
 from hcpdiff.utils.img_size_tool import types_support
 from hcpdiff.utils.utils import get_file_name, get_file_ext
 from .bucket import BaseBucket
-
+from .caption_loader import BaseCaptionLoader, auto_caption_loader
 
 class TextImagePairDataset(Dataset):
     """
     A dataset to prepare the instance and class images with the prompts for fine-tuning the model.
     It pre-processes the images and the tokenizes prompts.
     """
 
@@ -50,38 +48,35 @@
             source_metas.att_mask_path = {} if data_source.att_mask is None else \
                 {get_file_name(file):os.path.join(data_source.att_mask, file)
                     for file in os.listdir(data_source.att_mask) if get_file_ext(file) in types_support}
             source_metas.prompt_template = self.load_template(data_source.prompt_template)
             source_metas.image_transforms = data_source.image_transforms
             source_metas.tag_transforms = data_source.tag_transforms
             source_metas.bg_color = tuple(data_source.bg_color)
+            source_metas.repeat = getattr(data_source, 'repeat', 1)
 
             self.source_dict[os.path.dirname(data_source.img_root+'/')] = source_metas
 
     def load_image(self, path):
         image = Image.open(path)
         if image.mode == 'RGBA':
             img_root = os.path.dirname(path)
             x, y = image.size
             canvas = Image.new('RGBA', image.size, self.source_dict[img_root].bg_color)
             canvas.paste(image, (0, 0, x, y), image)
             image = canvas
         return image.convert("RGB")
 
-    def load_captions(self, caption_file):
+    def load_captions(self, caption_file: Union[str, BaseCaptionLoader]):
         if caption_file is None:
-            return dict()
-        elif caption_file.endswith('.json'):
-            with open(caption_file, 'r', encoding='utf-8') as f:
-                return json.loads(f.read())
-        elif caption_file.endswith('.yaml'):
-            with open(caption_file, 'r', encoding='utf-8') as f:
-                return yaml.load(f.read(), Loader=yaml.FullLoader)
+            return {}
+        elif isinstance(caption_file, str):
+            return auto_caption_loader(caption_file).load()
         else:
-            return dict()
+            return caption_file.load()
 
     def load_template(self, template_file):
         with open(template_file, 'r', encoding='utf-8') as f:
             return f.read().strip().split('\n')
 
     @torch.no_grad()
     def cache_latents(self, vae, weight_dtype, device, show_prog=True):
@@ -90,61 +85,61 @@
 
         for path, size in tqdm(self.bucket, disable=not show_prog):
             img_name = os.path.basename(path)
             if img_name not in self.latents:
                 data = self.load_data(path, size)
                 image = data['img'].unsqueeze(0).to(device, dtype=weight_dtype)
                 latents = vae.encode(image).latent_dist.sample().squeeze(0)
-                data['img'] = (latents * 0.18215).cpu()
+                data['img'] = (latents*0.18215).cpu()
                 self.latents[img_name] = data
 
     def get_att_map(self, img_root, img_name):
         if img_name not in self.source_dict[img_root].att_mask_path:
             return None
         att_mask = Image.open(self.source_dict[img_root].att_mask_path[img_name]).convert("L")
         np_mask = np.array(att_mask).astype(float)
-        np_mask[np_mask <= 127 + 0.1] = (np_mask[np_mask <= 127 + 0.1] / 127.)
-        np_mask[np_mask > 127] = ((np_mask[np_mask > 127] - 127) / 128.) * 4 + 1
+        np_mask[np_mask<=127+0.1] = (np_mask[np_mask<=127+0.1]/127.)
+        np_mask[np_mask>127] = ((np_mask[np_mask>127]-127)/128.)*4+1
         return np_mask
 
     def load_data(self, path, size):
         img_root, img_name = os.path.split(path)
         image = self.load_image(path)
         att_mask = self.get_att_map(img_root, get_file_name(img_name))
         if att_mask is None:
-            data = self.bucket.crop_resize({"img": image}, size)
+            data = self.bucket.crop_resize({"img":image}, size)
             image = self.source_dict[img_root].image_transforms(data['img'])  # resize to bucket size
-            att_mask = torch.ones((size[1] // 8, size[0] // 8))
+            att_mask = torch.ones((size[1]//8, size[0]//8))
         else:
-            data = self.bucket.crop_resize({"img": image, "mask": att_mask}, size)
+            data = self.bucket.crop_resize({"img":image, "mask":att_mask}, size)
             image = self.source_dict[img_root].image_transforms(data['img'])
-            att_mask = torch.tensor(cv2.resize(att_mask, (size[0] // 8, size[1] // 8), interpolation=cv2.INTER_LINEAR))
-        return {'img': image, 'mask': att_mask}
+            att_mask = torch.tensor(cv2.resize(att_mask, (size[0]//8, size[1]//8), interpolation=cv2.INTER_LINEAR))
+        return {'img':image, 'mask':att_mask}
 
     def __len__(self):
         return len(self.bucket)
 
     def __getitem__(self, index):
         path, size = self.bucket[index]
         img_root, img_name = os.path.split(path)
 
         if self.latents is None:
             data = self.load_data(path, size)
         else:
             data = self.latents[img_name]
 
         caption_ist = self.source_dict[img_root].caption_dict[img_name] if img_name in \
-                            self.source_dict[img_root].caption_dict else None
+                                                                           self.source_dict[img_root].caption_dict else None
         prompt_ist = self.source_dict[img_root].tag_transforms(
-            {'prompt': random.choice(self.source_dict[img_root].prompt_template), 'caption': caption_ist})['prompt']
+            {'prompt':random.choice(self.source_dict[img_root].prompt_template), 'caption':caption_ist})['prompt']
 
         # tokenize Sp or (Sn, Sp)
         prompt_ids = self.tokenizer(
             prompt_ist, truncation=True, padding="max_length", return_tensors="pt",
-            max_length=self.tokenizer.model_max_length * self.tokenizer_repeats).input_ids.squeeze()
+            max_length=self.tokenizer.model_max_length*self.tokenizer_repeats).input_ids.squeeze()
 
         data['prompt'] = prompt_ids
 
         if self.return_path:
             return data, path
         else:
             return data
@@ -175,8 +170,8 @@
 
         datas['img'] = torch.stack(datas['img'])
         datas['mask'] = torch.stack(datas['mask']).unsqueeze(1)
         if 'cond' in data0:
             datas['cond'] = torch.stack(datas['cond'])
         datas['prompt'] = torch.stack(sn_list)
 
-        return datas
+        return datas
```

### Comparing `hcpdiff-0.4.2/hcpdiff/data/utils.py` & `hcpdiff-0.5.4/hcpdiff/data/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-from PIL import Image
-import torch
 import cv2
 import numpy as np
-
+from PIL import Image
 from torchvision import transforms as T
 from torchvision.transforms import functional as F
 
-
 class DualRandomCrop(object):
     def __init__(self, size):
         self.size = size
 
     def __call__(self, img):
         crop_params = T.RandomCrop.get_params(img['img'], self.size)
         img['img'] = F.crop(img['img'], *crop_params)
@@ -18,44 +15,64 @@
             img['mask'] = self.crop(img['mask'], *crop_params)
         if "cond" in img:
             img['cond'] = F.crop(img['cond'], *crop_params)
         return img
 
     @staticmethod
     def crop(img: np.ndarray, top: int, left: int, height: int, width: int) -> np.ndarray:
-        right = left + width
-        bottom = top + height
-        return img[..., top:bottom, left:right]
+        right = left+width
+        bottom = top+height
+        return img[top:bottom, left:right, ...]
 
 def resize_crop_fix(img, target_size, mask_interp=cv2.INTER_CUBIC):
-    w,h=img['img'].size
-    if w==target_size[0] and h==target_size[1]:
+    w, h = img['img'].size
+    if w == target_size[0] and h == target_size[1]:
         return img
 
-    ratio_img=w/h
-    if ratio_img > target_size[0]/target_size[1]:
-        new_size = (int(ratio_img*target_size[1]), target_size[1])
+    ratio_img = w/h
+    if ratio_img>target_size[0]/target_size[1]:
+        new_size = (round(ratio_img*target_size[1]), target_size[1])
         interp_type = Image.ANTIALIAS if h>target_size[1] else Image.BICUBIC
     else:
-        new_size = (target_size[0], int(target_size[0]/ratio_img))
+        new_size = (target_size[0], round(target_size[0]/ratio_img))
         interp_type = Image.ANTIALIAS if w>target_size[0] else Image.BICUBIC
     img['img'] = img['img'].resize(new_size, interp_type)
     if "mask" in img:
         img['mask'] = cv2.resize(img['mask'], new_size, interpolation=mask_interp)
     if "cond" in img:
         img['cond'] = img['cond'].resize(new_size, interp_type)
 
     return DualRandomCrop(target_size[::-1])(img)
 
+def pad_crop_fix(img, target_size):
+    w, h = img['img'].size
+    if w == target_size[0] and h == target_size[1]:
+        return img
+
+    pad_size = [0, 0, max(target_size[0]-w, 0), max(target_size[1]-h, 0)]
+    if pad_size[2]>0 or pad_size[3]>0:
+        img['img'] = F.pad(img['img'], pad_size)
+        if "mask" in img:
+            img['mask'] = np.pad(img['mask'], ((0, pad_size[3]), (0, pad_size[2])), 'constant', constant_values=(0, 0))
+        if "cond" in img:
+            img['cond'] = F.pad(img['cond'], pad_size)
+
+    if pad_size[2]>0 and pad_size[3]>0:
+        return img  # No need to crop
+    else:
+        return DualRandomCrop(target_size[::-1])(img)
+
 class CycleData():
     def __init__(self, data_loader):
         self.data_loader = data_loader
 
     def __iter__(self):
         self.epoch = 0
+
         def cycle():
             while True:
                 self.data_loader.dataset.bucket.rest(self.epoch)
                 for data in self.data_loader:
                     yield data
-                self.epoch+=1
-        return cycle()
+                self.epoch += 1
+
+        return cycle()
```

### Comparing `hcpdiff-0.4.2/hcpdiff/loggers/base_logger.py` & `hcpdiff-0.5.4/hcpdiff/loggers/base_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/loggers/cli_logger.py` & `hcpdiff-0.5.4/hcpdiff/loggers/cli_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/loggers/tensorboard_logger.py` & `hcpdiff-0.5.4/hcpdiff/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/loggers/wandb_logger.py` & `hcpdiff-0.5.4/hcpdiff/loggers/wandb_logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from typing import Dict, Any
 
+import os
 import wandb
 from PIL import Image
 
 from .base_logger import BaseLogger
 
 
 class WanDBLogger(BaseLogger):
-    def __init__(self, exp_dir, out_path, enable_log_image=True, project='hcp-diffusion'):
-        super().__init__(exp_dir, out_path, enable_log_image)
+    def __init__(self, exp_dir, out_path=None, enable_log_image=True, project='hcp-diffusion', log_step=10):
+        super().__init__(exp_dir, out_path, enable_log_image, log_step)
         if exp_dir is not None:  # exp_dir is only available in local main process
-            wandb.init(project=project)
+            wandb.init(project=project, name=os.path.basename(exp_dir))
+            wandb.save(os.path.join(exp_dir, 'cfg.yaml'), base_path=exp_dir)
         else:
             self.writer = None
             self.disable()
 
     def _info(self, info):
         pass
 
     def _log(self, datas: Dict[str, Any], step: int = 0):
-        wandb.log({k: v['data'] for k, v in datas.items()}, step=step)
+        for k, v in datas.items():
+            if len(v['data']) == 1:
+                wandb.log({k: v['data'][0]}, step=step)
 
     def _log_image(self, imgs: Dict[str, Image.Image], step: int = 0):
         wandb.log({next(iter(imgs.keys())): list(imgs.values())}, step=step)
```

### Comparing `hcpdiff-0.4.2/hcpdiff/loss/min_snr_loss.py` & `hcpdiff-0.5.4/hcpdiff/loss/min_snr_loss.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/cfg_context.py` & `hcpdiff-0.5.4/hcpdiff/models/cfg_context.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/controlnet.py` & `hcpdiff-0.5.4/hcpdiff/models/controlnet.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/layers.py` & `hcpdiff-0.5.4/hcpdiff/models/layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/lora_base.py` & `hcpdiff-0.5.4/hcpdiff/models/lora_base.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/lora_layers.py` & `hcpdiff-0.5.4/hcpdiff/models/lora_layers.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/plugin.py` & `hcpdiff-0.5.4/hcpdiff/models/plugin.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/text_emb_ex.py` & `hcpdiff-0.5.4/hcpdiff/models/text_emb_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/textencoder_ex.py` & `hcpdiff-0.5.4/hcpdiff/models/textencoder_ex.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/models/tokenizer_ex.py` & `hcpdiff-0.5.4/hcpdiff/models/tokenizer_ex.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,16 @@
             else:
                 out_str = c + out_str
                 clean_str = c + clean_str
             i -= 1
         return mult_list, out_str, clean_str
 
     def parse_attn_mult_one(self, text: str):
+        if text is None or len(text)==0:
+            return torch.tensor([]), ""
         mult_list, out_str, clean_str = self.get_mult_list(text)
         mult_iter = iter(mult_list)
         token_seq = self.tokenizer.tokenize(out_str)
         mult = 1.0
         mult_seq = []
         for token in token_seq:
             if token[0] == '{' or token[0] == '}':
```

### Comparing `hcpdiff-0.4.2/hcpdiff/noise/noise_base.py` & `hcpdiff-0.5.4/hcpdiff/noise/noise_base.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/noise/pyramid_noise.py` & `hcpdiff-0.5.4/hcpdiff/noise/pyramid_noise.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from .noise_base import NoiseBase
+import random
+
 import torch
 from torch.nn import functional as F
-import random
 
+from .noise_base import NoiseBase
 
 class PyramidNoiseScheduler(NoiseBase):
     def __init__(self, base_scheduler, level: int = 10, discount: float = 0.9, step: float = 2., mode: str = 'bilinear'):
         super().__init__(base_scheduler)
         self.level = level
         self.step = step
         self.mode = mode
         self.discount = discount
 
     def add_noise(
-            self,
-            original_samples: torch.FloatTensor,
-            noise: torch.FloatTensor,
-            timesteps: torch.IntTensor,
+        self,
+        original_samples: torch.FloatTensor,
+        noise: torch.FloatTensor,
+        timesteps: torch.IntTensor,
     ) -> torch.FloatTensor:
         with torch.no_grad():
             b, c, h, w = noise.shape
             for i in range(1, self.level):
-                r = random.random() * 2 + self.step
-                wn, hn = max(1, int(w / (r ** i))), max(1, int(h / (r ** i)))
-                noise += F.interpolate(torch.randn(b, c, hn, wn).to(noise), (h, w), None, self.mode) * (self.discount ** i)
+                r = random.random()*2+self.step
+                wn, hn = max(1, int(w/(r**i))), max(1, int(h/(r**i)))
+                noise += F.interpolate(torch.randn(b, c, hn, wn).to(noise), (h, w), None, self.mode)*(self.discount**i)
                 if wn == 1 or hn == 1:
                     break
-            noise = noise / noise.std()
+            noise = noise/noise.std()
         return self.base_scheduler.add_noise(original_samples, noise, timesteps)
 
 # if __name__ == '__main__':
 #     noise = torch.randn(1,3,512,512)
 #     level=10
 #     discount=0.6
 #     b, c, h, w = noise.shape
```

### Comparing `hcpdiff-0.4.2/hcpdiff/tools/convert_caption_txt2json.py` & `hcpdiff-0.5.4/hcpdiff/tools/convert_caption_txt2json.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/tools/create_embedding.py` & `hcpdiff-0.5.4/hcpdiff/tools/create_embedding.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,41 +6,50 @@
 import os.path
 
 import torch
 from hcpdiff.utils.utils import str2bool
 from hcpdiff.utils.net_utils import import_text_encoder_class, save_emb
 from transformers import AutoTokenizer
 
+class PTCreator:
+    def __init__(self, pretrained_model_name_or_path, root='embs/'):
+        self.root=root
+
+        self.tokenizer = AutoTokenizer.from_pretrained(
+            pretrained_model_name_or_path,
+            subfolder="tokenizer",
+            revision=None,
+            use_fast=False,
+        )
+
+        text_encoder_cls = import_text_encoder_class(pretrained_model_name_or_path, None)
+        self.text_encoder = text_encoder_cls.from_pretrained(pretrained_model_name_or_path, subfolder="text_encoder", revision=None)
+
+        self.embed_dim = self.text_encoder.text_model.embeddings.token_embedding.embedding_dim
+
+    def creat_word_pt(self, name, n_word, init_text, replace=False):
+        if init_text.startswith('*'):
+            init_embs = torch.randn((n_word, self.embed_dim))
+            if len(init_text)>1:
+                init_embs *= float(init_text[1:])
+        else:
+            emb_pt = self.text_encoder.text_model.embeddings.token_embedding
+            prompt_ids = self.tokenizer(
+                init_text, truncation=True, padding="max_length", return_tensors="pt",
+                max_length=self.tokenizer.model_max_length).input_ids[0, 1:n_word+1]
+            init_embs = emb_pt(prompt_ids)
+        print(init_embs.shape)
+        save_emb(os.path.join(self.root, name+'.pt'), init_embs, replace)
+        print(f'embedding {name} is create.')
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='')
     parser.add_argument('pretrained_model_name_or_path', type=str)
     parser.add_argument('name', type=str)
     parser.add_argument('n_word', type=int, default=3)
     parser.add_argument('--init_text', type=str, default='*0.017', help='randn: *sigma (*0.5)')
     parser.add_argument('--root', type=str, default='embs/')
     parser.add_argument('--replace', type=str2bool, default=False)
     args = parser.parse_args()
 
-    tokenizer = AutoTokenizer.from_pretrained(
-        args.pretrained_model_name_or_path,
-        subfolder="tokenizer",
-        revision=None,
-        use_fast=False,
-    )
-
-    text_encoder_cls = import_text_encoder_class(args.pretrained_model_name_or_path, None)
-    text_encoder = text_encoder_cls.from_pretrained(args.pretrained_model_name_or_path, subfolder="text_encoder", revision=None)
-
-    embed_dim = text_encoder.text_model.embeddings.token_embedding.embedding_dim
-    if args.init_text.startswith('*'):
-        init_embs = torch.randn((args.n_word, embed_dim))
-        if len(args.init_text) > 1:
-            init_embs *= float(args.init_text[1:])
-    else:
-        emb_pt = text_encoder.text_model.embeddings.token_embedding
-        prompt_ids = tokenizer(
-            args.init_text, truncation=True, padding="max_length", return_tensors="pt",
-            max_length=tokenizer.model_max_length).input_ids[0, 1:args.n_word + 1]
-        init_embs = emb_pt(prompt_ids)
-    print(init_embs.shape)
-    save_emb(os.path.join(args.root, args.name + '.pt'), init_embs, args.replace)
-    print(f'embedding {args.name} is create.')
+    pt_creator = PTCreator(args.pretrained_model_name_or_path, args.root)
+    pt_creator.creat_word_pt(args.name, args.n_word, args.init_text, args.replace)
```

### Comparing `hcpdiff-0.4.2/hcpdiff/tools/gen_from_ptlist.py` & `hcpdiff-0.5.4/hcpdiff/tools/gen_from_ptlist.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,68 @@
+import argparse
+import json
 import os.path
+from typing import Callable
 
+import pyarrow.parquet as pq
 import torch
-from diffusers import StableDiffusionPipeline
 from PIL import Image
-import pyarrow.parquet as pq
-import argparse
-import json
+from diffusers import StableDiffusionPipeline
 from tqdm.auto import tqdm
 
-parser = argparse.ArgumentParser(description='Stable Diffusion Training')
-parser.add_argument('--prompt_file', type=str, default='')
-parser.add_argument('--model', type=str, default='runwayml/stable-diffusion-v1-5')
-parser.add_argument('--out_dir', type=str, default=r'./prompt_ds')
-parser.add_argument('--negative_prompt', type=str, default='lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry')
-parser.add_argument('--num', type=int, default=200)
-parser.add_argument('--bs', type=int, default=4)
-args = parser.parse_args()
-
-torch.backends.cudnn.benchmark = True
-
-os.makedirs(args.out_dir, exist_ok=True)
-
-def split_batch(data, bs):
-    return [data[i:i + bs] for i in range(0, len(data), bs)]
-
-
-data = pq.read_table(args.prompt_file).to_batches(args.bs)
-pipeline = StableDiffusionPipeline.from_pretrained(args.model, torch_dtype=torch.float16)
-pipeline.requires_safety_checker = False
-pipeline.safety_checker = None
-pipeline.to("cuda")
-pipeline.unet.to(memory_format=torch.channels_last)
-pipeline.enable_xformers_memory_efficient_attention()
-
-count = 0
-captions = {}
-with torch.inference_mode():
-    for i in tqdm(range(args.num)):
-        p_batch = data[i][0].to_pylist()
-        imgs = pipeline(p_batch, negative_prompt=[args.negative_prompt] * len(p_batch)).images
-        for prompt, img in zip(p_batch, imgs):
-            img.resize((512, 512), Image.BILINEAR).save(os.path.join(args.out_dir, f'{count}.png'), format='PNG')
-            captions[f'{count}.png'] = prompt
-            count += 1
+class DatasetCreator:
+    def __init__(self, pretrained_model, out_dir: str, img_w: int=512, img_h: int=512):
+        self.pipeline = StableDiffusionPipeline.from_pretrained(pretrained_model, torch_dtype=torch.float16)
+        self.pipeline.requires_safety_checker = False
+        self.pipeline.safety_checker = None
+        self.pipeline.to("cuda")
+        self.pipeline.unet.to(memory_format=torch.channels_last)
+        self.pipeline.enable_xformers_memory_efficient_attention()
+
+        self.out_dir = out_dir
+        self.img_w = img_w
+        self.img_h = img_h
+
+    def create_from_prompt_dataset(self, prompt_file: str, negative_prompt: str, bs: int, num: int,
+                                   callback: Callable[[int, int], bool] = None):
+        os.makedirs(self.out_dir, exist_ok=True)
+        data = pq.read_table(prompt_file).to_batches(bs)
+
+        count = 0
+        total = num*bs
+        captions = {}
+        with torch.inference_mode():
+            for i in tqdm(range(num)):
+                p_batch = data[i][0].to_pylist()
+                imgs = self.pipeline(p_batch, negative_prompt=[negative_prompt]*len(p_batch), width=self.img_w, height=self.img_h).images
+                for prompt, img in zip(p_batch, imgs):
+                    img.save(os.path.join(self.out_dir, f'{count}.png'), format='PNG')
+                    captions[f'{count}.png'] = prompt
+                    count += 1
+                if callback:
+                    if not callback(count, total):
+                        break
+
+        with open(os.path.join(self.out_dir, f'image_captions.json'), "w") as f:
+            json.dump(captions, f)
+            import huggingface_hub.utils._validators
+
+    @staticmethod
+    def split_batch(data, bs):
+        return [data[i:i+bs] for i in range(0, len(data), bs)]
+
+if __name__ == '__main__':
+    torch.backends.cudnn.benchmark = True
+    parser = argparse.ArgumentParser(description='Stable Diffusion Training')
+    parser.add_argument('--prompt_file', type=str, default='')
+    parser.add_argument('--model', type=str, default='runwayml/stable-diffusion-v1-5')
+    parser.add_argument('--out_dir', type=str, default=r'./prompt_ds')
+    parser.add_argument('--negative_prompt', type=str,
+                        default='lowres, bad anatomy, bad hands, text, error, missing fingers, extra digit, fewer digits, cropped, worst quality, low quality, normal quality, jpeg artifacts, signature, watermark, username, blurry')
+    parser.add_argument('--num', type=int, default=200)
+    parser.add_argument('--bs', type=int, default=4)
+    parser.add_argument('--img_w', type=int, default=512)
+    parser.add_argument('--img_h', type=int, default=512)
+    args = parser.parse_args()
 
-with open(os.path.join(args.out_dir, f'image_captions.json'), "w") as f:
-    json.dump(captions, f)
+    ds_creator = DatasetCreator(args.model, args.out_dir, args.img_w, args.img_h)
+    ds_creator.create_from_prompt_dataset(args.prompt_file, args.negative_prompt, args.bs, args.num)
```

### Comparing `hcpdiff-0.4.2/hcpdiff/tools/init_proj.py` & `hcpdiff-0.5.4/hcpdiff/tools/init_proj.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,9 +10,14 @@
         if os.path.exists(r'./cfgs'):
             shutil.rmtree(r'./cfgs')
         if os.path.exists(r'./prompt_tuning_template'):
             shutil.rmtree(r'./prompt_tuning_template')
         shutil.copytree(os.path.join(prefix, 'hcpdiff/cfgs'), r'./cfgs')
         shutil.copytree(os.path.join(prefix, 'hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
     except:
-        shutil.copytree(os.path.join(prefix, '../hcpdiff/cfgs'), r'./cfgs')
-        shutil.copytree(os.path.join(prefix, '../hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
+        try:
+            shutil.copytree(os.path.join(prefix, '../hcpdiff/cfgs'), r'./cfgs')
+            shutil.copytree(os.path.join(prefix, '../hcpdiff/prompt_tuning_template'), r'./prompt_tuning_template')
+        except:
+            this_file_dir = os.path.dirname(os.path.abspath(__file__))
+            shutil.copytree(os.path.join(this_file_dir, '../../cfgs'), r'./cfgs')
+            shutil.copytree(os.path.join(this_file_dir, '../../prompt_tuning_template'), r'./prompt_tuning_template')
```

### Comparing `hcpdiff-0.4.2/hcpdiff/tools/lora_convert.py` & `hcpdiff-0.5.4/hcpdiff/tools/lora_convert.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/tools/sd2diffusers.py` & `hcpdiff-0.5.4/hcpdiff/tools/sd2diffusers.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,37 +12,66 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ Conversion script for the LDM checkpoints. """
 
 import argparse
 import os.path
+import sys
+
+if sys.version_info < (3, 8):
+    import importlib_metadata
+else:
+    import importlib.metadata as importlib_metadata
+
+from packaging.version import parse
 
 import diffusers.pipelines.stable_diffusion.convert_from_ckpt as convert_from_ckpt
 import torch
 from diffusers import AutoencoderKL
 from diffusers.pipelines.stable_diffusion.convert_from_ckpt import (
     assign_to_checkpoint,
     conv_attn_to_linear,
     create_vae_diffusers_config,
     renew_vae_attention_paths,
     renew_vae_resnet_paths,
 )
+from diffusers.utils.import_utils import compare_versions
 from omegaconf import OmegaConf
 from transformers import CLIPTextModel
 
 from hcpdiff.ckpt_manager import CkptManagerSafe, CkptManagerPKL
 
 try:
     from diffusers.pipelines.stable_diffusion.convert_from_ckpt import download_from_original_stable_diffusion_ckpt as load_sd_ckpt
 except:
     from diffusers.pipelines.stable_diffusion.convert_from_ckpt import load_pipeline_from_original_stable_diffusion_ckpt as load_sd_ckpt
 
-def convert_ldm_clip_checkpoint(checkpoint):
-    text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14")
+def convert_ldm_clip_checkpoint(checkpoint, local_files_only=False):
+    text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14", local_files_only=local_files_only)
+
+    keys = list(checkpoint.keys())
+
+    text_model_dict = {}
+
+    add_prefix = 'cond_stage_model.transformer.embeddings.position_ids' in checkpoint
+
+    for key in keys:
+        if key.startswith("cond_stage_model.transformer"):
+            t_key = key[len("cond_stage_model.transformer."):]
+            if add_prefix:
+                t_key = 'text_model.'+t_key
+            text_model_dict[t_key] = checkpoint[key]
+
+    text_model.load_state_dict(text_model_dict)
+
+    return text_model
+
+def convert_ldm_clip_checkpoint_0_18(checkpoint, local_files_only=False, text_encoder=None):
+    text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14", local_files_only=local_files_only)
 
     keys = list(checkpoint.keys())
 
     text_model_dict = {}
 
     add_prefix = 'cond_stage_model.transformer.embeddings.position_ids' in checkpoint
 
@@ -217,15 +246,19 @@
         os.makedirs(args.dump_path, exist_ok=True)
         ckpt_manager._save_ckpt(sd_control, None, None, save_path=os.path.join(args.dump_path,
                                                                                f'controlnet.{"safetensors" if args.to_safetensors else "ckpt"}'))
     else:
         pipe.save_pretrained(args.dump_path, safe_serialization=args.to_safetensors)
 
 if __name__ == "__main__":
-    convert_from_ckpt.convert_ldm_clip_checkpoint = convert_ldm_clip_checkpoint
+    diffusers_version = importlib_metadata.version("diffusers")
+    if compare_versions(parse(diffusers_version), '>=', '0.18.0'):
+        convert_from_ckpt.convert_ldm_clip_checkpoint = convert_ldm_clip_checkpoint_0_18
+    else:
+        convert_from_ckpt.convert_ldm_clip_checkpoint = convert_ldm_clip_checkpoint
 
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "--checkpoint_path", default=None, type=str, help="Path to the checkpoint to convert."
     )
     # !wget https://raw.githubusercontent.com/CompVis/stable-diffusion/main/configs/stable-diffusion/v1-inference.yaml
```

### Comparing `hcpdiff-0.4.2/hcpdiff/train_ac.py` & `hcpdiff-0.5.4/hcpdiff/train_ac.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,65 +6,65 @@
     :Affiliation: HCP Lab, SYSU
     :Created:     10/03/2023
     :Licence:     Apache-2.0
 """
 
 import argparse
 import itertools
+import math
 import os
-import sys
 import time
 from functools import partial
 
 import diffusers
 import hydra
 import numpy as np
 import torch
-from torch import nn
+import torch.utils.checkpoint
+# fix checkpoint bug for train part of model
 import torch.utils.checkpoint
 import torch.utils.data
 import transformers
 from accelerate import Accelerator, DistributedDataParallelKwargs
 from accelerate.utils import set_seed
 from diffusers import AutoencoderKL, UNet2DConditionModel
 from diffusers.utils.import_utils import is_xformers_available
 from omegaconf import OmegaConf
+from torch import nn
 from transformers import AutoTokenizer
-from functools import partial
 
 from hcpdiff.ckpt_manager import CkptManagerPKL, CkptManagerSafe
 from hcpdiff.data import RatioBucket, DataGroup
 from hcpdiff.loggers import LoggerGroup
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, CFGContext, DreamArtistPTContext
+from hcpdiff.noise import NoiseBase
 from hcpdiff.utils.cfg_net_tools import make_hcpdiff, make_plugin
 from hcpdiff.utils.ema import ModelEMA
 from hcpdiff.utils.net_utils import get_scheduler, import_text_encoder_class, TEUnetWrapper, load_emb
 from hcpdiff.utils.utils import load_config_with_cli, get_cfg_range, mgcd
 from hcpdiff.visualizer import Visualizer
-from hcpdiff.noise import NoiseBase
 
-# fix checkpoint bug for train part of model
-import torch.utils.checkpoint
-def checkpoint_fix(function, *args, use_reentrant: bool = False, checkpoint_raw = torch.utils.checkpoint.checkpoint, **kwargs):
+def checkpoint_fix(function, *args, use_reentrant: bool = False, checkpoint_raw=torch.utils.checkpoint.checkpoint, **kwargs):
     return checkpoint_raw(function, *args, use_reentrant=use_reentrant, **kwargs)
+
 torch.utils.checkpoint.checkpoint = checkpoint_fix
 
 class Trainer:
     def __init__(self, cfgs_raw):
         cfgs = hydra.utils.instantiate(cfgs_raw)
         self.cfgs = cfgs
 
         self.init_context(cfgs_raw)
 
         if self.is_local_main_process:
             self.exp_dir = os.path.join(self.cfgs.exp_dir, f'{time.strftime("%Y-%m-%d-%H-%M-%S")}')
             os.makedirs(os.path.join(self.exp_dir, 'ckpts/'), exist_ok=True)
-            self.loggers: LoggerGroup = LoggerGroup([builder(exp_dir=self.exp_dir) for builder in self.cfgs.logger])
             with open(os.path.join(self.exp_dir, 'cfg.yaml'), 'w', encoding='utf-8') as f:
                 f.write(OmegaConf.to_yaml(cfgs_raw))
+            self.loggers: LoggerGroup = LoggerGroup([builder(exp_dir=self.exp_dir) for builder in self.cfgs.logger])
         else:
             self.loggers: LoggerGroup = LoggerGroup([builder(exp_dir=None) for builder in self.cfgs.logger])
 
         self.min_log_step = mgcd(*[item.log_step for item in self.loggers.logger_list])
 
         self.loggers.info(f'world_size: {self.world_size}')
         self.loggers.info(f'accumulation: {self.cfgs.train.gradient_accumulation_steps}')
@@ -104,16 +104,21 @@
             self.cfg_context = DreamArtistPTContext(self.cfg_scale, self.num_train_timesteps)
 
         with torch.no_grad():
             self.build_ema()
 
         self.load_resume()
 
-        if cfgs.allow_tf32:
-            torch.backends.cuda.matmul.allow_tf32 = True
+        torch.backends.cuda.matmul.allow_tf32 = cfgs.allow_tf32
+
+        self.steps_per_epoch = len(self.train_loader_group.loader_list[0])
+        if self.cfgs.train.train_epochs is not None:
+            self.cfgs.train.train_steps = self.cfgs.train.train_epochs*self.steps_per_epoch
+        else:
+            self.cfgs.train.train_epochs = math.ceil(self.cfgs.train.train_steps/self.steps_per_epoch)
 
         self.prepare()
 
     @property
     def device(self):
         return self.accelerator.device
 
@@ -186,15 +191,15 @@
         elif self.cfgs.model.pretrained_model_name_or_path:
             self.tokenizer = AutoTokenizer.from_pretrained(
                 self.cfgs.model.pretrained_model_name_or_path, subfolder="tokenizer",
                 revision=self.cfgs.model.revision, use_fast=False,
             )
 
         # Load scheduler and models
-        noise_scheduler=self.cfgs.model.noise_scheduler
+        noise_scheduler = self.cfgs.model.noise_scheduler
         noise_class = getattr(noise_scheduler.func, '__self__', noise_scheduler.func)  # support static or class method
         if issubclass(noise_class, NoiseBase):
             base_scheduler = noise_scheduler.keywords.pop('base_scheduler')(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
             self.noise_scheduler = noise_scheduler(base_scheduler)
         else:
             self.noise_scheduler = noise_scheduler(self.cfgs.model.pretrained_model_name_or_path, subfolder="scheduler")
 
@@ -288,28 +293,32 @@
         self.embedding_hook, self.ex_words_emb = EmbeddingPTHook.hook_from_dir(
             self.cfgs.tokenizer_pt.emb_dir, self.tokenizer, self.text_encoder, log=self.is_local_main_process,
             N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device)
 
         self.text_enc_hook = TEEXHook(self.text_encoder, self.tokenizer, N_repeats=self.cfgs.model.tokenizer_repeats, device=self.device,
                                       clip_skip=self.cfgs.model.clip_skip)
 
-    def build_data(self, data_builder: partial) -> torch.utils.data.DataLoader:
+    def build_dataset(self, data_builder: partial):
         batch_size = data_builder.keywords.pop('batch_size')
         cache_latents = data_builder.keywords.pop('cache_latents')
         self.batch_size_list.append(batch_size)
 
         train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
         train_dataset.bucket.build(batch_size*self.world_size,
-                                   img_root_list=[source.img_root for source in data_builder.keywords['source'].values()])
+                                   img_root_list=[(img_root, source.repeat) for img_root, source in train_dataset.source_dict.items()])
         arb = isinstance(train_dataset.bucket, RatioBucket)
         self.loggers.info(f"len(train_dataset): {len(train_dataset)}")
 
         if cache_latents:
             self.cache_latents = True
             train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
+        return train_dataset, batch_size, arb
+
+    def build_data(self, data_builder: partial) -> torch.utils.data.DataLoader:
+        train_dataset, batch_size, arb = self.build_dataset(data_builder)
 
         # Pytorch Data loader
         train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
                                                                         rank=self.local_rank, shuffle=not arb)
         train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size, num_workers=self.cfgs.train.workers,
                                                    sampler=train_sampler, collate_fn=train_dataset.collate_fn)
         return train_loader
@@ -414,14 +423,16 @@
                 if self.global_step%self.cfgs.train.save_step == 0:
                     self.save_model()
                 if self.global_step%self.min_log_step == 0:
                     lr_model = self.lr_scheduler.get_last_lr()[0] if hasattr(self, 'lr_scheduler') else 0.
                     lr_word = self.lr_scheduler_pt.get_last_lr()[0] if hasattr(self, 'lr_scheduler_pt') else 0.
                     self.loggers.log(datas={
                         'Step':{'format':'[{}/{}]', 'data':[self.global_step, self.cfgs.train.train_steps]},
+                        'Epoch':{'format':'[{}/{}]<{}/{}>', 'data':[self.global_step//self.steps_per_epoch, self.cfgs.train.train_epochs,
+                            self.global_step%self.steps_per_epoch, self.steps_per_epoch]},
                         'LR_model':{'format':'{:.2e}', 'data':[lr_model]},
                         'LR_word':{'format':'{:.2e}', 'data':[lr_word]},
                         'Loss':{'format':'{:.5f}', 'data':[loss_sum.mean()]},
                     }, step=self.global_step)
 
             if self.global_step>=self.cfgs.train.train_steps:
                 break
@@ -495,15 +506,15 @@
                 image = data.pop('img').to(self.device, dtype=self.weight_dtype)
                 att_mask = data.pop('mask').to(self.device) if 'mask' in data else None
                 prompt_ids = data.pop('prompt').to(self.device)
                 other_datas = {k:v.to(self.device, dtype=self.weight_dtype) for k, v in data.items()}
 
                 latents = self.get_latents(image, self.train_loader_group.get_dataset(idx))
                 model_pred, target, timesteps = self.forward(latents, prompt_ids, **other_datas)
-                loss = self.get_loss(model_pred, target, timesteps, att_mask) * self.train_loader_group.get_loss_weights(idx)
+                loss = self.get_loss(model_pred, target, timesteps, att_mask)*self.train_loader_group.get_loss_weights(idx)
                 self.accelerator.backward(loss)
 
             if hasattr(self, 'optimizer'):
                 if self.accelerator.sync_gradients:  # fine-tuning
                     params_to_clip = (
                         itertools.chain(self.unet.parameters(), self.text_encoder.parameters())
                         if self.train_TE else self.unet.parameters()
@@ -576,12 +587,12 @@
         if self.cfgs.vis_info.prompt:
             raise ValueError('vis_info.prompt is None. cannot generate without prompt.')
         viser.vis_to_dir(vis_dir, self.cfgs.vis_prompt)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default=None, required=True)
-    args, _ = parser.parse_known_args()
+    args, cfg_args = parser.parse_known_args()
 
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    conf = load_config_with_cli(args.cfg, args_list=cfg_args)  # skip --cfg
     trainer = Trainer(conf)
     trainer.train()
```

### Comparing `hcpdiff-0.4.2/hcpdiff/train_ac_single.py` & `hcpdiff-0.5.4/hcpdiff/train_ac_single.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,31 +42,21 @@
         self.train_loader_group.loader_list = list(prepared_obj[-ds_num:])
         prepared_obj = prepared_obj[:-ds_num]
 
         for name, obj in zip(prepare_name_list, prepared_obj):
             setattr(self, name, obj)
 
     def build_data(self, data_builder: partial) -> torch.utils.data.DataLoader:
-        batch_size = data_builder.keywords.pop('batch_size')
-        cache_latents = data_builder.keywords.pop('cache_latents')
-        self.batch_size_list.append(batch_size)
-
-        train_dataset = data_builder(tokenizer=self.tokenizer, tokenizer_repeats=self.cfgs.model.tokenizer_repeats)
-        train_dataset.bucket.build(batch_size*self.world_size,
-                                   img_root_list=[source.img_root for source in data_builder.keywords['source'].values()])
-        arb = isinstance(train_dataset.bucket, RatioBucket)
-        logger.info(f"len(train_dataset): {len(train_dataset)}")
-
-        if cache_latents:
-            self.cache_latents = True
-            train_dataset.cache_latents(self.vae, self.weight_dtype, self.device, show_prog=self.is_local_main_process)
+        train_dataset, batch_size, arb = self.build_dataset(data_builder)
 
         # Pytorch Data loader
-        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size,
-                                                   num_workers=self.cfgs.train.workers, shuffle=not arb, collate_fn=train_dataset.collate_fn)
+        train_sampler = torch.utils.data.distributed.DistributedSampler(train_dataset, num_replicas=self.world_size,
+                                                                        rank=self.local_rank, shuffle=not arb)
+        train_loader = torch.utils.data.DataLoader(train_dataset, batch_size=batch_size, num_workers=self.cfgs.train.workers,
+                                                   sampler=train_sampler, collate_fn=train_dataset.collate_fn)
         return train_loader
 
     def encode_decode(self, prompt_ids, noisy_latents, timesteps, **kwargs):
         input_all = dict(prompt_ids=prompt_ids, noisy_latents=noisy_latents, timesteps=timesteps, **kwargs)
         if hasattr(self.text_encoder, 'input_feeder'):
             for feeder in self.text_encoder.input_feeder:
                 feeder(input_all)
@@ -94,12 +84,12 @@
     @property
     def text_encoder_raw(self):
         return self.text_encoder
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
-    args, _ = parser.parse_known_args()
+    args, cfg_args = parser.parse_known_args()
 
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    conf = load_config_with_cli(args.cfg, args_list=cfg_args)  # skip --cfg
     trainer = TrainerSingleCard(conf)
     trainer.train()
```

### Comparing `hcpdiff-0.4.2/hcpdiff/train_colo.py` & `hcpdiff-0.5.4/hcpdiff/train_colo.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,12 +212,12 @@
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
     parser.add_argument( "--placement", type=str, default="cpu",
         help="Placement Policy for Gemini. Valid when using colossalai as dist plan.")
-    args, _ = parser.parse_known_args()
+    args, cfg_args = parser.parse_known_args()
 
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:]) # skip --cfg
+    conf = load_config_with_cli(args.cfg, args_list=cfg_args) # skip --cfg
     trainer=TrainerColo(conf)
     trainer.train()
```

### Comparing `hcpdiff-0.4.2/hcpdiff/train_deepspeed.py` & `hcpdiff-0.5.4/hcpdiff/train_deepspeed.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,12 +72,12 @@
                 self.lr_scheduler = self.cfgs.train.scheduler(optimizer=self.optimizer)
             else:
                 self.lr_scheduler = get_scheduler(optimizer=self.optimizer, **self.cfgs.train.scheduler)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='cfg/train/demo.yaml')
-    args, _ = parser.parse_known_args()
+    args, cfg_args = parser.parse_known_args()
 
-    conf = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    conf = load_config_with_cli(args.cfg, args_list=cfg_args)  # skip --cfg
     trainer = TrainerDeepSpeed(conf)
     trainer.train()
```

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/caption_tools.py` & `hcpdiff-0.5.4/hcpdiff/utils/caption_tools.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/cfg_net_tools.py` & `hcpdiff-0.5.4/hcpdiff/utils/cfg_net_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,25 +199,29 @@
                 else:
                     layer.requires_grad_(False)
                     layer.eval()
                 all_plugin_blocks[from_layer_name] = layer
         elif issubclass(plugin_class, WrapPluginBlock):
             layers_name = builder.keywords.pop('layers')
             for layer_name in get_match_layers(layers_name, named_modules):
-                parent_name, host_name = layers_name.rsplit('.', 1)
+                name_split = layer_name.rsplit('.', 1)
+                if len(name_split)==1:
+                    parent_name, host_name = '', name_split[0]
+                else:
+                    parent_name, host_name = name_split
                 layer = builder(name=plugin_name, host_model=model, host=named_modules[layer_name],
                                 parent_block=named_modules[parent_name], host_name=host_name)
                 if train_plugin:
                     layer.requires_grad_(True)
                     layer.train()
                     params_group.extend(layer.parameters())
                 else:
                     layer.requires_grad_(False)
                     layer.eval()
-                all_plugin_blocks[from_layer_name] = layer
+                all_plugin_blocks[layer_name] = layer
         else:
             raise NotImplementedError(f'Unknown plugin {plugin_class}')
         if train_plugin:
             train_params.append({'params':params_group, 'lr':lr})
         all_plugin_group[plugin_name] = PluginGroup(all_plugin_blocks)
     return train_params, all_plugin_group
 
@@ -229,15 +233,15 @@
 
     ckpt_manager_torch = CkptManagerPKL()
     ckpt_manager_safe = CkptManagerSafe()
 
     def get_ckpt_manager(path:str):
         return ckpt_manager_safe if path.endswith('.safetensors') else ckpt_manager_torch
 
-    if "lora" in cfg_merge and cfg_merge.lora is not None:
+    if getattr(cfg_merge, "lora", None) is not None:
         for lora_id, item in enumerate(cfg_merge.lora):
             lora_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['lora']
             lora_block_state = {}
             # get all layers in the lora_state
             for name, p in lora_state.items():
                 # lora_block. is the old format
                 prefix, block_name = name.split('.___.' if name.rfind('lora_block.')==-1 else '.lora_block.', 1)
@@ -266,27 +270,27 @@
                                                         alpha=getattr(item, 'alpha', 1.0), bias='layer.lora_up.bias' in lora_state,
                                                         rank_groups=rank_groups, alpha_auto_scale=getattr(item, 'alpha_auto_scale', True))
                 all_lora_blocks[f'{host_name}.{lora_block.name}'] = lora_block
                 lora_block.load_state_dict(lora_state, strict=False)
                 lora_block.set_mask(getattr(item, 'mask', None))
                 lora_block.to(model.device)
 
-    if "part" in cfg_merge and cfg_merge.part is not None:
+    if getattr(cfg_merge, "part", None) is not None:
         for item in cfg_merge.part:
             part_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')['base']
             if item.layers == 'all':
                 for k, v in part_state.items():
                     named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
             else:
                 match_blocks = get_match_layers(item.layers, named_modules)
                 state_add = {k:v for blk in match_blocks for k,v in part_state.items() if k.startswith(blk)}
                 for k, v in state_add.items():
                     named_params[k].data = cfg_merge.base_model_alpha * named_params[k].data + item.alpha * v
 
-    if "plugin" in cfg_merge and cfg_merge.plugin is not None:
+    if getattr(cfg_merge, "plugin", None) is not None:
         for name, item in cfg_merge.plugin.items():
             plugin_state = get_ckpt_manager(item.path).load_ckpt(item.path, map_location='cpu')
             if item.layers != 'all':
                 match_blocks = get_match_layers(item.layers, named_modules)
                 plugin_state = {k: v for blk in match_blocks for k, v in plugin_state.items() if k.startswith(blk)}
             plugin_state = {k.replace('___', name):v for k, v in plugin_state.items()} # replace placeholder to target plugin name
             model.load_state_dict(plugin_state, strict=False)
```

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/colo_utils.py` & `hcpdiff-0.5.4/hcpdiff/utils/colo_utils.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/ema.py` & `hcpdiff-0.5.4/hcpdiff/utils/ema.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/img_size_tool.py` & `hcpdiff-0.5.4/hcpdiff/utils/img_size_tool.py`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/net_utils.py` & `hcpdiff-0.5.4/hcpdiff/utils/net_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,23 +121,28 @@
     for k, v in named_modules.items():
         if isinstance(v, layer_class):
             parent, name = named_modules[k.rsplit('.', 1)]
             delattr(parent, name)
             del v
 
 def load_emb(path):
-    emb = torch.load(path, map_location='cpu')['string_to_param']['*']
+    state = torch.load(path, map_location='cpu')
+    if 'string_to_param' in state:
+        emb = state['string_to_param']['*']
+    else:
+        emb = state['emb_params']
     emb.requires_grad_(False)
     return emb
 
 def save_emb(path, emb: torch.Tensor, replace=False):
     name = os.path.basename(path)
     if os.path.exists(path) and not replace:
         raise FileExistsError(f'embedding "{name}" already exist.')
     name = name[:name.rfind('.')]
+    #torch.save({'emb_params':emb, 'name':name}, path)
     torch.save({'string_to_param':{'*':emb}, 'name':name}, path)
 
 def hook_compile(model):
     named_modules = {k:v for k, v in model.named_modules()}
 
     for name, block in named_modules.items():
         if len(block._forward_hooks)>0:
@@ -173,10 +178,12 @@
     return t.to('cpu') if t.device.type == 'cuda' else t
 
 def _convert_cuda(t):
     return t.to('cuda') if t.device.type == 'cpu' else t
 
 def to_cpu(model):
     model._apply(_convert_cpu)
+    torch.cuda.empty_cache()
+    torch.cuda.synchronize()
 
 def to_cuda(model):
     model._apply(_convert_cuda)
```

### Comparing `hcpdiff-0.4.2/hcpdiff/utils/utils.py` & `hcpdiff-0.5.4/hcpdiff/utils/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-from typing import Tuple
+import random
+from typing import Tuple, List, Iterable, Any
 
 import re
 import torch
 import math
-from omegaconf import OmegaConf
+from omegaconf import OmegaConf, ListConfig
+import hashlib
+
+OmegaConf.register_new_resolver("times", lambda a, b: a*b)
 
 size_mul = {'K': 1<<10, 'M':1<<20, 'G':1<<30, 'T':1<<40}
 size_key = 'TGMK'
 
 def str2bool(v):
     return v.lower() in ("yes", "true", "t", "1")
 
@@ -33,31 +37,45 @@
     if len(weight.shape) == 4:
         # U is (out_channels, rank) with 1x1 conv.
         U = U.reshape(U.shape[0], U.shape[1], 1, 1)
         # V is (rank, in_channels * kernel_size1 * kernel_size2)
         Vh = Vh.reshape(Vh.shape[0], in_ch, k1, k2)
     return U, Vh
 
-def load_config(path):
+def remove_config_undefined(cfg):
+    itr: Iterable[Any] = range(len(cfg)) if isinstance(cfg, ListConfig) else cfg
+
+    undefined_keys = []
+    for key in itr:
+        if cfg._get_child(key) == '---':
+            undefined_keys.append(key)
+        elif OmegaConf.is_config(cfg[key]):
+            remove_config_undefined(cfg[key])
+    for key in undefined_keys:
+        del cfg[key]
+    return cfg
+
+def load_config(path, remove_undefined=True):
     cfg = OmegaConf.load(path)
     if '_base_' in cfg:
         for base in cfg['_base_']:
-            cfg = OmegaConf.merge(load_config(base), cfg)
+            cfg = OmegaConf.merge(load_config(base, remove_undefined=False), cfg)
         del cfg['_base_']
+    if remove_undefined:
+        cfg = remove_config_undefined(cfg)
     return cfg
 
-def load_config_with_cli(path, args_list=None):
-    cfg = load_config(path)
+def load_config_with_cli(path, args_list=None, remove_undefined=True):
+    cfg = load_config(path, remove_undefined=False)
     cfg_cli = OmegaConf.from_cli(args_list)
     cfg = OmegaConf.merge(cfg, cfg_cli)
+    if remove_undefined:
+        cfg = remove_config_undefined(cfg)
     return cfg
 
-def _default(v, default):
-    return default if v is None else v
-
 def get_cfg_range(cfg_text:str):
     dy_cfg_f='ln'
     if cfg_text.find(':')!=-1:
         cfg_text, dy_cfg_f = cfg_text.split(':')
 
     if cfg_text.find('-')!=-1:
         l, h = cfg_text.split('-')
@@ -109,8 +127,14 @@
 
 def size_to_int(size):
     return int(size[:-3]) * size_mul[size[-3]]
 
 def int_to_size(size):
     for i,k in zip(range(40, 0, -10), size_key):
         if size >= 1<<i:
-            return f'{size>>i}{k}iB'
+            return f'{size>>i}{k}iB'
+
+def prepare_seed(seeds:List[int], device='cuda'):
+    return [torch.Generator(device=device).manual_seed(s or random.randint(0, 1<<30)) for s in seeds]
+
+def hash_str(data):
+    return hashlib.sha256(data.encode('utf-8')).hexdigest()
```

### Comparing `hcpdiff-0.4.2/hcpdiff/visualizer.py` & `hcpdiff-0.5.4/hcpdiff/visualizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 import argparse
 import os
+import random
 import sys
-import time
+from typing import List
 
 import hydra
-import numpy as np
 import torch
 from PIL import Image
 from accelerate import infer_auto_device_map, dispatch_model
-from diffusers import StableDiffusionPipeline, StableDiffusionImg2ImgPipeline, UNet2DConditionModel
-from diffusers.utils import PIL_INTERPOLATION
 from diffusers.utils.import_utils import is_xformers_available
-from matplotlib import pyplot as plt
-from omegaconf import OmegaConf
 from torch.cuda.amp import autocast
 
 from hcpdiff.models import EmbeddingPTHook, TEEXHook, TokenizerHook, LoraBlock
 from hcpdiff.utils.cfg_net_tools import load_hcpdiff, make_plugin
-from hcpdiff.utils.img_size_tool import types_support
 from hcpdiff.utils.net_utils import to_cpu, to_cuda
-from hcpdiff.utils.utils import to_validate_file, load_config_with_cli, load_config, size_to_int, int_to_size
-
-class UnetHook():  # for controlnet
-    def __init__(self, unet):
-        self.unet = unet
-        self.call_raw = UNet2DConditionModel.__call__
-        UNet2DConditionModel.__call__ = self.unet_call
-
-    def unet_call(self, sample, timestep, encoder_hidden_states, **kwargs):
-        return self.call_raw(self.unet, sample, timestep, encoder_hidden_states)
+from hcpdiff.utils.pipe_hook import HookPipe_T2I, HookPipe_I2I, HookPipe_Inpaint
+from hcpdiff.utils.utils import load_config_with_cli, load_config, size_to_int, int_to_size, prepare_seed
 
 class Visualizer:
     dtype_dict = {'fp32':torch.float32, 'amp':torch.float32, 'fp16':torch.float16}
 
     def __init__(self, cfgs):
         self.cfgs_raw = cfgs
         self.cfgs = hydra.utils.instantiate(self.cfgs_raw)
         self.cfg_merge = self.cfgs.merge
         self.offload = 'offload' in self.cfgs and self.cfgs.offload is not None
-
         self.dtype = self.dtype_dict[self.cfgs.dtype]
 
+        self.need_inter_imgs = any(item.need_inter_imgs for item in self.cfgs.interface)
+
         pipeline = self.get_pipeline()
         comp = pipeline.from_pretrained(self.cfgs.pretrained_model, safety_checker=None, requires_safety_checker=False,
                                         torch_dtype=self.dtype).components
         comp.update(self.cfgs.new_components)
         self.pipe = pipeline(**comp)
 
         if self.cfg_merge:
@@ -52,92 +40,99 @@
 
         self.pipe = self.pipe.to(torch_dtype=self.dtype)
 
         if 'save_model' in self.cfgs and self.cfgs.save_model is not None:
             self.save_model(self.cfgs.save_model)
             os._exit(0)
 
+        self.build_optimize()
+
+    def build_optimize(self):
         if self.offload:
             self.build_offload(self.cfgs.offload)
         else:
             self.pipe.unet.to('cuda')
+        self.build_vae_offload()
 
-            def decode_latents_offload(latents, decode_latents_raw=self.pipe.decode_latents):
-                to_cpu(self.pipe.unet)
-
-                self.pipe.vae.to('cuda')
-                res = decode_latents_raw(latents)
-                to_cpu(self.pipe.vae)
-
-                self.pipe.unet.to('cuda')
-                return res
+        if getattr(self.cfgs, 'vae_optimize', None) is not None:
+            if self.cfgs.vae_optimize.tiling:
+                self.pipe.vae.enable_tiling()
+            if self.cfgs.vae_optimize.slicing:
+                self.pipe.vae.enable_slicing()
 
-            self.pipe.decode_latents = decode_latents_offload
-
-        emb, _ = EmbeddingPTHook.hook_from_dir(self.cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder, N_repeats=self.cfgs.N_repeats)
+        self.emb_hook, _ = EmbeddingPTHook.hook_from_dir(self.cfgs.emb_dir, self.pipe.tokenizer, self.pipe.text_encoder,
+                                                         N_repeats=self.cfgs.N_repeats)
         self.te_hook = TEEXHook.hook_pipe(self.pipe, N_repeats=self.cfgs.N_repeats, clip_skip=self.cfgs.clip_skip)
         self.token_ex = TokenizerHook(self.pipe.tokenizer)
-        UnetHook(self.pipe.unet)
 
         if is_xformers_available():
             self.pipe.unet.enable_xformers_memory_efficient_attention()
             # self.te_hook.enable_xformers()
 
     def save_model(self, save_cfg):
-        for k,v in self.pipe.unet.named_modules():
+        for k, v in self.pipe.unet.named_modules():
             if isinstance(v, LoraBlock):
                 v.reparameterization_to_host()
                 v.remove()
-        for k,v in self.pipe.text_encoder.named_modules():
+        for k, v in self.pipe.text_encoder.named_modules():
             if isinstance(v, LoraBlock):
                 v.reparameterization_to_host()
                 v.remove()
 
         self.pipe.save_pretrained(save_cfg.path, safe_serialization=save_cfg.to_safetensors)
 
     def get_pipeline(self):
         if self.cfgs.condition is None:
-            pipe_cls = StableDiffusionPipeline
+            pipe_cls = HookPipe_T2I
         else:
             if self.cfgs.condition.type == 'i2i':
-                pipe_cls = StableDiffusionImg2ImgPipeline
-            elif self.cfgs.condition.type == 'controlnet':
-                pipe_cls = StableDiffusionPipeline
+                pipe_cls = HookPipe_I2I
+            elif self.cfgs.condition.type == 'inpaint':
+                pipe_cls = HookPipe_Inpaint
             else:
                 raise NotImplementedError(f'No condition type named {self.cfgs.condition.type}')
 
-        class CUDAPipe(pipe_cls):
-            @property
-            def _execution_device(self):
-                return torch.device('cuda')
-        return CUDAPipe
+        return pipe_cls
 
     def build_offload(self, offload_cfg):
         vram = size_to_int(offload_cfg.max_VRAM)
         device_map = infer_auto_device_map(self.pipe.unet, max_memory={0:int_to_size(vram >> 1), "cpu":offload_cfg.max_RAM}, dtype=self.dtype)
         self.pipe.unet = dispatch_model(self.pipe.unet, device_map)
         if not offload_cfg.vae_cpu:
             device_map = infer_auto_device_map(self.pipe.vae, max_memory={0:int_to_size(vram >> 5), "cpu":offload_cfg.max_RAM}, dtype=self.dtype)
             self.pipe.vae = dispatch_model(self.pipe.vae, device_map)
 
-        def decode_latents_offload(latents, decode_latents_raw=self.pipe.decode_latents):
-            to_cpu(self.pipe.unet)
-
-            if offload_cfg.vae_cpu:
-                self.pipe.vae.to(dtype=torch.float32)
-                res = decode_latents_raw(latents.cpu().to(dtype=torch.float32))
-            else:
+    def build_vae_offload(self):
+        def vae_decode_offload(latents, return_dict=True, decode_raw=self.pipe.vae.decode):
+            if self.need_inter_imgs:
                 to_cuda(self.pipe.vae)
-                res = decode_latents_raw(latents)
+                res = decode_raw(latents, return_dict=return_dict)
+            else:
+                to_cpu(self.pipe.unet)
 
+                if self.offload and self.cfgs.offload.vae_cpu:
+                    self.pipe.vae.to(dtype=torch.float32)
+                    res = decode_raw(latents.cpu().to(dtype=torch.float32), return_dict=return_dict)
+                else:
+                    to_cuda(self.pipe.vae)
+                    res = decode_raw(latents, return_dict=return_dict)
+
+                to_cpu(self.pipe.vae)
+                to_cuda(self.pipe.unet)
+            return res
+
+        self.pipe.vae.decode = vae_decode_offload
+
+        def vae_encode_offload(x, return_dict=True, encode_raw=self.pipe.vae.encode):
+            to_cuda(self.pipe.vae)
+            res = encode_raw(x, return_dict=return_dict)
             to_cpu(self.pipe.vae)
-            to_cuda(self.pipe.unet)
             return res
 
-        self.pipe.decode_latents = decode_latents_offload
+        self.pipe.vae.encode = vae_encode_offload
 
     def merge_model(self):
         if 'plugin_cfg' in self.cfg_merge:  # Build plugins
             plugin_cfg = hydra.utils.instantiate(load_config(self.cfg_merge.plugin_cfg))
             make_plugin(self.pipe.unet, plugin_cfg.plugin_unet)
             make_plugin(self.pipe.text_encoder, plugin_cfg.plugin_TE)
 
@@ -147,45 +142,34 @@
                     load_hcpdiff(self.pipe.unet, cfg_group)
                 elif cfg_group.type == 'TE':
                     load_hcpdiff(self.pipe.text_encoder, cfg_group)
 
     def set_scheduler(self, scheduler):
         self.pipe.scheduler = scheduler
 
-    def prepare_cond_image(self, image, width, height, batch_size, device):
-        if not isinstance(image, torch.Tensor):
-            if isinstance(image, Image.Image):
-                image = [image]
-
-            if isinstance(image[0], Image.Image):
-                image = [
-                    np.array(i.resize((width, height), resample=PIL_INTERPOLATION["lanczos"]))[None, :] for i in image
-                ]
-                image = np.concatenate(image, axis=0)
-                image = np.array(image).astype(np.float32)/255.0
-                image = image.transpose(0, 3, 1, 2)
-                image = torch.from_numpy(image)
-            elif isinstance(image[0], torch.Tensor):
-                image = torch.cat(image, dim=0)
-
-        image = image.repeat_interleave(batch_size, dim=0)
-        image = image.to(device=device)
-
-        return image
-
     def get_ex_input(self):
-        ex_input_dict = {}
+        ex_input_dict, pipe_input_dict = {}, {}
         if self.cfgs.condition is not None:
-            img = Image.open(self.cfgs.condition.image).convert('RGB')
-            ex_input_dict['cond'] = self.prepare_cond_image(img, self.cfgs.infer_args.width, self.cfgs.infer_args.height, self.cfgs.bs*2, 'cuda')
-        return ex_input_dict
+            if self.cfgs.condition.type == 'i2i':
+                pipe_input_dict['image'] = Image.open(self.cfgs.condition.image).convert('RGB')
+            elif self.cfgs.condition.type == 'inpaint':
+                pipe_input_dict['image'] = Image.open(self.cfgs.condition.image).convert('RGB')
+                pipe_input_dict['mask_image'] = Image.open(self.cfgs.condition.mask).convert('L')
+
+        if getattr(self.cfgs, 'ex_input', None) is not None:
+            for key, processor in self.cfgs.ex_input.items():
+                ex_input_dict[key] = processor(self.cfgs.infer_args.width, self.cfgs.infer_args.height, self.cfgs.bs*2, 'cuda', self.dtype)
+        return ex_input_dict, pipe_input_dict
 
     @torch.no_grad()
-    def vis_images(self, prompt, negative_prompt='', **kwargs):
-        ex_input_dict = self.get_ex_input()
+    def vis_images(self, prompt, negative_prompt='', seeds: List[int] = None, **kwargs):
+        G = prepare_seed(seeds or [None]*len(prompt))
+
+        ex_input_dict, pipe_input_dict = self.get_ex_input()
+        kwargs.update(pipe_input_dict)
 
         to_cuda(self.pipe.text_encoder)
 
         mult_p, clean_text_p = self.token_ex.parse_attn_mult(prompt)
         mult_n, clean_text_n = self.token_ex.parse_attn_mult(negative_prompt)
         with autocast(enabled=self.cfgs.dtype == 'amp'):
             emb_n, emb_p = self.te_hook.encode_prompt_to_emb(clean_text_n+clean_text_p).chunk(2)
@@ -195,56 +179,48 @@
             to_cpu(self.pipe.text_encoder)
             to_cuda(self.pipe.unet)
 
             if hasattr(self.pipe.unet, 'input_feeder'):
                 for feeder in self.pipe.unet.input_feeder:
                     feeder(ex_input_dict)
 
-            images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, **kwargs).images
+            images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, callback=self.inter_callback,
+                               generator=G, **kwargs).images
         return images
 
-    def save_images(self, images, root, prompt, negative_prompt='', save_cfg=True):
-        os.makedirs(root, exist_ok=True)
-        num_img_exist = max([0]+[int(x.split('-', 1)[0]) for x in os.listdir(root) if x.rsplit('.', 1)[-1] in types_support])+1
-
-        for p, pn, img in zip(prompt, negative_prompt, images):
-            img.save(os.path.join(root, f"{num_img_exist}-{to_validate_file(prompt[0])}.{self.cfgs.save.image_type}"), quality=self.cfgs.save.quality)
-
-            if save_cfg:
-                with open(os.path.join(root, f"{num_img_exist}-info.yaml"), 'w', encoding='utf-8') as f:
-                    f.write(OmegaConf.to_yaml(self.cfgs_raw))
-            num_img_exist += 1
-
-    def vis_to_dir(self, root, prompt, negative_prompt='', save_cfg=True, **kwargs):
-        images = self.vis_images(prompt, negative_prompt, **kwargs)
-        self.save_images(images, root, prompt, negative_prompt, save_cfg=save_cfg)
-
-    def show_latent(self, prompt, negative_prompt='', **kwargs):
-        emb_n, emb_p = self.te_hook.encode_prompt_to_emb(negative_prompt+prompt).chunk(2)
-        emb_p = self.te_hook.mult_attn(emb_p, self.token_ex.parse_attn_mult(prompt))
-        emb_n = self.te_hook.mult_attn(emb_n, self.token_ex.parse_attn_mult(negative_prompt))
-        images = self.pipe(prompt_embeds=emb_p, negative_prompt_embeds=emb_n, output_type='latent', **kwargs).images
-
-        for img in images:
-            plt.figure()
-            for i, feat in enumerate(img):
-                plt.subplot(221+i)
-                plt.imshow(feat)
-            plt.show()
+    def inter_callback(self, i, t, num_t, latents):
+        images = None
+        interrupt = False
+        for interface in self.cfgs.interface:
+            if interface.show_steps>0 and i%interface.show_steps == 0:
+                if self.need_inter_imgs and images is None:
+                    images = self.pipe.decode_latents(latents)
+                    images = self.pipe.numpy_to_pil(images)
+                feed_back = interface.on_inter_step(i, num_t, t, latents, images)
+                interrupt |= bool(feed_back)
+        return interrupt
+
+    def save_images(self, images, prompt, negative_prompt='', save_cfg=True, seeds: List[int] = None):
+        for interface in self.cfgs.interface:
+            interface.on_infer_finish(images, prompt, negative_prompt, self.cfgs_raw if save_cfg else None, seeds=seeds)
+
+    def vis_to_dir(self, prompt, negative_prompt='', save_cfg=True, seeds: List[int] = None, **kwargs):
+        seeds = [s or random.randint(0, 1 << 30) for s in seeds]
+
+        images = self.vis_images(prompt, negative_prompt, seeds=seeds, **kwargs)
+        self.save_images(images, prompt, negative_prompt, save_cfg=save_cfg, seeds=seeds)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Stable Diffusion Training')
     parser.add_argument('--cfg', type=str, default='')
-    args, _ = parser.parse_known_args()
-    cfgs = load_config_with_cli(args.cfg, args_list=sys.argv[3:])  # skip --cfg
+    args, cfg_args = parser.parse_known_args()
+    cfgs = load_config_with_cli(args.cfg, args_list=cfg_args)  # skip --cfg
 
-    os.makedirs(cfgs.out_dir, exist_ok=True)
     if cfgs.seed is not None:
-        G = torch.Generator()
-        G.manual_seed(cfgs.seed)
+        seeds = list(range(cfgs.seed, cfgs.seed+cfgs.num*cfgs.bs))
     else:
-        G = None
+        seeds = [None]*(cfgs.num*cfgs.bs)
 
     viser = Visualizer(cfgs)
     for i in range(cfgs.num):
-        viser.vis_to_dir(cfgs.out_dir, prompt=[cfgs.prompt]*cfgs.bs, negative_prompt=[cfgs.neg_prompt]*cfgs.bs,
-                         generator=G, save_cfg=cfgs.save.save_cfg, **cfgs.infer_args)
+        viser.vis_to_dir(prompt=[cfgs.prompt]*cfgs.bs, negative_prompt=[cfgs.neg_prompt]*cfgs.bs,
+                         seeds=seeds[i*cfgs.bs:(i+1)*cfgs.bs], save_cfg=cfgs.save.save_cfg, **cfgs.infer_args)
```

### Comparing `hcpdiff-0.4.2/hcpdiff.egg-info/PKG-INFO` & `hcpdiff-0.5.4/hcpdiff.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcpdiff
-Version: 0.4.2
+Version: 0.5.4
 Summary: A universal Stable-Diffusion toolbox
 Home-page: https://github.com/7eu7d7/HCP-Diffusion
 Author: Ziyi Dong
 Author-email: dzy7eu7d7@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -24,18 +24,18 @@
 [![GitHub license](https://img.shields.io/github/license/7eu7d7/HCP-Diffusion)](https://github.com/7eu7d7/HCP-Diffusion/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/7eu7d7/HCP-Diffusion/branch/main/graph/badge.svg)](https://codecov.io/gh/7eu7d7/HCP-Diffusion)
 [![open issues](https://isitmaintained.com/badge/open/7eu7d7/HCP-Diffusion.svg)](https://github.com/7eu7d7/HCP-Diffusion/issues)
 
 [📘中文说明](./README_cn.md)
 
 ## Introduction
-HCP-Diffusion is a toolbox for stable diffusion models based on diffusers.
-It facilitates flexiable configurations and component support for training, in comparison with webui and sd-scripts.
+HCP-Diffusion is a toolbox for Stable Diffusion models based on [🤗 Diffusers](https://github.com/huggingface/diffusers).
+It facilitates flexiable configurations and component support for training, in comparison with [webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui) and [sd-scripts](https://github.com/kohya-ss/sd-scripts).
 
-This toolbox supports **colossal-AI**, which can significantly reduce GPU memory usage.
+This toolbox supports [**Colossal-AI**](https://github.com/hpcaitech/ColossalAI), which can significantly reduce GPU memory usage.
 
 HCP-Diffusion can unify existing training methods for text-to-image generation (e.g., Prompt-tuning, Textual Inversion, DreamArtist, Fine-tuning, DreamBooth, LoRA, ControlNet, etc) and model structures through a single ```.yaml``` configuration file.
 
 The toolbox has also implemented an upgraded version of DreamArtist with LoRA, named DreamArtist++, for one-shot text-to-image generation.
 Compared to DreamArtist, DreamArtist++ is more stable with higher image quality and generation controllability, and faster training speed.
 
 ## Features
@@ -47,20 +47,21 @@
 * DreamArtist and DreamArtist++
 * Aspect Ratio Bucket (ARB) with automatic clustering
 * Multiple datasets with multiple data sources
 * Image attention mask
 * Word attention multiplier
 * Custom words that occupy multiple words
 * Maximum sentence length expansion
-* colossal-AI
-* xformers for unet and text-encoder
+* [🤗 Accelerate](https://github.com/huggingface/accelerate)
+* [Colossal-AI](https://github.com/hpcaitech/ColossalAI)
+* [xFormers](https://github.com/facebookresearch/xformers) for UNet and text-encoder
 * CLIP skip
 * Tag shuffle and dropout
-* safetensors support
-* Controlnet (support train)
+* [Safetensors](https://github.com/huggingface/safetensors) support
+* [Controlnet](https://github.com/lllyasviel/ControlNet) (support training)
 * Min-SNR loss
 * Custom optimizer (Lion, DAdaptation, pytorch-optimizer, ...)
 * Custom lr scheduler
 
 ## Install
 
 Install with pip:
@@ -75,76 +76,86 @@
 git clone https://github.com/7eu7d7/HCP-Diffusion.git
 cd HCP-Diffusion
 pip install -e .
 # Modified based on this project or start a new project and make initialization
 ## hcpinit
 ```
 
+To use xFormers to reduce VRAM usage and accelerate training:
+```bash
+# use conda
+conda install xformers -c xformers
+
+# use pip
+pip install xformers>=0.0.17
+```
+
 ## User guidance
 
-Training:
+### Training
+
+Training scripts based on 🤗 Accelerate or Colossal-AI are provided.
++ For 🤗 Accelerate, you may need to [configure the environment](https://github.com/huggingface/accelerate/tree/main#launching-script) before launching the scripts.
++ For Colossal-AI, you can use [torchrun](https://pytorch.org/docs/stable/elastic/run.html) to launch the scripts.
+
 ```yaml
-# with accelerate
+# with Accelerate
 accelerate launch -m hcpdiff.train_ac --cfg cfgs/train/cfg_file.yaml
-# with accelerate and only one gpu
+# with Accelerate and only one GPU
 accelerate launch -m hcpdiff.train_ac_single --cfg cfgs/train/cfg_file.yaml
-# with colossal-AI
+# with Colossal-AI
 torchrun --nproc_per_node 1 -m hcpdiff.train_colo --cfg cfgs/train/cfg_file.yaml
 ```
 
-Inference:
+### Inference
 ```yaml
 python -m hcpdiff.visualizer --cfg cfgs/infer/cfg.yaml pretrained_model=pretrained_model_path \
         prompt='positive_prompt' \
         neg_prompt='negative_prompt' \
         seed=42
 ```
 
-The framework is based on diffusers. So it needs to convert the original stable diffusion model into a supported format using the [scripts provided by diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
+### Conversion of Stable Diffusion models
+The framework is based on 🤗 Diffusers. So it needs to convert the original Stable Diffusion model into a supported format using the [scripts provided by 🤗 Diffusers](https://github.com/huggingface/diffusers/blob/main/scripts/convert_original_stable_diffusion_to_diffusers.py).
 + Download the [config file](https://huggingface.co/runwayml/stable-diffusion-v1-5/blob/main/v1-inference.yaml)
 + Convert models based on config file
 
 ```bash
 python -m hcpdiff.tools.sd2diffusers \
     --checkpoint_path "path_to_stable_diffusion_model" \
     --original_config_file "path_to_config_file" \
     --dump_path "save_directory" \
-    [--extract_ema] # Extract ema model
+    [--extract_ema] # Extract EMA model
     [--from_safetensors] # Whether the original model is in safetensors format
     [--to_safetensors] # Whether to save to safetensors format
 ```
 
 Convert VAE:
 ```bash
 python -m hcpdiff.tools.sd2diffusers \
     --vae_pt_path "path_to_VAE_model" \
     --original_config_file "path_to_config_file" \
     --dump_path "save_directory"
     [--from_safetensors]
 ```
 
+### Tutorials
 + [Model Training Tutorial](doc/guide_train.md)
 + [DreamArtist++ Tutorial](doc/guide_DA.md)
 + [Model Inference Tutorial](doc/guide_infer.md)
 + [Configuration File Explanation](doc/guide_cfg.md)
 + [webui Model Conversion Tutorial](doc/guide_webui_lora.md)
 
-Use xformer to reduce VRAM usage and accelerate training:
-```bash
-# use conda
-conda install xformers -c xformers
+## Contributing
 
-# use pip
-pip install xfromers>=0.0.17
-```
+You are welcome to contribute more models and features to this toolbox!
 
 ## Team
 
 This toolbox is maintained by [HCP-Lab, SYSU](https://www.sysu-hcp.net/).
-More models and features are welcome to contribute to this toolbox.
 
 ## Citation
 
 ```
 @article{DBLP:journals/corr/abs-2211-11337,
   author    = {Ziyi Dong and
                Pengxu Wei and
```

### Comparing `hcpdiff-0.4.2/hcpdiff.egg-info/SOURCES.txt` & `hcpdiff-0.5.4/hcpdiff.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,65 +4,78 @@
 cfgs/deepspeed.json
 cfgs/te_struct.txt
 cfgs/unet_struct.txt
 cfgs/infer/change_vae.yaml
 cfgs/infer/euler_a.yaml
 cfgs/infer/img2img.yaml
 cfgs/infer/img2img_controlnet.yaml
+cfgs/infer/inpaint.yaml
+cfgs/infer/load_unet_part.yaml
 cfgs/infer/offload_2GB.yaml
+cfgs/infer/save_model.yaml
 cfgs/infer/text2img.yaml
 cfgs/infer/text2img_DA++.yaml
+cfgs/infer/text2img_anime.yaml
 cfgs/plugins/plugin_controlnet.yaml
 cfgs/train/train_base.yaml
 cfgs/train/tuning_base.yaml
+cfgs/train/dataset/base_dataset.yaml
+cfgs/train/dataset/regularization_dataset.yaml
 cfgs/train/examples/CustomDiffusion.yaml
 cfgs/train/examples/DreamArtist++.yaml
 cfgs/train/examples/DreamArtist.yaml
 cfgs/train/examples/DreamBooth.yaml
 cfgs/train/examples/Lion_optimizer.yaml
 cfgs/train/examples/TextualInversion.yaml
+cfgs/train/examples/add_logger_tensorboard_wandb.yaml
 cfgs/train/examples/controlnet.yaml
 cfgs/train/examples/fine-tuning.yaml
 cfgs/train/examples/locon.yaml
+cfgs/train/examples/lora_anime.yaml
 cfgs/train/examples/lora_conventional.yaml
 cfgs/train/examples/min_snr.yaml
 hcpdiff/__init__.py
 hcpdiff/train_ac.py
 hcpdiff/train_ac_single.py
 hcpdiff/train_colo.py
 hcpdiff/train_deepspeed.py
 hcpdiff/visualizer.py
+hcpdiff/visualizer_reloadable.py
 hcpdiff.egg-info/PKG-INFO
 hcpdiff.egg-info/SOURCES.txt
 hcpdiff.egg-info/dependency_links.txt
 hcpdiff.egg-info/entry_points.txt
 hcpdiff.egg-info/requires.txt
 hcpdiff.egg-info/top_level.txt
 hcpdiff/ckpt_manager/__init__.py
 hcpdiff/ckpt_manager/ckpt_pkl.py
 hcpdiff/ckpt_manager/ckpt_safetensor.py
 hcpdiff/data/__init__.py
 hcpdiff/data/bucket.py
+hcpdiff/data/caption_loader.py
 hcpdiff/data/cond_pair_dataset.py
+hcpdiff/data/data_processor.py
 hcpdiff/data/pair_dataset.py
 hcpdiff/data/utils.py
 hcpdiff/loggers/__init__.py
 hcpdiff/loggers/base_logger.py
 hcpdiff/loggers/cli_logger.py
 hcpdiff/loggers/tensorboard_logger.py
 hcpdiff/loggers/wandb_logger.py
+hcpdiff/loggers/webui_logger.py
 hcpdiff/loss/__init__.py
 hcpdiff/loss/min_snr_loss.py
 hcpdiff/loss/mse_loss.py
 hcpdiff/models/__init__.py
 hcpdiff/models/cfg_context.py
 hcpdiff/models/controlnet.py
 hcpdiff/models/layers.py
 hcpdiff/models/lora_base.py
 hcpdiff/models/lora_layers.py
+hcpdiff/models/multi_textencoder.py
 hcpdiff/models/plugin.py
 hcpdiff/models/text_emb_ex.py
 hcpdiff/models/textencoder_ex.py
 hcpdiff/models/tokenizer_ex.py
 hcpdiff/noise/__init__.py
 hcpdiff/noise/noise_base.py
 hcpdiff/noise/pyramid_noise.py
@@ -76,15 +89,20 @@
 hcpdiff/utils/__init__.py
 hcpdiff/utils/caption_tools.py
 hcpdiff/utils/cfg_net_tools.py
 hcpdiff/utils/colo_utils.py
 hcpdiff/utils/ema.py
 hcpdiff/utils/img_size_tool.py
 hcpdiff/utils/net_utils.py
+hcpdiff/utils/pipe_hook.py
 hcpdiff/utils/utils.py
+hcpdiff/vis/__init__.py
+hcpdiff/vis/base_interface.py
+hcpdiff/vis/disk_interface.py
+hcpdiff/vis/webui_interface.py
 prompt_tuning_template/caption.txt
 prompt_tuning_template/name.txt
 prompt_tuning_template/name_2pt_caption.txt
 prompt_tuning_template/name_caption.txt
 prompt_tuning_template/object.txt
 prompt_tuning_template/object_caption.txt
 prompt_tuning_template/style.txt
```

### Comparing `hcpdiff-0.4.2/prompt_tuning_template/object.txt` & `hcpdiff-0.5.4/prompt_tuning_template/object.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/prompt_tuning_template/object_caption.txt` & `hcpdiff-0.5.4/prompt_tuning_template/object_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/prompt_tuning_template/style.txt` & `hcpdiff-0.5.4/prompt_tuning_template/style.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/prompt_tuning_template/style_caption.txt` & `hcpdiff-0.5.4/prompt_tuning_template/style_caption.txt`

 * *Files identical despite different names*

### Comparing `hcpdiff-0.4.2/setup.py` & `hcpdiff-0.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             file_dict[prefix+root].append(os.path.join(root, name))
     return [(k, v) for k, v in file_dict.items()]
 
 
 setuptools.setup(
     name="hcpdiff",
     py_modules=["hcpdiff"],
-    version="0.4.2",
+    version="0.5.4",
     author="Ziyi Dong",
     author_email="dzy7eu7d7@gmail.com",
     description="A universal Stable-Diffusion toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/7eu7d7/HCP-Diffusion",
     packages=setuptools.find_packages(),
```

