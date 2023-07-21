# Comparing `tmp/hepai-1.0.8.1.tar.gz` & `tmp/hepai-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hepai-1.0.8.1.tar", last modified: Fri Apr 21 13:38:40 2023, max compression
+gzip compressed data, was "dist/hepai-1.0.9.tar", last modified: Fri Apr 21 13:39:19 2023, max compression
```

## Comparing `hepai-1.0.8.1.tar` & `hepai-1.0.9.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.0.8.1/MANIFEST.in
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4048 2023-04-21 13:38:40.000000 hepai-1.0.8.1/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3263 2023-04-21 13:21:07.000000 hepai-1.0.8.1/README.md
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1293 2023-04-21 07:42:34.000000 hepai-1.0.8.1/hai/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1938 2023-04-21 07:42:31.000000 hepai-1.0.8.1/hai/apis/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/basic/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-30 09:36:57.000000 hepai-1.0.8.1/hai/apis/basic/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/basic/argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/basic/base.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/basic/grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/basic/registry.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/basic/utils.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/hub/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.0.8.1/hai/apis/hub/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.0.8.1/hai/apis/hub/hubs.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/modules/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/modules/ResNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/modules/ResNet/ResNet.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/modules/ResNet/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/modules/UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/modules/UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.0.8.1/hai/apis/modules/UNet/argparse_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.0.8.1/hai/apis/modules/UNet/evaluate_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.0.8.1/hai/apis/modules/UNet/predict_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.0.8.1/hai/apis/modules/UNet/train_api.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/modules/UNet/unet_api.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/modules/YOLOv5/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/apis/modules/YOLOv5/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.0.8.1/hai/apis/modules/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/workers_api/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.0.8.1/hai/apis/workers_api/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/apis/workers_api/llm/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.0.8.1/hai/apis/workers_api/llm/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1415 2023-04-21 10:25:12.000000 hepai-1.0.8.1/hai/apis/workers_api/llm/llm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.0.8.1/hai/apis/workers_api/llm/tokenizer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      403 2023-04-21 07:47:44.000000 hepai-1.0.8.1/hai/apis/workers_api/model.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/configs/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/configs/Base/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.0.8.1/hai/configs/Base/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/configs/Base/hai_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/configs/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/configs/uaii_deepsort_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/configs/uaii_seyolov5_config.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/configs/uaii_stream_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/configs/urls/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.0.8.1/hai/configs/urls/datasets.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.0.8.1/hai/configs/urls/hub_models.json
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/configs/visible_loader_config.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.0.8.1/hai/modules/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/detection/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.0.8.1/hai/modules/detection/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.0.8.1/hai/modules/exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/exporter/images_exporter/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/modules/exporter/images_exporter/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.0.8.1/hai/modules/loader/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/loader/images_loader/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/modules/loader/images_loader/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.0.8.1/hai/modules/loader/images_loader/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.0.8.1/hai/modules/loader/images_loader/dataset_torch.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.0.8.1/hai/modules/loader/images_loader/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.0.8.1/hai/modules/model_hub.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/segmentation/
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/evaluate.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/hubconf.py
--rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/predict.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/train.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/unet/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.0.8.1/hai/modules/segmentation/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/testor/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.0.8.1/hai/testor/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/testor/test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/testor/test_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.0.8.1/hai/testor/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/actuator/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.0.8.1/hai/uaii/actuator/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.0.8.1/hai/uaii/actuator/trainer.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/cli/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.0.8.1/hai/uaii/cli/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3692 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/uaii/cli/cli_functions.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/uaii/cli/cli_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/datasets/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/datasets/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.0.8.1/hai/uaii/datasets/dataloader.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     8489 2023-04-21 12:07:18.000000 hepai-1.0.8.1/hai/uaii/datasets/dataset_utils.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/datasets/datasets.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.0.8.1/hai/uaii/datasets/datasets_hub.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.0.8.1/hai/uaii/datasets/uaii_loaders.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/registry/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.0.8.1/hai/uaii/registry/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.0.8.1/hai/uaii/registry/init_register.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.0.8.1/hai/uaii/registry/registy.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/registry/testor.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/registry/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/registry/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/registry/utils/general.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.0.8.1/hai/uaii/server/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/grpc/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/grpc/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/example/grpc-client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/example/grpc-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/example/hello_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/example/hello_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.0.8.1/hai/uaii/server/grpc/grpc_pb2.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.0.8.1/hai/uaii/server/grpc/grpc_pb2_grpc.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.0.8.1/hai/uaii/server/grpc/grpc_secure_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/uaii/server/grpc/grpc_secure_server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/grpc_xai_client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/grpc/grpc_xai_server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/commons.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/exception.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/files.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/listener.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/params.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos/timer.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/nacos-test.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/nacos/request_test.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/server/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.0.8.1/hai/uaii/server/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/socket/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/socket/__init__.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/socket/example/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/socket/example/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/socket/example/client.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/socket/example/server.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/socket/server.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/stream/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/stream/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/stream/base_input.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/uaii/stream/base_module.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/stream/base_output.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/stream/base_queue.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/stream/rabbit_qm.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.0.8.1/hai/uaii/stream/stream.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/stream/streams.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.0.8.1/hai/uaii/uaii_main.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hai/uaii/utils/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.8.1/hai/uaii/utils/__init__.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.0.8.1/hai/uaii/utils/arbitrary_import.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.0.8.1/hai/uaii/utils/base_uaii.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)    15272 2023-04-21 07:34:39.000000 hepai-1.0.8.1/hai/uaii/utils/config_loader.py
--rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.0.8.1/hai/uaii/utils/fake_argparse.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     3729 2022-09-29 09:48:36.000000 hepai-1.0.8.1/hai/uaii/utils/general.py
--rw-rw-r--   0 zzd       (1000) zzd       (1000)      341 2023-04-21 13:38:38.000000 hepai-1.0.8.1/hai/version.py
-drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4048 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/PKG-INFO
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4685 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/SOURCES.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/dependency_links.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/entry_points.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       43 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/requires.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2023-04-21 13:38:40.000000 hepai-1.0.8.1/hepai.egg-info/top_level.txt
--rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2023-04-21 13:38:40.000000 hepai-1.0.8.1/setup.cfg
--rw-rw-r--   0 zzd       (1000) zzd       (1000)     4815 2023-04-21 12:07:47.000000 hepai-1.0.8.1/setup.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      118 2022-10-28 08:51:38.000000 hepai-1.0.9/MANIFEST.in
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 13:39:19.000000 hepai-1.0.9/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3263 2023-04-21 13:21:07.000000 hepai-1.0.9/README.md
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1293 2023-04-21 07:42:34.000000 hepai-1.0.9/hai/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1938 2023-04-21 07:42:31.000000 hepai-1.0.9/hai/apis/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/basic/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-30 09:36:57.000000 hepai-1.0.9/hai/apis/basic/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       55 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/basic/argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      458 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/basic/base.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       54 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/basic/grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      122 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/basic/registry.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      141 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/basic/utils.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/hub/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-04 00:48:55.000000 hepai-1.0.9/hai/apis/hub/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      803 2022-10-08 09:52:47.000000 hepai-1.0.9/hai/apis/hub/hubs.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/modules/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/modules/ResNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1057 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/modules/ResNet/ResNet.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      415 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/modules/ResNet/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/modules/UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      637 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/modules/UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2478 2022-09-22 09:20:00.000000 hepai-1.0.9/hai/apis/modules/UNet/argparse_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-09-02 00:21:08.000000 hepai-1.0.9/hai/apis/modules/UNet/evaluate_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4730 2022-09-03 22:56:22.000000 hepai-1.0.9/hai/apis/modules/UNet/predict_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9139 2022-09-22 08:22:39.000000 hepai-1.0.9/hai/apis/modules/UNet/train_api.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3099 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/modules/UNet/unet_api.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/modules/YOLOv5/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      434 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/apis/modules/YOLOv5/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:54:43.000000 hepai-1.0.9/hai/apis/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/workers_api/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:36:18.000000 hepai-1.0.9/hai/apis/workers_api/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/apis/workers_api/llm/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2023-04-21 07:22:46.000000 hepai-1.0.9/hai/apis/workers_api/llm/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1415 2023-04-21 10:25:12.000000 hepai-1.0.9/hai/apis/workers_api/llm/llm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        3 2023-04-21 09:02:06.000000 hepai-1.0.9/hai/apis/workers_api/llm/tokenizer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      403 2023-04-21 07:47:44.000000 hepai-1.0.9/hai/apis/workers_api/model.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/configs/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/configs/Base/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:19:48.000000 hepai-1.0.9/hai/configs/Base/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      407 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/configs/Base/hai_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/configs/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      285 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/configs/uaii_deepsort_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2706 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/configs/uaii_seyolov5_config.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1476 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/configs/uaii_stream_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/configs/urls/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1752 2022-10-19 18:44:14.000000 hepai-1.0.9/hai/configs/urls/datasets.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      960 2022-10-19 20:40:27.000000 hepai-1.0.9/hai/configs/urls/hub_models.json
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      534 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/configs/visible_loader_config.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:42:32.000000 hepai-1.0.9/hai/modules/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/detection/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:41:52.000000 hepai-1.0.9/hai/modules/detection/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:29.000000 hepai-1.0.9/hai/modules/exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/exporter/images_exporter/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5282 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/modules/exporter/images_exporter/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:46:28.000000 hepai-1.0.9/hai/modules/loader/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/loader/images_loader/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1618 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/modules/loader/images_loader/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3346 2023-04-21 12:08:18.000000 hepai-1.0.9/hai/modules/loader/images_loader/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    14091 2022-10-18 10:33:57.000000 hepai-1.0.9/hai/modules/loader/images_loader/dataset_torch.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    26952 2022-10-18 11:10:17.000000 hepai-1.0.9/hai/modules/loader/images_loader/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1446 2022-10-18 17:35:03.000000 hepai-1.0.9/hai/modules/model_hub.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/segmentation/
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:56:25.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1573 2022-08-31 21:12:48.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/evaluate.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      842 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/hubconf.py
+-rwxrwxr-x   0 zzd       (1000) zzd       (1000)     3997 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/predict.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8621 2022-08-31 21:12:32.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/train.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/unet/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       29 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/unet/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1130 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2602 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2991 2022-10-08 08:56:24.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-30 18:18:45.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      533 2022-09-30 09:30:48.000000 hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:55:50.000000 hepai-1.0.9/hai/modules/segmentation/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/testor/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      166 2023-04-21 07:26:13.000000 hepai-1.0.9/hai/testor/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      189 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/testor/test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      281 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/testor/test_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      406 2023-04-21 07:26:41.000000 hepai-1.0.9/hai/testor/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       46 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/actuator/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       71 2022-12-07 09:16:51.000000 hepai-1.0.9/hai/uaii/actuator/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      430 2022-12-07 09:20:22.000000 hepai-1.0.9/hai/uaii/actuator/trainer.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/cli/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-10-08 08:00:08.000000 hepai-1.0.9/hai/uaii/cli/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3692 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/uaii/cli/cli_functions.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     9276 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/uaii/cli/cli_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/datasets/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       28 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/datasets/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3240 2023-04-21 12:05:26.000000 hepai-1.0.9/hai/uaii/datasets/dataloader.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     8489 2023-04-21 12:07:18.000000 hepai-1.0.9/hai/uaii/datasets/dataset_utils.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    40434 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/datasets/datasets.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4673 2022-10-19 18:52:31.000000 hepai-1.0.9/hai/uaii/datasets/datasets_hub.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 12:05:05.000000 hepai-1.0.9/hai/uaii/datasets/uaii_loaders.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/registry/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      374 2022-09-22 05:57:37.000000 hepai-1.0.9/hai/uaii/registry/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5669 2023-04-04 04:04:35.000000 hepai-1.0.9/hai/uaii/registry/init_register.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    11103 2022-09-22 03:26:47.000000 hepai-1.0.9/hai/uaii/registry/registy.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       81 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/registry/testor.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/registry/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/registry/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1619 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/registry/utils/general.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1893 2022-12-02 17:03:40.000000 hepai-1.0.9/hai/uaii/server/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/grpc/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/grpc/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      517 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/example/grpc-client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1353 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/example/grpc-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3163 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/example/hello_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2242 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/example/hello_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6022 2022-09-02 03:06:02.000000 hepai-1.0.9/hai/uaii/server/grpc/grpc_pb2.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3707 2022-10-18 10:41:24.000000 hepai-1.0.9/hai/uaii/server/grpc/grpc_pb2_grpc.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5517 2022-09-02 04:56:59.000000 hepai-1.0.9/hai/uaii/server/grpc/grpc_secure_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    10437 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/uaii/server/grpc/grpc_secure_server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     6172 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/grpc_xai_client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     5648 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/grpc/grpc_xai_server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      184 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    47889 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      752 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/commons.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       98 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/exception.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1645 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/files.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2403 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/listener.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      624 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/params.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4363 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos/timer.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1555 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/nacos-test.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2388 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/nacos/request_test.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/server/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      674 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2131 2022-09-02 03:01:13.000000 hepai-1.0.9/hai/uaii/server/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/socket/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/socket/__init__.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/socket/example/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/socket/example/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      730 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/socket/example/client.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      672 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/socket/example/server.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2153 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/socket/server.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/stream/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/stream/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     1411 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/stream/base_input.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     7745 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/uaii/stream/base_module.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     2575 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/stream/base_output.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      354 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/stream/base_queue.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/stream/rabbit_qm.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15802 2022-09-27 10:17:02.000000 hepai-1.0.9/hai/uaii/stream/stream.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4094 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/stream/streams.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    12294 2022-08-24 17:25:48.000000 hepai-1.0.9/hai/uaii/uaii_main.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hai/uaii/utils/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        0 2022-08-23 05:06:00.000000 hepai-1.0.9/hai/uaii/utils/__init__.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      921 2022-09-22 07:46:07.000000 hepai-1.0.9/hai/uaii/utils/arbitrary_import.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    17055 2023-04-21 12:06:51.000000 hepai-1.0.9/hai/uaii/utils/base_uaii.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)    15272 2023-04-21 07:34:39.000000 hepai-1.0.9/hai/uaii/utils/config_loader.py
+-rw-r--r--   0 zzd       (1000) zzd       (1000)     4472 2022-09-30 05:15:38.000000 hepai-1.0.9/hai/uaii/utils/fake_argparse.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     3729 2022-09-29 09:48:36.000000 hepai-1.0.9/hai/uaii/utils/general.py
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)      339 2023-04-21 13:39:17.000000 hepai-1.0.9/hai/version.py
+drwxrwxr-x   0 zzd       (1000) zzd       (1000)        0 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4046 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/PKG-INFO
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4685 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/SOURCES.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        1 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/dependency_links.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       50 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/entry_points.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       43 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/requires.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)        4 2023-04-21 13:39:19.000000 hepai-1.0.9/hepai.egg-info/top_level.txt
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)       38 2023-04-21 13:39:19.000000 hepai-1.0.9/setup.cfg
+-rw-rw-r--   0 zzd       (1000) zzd       (1000)     4815 2023-04-21 12:07:47.000000 hepai-1.0.9/setup.py
```

### Comparing `hepai-1.0.8.1/PKG-INFO` & `hepai-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
 Author-email: zdzhang@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.0.8.1 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.0.9 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
 zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `hepai-1.0.8.1/README.md` & `hepai-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/__init__.py` & `hepai-1.0.9/hai/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/__init__.py` & `hepai-1.0.9/hai/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/hub/hubs.py` & `hepai-1.0.9/hai/apis/hub/hubs.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/ResNet/ResNet.py` & `hepai-1.0.9/hai/apis/modules/ResNet/ResNet.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/UNet/__init__.py` & `hepai-1.0.9/hai/apis/modules/UNet/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/UNet/argparse_config.py` & `hepai-1.0.9/hai/apis/modules/UNet/argparse_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/UNet/evaluate_api.py` & `hepai-1.0.9/hai/apis/modules/UNet/evaluate_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/UNet/predict_api.py` & `hepai-1.0.9/hai/apis/modules/UNet/predict_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/UNet/train_api.py` & `hepai-1.0.9/hai/apis/modules/UNet/train_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/modules/UNet/unet_api.py` & `hepai-1.0.9/hai/apis/modules/UNet/unet_api.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/apis/workers_api/llm/llm.py` & `hepai-1.0.9/hai/apis/workers_api/llm/llm.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/configs/uaii_seyolov5_config.py` & `hepai-1.0.9/hai/configs/uaii_seyolov5_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/configs/uaii_stream_config.py` & `hepai-1.0.9/hai/configs/uaii_stream_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/configs/urls/datasets.json` & `hepai-1.0.9/hai/configs/urls/datasets.json`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/configs/urls/hub_models.json` & `hepai-1.0.9/hai/configs/urls/hub_models.json`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/configs/visible_loader_config.py` & `hepai-1.0.9/hai/configs/visible_loader_config.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/exporter/images_exporter/__init__.py` & `hepai-1.0.9/hai/modules/exporter/images_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/loader/images_loader/__init__.py` & `hepai-1.0.9/hai/modules/loader/images_loader/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/loader/images_loader/dataloader.py` & `hepai-1.0.9/hai/modules/loader/images_loader/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/loader/images_loader/dataset_torch.py` & `hepai-1.0.9/hai/modules/loader/images_loader/dataset_torch.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/loader/images_loader/datasets.py` & `hepai-1.0.9/hai/modules/loader/images_loader/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/model_hub.py` & `hepai-1.0.9/hai/modules/model_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/evaluate.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/evaluate.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/hubconf.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/hubconf.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/predict.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/predict.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/train.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/train.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/unet/unet_model.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/unet/unet_parts.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/data_loading.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/dice_score.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/modules/segmentation/Pytorch_UNet/utils/utils.py` & `hepai-1.0.9/hai/modules/segmentation/Pytorch_UNet/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/cli/cli_functions.py` & `hepai-1.0.9/hai/uaii/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/cli/cli_main.py` & `hepai-1.0.9/hai/uaii/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/datasets/dataloader.py` & `hepai-1.0.9/hai/uaii/datasets/dataloader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/datasets/dataset_utils.py` & `hepai-1.0.9/hai/uaii/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/datasets/datasets.py` & `hepai-1.0.9/hai/uaii/datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/datasets/datasets_hub.py` & `hepai-1.0.9/hai/uaii/datasets/datasets_hub.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/datasets/uaii_loaders.py` & `hepai-1.0.9/hai/uaii/datasets/uaii_loaders.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/registry/init_register.py` & `hepai-1.0.9/hai/uaii/registry/init_register.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/registry/registy.py` & `hepai-1.0.9/hai/uaii/registry/registy.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/registry/utils/general.py` & `hepai-1.0.9/hai/uaii/registry/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/__init__.py` & `hepai-1.0.9/hai/uaii/server/__init__.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/example/grpc-client.py` & `hepai-1.0.9/hai/uaii/server/grpc/example/grpc-client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/example/grpc-test.py` & `hepai-1.0.9/hai/uaii/server/grpc/example/grpc-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/example/hello_pb2.py` & `hepai-1.0.9/hai/uaii/server/grpc/example/hello_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/example/hello_pb2_grpc.py` & `hepai-1.0.9/hai/uaii/server/grpc/example/hello_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/grpc_pb2.py` & `hepai-1.0.9/hai/uaii/server/grpc/grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/grpc_pb2_grpc.py` & `hepai-1.0.9/hai/uaii/server/grpc/grpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/grpc_secure_client.py` & `hepai-1.0.9/hai/uaii/server/grpc/grpc_secure_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/grpc_secure_server.py` & `hepai-1.0.9/hai/uaii/server/grpc/grpc_secure_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/grpc_xai_client.py` & `hepai-1.0.9/hai/uaii/server/grpc/grpc_xai_client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/grpc/grpc_xai_server.py` & `hepai-1.0.9/hai/uaii/server/grpc/grpc_xai_server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos/client.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos/commons.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos/commons.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos/files.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos/files.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos/listener.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos/listener.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos/params.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos/params.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos/timer.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos/timer.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/nacos-test.py` & `hepai-1.0.9/hai/uaii/server/nacos/nacos-test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/nacos/request_test.py` & `hepai-1.0.9/hai/uaii/server/nacos/request_test.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/socket/example/client.py` & `hepai-1.0.9/hai/uaii/server/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/socket/example/server.py` & `hepai-1.0.9/hai/uaii/server/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/server/socket/server.py` & `hepai-1.0.9/hai/uaii/server/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/socket/example/client.py` & `hepai-1.0.9/hai/uaii/socket/example/client.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/socket/example/server.py` & `hepai-1.0.9/hai/uaii/socket/example/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/socket/server.py` & `hepai-1.0.9/hai/uaii/socket/server.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/stream/base_input.py` & `hepai-1.0.9/hai/uaii/stream/base_input.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/stream/base_module.py` & `hepai-1.0.9/hai/uaii/stream/base_module.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/stream/base_output.py` & `hepai-1.0.9/hai/uaii/stream/base_output.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/stream/stream.py` & `hepai-1.0.9/hai/uaii/stream/stream.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/stream/streams.py` & `hepai-1.0.9/hai/uaii/stream/streams.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/uaii_main.py` & `hepai-1.0.9/hai/uaii/uaii_main.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/utils/arbitrary_import.py` & `hepai-1.0.9/hai/uaii/utils/arbitrary_import.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/utils/base_uaii.py` & `hepai-1.0.9/hai/uaii/utils/base_uaii.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/utils/config_loader.py` & `hepai-1.0.9/hai/uaii/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/utils/fake_argparse.py` & `hepai-1.0.9/hai/uaii/utils/fake_argparse.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hai/uaii/utils/general.py` & `hepai-1.0.9/hai/uaii/utils/general.py`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/hepai.egg-info/PKG-INFO` & `hepai-1.0.9/hepai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hepai
-Version: 1.0.8.1
+Version: 1.0.9
 Summary: High energy phscis Artificial Intelligence plateform, HAI.
 Home-page: https://github.com/zhangzhengde0225/hai
 Author: Zhengde Zhang
 Author-email: zdzhang@163.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hepai Version: 1.0.8.1 Summary: High energy phscis
+Metadata-Version: 2.1 Name: hepai Version: 1.0.9 Summary: High energy phscis
 Artificial Intelligence plateform, HAI. Home-page: https://github.com/
 zhangzhengde0225/hai Author: Zhengde Zhang Author-email: zdzhang@163.com
 License: MIT Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `hepai-1.0.8.1/hepai.egg-info/SOURCES.txt` & `hepai-1.0.9/hepai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hepai-1.0.8.1/setup.py` & `hepai-1.0.9/setup.py`

 * *Files identical despite different names*

