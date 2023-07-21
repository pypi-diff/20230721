# Comparing `tmp/meta-core-3.7.19.tar.gz` & `tmp/meta-core-3.7.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-core-3.7.19.tar", last modified: Fri Jul 21 07:47:29 2023, max compression
+gzip compressed data, was "dist/meta-core-3.7.20.tar", last modified: Fri Jul 21 08:26:00 2023, max compression
```

## Comparing `meta-core-3.7.19.tar` & `meta-core-3.7.20.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 07:47:29.000000 meta-core-3.7.19/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.19/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)     3911 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 07:47:29.000000 meta-core-3.7.19/meta_core.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/metacore/
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.19/metacore/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/metacore/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.19/metacore/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4391 2023-07-21 07:00:51.000000 meta-core-3.7.19/metacore/app/ad_segment.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.19/metacore/app/segment.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/metacore/open_clip/
--rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)  1356917 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/coca_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/constants.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-21 07:44:42.000000 meta-core-3.7.19/metacore/open_clip/factory.py
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/generation_utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/hf_configs.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/hf_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/loss.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/metacore/open_clip/model_configs/
--rw-rw-r--   0 cash      (1000) cash      (1000)      388 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN101-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN101.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      389 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN50-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN50.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN50x16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN50x4.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      370 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/RN50x64.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-B-16-plus-240.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-B-16-plus.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-B-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-B-32-plus-256.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      318 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-H-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-L-14-280.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-L-14-336.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-L-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-L-16-320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-L-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-M-16-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-M-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-M-32-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-M-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-S-16-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-S-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-S-32-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-S-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-bigG-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-e-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      353 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/ViT-g-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      659 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/coca_ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      664 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/coca_ViT-L-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      669 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/coca_base.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      517 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      421 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_base.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_base_w.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_base_w_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      423 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_large.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_large_d.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_large_d_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_small.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_tiny.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      426 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_xlarge.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_xxlarge.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/convnext_xxlarge_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/mt5-base-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      349 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/mt5-xl-ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      343 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/roberta-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      380 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/swin_base_patch4_window7_224.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      377 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/vit_medium_patch16_gap_256.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      384 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/vit_relpos_medium_patch16_cls_224.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      327 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      357 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)     7216 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/modified_resnet.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/openai.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/pretrained.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/push_to_hf_hub.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/timm_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-21 07:44:52.000000 meta-core-3.7.19/metacore/open_clip/tokenizer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/transform.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/transformer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.19/metacore/open_clip/version.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 07:47:29.000000 meta-core-3.7.19/metacore/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.19/metacore/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.19/metacore/utils/f3net.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.19/metacore/utils/model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.19/metacore/utils/prompt_ensemble.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-21 07:47:29.000000 meta-core-3.7.19/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      755 2023-07-21 07:47:18.000000 meta-core-3.7.19/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 08:26:00.000000 meta-core-3.7.20/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.20/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3911 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 08:26:00.000000 meta-core-3.7.20/meta_core.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/metacore/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.20/metacore/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/metacore/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.20/metacore/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4442 2023-07-21 08:16:25.000000 meta-core-3.7.20/metacore/app/ad_segment.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.20/metacore/app/segment.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/metacore/open_clip/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)  1356917 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/coca_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/constants.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-21 07:44:42.000000 meta-core-3.7.20/metacore/open_clip/factory.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/generation_utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/hf_configs.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/hf_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/loss.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/metacore/open_clip/model_configs/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      388 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN101-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN101.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      389 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN50-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN50.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN50x16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN50x4.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      370 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/RN50x64.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-B-16-plus-240.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-B-16-plus.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-B-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-B-32-plus-256.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      318 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-H-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-L-14-280.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-L-14-336.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-L-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-L-16-320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-L-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-M-16-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-M-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-M-32-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-M-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-S-16-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-S-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-S-32-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-S-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-bigG-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-e-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      353 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/ViT-g-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      659 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/coca_ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      664 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/coca_ViT-L-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      669 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/coca_base.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      517 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      421 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_base.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_base_w.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_base_w_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      423 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_large.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_large_d.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_large_d_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_small.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_tiny.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      426 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_xlarge.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_xxlarge.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/convnext_xxlarge_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/mt5-base-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      349 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/mt5-xl-ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      343 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/roberta-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      380 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/swin_base_patch4_window7_224.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      377 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/vit_medium_patch16_gap_256.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      384 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/vit_relpos_medium_patch16_cls_224.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      327 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      357 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7216 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/modified_resnet.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/openai.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/pretrained.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/push_to_hf_hub.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/timm_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-21 07:44:52.000000 meta-core-3.7.20/metacore/open_clip/tokenizer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/transform.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/transformer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.20/metacore/open_clip/version.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 08:26:00.000000 meta-core-3.7.20/metacore/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.20/metacore/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.20/metacore/utils/f3net.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.20/metacore/utils/model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.20/metacore/utils/prompt_ensemble.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-21 08:26:00.000000 meta-core-3.7.20/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      755 2023-07-21 08:25:50.000000 meta-core-3.7.20/setup.py
```

### Comparing `meta-core-3.7.19/meta_core.egg-info/SOURCES.txt` & `meta-core-3.7.20/meta_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/app/ad_segment.py` & `meta-core-3.7.20/metacore/app/ad_segment.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                  model_name="ViT-L-14-336"):
         self.obj_list = obj_list
         self.image_size = image_size
         self.features_list = features_list
         self.device = "cuda:0" if torch.cuda.is_available() else "cpu"
         # clip
         self.clip, _, self.transform = open_clip.create_model_and_transforms(model_name, image_size,
-                                                                             pretrained="openai", device=self.device)
+                                                                             pretrained="openai")
         self.clip.to(self.device)
         tokenizer = open_clip.get_tokenizer(model_name)
         # seg
         with open(config_path, 'r') as f:
             model_configs = json.load(f)
         self.model = LinearLayer(model_configs['vision_cfg']['width'],
                                  model_configs['embed_dim'],
@@ -54,14 +54,15 @@
         checkpoint = torch.load(model_path)
         self.model.load_state_dict(checkpoint["trainable_linearlayer"])
         # text prompt
         with torch.cuda.amp.autocast(), torch.no_grad():
             self.text_prompts = encode_text_with_prompt_ensemble(self.clip, obj_list, tokenizer, self.device)
 
     def predict(self, image, thre=0.5):
+        h, w = image.shape[:2]
         image_tensor = self.transform(Image.fromarray(image))
         image_tensor = image_tensor.unsqueeze(0)
         image_tensor = image_tensor.cuda()
 
         with torch.no_grad(), torch.cuda.amp.autocast():
             image_features, patch_tokens = self.clip.encode_image(image_tensor, self.features_list)
             image_features /= image_features.norm(dim=-1, keepdim=True)
@@ -78,15 +79,16 @@
                 H = int(np.sqrt(L))
                 anomaly_map = F.interpolate(anomaly_map.permute(0, 2, 1).view(B, 2, H, H),
                                             size=self.image_size, mode='bilinear', align_corners=True)
                 anomaly_map = torch.softmax(anomaly_map, dim=1)[:, 1, :, :]
                 anomaly_maps.append(anomaly_map.cpu().numpy())
             anomaly_map = np.sum(anomaly_maps, axis=0)
 
-        mask = normalize(anomaly_map[0]) > thre
+        mask = cv2.resize(normalize(anomaly_map[0]), (w, h))
+        mask = mask > thre
         torch.cuda.empty_cache()
         return mask
 
     @staticmethod
     def get_rect(mask):
         mask = (mask * 255).astype(np.uint8)
         _, pred = cv2.threshold(mask, 128, 255, cv2.THRESH_BINARY)
```

### Comparing `meta-core-3.7.19/metacore/app/segment.py` & `meta-core-3.7.20/metacore/app/segment.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/__init__.py` & `meta-core-3.7.20/metacore/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz` & `meta-core-3.7.20/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/coca_model.py` & `meta-core-3.7.20/metacore/open_clip/coca_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/factory.py` & `meta-core-3.7.20/metacore/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/hf_configs.py` & `meta-core-3.7.20/metacore/open_clip/hf_configs.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/hf_model.py` & `meta-core-3.7.20/metacore/open_clip/hf_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/loss.py` & `meta-core-3.7.20/metacore/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/model.py` & `meta-core-3.7.20/metacore/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/model_configs/coca_ViT-B-32.json` & `meta-core-3.7.20/metacore/open_clip/model_configs/coca_ViT-B-32.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/model_configs/coca_ViT-L-14.json` & `meta-core-3.7.20/metacore/open_clip/model_configs/coca_ViT-L-14.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/model_configs/coca_base.json` & `meta-core-3.7.20/metacore/open_clip/model_configs/coca_base.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json` & `meta-core-3.7.20/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/modified_resnet.py` & `meta-core-3.7.20/metacore/open_clip/modified_resnet.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/openai.py` & `meta-core-3.7.20/metacore/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/pretrained.py` & `meta-core-3.7.20/metacore/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/push_to_hf_hub.py` & `meta-core-3.7.20/metacore/open_clip/push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/timm_model.py` & `meta-core-3.7.20/metacore/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/tokenizer.py` & `meta-core-3.7.20/metacore/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/transform.py` & `meta-core-3.7.20/metacore/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/transformer.py` & `meta-core-3.7.20/metacore/open_clip/transformer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/open_clip/utils.py` & `meta-core-3.7.20/metacore/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/utils/f3net.py` & `meta-core-3.7.20/metacore/utils/f3net.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/utils/model.py` & `meta-core-3.7.20/metacore/utils/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/metacore/utils/prompt_ensemble.py` & `meta-core-3.7.20/metacore/utils/prompt_ensemble.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.19/setup.py` & `meta-core-3.7.20/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     'opencv-python',
     'setuptools',
     'numpy',
     'pillow',
     'torch'
 ]
 
-__version__ = 'V3.07.19'
+__version__ = 'V3.07.20'
 
 setup(
     name='meta-core',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

