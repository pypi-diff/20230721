# Comparing `tmp/meta-core-3.7.24.tar.gz` & `tmp/meta-core-3.7.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-core-3.7.24.tar", last modified: Fri Jul 21 10:54:09 2023, max compression
+gzip compressed data, was "dist/meta-core-3.7.25.tar", last modified: Fri Jul 21 11:24:15 2023, max compression
```

## Comparing `meta-core-3.7.24.tar` & `meta-core-3.7.25.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 10:54:09.000000 meta-core-3.7.24/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.24/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/meta_core.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 10:54:08.000000 meta-core-3.7.24/meta_core.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)     3911 2023-07-21 10:54:09.000000 meta-core-3.7.24/meta_core.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 10:54:08.000000 meta-core-3.7.24/meta_core.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       44 2023-07-21 10:54:08.000000 meta-core-3.7.24/meta_core.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 10:54:08.000000 meta-core-3.7.24/meta_core.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 10:54:08.000000 meta-core-3.7.24/meta_core.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/metacore/
--rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.24/metacore/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/metacore/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.24/metacore/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4442 2023-07-21 08:16:25.000000 meta-core-3.7.24/metacore/app/ad_segment.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.24/metacore/app/segment.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/metacore/open_clip/
--rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)  1356917 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz
--rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/coca_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/constants.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-21 07:44:42.000000 meta-core-3.7.24/metacore/open_clip/factory.py
--rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/generation_utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/hf_configs.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/hf_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/loss.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/metacore/open_clip/model_configs/
--rw-rw-r--   0 cash      (1000) cash      (1000)      388 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN101-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN101.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      389 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN50-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN50.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN50x16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN50x4.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      370 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/RN50x64.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-B-16-plus-240.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-B-16-plus.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-B-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-B-32-plus-256.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      318 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-B-32-quickgelu.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-H-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-L-14-280.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-L-14-336.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-L-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-L-16-320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-L-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-M-16-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-M-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-M-32-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-M-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-S-16-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-S-16.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-S-32-alt.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-S-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-bigG-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-e-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      353 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/ViT-g-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      659 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/coca_ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      664 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/coca_ViT-L-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      669 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/coca_base.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      517 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      421 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_base.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_base_w.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_base_w_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      423 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_large.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_large_d.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_large_d_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_small.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_tiny.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      426 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_xlarge.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_xxlarge.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/convnext_xxlarge_320.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/mt5-base-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      349 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/mt5-xl-ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      343 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/roberta-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      380 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/swin_base_patch4_window7_224.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      377 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/vit_medium_patch16_gap_256.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      384 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/vit_relpos_medium_patch16_cls_224.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      327 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
--rw-rw-r--   0 cash      (1000) cash      (1000)      357 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
--rw-rw-r--   0 cash      (1000) cash      (1000)     7216 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/modified_resnet.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/openai.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/pretrained.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/push_to_hf_hub.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/timm_model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-21 07:44:52.000000 meta-core-3.7.24/metacore/open_clip/tokenizer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/transform.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/transformer.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/utils.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.24/metacore/open_clip/version.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 10:54:09.000000 meta-core-3.7.24/metacore/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.24/metacore/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.24/metacore/utils/f3net.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.24/metacore/utils/model.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.24/metacore/utils/prompt_ensemble.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-21 10:54:09.000000 meta-core-3.7.24/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      755 2023-07-21 10:53:57.000000 meta-core-3.7.24/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 11:24:15.000000 meta-core-3.7.25/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 05:38:11.000000 meta-core-3.7.25/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      250 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3911 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       55 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        9 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-07-21 11:24:15.000000 meta-core-3.7.25/meta_core.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/metacore/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       36 2023-07-21 03:33:13.000000 meta-core-3.7.25/metacore/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/metacore/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       63 2023-07-21 03:32:52.000000 meta-core-3.7.25/metacore/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4442 2023-07-21 08:16:25.000000 meta-core-3.7.25/metacore/app/ad_segment.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2669 2023-07-21 03:36:00.000000 meta-core-3.7.25/metacore/app/segment.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/metacore/open_clip/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      963 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)  1356917 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17824 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/coca_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      116 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/constants.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    15355 2023-07-21 07:44:42.000000 meta-core-3.7.25/metacore/open_clip/factory.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)        0 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/generation_utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1675 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/hf_configs.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6298 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/hf_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7943 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/loss.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    17866 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/metacore/open_clip/model_configs/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      388 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN101-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN101.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      389 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN50-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      364 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN50.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN50x16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      365 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN50x4.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      370 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/RN50x64.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-B-16-plus-240.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-B-16-plus.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-B-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      295 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-B-32-plus-256.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      318 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-B-32-quickgelu.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      324 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-H-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-L-14-280.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-L-14-336.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-L-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-L-16-320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      296 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-L-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-M-16-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-M-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-M-32-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-M-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-S-16-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-S-16.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-S-32-alt.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      294 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-S-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-bigG-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      354 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-e-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      353 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/ViT-g-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      659 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/coca_ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      664 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/coca_ViT-L-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      669 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/coca_base.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      517 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      421 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_base.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_base_w.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_base_w_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      423 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_large.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_large_d.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      420 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_large_d_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_small.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      422 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_tiny.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      426 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_xlarge.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_xxlarge.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      427 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/convnext_xxlarge_320.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      325 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/mt5-base-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      349 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/mt5-xl-ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      343 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/roberta-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      380 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/swin_base_patch4_window7_224.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      377 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/vit_medium_patch16_gap_256.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      384 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/vit_relpos_medium_patch16_cls_224.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      327 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/xlm-roberta-base-ViT-B-32.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)      357 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/model_configs/xlm-roberta-large-ViT-H-14.json
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7207 2023-07-21 11:10:23.000000 meta-core-3.7.25/metacore/open_clip/modified_resnet.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5446 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/openai.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    14144 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/pretrained.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7660 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/push_to_hf_hub.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     5077 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/timm_model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     7411 2023-07-21 07:44:52.000000 meta-core-3.7.25/metacore/open_clip/tokenizer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4807 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/transform.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    28483 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/transformer.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2223 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/utils.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       23 2023-07-18 04:03:16.000000 meta-core-3.7.25/metacore/open_clip/version.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-07-21 11:24:15.000000 meta-core-3.7.25/metacore/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      118 2023-07-21 03:18:21.000000 meta-core-3.7.25/metacore/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     8749 2023-07-21 01:36:04.000000 meta-core-3.7.25/metacore/utils/f3net.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      742 2023-07-18 14:30:35.000000 meta-core-3.7.25/metacore/utils/model.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     2624 2023-07-18 14:30:35.000000 meta-core-3.7.25/metacore/utils/prompt_ensemble.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-07-21 11:24:15.000000 meta-core-3.7.25/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      781 2023-07-21 11:23:58.000000 meta-core-3.7.25/setup.py
```

### Comparing `meta-core-3.7.24/meta_core.egg-info/SOURCES.txt` & `meta-core-3.7.25/meta_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/app/ad_segment.py` & `meta-core-3.7.25/metacore/app/ad_segment.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/app/segment.py` & `meta-core-3.7.25/metacore/app/segment.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/__init__.py` & `meta-core-3.7.25/metacore/open_clip/__init__.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz` & `meta-core-3.7.25/metacore/open_clip/bpe_simple_vocab_16e6.txt.gz`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/coca_model.py` & `meta-core-3.7.25/metacore/open_clip/coca_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/factory.py` & `meta-core-3.7.25/metacore/open_clip/factory.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/hf_configs.py` & `meta-core-3.7.25/metacore/open_clip/hf_configs.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/hf_model.py` & `meta-core-3.7.25/metacore/open_clip/hf_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/loss.py` & `meta-core-3.7.25/metacore/open_clip/loss.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/model.py` & `meta-core-3.7.25/metacore/open_clip/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/model_configs/coca_ViT-B-32.json` & `meta-core-3.7.25/metacore/open_clip/model_configs/coca_ViT-B-32.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/model_configs/coca_ViT-L-14.json` & `meta-core-3.7.25/metacore/open_clip/model_configs/coca_ViT-L-14.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/model_configs/coca_base.json` & `meta-core-3.7.25/metacore/open_clip/model_configs/coca_base.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json` & `meta-core-3.7.25/metacore/open_clip/model_configs/coca_roberta-ViT-B-32.json`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/modified_resnet.py` & `meta-core-3.7.25/metacore/open_clip/modified_resnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import OrderedDict
 
 import torch
 from torch import nn
 from torch.nn import functional as F
 
-from open_clip.utils import freeze_batch_norm_2d
+from .utils import freeze_batch_norm_2d
 
 
 class Bottleneck(nn.Module):
     expansion = 4
 
     def __init__(self, inplanes, planes, stride=1):
         super().__init__()
```

### Comparing `meta-core-3.7.24/metacore/open_clip/openai.py` & `meta-core-3.7.25/metacore/open_clip/openai.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/pretrained.py` & `meta-core-3.7.25/metacore/open_clip/pretrained.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/push_to_hf_hub.py` & `meta-core-3.7.25/metacore/open_clip/push_to_hf_hub.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/timm_model.py` & `meta-core-3.7.25/metacore/open_clip/timm_model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/tokenizer.py` & `meta-core-3.7.25/metacore/open_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/transform.py` & `meta-core-3.7.25/metacore/open_clip/transform.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/transformer.py` & `meta-core-3.7.25/metacore/open_clip/transformer.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/open_clip/utils.py` & `meta-core-3.7.25/metacore/open_clip/utils.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/utils/f3net.py` & `meta-core-3.7.25/metacore/utils/f3net.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/utils/model.py` & `meta-core-3.7.25/metacore/utils/model.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/metacore/utils/prompt_ensemble.py` & `meta-core-3.7.25/metacore/utils/prompt_ensemble.py`

 * *Files identical despite different names*

### Comparing `meta-core-3.7.24/setup.py` & `meta-core-3.7.25/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 requirements = [
     'opencv-python',
     'setuptools',
     'numpy',
     'pillow',
-    'torch'
+    'torch',
+    'ftfy',
+    'regex',
 ]
 
-__version__ = 'V3.07.24'
+__version__ = 'V3.07.25'
 
 setup(
     name='meta-core',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvreid',
```

