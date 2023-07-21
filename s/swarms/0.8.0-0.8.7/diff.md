# Comparing `tmp/swarms-0.8.0.tar.gz` & `tmp/swarms-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swarms-0.8.0.tar", last modified: Sat Jul  8 21:37:13 2023, max compression
+gzip compressed data, was "swarms-0.8.7.tar", last modified: Fri Jul 21 21:39:42 2023, max compression
```

## Comparing `swarms-0.8.0.tar` & `swarms-0.8.7.tar`

### file list

```diff
@@ -1,120 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.283095 swarms-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-08 21:37:03.000000 swarms-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-08 21:37:13.283095 swarms-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17658 2023-07-08 21:37:03.000000 swarms-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.251095 swarms-0.8.0/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-08 21:37:03.000000 swarms-0.8.0/api/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-08 21:37:03.000000 swarms-0.8.0/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-08 21:37:03.000000 swarms-0.8.0/api/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:37:13.283095 swarms-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-08 21:37:03.000000 swarms-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.251095 swarms-0.8.0/swarms/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.255095 swarms-0.8.0/swarms/agents/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.255095 swarms-0.8.0/swarms/agents/boss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/boss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/boss/babyagi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/boss/boss_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34590 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/auto_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/metaprompt_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.259095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.263095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.263095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.267095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.267095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.271095 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.271095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.275095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.275095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/models/segment_anything/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/omni_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/visual_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/agents/workers/worker_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.279095 swarms-0.8.0/swarms/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)    20151 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/swarms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.283095 swarms-0.8.0/swarms/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/tools/agent_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    71643 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/tools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.283095 swarms-0.8.0/swarms/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-08 21:37:03.000000 swarms-0.8.0/swarms/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 21:37:13.255095 swarms-0.8.0/swarms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 21:37:13.000000 swarms-0.8.0/swarms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.538770 swarms-0.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 21:39:30.000000 swarms-0.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 21:39:42.538770 swarms-0.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-21 21:39:30.000000 swarms-0.8.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.506770 swarms-0.8.7/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-21 21:39:30.000000 swarms-0.8.7/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 21:39:42.538770 swarms-0.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-21 21:39:30.000000 swarms-0.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.506770 swarms-0.8.7/swarms/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/boss/
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/boss/BossNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/boss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18115 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/memory/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22333 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/memory/chroma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/models/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/prompts/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/agent_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/tools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms/agents/tools/core/code_interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/core/code_interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27478 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/core/code_interpreter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73358 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/tools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.514770 swarms-0.8.7/swarms/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/Agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/Calback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/ChatOpenAI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/ConversationalChatAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/agent_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/agent_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/utils/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.514770 swarms-0.8.7/swarms/agents/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/MultiModalVisualAgentTool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/OmniWorkerAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/PromptWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/WorkerNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/generative_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.518770 swarms-0.8.7/swarms/agents/workers/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.518770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.518770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.518770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.518770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.518770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.522770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.522770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16669 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.522770 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.522770 swarms-0.8.7/swarms/agents/workers/models/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.526770 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15148 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.526770 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14420 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.526770 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/models/segment_anything/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.526770 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79584 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.530770 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31378 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45882 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/worker_agent_ultra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/agents/workers/worker_ultra_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/hivemind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/swarms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.530770 swarms-0.8.7/swarms/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.530770 swarms-0.8.7/swarms/utils/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.538770 swarms-0.8.7/swarms/utils/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-21 21:39:30.000000 swarms-0.8.7/swarms/utils/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 21:39:42.510770 swarms-0.8.7/swarms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-21 21:39:42.000000 swarms-0.8.7/swarms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-07-21 21:39:42.000000 swarms-0.8.7/swarms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 21:39:42.000000 swarms-0.8.7/swarms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-21 21:39:42.000000 swarms-0.8.7/swarms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-21 21:39:42.000000 swarms-0.8.7/swarms.egg-info/top_level.txt
```

### Comparing `swarms-0.8.0/LICENSE` & `swarms-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/PKG-INFO` & `swarms-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.8.0
+Version: 0.8.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.8.0/setup.py` & `swarms-0.8.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
-# 
+#
 
 setup(
   name = 'swarms',
   packages = find_packages(exclude=[]),
-  version = '0.8.0',
+  version = '0.8.7',
   license='MIT',
   description = 'Swarms - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/swarms',
   keywords = [
@@ -68,25 +68,24 @@
         'llama-index',
         'fastapi==0.94.1',
         'pydantic==1.10.6',
         'tenacity==8.2.2',
         'python-dotenv',
         'boto3',
         'uvicorn==0.21.1',
-        'python-ptrace==0.9.8',
         'jinja2==3.1.2',
         'python-multipart==0.0.6',
         'celery==5.2.7',
         'redis==4.5.4',
-        'sentencepiece==0.1.97',
+        'sentencepiece',
         'bitsandbytes==0.37.2',
         'psycopg2-binary==2.9.5',
         'google-search-results==2.4.2',
         'black==23.1.0',
-        'Pillow==9.0.0',
+        'Pillow',
         'selenium',
         'diffusers',
         'controlnet_aux',
         'tiktoken',
         'espnet==202301',
         'espnet_model_zoo==0.1.7',
         'flask==2.2.3',
@@ -94,14 +93,16 @@
         'waitress==2.1.2',
         'asteroid',
         'speechbrain',
         'timm',
         'typeguard',
         'pytesseract',
         'huggingface_hub',
+        'fastapi_cache',
+        'fastapi-limiter',
     ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `swarms-0.8.0/swarms/agents/workers/metaprompt_worker.py` & `swarms-0.8.7/swarms/agents/workers/PromptWorker.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/GroundingDINO/setup.py` & `swarms-0.8.7/swarms/agents/workers/models/GroundingDINO/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/__init__.py` & `swarms-0.8.7/swarms/agents/workers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/models/segment_anything/setup.py` & `swarms-0.8.7/swarms/agents/workers/models/segment_anything/setup.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py` & `swarms-0.8.7/swarms/agents/workers/multi_modal_workers/multi_modal_agent.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py` & `swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py` & `swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py` & `swarms-0.8.7/swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/agents/workers/omni_worker.py` & `swarms-0.8.7/swarms/agents/workers/OmniWorkerAgent.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,23 +18,7 @@
 
         if not(api_key and api_type and api_endpoint):
             raise ValueError("Please provide api_key, api_type, and api_endpoint")
         
         response = chat_huggingface(messages, api_key, api_type, api_endpoint)
         return response
 
-
-
-# #usage
-# agent = OmniWorkerAgent(api_key="your key", api_endpoint="api endpoint", api_type="you types")
-
-# data = {
-#     "messages": "your_messages",
-#     "api_key": "your_api_key",
-#     "api_endpoint": "your_api_endpoint",
-#     "api_type": "your_api_type"
-# }
-
-# response = agent.chat(data)
-
-
-# print(response)  # Prints the response
```

### Comparing `swarms-0.8.0/swarms/agents/workers/visual_worker.py` & `swarms-0.8.7/swarms/agents/workers/MultiModalVisualAgentTool.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/prompts/prompts.py` & `swarms-0.8.7/swarms/agents/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `swarms-0.8.0/swarms/tools/agent_tools.py` & `swarms-0.8.7/swarms/agents/tools/agent_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.tools import BaseTool, DuckDuckGoSearchRun
 from langchain.tools.file_management.read import ReadFileTool
 
 from langchain.tools.file_management.write import WriteFileTool
 from langchain.tools.human.tool import HumanInputRun
-from swarms.tools.main import process_csv, WebpageQATool
+from swarms.agents.tools.main import process_csv, WebpageQATool
 
 from langchain.experimental.autonomous_agents.autogpt.agent import AutoGPT
 from langchain.chat_models import ChatOpenAI
 from langchain.tools import tool
 
 # ---------- Constants ----------
 ROOT_DIR = "./data/"
```

### Comparing `swarms-0.8.0/swarms/tools/main.py` & `swarms-0.8.7/swarms/agents/tools/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 
 import os
 import subprocess
 import time
 from datetime import datetime
 from typing import Dict, List
 
-from swarms.utils.utils import ANSI, Color, Style # test
+from swarms.utils.main import ANSI, Color, Style # test
 
 class Terminal(BaseToolSet):
     def __init__(self):
         self.sessions: Dict[str, List[SyscallTracer]] = {}
 
     @tool(
         name="Terminal",
@@ -1096,15 +1096,15 @@
     BlipForQuestionAnswering,
     BlipProcessor,
     CLIPSegForImageSegmentation,
     CLIPSegProcessor,
 )
 
 
-from swarms.utils.utils import get_new_image_name
+from swarms.utils.main import get_new_image_name
 
 
 class MaskFormer(BaseToolSet):
     def __init__(self, device):
         print("Initializing MaskFormer to %s" % device)
         self.device = device
         self.processor = CLIPSegProcessor.from_pretrained("CIDAS/clipseg-rd64-refined")
@@ -1296,14 +1296,64 @@
         logger.debug(
             f"\nProcessed VisualQuestionAnswering, Input Image: {image_path}, Input Question: {question}, "
             f"Output Answer: {answer}"
         )
 
         return answer
     
+
+#========================> handlers/image
+import torch
+from PIL import Image
+from transformers import BlipForConditionalGeneration, BlipProcessor
+
+# from core.prompts.file import IMAGE_PROMPT
+from swarms.prompts.prompts import IMAGE_PROMPT
+
+from swarms.utils.main import BaseHandler
+
+class ImageCaptioning(BaseHandler):
+    def __init__(self, device):
+        print("Initializing ImageCaptioning to %s" % device)
+        self.device = device
+        self.torch_dtype = torch.float16 if "cuda" in device else torch.float32
+        self.processor = BlipProcessor.from_pretrained(
+            "Salesforce/blip-image-captioning-base"
+        )
+        self.model = BlipForConditionalGeneration.from_pretrained(
+            "Salesforce/blip-image-captioning-base", torch_dtype=self.torch_dtype
+        ).to(self.device)
+
+    def handle(self, filename: str):
+        img = Image.open(filename)
+        width, height = img.size
+        ratio = min(512 / width, 512 / height)
+        width_new, height_new = (round(width * ratio), round(height * ratio))
+        img = img.resize((width_new, height_new))
+        img = img.convert("RGB")
+        img.save(filename, "PNG")
+        print(f"Resize image form {width}x{height} to {width_new}x{height_new}")
+
+        inputs = self.processor(Image.open(filename), return_tensors="pt").to(
+            self.device, self.torch_dtype
+        )
+        out = self.model.generate(**inputs)
+        description = self.processor.decode(out[0], skip_special_tokens=True)
+        print(
+            f"\nProcessed ImageCaptioning, Input Image: {filename}, Output Text: {description}"
+        )
+
+        return IMAGE_PROMPT.format(filename=filename, description=description)
+    
+
+
+
+
+
+
 #segment anything:
 
 ########################### MODELS
 
 
 # #########==========================> 
 # from selenium import webdriver
@@ -1448,26 +1498,26 @@
     try:
         yield
     finally:
         os.chdir(prev_dir)
 
 @tool
 def process_csv(
-    csv_file_path: str, instructions: str, output_path: Optional[str] = None
+    llm, csv_file_path: str, instructions: str, output_path: Optional[str] = None
 ) -> str:
     """Process a CSV by with pandas in a limited REPL.\
  Only use this after writing data to disk as a csv file.\
  Any figures must be saved to disk to be viewed by the human.\
  Instructions should be written in natural language, not code. Assume the dataframe is already loaded."""
     with pushd(ROOT_DIR):
         try:
             df = pd.read_csv(csv_file_path)
         except Exception as e:
             return f"Error: {e}"
-        agent = create_pandas_dataframe_agent(llm, df, max_iterations=30, verbose=True)
+        agent = create_pandas_dataframe_agent(llm, df, max_iterations=30, verbose=False)
         if output_path is not None:
             instructions += f" Save output to disk at {output_path}"
         try:
             result = agent.run(instructions)
             return result
         except Exception as e:
             return f"Error: {e}"
```

### Comparing `swarms-0.8.0/swarms/utils/llm.py` & `swarms-0.8.7/swarms/agents/models/llm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,77 @@
 from typing import Optional
 import os
 import logging
 
-from langchain import PromptTemplate, HuggingFaceHub, ChatOpenAI, LLMChain
+from langchain import PromptTemplate, LLMChain, HuggingFaceHub
+from langchain.chat_models import ChatOpenAI
 
-# Configure logging
+
+# Configure logging-
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
+
 class LLM:
     def __init__(self,
                  openai_api_key: Optional[str] = None,
                  hf_repo_id: Optional[str] = None,
                  hf_api_token: Optional[str] = None,
-                 model_kwargs: Optional[dict] = None):
+                 temperature: Optional[float] = 0.5,
+                 max_length: Optional[int] = 64):
 
         # Check if keys are in the environment variables
         openai_api_key = openai_api_key or os.getenv('OPENAI_API_KEY')
         hf_api_token = hf_api_token or os.getenv('HUGGINGFACEHUB_API_TOKEN')
 
         self.openai_api_key = openai_api_key
         self.hf_repo_id = hf_repo_id
         self.hf_api_token = hf_api_token
-        self.model_kwargs = model_kwargs if model_kwargs else {}
+        self.temperature = temperature
+        self.max_length = max_length
 
         # If the HuggingFace API token is provided, set it in environment variables
         if self.hf_api_token:
             os.environ["HUGGINGFACEHUB_API_TOKEN"] = self.hf_api_token
 
-        # Create the LLM object based on the provided keys
+        # Initialize the LLM object
+        self.initialize_llm()
+
+    def initialize_llm(self):
+        model_kwargs = {"temperature": self.temperature, "max_length": self.max_length}
         try:
             if self.hf_repo_id and self.hf_api_token:
-                self.llm = HuggingFaceHub(repo_id=self.hf_repo_id, model_kwargs=self.model_kwargs)
+                self.llm = HuggingFaceHub(repo_id=self.hf_repo_id, model_kwargs=model_kwargs)
             elif self.openai_api_key:
-                self.llm = ChatOpenAI(api_key=self.openai_api_key, model_kwargs=self.model_kwargs)
+                self.llm = ChatOpenAI(api_key=self.openai_api_key, model_kwargs=model_kwargs)
             else:
                 raise ValueError("Please provide either OpenAI API key or both HuggingFace repository ID and API token.")
         except Exception as e:
             logger.error("Failed to initialize LLM: %s", e)
             raise
         
     def run(self, prompt: str) -> str:
         template = """Question: {question}
         Answer: Let's think step by step."""
-        
         try:
             prompt_template = PromptTemplate(template=template, input_variables=["question"])
             llm_chain = LLMChain(prompt=prompt_template, llm=self.llm)
             return llm_chain.run({"question": prompt})
         except Exception as e:
             logger.error("Failed to generate response: %s", e)
             raise
 
-# example
-llm_instance = LLM(openai_api_key="your_openai_key")
-result = llm_instance.run("Who won the FIFA World Cup in 1998?")
-print(result)
-
-# using HuggingFaceHub
-llm_instance = LLM(hf_repo_id="google/flan-t5-xl", hf_api_token="your_hf_api_token")
-result = llm_instance.run("Who won the FIFA World Cup in 1998?")
-print(result)
+# # example
+# from swarms.utils.llm import LLM
+# llm_instance = LLM(openai_api_key="your_openai_key")
+# result = llm_instance.run("Who won the FIFA World Cup in 1998?")
+# print(result)
+
+# # using HuggingFaceHub
+# llm_instance = LLM(hf_repo_id="google/flan-t5-xl", hf_api_token="your_hf_api_token")
+# result = llm_instance.run("Who won the FIFA World Cup in 1998?")
+# print(result)
+
+
+# make super easy to chaneg parameters, in class, use cpu and 
+#add qlora, 8bit inference
+# look into adding deepspeed
```

### Comparing `swarms-0.8.0/swarms/utils/utils.py` & `swarms-0.8.7/swarms/utils/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     def from_settings() -> "AbstractUploader":
         pass
 
 #================================> upload end
 
 
 #========================= upload s3
-import os
+
 
 import boto3
 
 
 class S3Uploader(AbstractUploader):
     def __init__(self, accessKey: str, secretKey: str, region: str, bucket: str):
         self.accessKey = accessKey
@@ -258,28 +258,30 @@
         object_name = os.path.basename(filepath)
         self.client.upload_file(filepath, self.bucket, object_name)
         return self.get_url(object_name)
 
 #========================= upload s3
 
 #========================> upload/static
-import os
 import shutil
 from pathlib import Path
 
 
 class StaticUploader(AbstractUploader):
     def __init__(self, server: str, path: Path, endpoint: str):
         self.server = server
         self.path = path
         self.endpoint = endpoint
 
     @staticmethod
     def from_settings(path: Path, endpoint: str) -> "StaticUploader":
-        return StaticUploader(os.environ["SERVER"], path, endpoint)
+        server = os.environ.get("SERVER", "http://localhost:8000")
+        return StaticUploader(server, path, endpoint)
+
+
 
     def get_url(self, uploaded_path: str) -> str:
         return f"{self.server}/{uploaded_path}"
 
     def upload(self, filepath: str):
         relative_path = Path("generated") / filepath.split("/")[-1]
         file_path = self.path / relative_path
@@ -287,19 +289,17 @@
         shutil.copy(filepath, file_path)
         endpoint_path = self.endpoint / relative_path
         return f"{self.server}/{endpoint_path}"
     
 
 
 #========================> handlers/base
-import os
-import shutil
+
 import uuid
 from enum import Enum
-from pathlib import Path
 from typing import Dict
 
 import requests
 
 # from env import settings
 
 
@@ -366,51 +366,47 @@
         with open(local_filename, "wb") as f:
             size = f.write(data)
         print(f"Inputs: {url} ({size//1000}MB)  => {local_filename}")
         return local_filename
 
     def handle(self, url: str) -> str:
         try:
-            if url.startswith(settings["SERVER"]):
-                local_filepath = url[len(settings["SERVER"]) + 1 :]
+            if url.startswith(os.environ.get("SERVER", "http://localhost:8000")):
+                local_filepath = url[len(os.environ.get("SERVER", "http://localhost:8000")) + 1 :]
                 local_filename = Path("file") / local_filepath.split("/")[-1]
                 src = self.path / local_filepath
-                dst = self.path / settings["PLAYGROUND_DIR"] / local_filename
+                dst = self.path / os.environ.get("PLAYGROUND_DIR", "./playground") / local_filename
                 os.makedirs(os.path.dirname(dst), exist_ok=True)
                 shutil.copy(src, dst)
             else:
                 local_filename = self.download(url)
-
-            try:
-                handler = self.handlers[FileType.from_url(url)]
-            except KeyError:
+            handler = self.handlers.get(FileType.from_url(url))
+            if handler is None:
                 if FileType.from_url(url) == FileType.IMAGE:
                     raise Exception(
                         f"No handler for {FileType.from_url(url)}. "
                         f"Please set USE_GPU to True in env/settings.py"
                     )
                 else:
                     raise Exception(f"No handler for {FileType.from_url(url)}")
-            handler.handle(local_filename)
+            return handler.handle(local_filename)
         except Exception as e:
             raise e
-        
 ########################### =>  base end
 
 
 
 
 
 
 #############===========================>
-import pandas as pd
 
 from swarms.prompts.prompts import DATAFRAME_PROMPT
 
-
+import pandas as pd
 class CsvToDataframe(BaseHandler):
     def handle(self, filename: str):
         df = pd.read_csv(filename)
         description = (
             f"Dataframe with {len(df)} rows and {len(df.columns)} columns. "
             "Columns are: "
             f"{', '.join(df.columns)}"
@@ -421,81 +417,7 @@
         )
 
         return DATAFRAME_PROMPT.format(filename=filename, description=description)
 
 
 
 
-
-#========================> handlers/image
-import torch
-from PIL import Image
-from transformers import BlipForConditionalGeneration, BlipProcessor
-
-# from core.prompts.file import IMAGE_PROMPT
-from swarms.prompts.prompts import IMAGE_PROMPT
-
-
-
-class ImageCaptioning(BaseHandler):
-    def __init__(self, device):
-        print("Initializing ImageCaptioning to %s" % device)
-        self.device = device
-        self.torch_dtype = torch.float16 if "cuda" in device else torch.float32
-        self.processor = BlipProcessor.from_pretrained(
-            "Salesforce/blip-image-captioning-base"
-        )
-        self.model = BlipForConditionalGeneration.from_pretrained(
-            "Salesforce/blip-image-captioning-base", torch_dtype=self.torch_dtype
-        ).to(self.device)
-
-    def handle(self, filename: str):
-        img = Image.open(filename)
-        width, height = img.size
-        ratio = min(512 / width, 512 / height)
-        width_new, height_new = (round(width * ratio), round(height * ratio))
-        img = img.resize((width_new, height_new))
-        img = img.convert("RGB")
-        img.save(filename, "PNG")
-        print(f"Resize image form {width}x{height} to {width_new}x{height_new}")
-
-        inputs = self.processor(Image.open(filename), return_tensors="pt").to(
-            self.device, self.torch_dtype
-        )
-        out = self.model.generate(**inputs)
-        description = self.processor.decode(out[0], skip_special_tokens=True)
-        print(
-            f"\nProcessed ImageCaptioning, Input Image: {filename}, Output Text: {description}"
-        )
-
-        return IMAGE_PROMPT.format(filename=filename, description=description)
-    
-
-
-
-# from autogpt.agent import Agent
-# from swarms.agents.swarms import worker_node
-
-# class MultiAgent(worker_node):
-
-#     def __init__(
-#             self,
-#             ai_name,
-#             memory,
-#             full_message_history,
-#             prompt,
-#             user_input,
-#             agent_id
-#     ):
-#         super().__init__(
-#             ai_name=ai_name,
-#             memory=memory,
-#             full_message_history=full_message_history,
-#             next_action_count=0,
-#             prompt=prompt,
-#             user_input=user_input,
-#         )
-#         self.agent_id = agent_id
-#         self.auditory_buffer = []  # contains the non processed parts of the conversation
-
-#     def receive_message(self, speaker, message):
-#         self.auditory_buffer.append((speaker.ai_name, message))
```

### Comparing `swarms-0.8.0/swarms.egg-info/PKG-INFO` & `swarms-0.8.7/swarms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swarms
-Version: 0.8.0
+Version: 0.8.7
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/swarms
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `swarms-0.8.0/swarms.egg-info/SOURCES.txt` & `swarms-0.8.7/swarms.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,54 @@
 LICENSE
 README.md
 setup.py
 api/__init__.py
-api/container.py
-api/main.py
-api/worker.py
+api/app.py
 swarms/__init__.py
+swarms/hivemind.py
 swarms/swarms.py
 swarms.egg-info/PKG-INFO
 swarms.egg-info/SOURCES.txt
 swarms.egg-info/dependency_links.txt
 swarms.egg-info/requires.txt
 swarms.egg-info/top_level.txt
 swarms/agents/__init__.py
+swarms/agents/boss/BossNode.py
 swarms/agents/boss/__init__.py
-swarms/agents/boss/babyagi_agent.py
-swarms/agents/boss/boss_agent.py
+swarms/agents/memory/__init__.py
+swarms/agents/memory/base.py
+swarms/agents/memory/chroma.py
+swarms/agents/models/__init__.py
+swarms/agents/models/llm.py
+swarms/agents/prompts/__init__.py
+swarms/agents/prompts/prompts.py
+swarms/agents/tools/__init__.py
+swarms/agents/tools/agent_tools.py
+swarms/agents/tools/base.py
+swarms/agents/tools/main.py
+swarms/agents/tools/core/__init__.py
+swarms/agents/tools/core/code_interpreter/__init__.py
+swarms/agents/tools/core/code_interpreter/main.py
+swarms/agents/utils/Agent.py
+swarms/agents/utils/Calback.py
+swarms/agents/utils/ChatOpenAI.py
+swarms/agents/utils/ConversationalChatAgent.py
+swarms/agents/utils/__init__.py
+swarms/agents/utils/agent_creator.py
+swarms/agents/utils/agent_setup.py
+swarms/agents/utils/output_parser.py
+swarms/agents/utils/prompts.py
+swarms/agents/workers/MultiModalVisualAgentTool.py
+swarms/agents/workers/OmniWorkerAgent.py
+swarms/agents/workers/PromptWorker.py
+swarms/agents/workers/WorkerNode.py
 swarms/agents/workers/__init__.py
-swarms/agents/workers/agents.py
-swarms/agents/workers/auto_worker.py
-swarms/agents/workers/metaprompt_worker.py
-swarms/agents/workers/omni_worker.py
-swarms/agents/workers/visual_worker.py
-swarms/agents/workers/worker_agent.py
+swarms/agents/workers/generative_worker.py
+swarms/agents/workers/worker_agent_ultra.py
+swarms/agents/workers/worker_ultra_node.py
 swarms/agents/workers/models/__init__.py
 swarms/agents/workers/models/GroundingDINO/__init__.py
 swarms/agents/workers/models/GroundingDINO/setup.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/__init__.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinB_cfg.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py
 swarms/agents/workers/models/GroundingDINO/groundingdino/config/__init__.py
@@ -78,16 +100,16 @@
 swarms/agents/workers/models/segment_anything/segment_anything/utils/transforms.py
 swarms/agents/workers/multi_modal_workers/__init__.py
 swarms/agents/workers/multi_modal_workers/multi_modal_agent.py
 swarms/agents/workers/multi_modal_workers/omni_agent/__init__.py
 swarms/agents/workers/multi_modal_workers/omni_agent/get_token_ids.py
 swarms/agents/workers/multi_modal_workers/omni_agent/model_server.py
 swarms/agents/workers/multi_modal_workers/omni_agent/omni_chat.py
-swarms/prompts/__init__.py
-swarms/prompts/prompts.py
-swarms/tools/__init__.py
-swarms/tools/agent_tools.py
-swarms/tools/main.py
 swarms/utils/__init__.py
-swarms/utils/llm.py
 swarms/utils/logger.py
-swarms/utils/utils.py
+swarms/utils/main.py
+swarms/utils/static.py
+swarms/utils/task.py
+swarms/utils/embeddings/__init__.py
+swarms/utils/embeddings/base.py
+swarms/utils/schema/__init__.py
+swarms/utils/schema/base.py
```

