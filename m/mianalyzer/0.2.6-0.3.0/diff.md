# Comparing `tmp/mianalyzer-0.2.6.tar.gz` & `tmp/mianalyzer-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mianalyzer-0.2.6.tar", last modified: Thu Oct 13 14:53:26 2022, max compression
+gzip compressed data, was "mianalyzer-0.3.0.tar", last modified: Fri Jul 21 11:58:36 2023, max compression
```

## Comparing `mianalyzer-0.2.6.tar` & `mianalyzer-0.3.0.tar`

### file list

```diff
@@ -1,226 +1,248 @@
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.258442 mianalyzer-0.2.6/
--rw-rw-rw-   0        0        0    35149 2021-12-20 09:08:37.000000 mianalyzer-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      682 2022-10-13 14:53:26.258442 mianalyzer-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1878 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.111325 mianalyzer-0.2.6/mia/
--rw-rw-rw-   0        0        0      149 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/__init__.py
--rw-rw-rw-   0        0        0       62 2022-10-13 14:53:07.000000 mianalyzer-0.2.6/mia/__version__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.111325 mianalyzer-0.2.6/mia/dl/
--rw-rw-rw-   0        0        0    11454 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/dl/DeepLearning.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.111325 mianalyzer-0.2.6/mia/dl/data/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/data/__init__.py
--rw-rw-rw-   0        0        0    11571 2022-05-24 10:06:51.000000 mianalyzer-0.2.6/mia/dl/data/imagedata.py
--rw-rw-rw-   0        0        0     5105 2022-05-24 10:06:51.000000 mianalyzer-0.2.6/mia/dl/data/labels.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.111325 mianalyzer-0.2.6/mia/dl/loss/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/loss/__init__.py
--rw-rw-rw-   0        0        0     1898 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/loss/classification_losses.py
--rw-rw-rw-   0        0        0     6053 2022-02-01 16:19:20.000000 mianalyzer-0.2.6/mia/dl/loss/loss_functions.py
--rw-rw-rw-   0        0        0      688 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/loss/losses.py
--rw-rw-rw-   0        0        0     1032 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/loss/regression_losses.py
--rw-rw-rw-   0        0        0     2712 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/loss/segmentation_losses.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.111325 mianalyzer-0.2.6/mia/dl/machine_learning/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/__init__.py
--rw-rw-rw-   0        0        0     8186 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/machine_learning/deploy.prototxt
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.126963 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/__init__.py
--rw-rw-rw-   0        0        0     3650 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/classifiers.py
--rw-rw-rw-   0        0        0     1308 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/dextr.py
--rw-rw-rw-   0        0        0     2275 2021-12-20 14:14:09.000000 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/dextr_segmentation.py
--rw-rw-rw-   0        0        0    10541 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/helpers.py
--rw-rw-rw-   0        0        0     7363 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/dextr/resnet.py
--rw-rw-rw-   0        0        0      975 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/machine_learning/grabcut_segmentation.py
--rw-rw-rw-   0        0        0     2632 2021-12-20 15:55:01.000000 mianalyzer-0.2.6/mia/dl/machine_learning/hed.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.126963 mianalyzer-0.2.6/mia/dl/method/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/method/__init__.py
--rw-rw-rw-   0        0        0     6698 2022-05-24 10:06:51.000000 mianalyzer-0.2.6/mia/dl/method/classification.py
--rw-rw-rw-   0        0        0     3344 2021-11-26 09:23:09.000000 mianalyzer-0.2.6/mia/dl/method/mode.py
--rw-rw-rw-   0        0        0     5621 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/dl/method/objectcounting.py
--rw-rw-rw-   0        0        0    10483 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/dl/method/pixelbasedprediction.py
--rw-rw-rw-   0        0        0     3795 2021-11-26 09:23:09.000000 mianalyzer-0.2.6/mia/dl/method/segmentation.py
--rw-rw-rw-   0        0        0     1149 2021-11-26 09:23:09.000000 mianalyzer-0.2.6/mia/dl/method/undefinedmode.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.126963 mianalyzer-0.2.6/mia/dl/metric/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/metric/__init__.py
--rw-rw-rw-   0        0        0     1155 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/metric/classification_metrics.py
--rw-rw-rw-   0        0        0     5288 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/metric/metric_functions.py
--rw-rw-rw-   0        0        0      756 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/metric/metrics.py
--rw-rw-rw-   0        0        0     1094 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/metric/regression_metrics.py
--rw-rw-rw-   0        0        0     2313 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/metric/segmentation_metrics.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.126963 mianalyzer-0.2.6/mia/dl/models/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.142584 mianalyzer-0.2.6/mia/dl/models/classification_models/
--rw-rw-rw-   0        0        0      508 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/__init__.py
--rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/__version__.py
--rw-rw-rw-   0        0        0    12132 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/classification_models.py
--rw-rw-rw-   0        0        0      347 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/keras.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.142584 mianalyzer-0.2.6/mia/dl/models/classification_models/models/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/models/__init__.py
--rw-rw-rw-   0        0        0     4470 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/models/_common_blocks.py
--rw-rw-rw-   0        0        0    13989 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/models/resnet.py
--rw-rw-rw-   0        0        0    10009 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/models/resnext.py
--rw-rw-rw-   0        0        0    15389 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/models/senet.py
--rw-rw-rw-   0        0        0     3417 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/models_factory.py
--rw-rw-rw-   0        0        0      381 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/tfkeras.py
--rw-rw-rw-   0        0        0     1279 2021-12-20 15:29:13.000000 mianalyzer-0.2.6/mia/dl/models/classification_models/weights.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.142584 mianalyzer-0.2.6/mia/dl/models/deeplab/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/deeplab/__init__.py
--rw-rw-rw-   0        0        0    22058 2022-01-31 10:47:17.000000 mianalyzer-0.2.6/mia/dl/models/deeplab/deeplab.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.158206 mianalyzer-0.2.6/mia/dl/models/efficientnet/
--rw-rw-rw-   0        0        0     2769 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/efficientnet/__init__.py
--rw-rw-rw-   0        0        0      772 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/efficientnet/__version__.py
--rw-rw-rw-   0        0        0      708 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/efficientnet/keras.py
--rw-rw-rw-   0        0        0    23520 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/efficientnet/model.py
--rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/efficientnet/preprocessing.py
--rw-rw-rw-   0        0        0      732 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/efficientnet/tfkeras.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.158206 mianalyzer-0.2.6/mia/dl/models/keras_applications/
--rw-rw-rw-   0        0        0     2059 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/__init__.py
--rw-rw-rw-   0        0        0    10731 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/densenet.py
--rw-rw-rw-   0        0        0    12855 2021-12-20 15:53:29.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/imagenet_utils.py
--rw-rw-rw-   0        0        0    14086 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/inception_resnet_v2.py
--rw-rw-rw-   0        0        0    13814 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/inception_v3.py
--rw-rw-rw-   0        0        0    18056 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/mobilenet.py
--rw-rw-rw-   0        0        0    19723 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/mobilenet_v2.py
--rw-rw-rw-   0        0        0    28646 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/nasnet.py
--rw-rw-rw-   0        0        0     1041 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet.py
--rw-rw-rw-   0        0        0    11888 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet50.py
--rw-rw-rw-   0        0        0    20729 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet_common.py
--rw-rw-rw-   0        0        0     1051 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet_v2.py
--rw-rw-rw-   0        0        0     1020 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/resnext.py
--rw-rw-rw-   0        0        0     7706 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/vgg16.py
--rw-rw-rw-   0        0        0     8178 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/vgg19.py
--rw-rw-rw-   0        0        0    12771 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/keras_applications/xception.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.173827 mianalyzer-0.2.6/mia/dl/models/segmentation_models/
--rw-rw-rw-   0        0        0     4162 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/__init__.py
--rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/__version__.py
--rw-rw-rw-   0        0        0     8428 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/_losses.py
--rw-rw-rw-   0        0        0     8812 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/_metrics.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.173827 mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/__init__.py
--rw-rw-rw-   0        0        0     5302 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/backbones_factory.py
--rw-rw-rw-   0        0        0    14288 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py
--rw-rw-rw-   0        0        0    13856 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/inception_v3.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.173827 mianalyzer-0.2.6/mia/dl/models/segmentation_models/base/
--rw-rw-rw-   0        0        0       71 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/base/__init__.py
--rw-rw-rw-   0        0        0    11669 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/base/functional.py
--rw-rw-rw-   0        0        0     2687 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/base/objects.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.173827 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/__init__.py
--rw-rw-rw-   0        0        0     2143 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/_common_blocks.py
--rw-rw-rw-   0        0        0      377 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/_utils.py
--rw-rw-rw-   0        0        0     9035 2022-01-31 10:47:17.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/fpn.py
--rw-rw-rw-   0        0        0     9703 2022-01-31 10:47:17.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/linknet.py
--rw-rw-rw-   0        0        0     8440 2022-01-31 10:47:17.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/pspnet.py
--rw-rw-rw-   0        0        0     8355 2022-01-31 10:47:17.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/unet.py
--rw-rw-rw-   0        0        0     3012 2021-12-20 08:40:49.000000 mianalyzer-0.2.6/mia/dl/models/segmentation_models/utils.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.173827 mianalyzer-0.2.6/mia/dl/optimizer/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/optimizer/__init__.py
--rw-rw-rw-   0        0        0     1693 2021-11-26 09:23:09.000000 mianalyzer-0.2.6/mia/dl/optimizer/optimizer.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.189448 mianalyzer-0.2.6/mia/dl/training/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/training/__init__.py
--rw-rw-rw-   0        0        0    11693 2021-11-26 09:23:09.000000 mianalyzer-0.2.6/mia/dl/training/augment.py
--rw-rw-rw-   0        0        0     6317 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/dl/training/datagenerator.py
--rw-rw-rw-   0        0        0     1664 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/training/lrschedule.py
--rw-rw-rw-   0        0        0     2929 2022-02-01 15:15:32.000000 mianalyzer-0.2.6/mia/dl/training/training_record.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.189448 mianalyzer-0.2.6/mia/dl/utils/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/dl/utils/__init__.py
--rw-rw-rw-   0        0        0    21488 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/dl/utils/dl_downloads.py
--rw-rw-rw-   0        0        0     6657 2022-05-24 10:06:51.000000 mianalyzer-0.2.6/mia/dl/utils/dl_utils.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.211574 mianalyzer-0.2.6/mia/icons/
--rw-rw-rw-   0        0        0     1282 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/addobject.png
--rw-rw-rw-   0        0        0     3070 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/assign.png
--rw-rw-rw-   0        0        0     1554 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/assignclass.png
--rw-rw-rw-   0        0        0     2432 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/augmentation.png
--rw-rw-rw-   0        0        0     2436 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/clear.png
--rw-rw-rw-   0        0        0     2144 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/delete.png
--rw-rw-rw-   0        0        0     3607 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/dextr.png
--rw-rw-rw-   0        0        0     2444 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/drag.png
--rw-rw-rw-   0        0        0     2215 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/draw.png
--rw-rw-rw-   0        0        0     1233 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/expand.png
--rw-rw-rw-   0        0        0     3697 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/exportallmasks.png
--rw-rw-rw-   0        0        0     5231 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/exportmask.png
--rw-rw-rw-   0        0        0     1445 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/load.png
--rw-rw-rw-   0        0        0    52773 2022-01-17 10:13:34.000000 mianalyzer-0.2.6/mia/icons/loading.png
--rw-rw-rw-   0        0        0     1676 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/loadmodel.png
--rw-rw-rw-   0        0        0    23516 2022-01-17 10:33:29.000000 mianalyzer-0.2.6/mia/icons/logo.png
--rw-rw-rw-   0        0        0     1951 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/magicwand.png
--rw-rw-rw-   0        0        0     3934 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/measure.png
--rw-rw-rw-   0        0        0     2879 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/next.png
--rw-rw-rw-   0        0        0     2797 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/objectcolor.png
--rw-rw-rw-   0        0        0     2012 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/objectnumber.png
--rw-rw-rw-   0        0        0     4019 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/poly.png
--rw-rw-rw-   0        0        0     3365 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/postprocessing.png
--rw-rw-rw-   0        0        0     7403 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/predict.png
--rw-rw-rw-   0        0        0     4157 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/predictall.png
--rw-rw-rw-   0        0        0     2975 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/previous.png
--rw-rw-rw-   0        0        0     4149 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/reset.png
--rw-rw-rw-   0        0        0     2703 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/results.png
--rw-rw-rw-   0        0        0     2682 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/saveall.png
--rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/savemodel.png
--rw-rw-rw-   0        0        0     2502 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/setclass.png
--rw-rw-rw-   0        0        0     4695 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/settings.png
--rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/shift.png
--rw-rw-rw-   0        0        0     3505 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/tracking.png
--rw-rw-rw-   0        0        0     7888 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/icons/train.png
--rw-rw-rw-   0        0        0    45066 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/mia_gui.py
--rw-rw-rw-   0        0        0      802 2022-10-13 14:15:39.000000 mianalyzer-0.2.6/mia/startup.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.227199 mianalyzer-0.2.6/mia/ui/
--rw-rw-rw-   0        0        0    25386 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/ui/Tools.py
--rw-rw-rw-   0        0        0    28487 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/ui/UI.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.227199 mianalyzer-0.2.6/mia/ui/classification/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/classification/__init__.py
--rw-rw-rw-   0        0        0     1878 2022-02-01 14:06:24.000000 mianalyzer-0.2.6/mia/ui/classification/ui_ClassResults.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.227199 mianalyzer-0.2.6/mia/ui/objectdetection/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/objectdetection/__init__.py
--rw-rw-rw-   0        0        0     1558 2022-02-01 14:06:24.000000 mianalyzer-0.2.6/mia/ui/objectdetection/ui_ODPostProcessing.py
--rw-rw-rw-   0        0        0     4816 2022-02-18 13:59:46.000000 mianalyzer-0.2.6/mia/ui/objectdetection/ui_ODResults.py
--rw-rw-rw-   0        0        0     4995 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/ui/objectdetection/ui_ODSettings.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.242820 mianalyzer-0.2.6/mia/ui/painter/
--rw-rw-rw-   0        0        0     7759 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/ui/painter/ContourPainter.py
--rw-rw-rw-   0        0        0     3687 2022-05-24 10:06:51.000000 mianalyzer-0.2.6/mia/ui/painter/ImageLabelPainter.py
--rw-rw-rw-   0        0        0      490 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/painter/NoPainter.py
--rw-rw-rw-   0        0        0     6900 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/ui/painter/ObjectPainter.py
--rw-rw-rw-   0        0        0    11928 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/ui/painter/Painter.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/painter/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.242820 mianalyzer-0.2.6/mia/ui/segmentation/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/segmentation/__init__.py
--rw-rw-rw-   0        0        0     6103 2022-02-01 14:06:24.000000 mianalyzer-0.2.6/mia/ui/segmentation/ui_SegPostProcessing.py
--rw-rw-rw-   0        0        0     8869 2022-02-01 15:26:27.000000 mianalyzer-0.2.6/mia/ui/segmentation/ui_SegResults.py
--rw-rw-rw-   0        0        0     5082 2022-02-01 14:06:24.000000 mianalyzer-0.2.6/mia/ui/segmentation/ui_SegSettings.py
--rw-rw-rw-   0        0        0     3597 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/settings.py
--rw-rw-rw-   0        0        0     2272 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/ui/style.py
--rw-rw-rw-   0        0        0      886 2022-02-01 14:04:45.000000 mianalyzer-0.2.6/mia/ui/ui_Abstract.py
--rw-rw-rw-   0        0        0    13878 2022-02-01 14:26:11.000000 mianalyzer-0.2.6/mia/ui/ui_Augment.py
--rw-rw-rw-   0        0        0    14170 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/ui/ui_Canvas.py
--rw-rw-rw-   0        0        0      886 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/ui/ui_Log.py
--rw-rw-rw-   0        0        0    11122 2022-05-24 10:06:51.000000 mianalyzer-0.2.6/mia/ui/ui_Results.py
--rw-rw-rw-   0        0        0    11618 2022-04-14 12:14:09.000000 mianalyzer-0.2.6/mia/ui/ui_Settings.py
--rw-rw-rw-   0        0        0     7685 2022-02-01 14:04:45.000000 mianalyzer-0.2.6/mia/ui/ui_TrainPlot.py
--rw-rw-rw-   0        0        0    18156 2022-02-01 14:04:45.000000 mianalyzer-0.2.6/mia/ui/ui_TrainSettings.py
--rw-rw-rw-   0        0        0    16270 2022-02-18 10:26:13.000000 mianalyzer-0.2.6/mia/ui/ui_Training.py
--rw-rw-rw-   0        0        0    10712 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/ui/ui_utils.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.242820 mianalyzer-0.2.6/mia/utils/
--rw-rw-rw-   0        0        0     9081 2022-02-18 10:26:13.000000 mianalyzer-0.2.6/mia/utils/FilesAndFolders.py
--rw-rw-rw-   0        0        0     7370 2022-10-13 11:57:14.000000 mianalyzer-0.2.6/mia/utils/Image.py
--rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/Observer.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.242820 mianalyzer-0.2.6/mia/utils/postprocessing/
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     9443 2021-11-26 09:23:09.000000 mianalyzer-0.2.6/mia/utils/postprocessing/tracking.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.242820 mianalyzer-0.2.6/mia/utils/shapes/
--rw-rw-rw-   0        0        0    16247 2022-10-13 14:15:31.000000 mianalyzer-0.2.6/mia/utils/shapes/Contour.py
--rw-rw-rw-   0        0        0     1533 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/shapes/ImageLabel.py
--rw-rw-rw-   0        0        0     4433 2022-05-31 12:40:55.000000 mianalyzer-0.2.6/mia/utils/shapes/Point.py
--rw-rw-rw-   0        0        0     2966 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/shapes/Shape.py
--rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/shapes/__init__.py
--rw-rw-rw-   0        0        0       86 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/utility_functions.py
--rw-rw-rw-   0        0        0      578 2021-06-29 14:36:14.000000 mianalyzer-0.2.6/mia/utils/workerthread.py
-drwxrwxrwx   0        0        0        0 2022-10-13 14:53:26.258442 mianalyzer-0.2.6/mianalyzer.egg-info/
--rw-rw-rw-   0        0        0      682 2022-10-13 14:53:26.000000 mianalyzer-0.2.6/mianalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6396 2022-10-13 14:53:26.000000 mianalyzer-0.2.6/mianalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-13 14:53:26.000000 mianalyzer-0.2.6/mianalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2022-10-13 14:53:26.000000 mianalyzer-0.2.6/mianalyzer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        4 2022-10-13 14:53:26.000000 mianalyzer-0.2.6/mianalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-23 09:23:41.000000 mianalyzer-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-13 14:53:26.258442 mianalyzer-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0     2444 2022-01-17 08:39:54.000000 mianalyzer-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/
+-rw-rw-rw-   0        0        0    35149 2021-12-20 09:08:37.000000 mianalyzer-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     2639 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2021 2023-07-17 14:38:35.000000 mianalyzer-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.867961 mianalyzer-0.3.0/mia/
+-rw-rw-rw-   0        0        0      149 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/__init__.py
+-rw-rw-rw-   0        0        0      147 2023-07-21 11:52:39.000000 mianalyzer-0.3.0/mia/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.871962 mianalyzer-0.3.0/mia/dl/
+-rw-rw-rw-   0        0        0    12475 2023-07-10 09:57:49.000000 mianalyzer-0.3.0/mia/dl/DeepLearning.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.875963 mianalyzer-0.3.0/mia/dl/data/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/data/__init__.py
+-rw-rw-rw-   0        0        0    11571 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/data/imagedata.py
+-rw-rw-rw-   0        0        0     5105 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/data/labels.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.883960 mianalyzer-0.3.0/mia/dl/loss/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/__init__.py
+-rw-rw-rw-   0        0        0     1898 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/classification_losses.py
+-rw-rw-rw-   0        0        0     6053 2022-02-01 16:19:20.000000 mianalyzer-0.3.0/mia/dl/loss/loss_functions.py
+-rw-rw-rw-   0        0        0      688 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/losses.py
+-rw-rw-rw-   0        0        0     1032 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/regression_losses.py
+-rw-rw-rw-   0        0        0     2712 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/loss/segmentation_losses.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.887959 mianalyzer-0.3.0/mia/dl/machine_learning/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0     8186 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/machine_learning/deploy.prototxt
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.895959 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/__init__.py
+-rw-rw-rw-   0        0        0     3650 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/classifiers.py
+-rw-rw-rw-   0        0        0     1308 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr.py
+-rw-rw-rw-   0        0        0     2275 2021-12-20 14:14:09.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr_segmentation.py
+-rw-rw-rw-   0        0        0    10541 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/helpers.py
+-rw-rw-rw-   0        0        0     7363 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/dextr/resnet.py
+-rw-rw-rw-   0        0        0      975 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/machine_learning/grabcut_segmentation.py
+-rw-rw-rw-   0        0        0     2632 2021-12-20 15:55:01.000000 mianalyzer-0.3.0/mia/dl/machine_learning/hed.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.899984 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/
+-rw-rw-rw-   0        0        0      427 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/__init__.py
+-rw-rw-rw-   0        0        0    15148 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/automatic_mask_generator.py
+-rw-rw-rw-   0        0        0     2941 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/build_sam.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.911961 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/
+-rw-rw-rw-   0        0        0      385 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/__init__.py
+-rw-rw-rw-   0        0        0     1479 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/common.py
+-rw-rw-rw-   0        0        0    14420 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/image_encoder.py
+-rw-rw-rw-   0        0        0     6615 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/mask_decoder.py
+-rw-rw-rw-   0        0        0     8594 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/prompt_encoder.py
+-rw-rw-rw-   0        0        0     7226 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/sam.py
+-rw-rw-rw-   0        0        0     8397 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/modeling/transformer.py
+-rw-rw-rw-   0        0        0    11633 2023-04-14 12:37:02.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/predictor.py
+-rw-rw-rw-   0        0        0     2666 2023-06-30 12:58:42.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/sam.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.911961 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/
+-rw-rw-rw-   0        0        0      197 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/__init__.py
+-rw-rw-rw-   0        0        0    12712 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/amg.py
+-rw-rw-rw-   0        0        0     5812 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/onnx.py
+-rw-rw-rw-   0        0        0     3972 2023-04-14 11:35:19.000000 mianalyzer-0.3.0/mia/dl/machine_learning/segment_anything/utils/transforms.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.923288 mianalyzer-0.3.0/mia/dl/method/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/method/__init__.py
+-rw-rw-rw-   0        0        0     6698 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/method/classification.py
+-rw-rw-rw-   0        0        0     3344 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/method/mode.py
+-rw-rw-rw-   0        0        0     5621 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/dl/method/objectcounting.py
+-rw-rw-rw-   0        0        0    10483 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/dl/method/pixelbasedprediction.py
+-rw-rw-rw-   0        0        0     3795 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/method/segmentation.py
+-rw-rw-rw-   0        0        0     1149 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/method/undefinedmode.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.927291 mianalyzer-0.3.0/mia/dl/metric/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/__init__.py
+-rw-rw-rw-   0        0        0     1155 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/classification_metrics.py
+-rw-rw-rw-   0        0        0     5288 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/metric_functions.py
+-rw-rw-rw-   0        0        0      756 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/metrics.py
+-rw-rw-rw-   0        0        0     1094 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/regression_metrics.py
+-rw-rw-rw-   0        0        0     2313 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/metric/segmentation_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.931290 mianalyzer-0.3.0/mia/dl/models/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.939290 mianalyzer-0.3.0/mia/dl/models/classification_models/
+-rw-rw-rw-   0        0        0      508 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/__init__.py
+-rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/__version__.py
+-rw-rw-rw-   0        0        0    12132 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/classification_models.py
+-rw-rw-rw-   0        0        0      347 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/keras.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.943290 mianalyzer-0.3.0/mia/dl/models/classification_models/models/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/__init__.py
+-rw-rw-rw-   0        0        0     4470 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/_common_blocks.py
+-rw-rw-rw-   0        0        0    13989 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnet.py
+-rw-rw-rw-   0        0        0    10009 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnext.py
+-rw-rw-rw-   0        0        0    15389 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models/senet.py
+-rw-rw-rw-   0        0        0     3417 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/models_factory.py
+-rw-rw-rw-   0        0        0      381 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/tfkeras.py
+-rw-rw-rw-   0        0        0     1279 2021-12-20 15:29:13.000000 mianalyzer-0.3.0/mia/dl/models/classification_models/weights.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.947290 mianalyzer-0.3.0/mia/dl/models/deeplab/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/deeplab/__init__.py
+-rw-rw-rw-   0        0        0    21934 2023-07-07 15:01:40.000000 mianalyzer-0.3.0/mia/dl/models/deeplab/deeplab.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.956069 mianalyzer-0.3.0/mia/dl/models/efficientnet/
+-rw-rw-rw-   0        0        0     2769 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/__init__.py
+-rw-rw-rw-   0        0        0      772 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/__version__.py
+-rw-rw-rw-   0        0        0      708 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/keras.py
+-rw-rw-rw-   0        0        0    23513 2023-07-10 10:00:11.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/model.py
+-rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/preprocessing.py
+-rw-rw-rw-   0        0        0      732 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/efficientnet/tfkeras.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.972802 mianalyzer-0.3.0/mia/dl/models/keras_applications/
+-rw-rw-rw-   0        0        0     2059 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/__init__.py
+-rw-rw-rw-   0        0        0    10731 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/densenet.py
+-rw-rw-rw-   0        0        0    12855 2021-12-20 15:53:29.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/imagenet_utils.py
+-rw-rw-rw-   0        0        0    14086 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_resnet_v2.py
+-rw-rw-rw-   0        0        0    13814 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_v3.py
+-rw-rw-rw-   0        0        0    18056 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet.py
+-rw-rw-rw-   0        0        0    19723 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet_v2.py
+-rw-rw-rw-   0        0        0    28646 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/nasnet.py
+-rw-rw-rw-   0        0        0     1041 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet.py
+-rw-rw-rw-   0        0        0    11888 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet50.py
+-rw-rw-rw-   0        0        0    20729 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_common.py
+-rw-rw-rw-   0        0        0     1051 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_v2.py
+-rw-rw-rw-   0        0        0     1020 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/resnext.py
+-rw-rw-rw-   0        0        0     7706 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg16.py
+-rw-rw-rw-   0        0        0     8178 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg19.py
+-rw-rw-rw-   0        0        0    12771 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/keras_applications/xception.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.976804 mianalyzer-0.3.0/mia/dl/models/segmentation_models/
+-rw-rw-rw-   0        0        0     4162 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/__init__.py
+-rw-rw-rw-   0        0        0       63 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/__version__.py
+-rw-rw-rw-   0        0        0     8428 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/_losses.py
+-rw-rw-rw-   0        0        0     8812 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/_metrics.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.984883 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/__init__.py
+-rw-rw-rw-   0        0        0     5302 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/backbones_factory.py
+-rw-rw-rw-   0        0        0    14288 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py
+-rw-rw-rw-   0        0        0    13856 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_v3.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.984883 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/
+-rw-rw-rw-   0        0        0       71 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/__init__.py
+-rw-rw-rw-   0        0        0    11669 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/functional.py
+-rw-rw-rw-   0        0        0     2687 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/objects.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.992804 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/__init__.py
+-rw-rw-rw-   0        0        0     2143 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/_common_blocks.py
+-rw-rw-rw-   0        0        0      377 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/_utils.py
+-rw-rw-rw-   0        0        0     9035 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/fpn.py
+-rw-rw-rw-   0        0        0     9703 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/linknet.py
+-rw-rw-rw-   0        0        0     8440 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/pspnet.py
+-rw-rw-rw-   0        0        0     8355 2022-01-31 10:47:17.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/unet.py
+-rw-rw-rw-   0        0        0     3012 2021-12-20 08:40:49.000000 mianalyzer-0.3.0/mia/dl/models/segmentation_models/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:35.992804 mianalyzer-0.3.0/mia/dl/optimizer/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     1693 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/optimizer/optimizer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.002366 mianalyzer-0.3.0/mia/dl/training/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/training/__init__.py
+-rw-rw-rw-   0        0        0    11693 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/dl/training/augment.py
+-rw-rw-rw-   0        0        0     6288 2023-07-10 09:57:49.000000 mianalyzer-0.3.0/mia/dl/training/datagenerator.py
+-rw-rw-rw-   0        0        0     1664 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/training/lrschedule.py
+-rw-rw-rw-   0        0        0     2929 2022-02-01 15:15:32.000000 mianalyzer-0.3.0/mia/dl/training/training_record.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.006369 mianalyzer-0.3.0/mia/dl/utils/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/dl/utils/__init__.py
+-rw-rw-rw-   0        0        0    22005 2023-07-10 10:00:11.000000 mianalyzer-0.3.0/mia/dl/utils/dl_downloads.py
+-rw-rw-rw-   0        0        0     6657 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/dl/utils/dl_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.045312 mianalyzer-0.3.0/mia/icons/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/__init__.py
+-rw-rw-rw-   0        0        0     1282 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/addobject.png
+-rw-rw-rw-   0        0        0     3070 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/assign.png
+-rw-rw-rw-   0        0        0     1554 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/assignclass.png
+-rw-rw-rw-   0        0        0     2432 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/augmentation.png
+-rw-rw-rw-   0        0        0     2436 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/clear.png
+-rw-rw-rw-   0        0        0     2144 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/delete.png
+-rw-rw-rw-   0        0        0     3607 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/dextr.png
+-rw-rw-rw-   0        0        0     2444 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/drag.png
+-rw-rw-rw-   0        0        0     2215 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/draw.png
+-rw-rw-rw-   0        0        0     1233 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/expand.png
+-rw-rw-rw-   0        0        0     3697 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/exportallmasks.png
+-rw-rw-rw-   0        0        0     5231 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/exportmask.png
+-rw-rw-rw-   0        0        0     1445 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/load.png
+-rw-rw-rw-   0        0        0    52773 2022-01-17 10:13:34.000000 mianalyzer-0.3.0/mia/icons/loading.png
+-rw-rw-rw-   0        0        0     1676 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/loadmodel.png
+-rw-rw-rw-   0        0        0    23516 2022-01-17 10:33:29.000000 mianalyzer-0.3.0/mia/icons/logo.png
+-rw-rw-rw-   0        0        0     1951 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/magicwand.png
+-rw-rw-rw-   0        0        0     3934 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/measure.png
+-rw-rw-rw-   0        0        0     2879 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/next.png
+-rw-rw-rw-   0        0        0     2797 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/objectcolor.png
+-rw-rw-rw-   0        0        0     2012 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/objectnumber.png
+-rw-rw-rw-   0        0        0     4019 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/poly.png
+-rw-rw-rw-   0        0        0     3365 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/postprocessing.png
+-rw-rw-rw-   0        0        0     7403 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/predict.png
+-rw-rw-rw-   0        0        0     4157 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/predictall.png
+-rw-rw-rw-   0        0        0     2975 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/previous.png
+-rw-rw-rw-   0        0        0     4149 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/reset.png
+-rw-rw-rw-   0        0        0     2703 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/results.png
+-rw-rw-rw-   0        0        0     1599 2023-06-26 14:16:10.000000 mianalyzer-0.3.0/mia/icons/sam.png
+-rw-rw-rw-   0        0        0     2682 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/saveall.png
+-rw-rw-rw-   0        0        0     1702 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/savemodel.png
+-rw-rw-rw-   0        0        0     3221 2022-05-24 12:04:22.000000 mianalyzer-0.3.0/mia/icons/setallclass.png
+-rw-rw-rw-   0        0        0     2502 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/setclass.png
+-rw-rw-rw-   0        0        0     4695 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/settings.png
+-rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/shift.png
+-rw-rw-rw-   0        0        0     3505 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/tracking.png
+-rw-rw-rw-   0        0        0     7888 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/icons/train.png
+-rw-rw-rw-   0        0        0    45731 2023-06-30 12:51:41.000000 mianalyzer-0.3.0/mia/mia_gui.py
+-rw-rw-rw-   0        0        0      802 2023-07-07 15:01:40.000000 mianalyzer-0.3.0/mia/startup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.061363 mianalyzer-0.3.0/mia/ui/
+-rw-rw-rw-   0        0        0    30223 2023-06-30 12:48:33.000000 mianalyzer-0.3.0/mia/ui/Tools.py
+-rw-rw-rw-   0        0        0    31651 2023-06-30 12:30:19.000000 mianalyzer-0.3.0/mia/ui/UI.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.069391 mianalyzer-0.3.0/mia/ui/classification/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/classification/__init__.py
+-rw-rw-rw-   0        0        0     1878 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/classification/ui_ClassResults.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.073362 mianalyzer-0.3.0/mia/ui/objectdetection/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/objectdetection/__init__.py
+-rw-rw-rw-   0        0        0     1558 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODPostProcessing.py
+-rw-rw-rw-   0        0        0     4816 2022-02-18 13:59:46.000000 mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODResults.py
+-rw-rw-rw-   0        0        0     4995 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODSettings.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.077363 mianalyzer-0.3.0/mia/ui/painter/
+-rw-rw-rw-   0        0        0     8971 2023-06-30 10:23:21.000000 mianalyzer-0.3.0/mia/ui/painter/ContourPainter.py
+-rw-rw-rw-   0        0        0     3687 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/ui/painter/ImageLabelPainter.py
+-rw-rw-rw-   0        0        0      490 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/painter/NoPainter.py
+-rw-rw-rw-   0        0        0     6900 2022-05-31 12:40:55.000000 mianalyzer-0.3.0/mia/ui/painter/ObjectPainter.py
+-rw-rw-rw-   0        0        0    12001 2023-04-26 14:49:10.000000 mianalyzer-0.3.0/mia/ui/painter/Painter.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/painter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.085001 mianalyzer-0.3.0/mia/ui/segmentation/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/segmentation/__init__.py
+-rw-rw-rw-   0        0        0     6103 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/segmentation/ui_SegPostProcessing.py
+-rw-rw-rw-   0        0        0     8869 2022-02-01 15:26:27.000000 mianalyzer-0.3.0/mia/ui/segmentation/ui_SegResults.py
+-rw-rw-rw-   0        0        0     5082 2022-02-01 14:06:24.000000 mianalyzer-0.3.0/mia/ui/segmentation/ui_SegSettings.py
+-rw-rw-rw-   0        0        0     3597 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/settings.py
+-rw-rw-rw-   0        0        0     2272 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/ui/style.py
+-rw-rw-rw-   0        0        0      886 2022-02-01 14:04:45.000000 mianalyzer-0.3.0/mia/ui/ui_Abstract.py
+-rw-rw-rw-   0        0        0    13878 2022-02-01 14:26:11.000000 mianalyzer-0.3.0/mia/ui/ui_Augment.py
+-rw-rw-rw-   0        0        0    14250 2023-04-14 12:57:59.000000 mianalyzer-0.3.0/mia/ui/ui_Canvas.py
+-rw-rw-rw-   0        0        0      886 2022-04-14 12:14:09.000000 mianalyzer-0.3.0/mia/ui/ui_Log.py
+-rw-rw-rw-   0        0        0    11122 2022-05-24 10:06:51.000000 mianalyzer-0.3.0/mia/ui/ui_Results.py
+-rw-rw-rw-   0        0        0    12026 2023-06-26 11:44:10.000000 mianalyzer-0.3.0/mia/ui/ui_Settings.py
+-rw-rw-rw-   0        0        0     7685 2022-02-01 14:04:45.000000 mianalyzer-0.3.0/mia/ui/ui_TrainPlot.py
+-rw-rw-rw-   0        0        0    18156 2022-02-01 14:04:45.000000 mianalyzer-0.3.0/mia/ui/ui_TrainSettings.py
+-rw-rw-rw-   0        0        0    16270 2022-02-18 10:26:13.000000 mianalyzer-0.3.0/mia/ui/ui_Training.py
+-rw-rw-rw-   0        0        0    10712 2022-05-31 12:40:55.000000 mianalyzer-0.3.0/mia/ui/ui_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.088349 mianalyzer-0.3.0/mia/utils/
+-rw-rw-rw-   0        0        0     9081 2022-02-18 10:26:13.000000 mianalyzer-0.3.0/mia/utils/FilesAndFolders.py
+-rw-rw-rw-   0        0        0     7370 2022-10-13 11:57:14.000000 mianalyzer-0.3.0/mia/utils/Image.py
+-rw-rw-rw-   0        0        0     2398 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/Observer.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.092431 mianalyzer-0.3.0/mia/utils/postprocessing/
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     9443 2021-11-26 09:23:09.000000 mianalyzer-0.3.0/mia/utils/postprocessing/tracking.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.096352 mianalyzer-0.3.0/mia/utils/shapes/
+-rw-rw-rw-   0        0        0    16247 2022-10-13 14:15:31.000000 mianalyzer-0.3.0/mia/utils/shapes/Contour.py
+-rw-rw-rw-   0        0        0     1533 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/shapes/ImageLabel.py
+-rw-rw-rw-   0        0        0     4433 2022-05-31 12:40:55.000000 mianalyzer-0.3.0/mia/utils/shapes/Point.py
+-rw-rw-rw-   0        0        0     2966 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/shapes/Shape.py
+-rw-rw-rw-   0        0        0        0 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/shapes/__init__.py
+-rw-rw-rw-   0        0        0       86 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/utility_functions.py
+-rw-rw-rw-   0        0        0      578 2021-06-29 14:36:14.000000 mianalyzer-0.3.0/mia/utils/workerthread.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/mianalyzer.egg-info/
+-rw-rw-rw-   0        0        0     2639 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7414 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        4 2023-07-21 11:58:35.000000 mianalyzer-0.3.0/mianalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      730 2023-07-21 11:58:21.000000 mianalyzer-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-21 11:58:36.112635 mianalyzer-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2474 2023-04-21 11:45:16.000000 mianalyzer-0.3.0/setup.py
```

### Comparing `mianalyzer-0.2.6/LICENSE` & `mianalyzer-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/README.md` & `mianalyzer-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 A quickstart guide can be found [here](https://mianalyzer.github.io/gettingstarted/quickstart.html) and the complete user manual [here](https://mianalyzer.github.io/).
 
 Please use [image.sc](https://forum.image.sc/tag/mia) with the ```mia```-tag for general discussion, questions about how to use the software or feature requests. Bugs can be reported directly in the [issues](https://github.com/MIAnalyzer/MIA/issues) panel on github.
 
 ## Reference
 If you use this code for your research, please cite: 
 
-https://biorxiv.org/cgi/content/short/2022.01.14.476308v1
+https://www.cell.com/cell-reports-methods/pdf/S2667-2375(23)00146-7.pdf
+
+Körber, MIA is an open-source standalone deep learning application for microscopic image analysis, Cell Reports Methods (2023)
 
 
 ## Requirements
 
 In general, MIA should run on any system with Linux or windows. You can use the cpu only, but it is highly recommended to have a system with a [cuda-compatible](https://developer.nvidia.com/cuda-gpus) gpu (from NVIDIA) to accelerate neural network training.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mianalyzer-0.2.6/mia/dl/DeepLearning.py` & `mianalyzer-0.3.0/mia/dl/DeepLearning.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,54 +8,51 @@
 
 from tensorflow.keras import losses
 from tensorflow.keras.metrics import MeanIoU
 from tensorflow.keras.models import load_model
 import tensorflow as tf
 
 
-import math
 import cv2
-import glob
-import os
 import numpy as np
 import threading
-import traceback
-import sys
+
 
 
 import dl.training.datagenerator as datagenerator
 import dl.training.training_record as training_record
 import dl.training.augment as augment
 import dl.training.lrschedule as schedule
 import dl.machine_learning.hed as hed
 import dl.machine_learning.dextr.dextr_segmentation as dextr
 import dl.machine_learning.grabcut_segmentation as gcs
+import dl.machine_learning.segment_anything.sam as sam
 import dl.data.imagedata as imagedata
 from dl.method.segmentation import Segmentation
 from dl.method.objectcounting import ObjectCounting
 from dl.method.classification import Classification
 from dl.method.undefinedmode import UndefinedMode
 from dl.method.mode import dlMode, dlPreprocess
 from dl.optimizer.optimizer import Optimizer
 
 from utils.Observer import dlObservable
 import gc
 
-import utils.shapes.Contour
 import multiprocessing
 
 class DeepLearning(dlObservable):
     def __init__(self):
         super().__init__()
         self.TrainInMemory = True
         self.ImageScaleFactor = 1
         self.worker = multiprocessing.cpu_count() // 2
         self.hed = hed.HED_Segmentation()
         self.dextr = dextr.DEXTR_Segmentation()
         self.grabcut = gcs.GrabCutSegmentation()
+        self.sam = sam.SegmentAnything()
         self.data = imagedata.ImageData(self)
         self.augmentation = augment.ImageAugment(self)
         self.record = training_record.TrainingRecording(self)
         
         self.Model = None
         # split factor and border need to be reworked and reasonable, get it from network
         self.split_factor = 32
@@ -255,24 +252,50 @@
     def executePrediction(self, image):
         # prediction would be much faster when all images where predicted from here compared to 1-by-1
         try:
             prediction = self.Mode.PredictImage(image)
         except:
             self.notifyError() 
         self.notifyPredictionFinished(prediction)
+        
+    def SAM(self, image, bbox, points, labels):
+        width = image.shape[1]
+        height = image.shape[0]
+        image = cv2.resize(image, (int(width*self.ImageScaleFactor), int(height*self.ImageScaleFactor)))
+        
+        
+        if bbox is not None:
+            bbox = bbox*self.ImageScaleFactor
+        if points is not None:
+            points = points*self.ImageScaleFactor
+
+        self.sam.setImage(image)
+        mask = np.squeeze(self.sam.getMask(bbox, points, labels)).astype(np.uint8)
+        return cv2.resize(mask, (width, height), interpolation=cv2.INTER_NEAREST)
+    
+    def SAM_AutoSegment(self, image):    
+        if image is None:
+            return None
 
+        width = image.shape[1]
+        height = image.shape[0]
+        image = cv2.resize(image, (int(width*self.ImageScaleFactor), int(height*self.ImageScaleFactor)))
+        
+        pred = self.sam.SegmentImage(image)
+        return cv2.resize(pred, (width, height), interpolation=cv2.INTER_NEAREST)
 
     def AutoSegment(self, image):    
         if image is None:
             return None
 
         width = image.shape[1]
         height = image.shape[0]
         image = cv2.resize(image, (int(width*self.ImageScaleFactor), int(height*self.ImageScaleFactor)))
-        
+
+
         pred = self.hed.applyHED(image)
         _,thresh = cv2.threshold(pred,0,1,cv2.THRESH_BINARY+cv2.THRESH_OTSU)
         ret = cv2.resize(thresh, (width, height), interpolation=cv2.INTER_NEAREST)
         return ret
 
     def AssistedSegmentation(self, image, extremepoints):      
         # no resizing here, as image is cropped to target network size (512,512) anyway
```

### Comparing `mianalyzer-0.2.6/mia/dl/data/imagedata.py` & `mianalyzer-0.3.0/mia/dl/data/imagedata.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/data/labels.py` & `mianalyzer-0.3.0/mia/dl/data/labels.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/loss/classification_losses.py` & `mianalyzer-0.3.0/mia/dl/loss/classification_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/loss/loss_functions.py` & `mianalyzer-0.3.0/mia/dl/loss/loss_functions.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/loss/losses.py` & `mianalyzer-0.3.0/mia/dl/loss/losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/loss/regression_losses.py` & `mianalyzer-0.3.0/mia/dl/loss/regression_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/loss/segmentation_losses.py` & `mianalyzer-0.3.0/mia/dl/loss/segmentation_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/deploy.prototxt` & `mianalyzer-0.3.0/mia/dl/machine_learning/deploy.prototxt`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/dextr/classifiers.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/classifiers.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/dextr/dextr.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/dextr/dextr_segmentation.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/dextr_segmentation.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/dextr/helpers.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/helpers.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/dextr/resnet.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/dextr/resnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/grabcut_segmentation.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/grabcut_segmentation.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/machine_learning/hed.py` & `mianalyzer-0.3.0/mia/dl/machine_learning/hed.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/method/classification.py` & `mianalyzer-0.3.0/mia/dl/method/classification.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/method/mode.py` & `mianalyzer-0.3.0/mia/dl/method/mode.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/method/objectcounting.py` & `mianalyzer-0.3.0/mia/dl/method/objectcounting.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/method/pixelbasedprediction.py` & `mianalyzer-0.3.0/mia/dl/method/pixelbasedprediction.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/method/segmentation.py` & `mianalyzer-0.3.0/mia/dl/method/segmentation.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/method/undefinedmode.py` & `mianalyzer-0.3.0/mia/dl/method/undefinedmode.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/metric/classification_metrics.py` & `mianalyzer-0.3.0/mia/dl/metric/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/metric/metric_functions.py` & `mianalyzer-0.3.0/mia/dl/metric/metric_functions.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/metric/metrics.py` & `mianalyzer-0.3.0/mia/dl/metric/metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/metric/regression_metrics.py` & `mianalyzer-0.3.0/mia/dl/metric/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/metric/segmentation_metrics.py` & `mianalyzer-0.3.0/mia/dl/metric/segmentation_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/classification_models.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/classification_models.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/models/_common_blocks.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/models/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/models/resnet.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/models/resnext.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/models/resnext.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/models/senet.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/models/senet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/models_factory.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/models_factory.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/classification_models/weights.py` & `mianalyzer-0.3.0/mia/dl/models/classification_models/weights.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/deeplab/deeplab.py` & `mianalyzer-0.3.0/mia/dl/models/deeplab/deeplab.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,30 +22,30 @@
 
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
 import tensorflow as tf
 
-from tensorflow.python.keras.models import Model
-from tensorflow.python.keras import layers
-from tensorflow.python.keras.layers import Input
-from tensorflow.python.keras.layers import Lambda
-from tensorflow.python.keras.layers import Activation
-from tensorflow.python.keras.layers import Concatenate
-from tensorflow.python.keras.layers import Add
-from tensorflow.python.keras.layers import Dropout
-from tensorflow.python.keras.layers import BatchNormalization
-from tensorflow.python.keras.layers import Conv2D
-from tensorflow.python.keras.layers import DepthwiseConv2D
-from tensorflow.python.keras.layers import ZeroPadding2D
-from tensorflow.python.keras.layers import GlobalAveragePooling2D
-from tensorflow.python.keras.utils.layer_utils import get_source_inputs
-from tensorflow.python.keras import backend as K
-from tensorflow.python.keras.applications.imagenet_utils import preprocess_input
+from tensorflow.keras.models import Model
+from tensorflow.keras import layers
+from tensorflow.keras.layers import Input
+from tensorflow.keras.layers import Lambda
+from tensorflow.keras.layers import Activation
+from tensorflow.keras.layers import Concatenate
+from tensorflow.keras.layers import Add
+from tensorflow.keras.layers import Dropout
+from tensorflow.keras.layers import BatchNormalization
+from tensorflow.keras.layers import Conv2D
+from tensorflow.keras.layers import DepthwiseConv2D
+from tensorflow.keras.layers import ZeroPadding2D
+from tensorflow.keras.layers import GlobalAveragePooling2D
+from tensorflow.keras.utils import get_source_inputs
+from tensorflow.keras import backend as K
+from tensorflow.keras.applications.imagenet_utils import preprocess_input
 from tensorflow.keras.utils import get_custom_objects
 
 
 from dl.utils.dl_downloads import get_deeplabX, get_deeplabM
 
 
 def SepConv_BN(x, filters, prefix, stride=1, kernel_size=3, rate=1, depth_activation=False, epsilon=1e-3):
```

### Comparing `mianalyzer-0.2.6/mia/dl/models/efficientnet/__init__.py` & `mianalyzer-0.3.0/mia/dl/models/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/efficientnet/__version__.py` & `mianalyzer-0.3.0/mia/dl/models/efficientnet/__version__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/efficientnet/keras.py` & `mianalyzer-0.3.0/mia/dl/models/efficientnet/keras.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/efficientnet/model.py` & `mianalyzer-0.3.0/mia/dl/models/efficientnet/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
                                       require_flatten=include_top,
                                       weights=weights)
 
     if input_tensor is None:
         img_input = layers.Input(shape=input_shape)
     else:
         if backend.backend() == 'tensorflow':
-            from tensorflow.python.keras.backend import is_keras_tensor
+            from tensorflow.keras.backend import is_keras_tensor
         else:
             is_keras_tensor = backend.is_keras_tensor
         if not is_keras_tensor(input_tensor):
             img_input = layers.Input(tensor=input_tensor, shape=input_shape)
         else:
             img_input = input_tensor
```

### Comparing `mianalyzer-0.2.6/mia/dl/models/efficientnet/preprocessing.py` & `mianalyzer-0.3.0/mia/dl/models/efficientnet/preprocessing.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/efficientnet/tfkeras.py` & `mianalyzer-0.3.0/mia/dl/models/efficientnet/tfkeras.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/__init__.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/__init__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/densenet.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/densenet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/imagenet_utils.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/inception_resnet_v2.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/inception_v3.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/mobilenet.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/mobilenet_v2.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/nasnet.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet50.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet50.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet_common.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_common.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/resnet_v2.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/resnext.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/resnext.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/vgg16.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/vgg19.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/keras_applications/xception.py` & `mianalyzer-0.3.0/mia/dl/models/keras_applications/xception.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/__init__.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/__init__.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/_losses.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/_losses.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/_metrics.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/_metrics.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/backbones_factory.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/backbones_factory.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/backbones/inception_v3.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/backbones/inception_v3.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/base/functional.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/functional.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/base/objects.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/base/objects.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/_common_blocks.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/_common_blocks.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/fpn.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/fpn.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/linknet.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/linknet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/pspnet.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/pspnet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/models/unet.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/models/unet.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/models/segmentation_models/utils.py` & `mianalyzer-0.3.0/mia/dl/models/segmentation_models/utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/optimizer/optimizer.py` & `mianalyzer-0.3.0/mia/dl/optimizer/optimizer.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/training/augment.py` & `mianalyzer-0.3.0/mia/dl/training/augment.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/training/datagenerator.py` & `mianalyzer-0.3.0/mia/dl/training/datagenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 
 
 import cv2
 import numpy as np
 import random
 import threading
 from tensorflow.keras.preprocessing.image import ImageDataGenerator
-import time
-from tensorflow.python.keras.utils.data_utils import Sequence
+from tensorflow.keras.utils import Sequence
 import dl.utils.dl_utils as dl_utils
 
+
 class TrainingDataGenerator(Sequence):
     def __init__(self, parent, validation = False):
         self.parent = parent
         self.lock = threading.Lock()
         self.inMemory  = parent.TrainInMemory
         self.validation = validation
         if self.inMemory:
```

### Comparing `mianalyzer-0.2.6/mia/dl/training/lrschedule.py` & `mianalyzer-0.3.0/mia/dl/training/lrschedule.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/training/training_record.py` & `mianalyzer-0.3.0/mia/dl/training/training_record.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/dl/utils/dl_downloads.py` & `mianalyzer-0.3.0/mia/dl/utils/dl_downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 
 ### to do:
 # rework and unify
     
 import os
-from tensorflow.python.keras.utils.data_utils import get_file
+from tensorflow.keras.utils import get_file
 
 SUBDIR = 'models'
 MIAURL = 'https://github.com/MIAnalyzer/MIA/releases/download/weights/'
 
 
 def startFunction():
     return True
@@ -58,14 +58,28 @@
 
 def get_dextr():
     fname = 'dextr_coco.h5'
     url = MIAURL + fname
     fhash = '16415d65f6e15d3fa053afa21d5927e0'
     return getTargetFile(fname, url, fhash)
 
+def get_sam(model_name):
+    if model_name == 'vit_b':
+        fname = 'sam_vit_b_01ec64.pth'
+        fhash = '01ec64d29a2fca3f0661936605ae66f8'
+    elif model_name == 'vit_l':
+        fname = 'sam_vit_l_0b3195.pth'
+        fhash = '0b3195507c641ddb6910d2bb5adee89c'
+    # can not store on github atm, because file is larger 2GB
+    elif model_name == 'vit_h':
+        fname = 'sam_vit_h_4b8939.pth'
+        fhash = '4b8939a88964f0f4ff5f5b2642c598a6'
+    url = MIAURL + fname
+    return getTargetFile(fname, url, fhash)
+
 def get_deeplabX():
     fname = 'deeplabv3_xception_tf_dim_ordering_tf_kernels.h5'
     url = MIAURL + fname
     fhash = "b979702082524aca6a249fd546f8ea13"
     return getTargetFile(fname, url, fhash)
     
 def get_deeplabM():
```

### Comparing `mianalyzer-0.2.6/mia/dl/utils/dl_utils.py` & `mianalyzer-0.3.0/mia/dl/utils/dl_utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/addobject.png` & `mianalyzer-0.3.0/mia/icons/addobject.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/assign.png` & `mianalyzer-0.3.0/mia/icons/assign.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/assignclass.png` & `mianalyzer-0.3.0/mia/icons/assignclass.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/augmentation.png` & `mianalyzer-0.3.0/mia/icons/augmentation.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/clear.png` & `mianalyzer-0.3.0/mia/icons/clear.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/delete.png` & `mianalyzer-0.3.0/mia/icons/delete.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/dextr.png` & `mianalyzer-0.3.0/mia/icons/dextr.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/drag.png` & `mianalyzer-0.3.0/mia/icons/drag.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/draw.png` & `mianalyzer-0.3.0/mia/icons/draw.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/expand.png` & `mianalyzer-0.3.0/mia/icons/expand.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/exportallmasks.png` & `mianalyzer-0.3.0/mia/icons/exportallmasks.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/exportmask.png` & `mianalyzer-0.3.0/mia/icons/exportmask.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/load.png` & `mianalyzer-0.3.0/mia/icons/load.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/loading.png` & `mianalyzer-0.3.0/mia/icons/loading.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/loadmodel.png` & `mianalyzer-0.3.0/mia/icons/loadmodel.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/logo.png` & `mianalyzer-0.3.0/mia/icons/logo.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/magicwand.png` & `mianalyzer-0.3.0/mia/icons/magicwand.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/measure.png` & `mianalyzer-0.3.0/mia/icons/measure.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/next.png` & `mianalyzer-0.3.0/mia/icons/next.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/objectcolor.png` & `mianalyzer-0.3.0/mia/icons/objectcolor.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/objectnumber.png` & `mianalyzer-0.3.0/mia/icons/objectnumber.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/poly.png` & `mianalyzer-0.3.0/mia/icons/poly.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/postprocessing.png` & `mianalyzer-0.3.0/mia/icons/postprocessing.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/predict.png` & `mianalyzer-0.3.0/mia/icons/predict.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/predictall.png` & `mianalyzer-0.3.0/mia/icons/predictall.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/previous.png` & `mianalyzer-0.3.0/mia/icons/previous.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/reset.png` & `mianalyzer-0.3.0/mia/icons/reset.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/results.png` & `mianalyzer-0.3.0/mia/icons/results.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/saveall.png` & `mianalyzer-0.3.0/mia/icons/saveall.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/savemodel.png` & `mianalyzer-0.3.0/mia/icons/savemodel.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/setclass.png` & `mianalyzer-0.3.0/mia/icons/setclass.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/settings.png` & `mianalyzer-0.3.0/mia/icons/settings.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/shift.png` & `mianalyzer-0.3.0/mia/icons/shift.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/tracking.png` & `mianalyzer-0.3.0/mia/icons/tracking.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/icons/train.png` & `mianalyzer-0.3.0/mia/icons/train.png`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/mia_gui.py` & `mianalyzer-0.3.0/mia/mia_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,40 +175,39 @@
         self.Bdrag.clicked.connect(self.setCanvasMode)
         self.Bdraw.clicked.connect(self.setCanvasMode)
         self.Bassign.clicked.connect(self.setCanvasMode)
         self.Bextend.clicked.connect(self.setCanvasMode)
         self.Bdelete.clicked.connect(self.setCanvasMode)
         self.Bpoly.clicked.connect(self.setCanvasMode)
         self.Bassist.clicked.connect(self.setCanvasMode)
+        self.BsamTool.clicked.connect(self.setCanvasMode)
         
         self.BassignClass.clicked.connect(self.setCanvasMode)
         self.BsetClass.clicked.connect(self.setCanvasMode)
         self.BsetallClass.clicked.connect(self.setCanvasMode)
         
         self.BsetObject.clicked.connect(self.setCanvasMode)
         self.BshiftObject.clicked.connect(self.setCanvasMode)
 
         self.BSetObjectNumber.clicked.connect(self.setCanvasMode)
         self.BDeleteObject.clicked.connect(self.setCanvasMode)
         self.BChangeObjectColor.clicked.connect(self.setCanvasMode)
 
-        
+        self.CBSAM.stateChanged.connect(self.showSAMFrame)
         self.Btrain.clicked.connect(self.showTrainingWindow)
         self.Bpredictall.clicked.connect(self.predictAllImages)
         self.Bpredict.clicked.connect(self.predictImage)
         self.Bloadmodel.clicked.connect(self.loadModel)
         self.Bsavemodel.clicked.connect(self.saveModel)
         self.Bautoseg.clicked.connect(self.autoSegment)
         self.CBSmartMode.stateChanged.connect(self.setSmartMode)
-        self.CBInner.stateChanged.connect(self.updateImage)
 
         self.Bresetmodel.clicked.connect(self.resetModel)
         self.Bautodect.clicked.connect(self.autoPointDetection)
         
-        
         self.Bresults.clicked.connect(self.showResultsWindow)
         self.BSettings.clicked.connect(self.showSettingsWindow)
         self.BPostProcessing.clicked.connect(self.showPostProcessingWindow)
         
         self.Baddclass.clicked.connect(self.addClass)
         self.Bdelclass.clicked.connect(self.removeLastClass)
 
@@ -236,14 +235,18 @@
         self.ASetTestFolder.triggered.connect(self.setTestFolder)
         self.ASaveSettings.triggered.connect(self.SaveSettings)
         self.ALoadSettings.triggered.connect(self.LoadSettings)
         self.ASaveDeepLearning.triggered.connect(self.saveDLClass)
         self.AOpenManual.triggered.connect(self.OpenManual)
         self.AOpenGithub.triggered.connect(self.OpenGithub)
         self.AOpenLog.triggered.connect(self.showLog)
+
+        self.Asam_vit_b.triggered.connect(self.set_sam_Model)
+        self.Asam_vit_l.triggered.connect(self.set_sam_Model)
+        self.Asam_vit_h.triggered.connect(self.set_sam_Model)
         
         self.AExit.triggered.connect(self.close)
         self.ASettings.triggered.connect(self.showSettingsWindow)
         
         # monkey patching download request for model weights
         import dl.utils.dl_downloads as down
         down.callBackstart = lambda: self.ConfirmPopup('Do you want to download model weights')
@@ -433,25 +436,25 @@
     def setSmartMode(self):
         assert (self.LearningMode() == dlMode.Segmentation)
         self.canvas.painter.smartmode = self.CBSmartMode.isChecked()
         self.setCanvasFocus()
         
     @property
     def allowInnerContours(self):
-        return self.CBInner.isChecked()
+        return self.settings_form.CBInner.isChecked()
         
     def changeLearningMode(self, i):
         self.dl.WorkingMode = dlMode(i)
         self.canvas.setCanvasMode(self.LearningMode())
         self.closeModeWindows()
         if self.LearningMode() == dlMode.Segmentation:
             self.SegmentationSettings.show()
         else:
             self.SegmentationSettings.hide()
-            
+
         if self.LearningMode() == dlMode.Object_Counting:
             self.DetectionSettings.show()
         else:
             self.DetectionSettings.hide()
         
         if self.LearningMode() == dlMode.Classification:
             self.ClassificationToolButtons.show()
@@ -467,14 +470,16 @@
 
             self.segpostprocessing_form.enableTrackingMode()
             self.odpostprocessing_form.enableTrackingMode()
             
 
         self.setWorkingFolder()
 
+
+
     def TrackingSupported(self):
         if self.LearningMode() == dlMode.Segmentation:
             return True
         if self.LearningMode() == dlMode.Object_Counting:
             return True
         else:
             return False
@@ -511,14 +516,21 @@
     
     @property
     def TrackingModeEnabled(self):
         if not self.files.train_test_dir and self.TrackingSupported():
             return self.Tracking.isVisible()
         return False
 
+    def showSAMFrame(self):
+        if self.CBSAM.isChecked():
+            self.SAMSettings.show()
+        else:
+            self.SAMSettings.hide()
+    
+
     def setToolButtons(self):
         if self.activeClass() == 0:
             self.canvas.painter.enableDrawBackgroundMode()                
         else:
             self.canvas.painter.disableDrawBackgroundMode()
             
         # we need to first set all to invisible as otherwise the widget_width is extended 
@@ -1147,14 +1159,22 @@
     def autoSegment(self):
         with self.wait_cursor():
             self.canvas.painter.autosegment()
     
     def autoPointDetection(self):
         with self.wait_cursor():
             self.canvas.painter.autodetection()
+
+    def set_sam_Model(self):
+        if self.Asam_vit_b.isChecked():
+            self.dl.sam.setModel('vit_b')
+        elif self.Asam_vit_l.isChecked():
+            self.dl.sam.setModel('vit_l')
+        elif self.Asam_vit_h.isChecked():
+            self.dl.sam.setModel('vit_h')
         
     def saveDLClass(self):
         
         defaultname = 'model_' + time.strftime("%Y-%m-%d_%H-%M-%S")
         filename = saveFile("Save Settings","Settings File (*.pkl)", 'pkl', defaultname)
         if filename:
             filehandler = open(filename, 'wb')
```

### Comparing `mianalyzer-0.2.6/mia/startup.py` & `mianalyzer-0.3.0/mia/startup.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/Tools.py` & `mianalyzer-0.3.0/mia/ui/Tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     drag = 'drag'
     draw = 'draw'
     assign = 'assign'
     delete = 'delete'
     extend = 'extend'
     poly =  'poly'
     assist = 'assist'
+    sam = 'sam'
     scale =  'scale'
     shift = 'shift'
     point = 'point'
     setimageclass = 'setimageclass'
     setallimagesclass = 'setallimagesclass'
     assignimageclass = 'assignimageclass'
     objectnumber = 'objectnumber'
@@ -468,14 +469,133 @@
                 self.canvas.painter.assistedSegmentation(self.extremePoints)
                 self.extremePoints.clear()
 
     def mousePressEvent(self,e):
         pass
     def Cursor(self):
         return Qt.ArrowCursor  
+    
+class SAMTool(AbstractTool):
+    def __init__(self, canvas):
+        super().__init__(canvas)
+        self.canvas = canvas
+        self.Text = 'Segment Anything'
+        self.type = canvasTool.sam
+        self.Points = []
+        self.Labels = []
+        self.BoundingBox = np.array([0, 0, 0, 0])
+        self.beginbb = False
+        self.drawimage = None
+
+    def __del__(self): 
+        self.Points.clear()
+        self.Labels.clear()
+        self.BoundingBox = np.array([0, 0, 0, 0])
+        self.canvas.redrawImage()
+        self.drawimage = None  
+
+    @property
+    def mode(self):
+        # 0: negative points; 1: positive points; 2: bounding box
+        if self.canvas.parent.RBsamneg.isChecked():
+            return 0
+        elif self.canvas.parent.RBsampos.isChecked():
+            return 1
+        elif self.canvas.parent.RBsambb.isChecked():
+            return 2
+        
+    def mouseMoveEvent(self, e):     
+        if not self.canvas.fastPainting:
+            if self.mode == 2:
+                if self.beginbb:
+                    p = self.canvas.f2intPoint(self.canvas.mapToScene(e.pos()))
+                    if self.drawimage is None:
+                        self.drawimage = self.canvas.image().copy()
+                    self.canvas.copyRect(self.drawimage, self.canvas.image(),self.canvas.getFieldOfViewRect())
+                    x = self.BoundingBox[0]
+                    y = self.BoundingBox[1]
+                    h = p.x()-self.BoundingBox[0]
+                    w = p.y()-self.BoundingBox[1]  
+                    self.canvas.painter.addRectangle(x, y, h, w, filled = False)
+
+    @validTool  
+    def mouseReleaseEvent(self,e):
+        if self.canvas.image() is None:
+            return
+        
+        if e.button() == Qt.LeftButton:  
+            if self.mode == 0 or self.mode == 1:
+                p = self.canvas.mapToScene(e.pos())
+    
+                h = max(self.canvas.pen_size,2)
+                w = max(self.canvas.pen_size,2)
+                x = p.x() - w//2
+                y = p.y() - h//2
+
+                if self.mode == 0:
+                    color = QColor(255,0,0)
+                if self.mode == 1:
+                    color = QColor(0,255,0)
+                self.canvas.painter.addRectangle(x, y, h, w, color)
+                self.Points.append(self.canvas.QPoint2npPoint(self.canvas.f2intPoint(p)))
+                self.Labels.append(self.mode)
+            elif self.mode == 2:
+                p = self.canvas.mapToScene(e.pos())
+                self.BoundingBox[2] = p.x()
+                self.BoundingBox[3] = p.y()
+                
+                
+                         
+                if self.BoundingBox[2] < self.BoundingBox[0]:
+                    self.BoundingBox[2], self.BoundingBox[0] = self.BoundingBox[0], self.BoundingBox[2]
+                if self.BoundingBox[3] < self.BoundingBox[1]:
+                    self.BoundingBox[3], self.BoundingBox[1] = self.BoundingBox[1], self.BoundingBox[3]
+
+                if self.canvas.fastPainting:
+                    x = self.BoundingBox[0]
+                    y = self.BoundingBox[1]
+                    h = self.BoundingBox[2]-self.BoundingBox[0]
+                    w = self.BoundingBox[3]-self.BoundingBox[1]
+                    self.canvas.painter.addRectangle(x, y, h, w, filled = False)
+                    
+                self.beginbb = False
+            
+        modifiers = QApplication.keyboardModifiers()
+        if e.button() == Qt.RightButton:  
+            if modifiers == Qt.ShiftModifier or modifiers == Qt.ControlModifier:
+                if self.mode == 0:
+                    self.canvas.parent.RBsambb.setChecked(True) 
+                elif self.mode == 1:
+                    self.canvas.parent.RBsamneg.setChecked(True)
+                elif self.mode == 2:
+                    self.canvas.parent.RBsampos.setChecked(True)
+                self.canvas.setCursor(self.Cursor())
+            else:
+                if self.Points or self.BoundingBox.any():
+                    self.canvas.painter.SegmentAnything(self.Points, self.Labels, self.BoundingBox)
+                    self.Points.clear()
+                    self.Labels.clear()
+                    self.BoundingBox = np.zeros_like(self.BoundingBox)
+
+        
+
+    def mousePressEvent(self,e):
+        if self.canvas.image() is None:
+            return
+
+        if e.button() == Qt.LeftButton: 
+            if self.mode == 2:
+                p = self.canvas.mapToScene(e.pos())
+                self.BoundingBox[0] = p.x()
+                self.BoundingBox[1] = p.y()
+                self.beginbb = True
+                self.drawimage = None
+            
+    def Cursor(self):
+        return Qt.ArrowCursor  
 
         
 class PointTool(AbstractTool):
     
     def __init__(self, canvas):
         super().__init__(canvas)
         self.canvas = canvas
```

### Comparing `mianalyzer-0.2.6/mia/ui/UI.py` & `mianalyzer-0.3.0/mia/ui/UI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Oct 10 11:28:44 2019
 
 @author: Koerber
 """
 
+from msilib.schema import RadioButton
 from PyQt5.QtGui import *
 from PyQt5.QtWidgets import *
 from PyQt5.QtCore import *
 
 from ui.ui_utils import ClassList, ClassWidget, DCDButton, LabelledSpinBox
 from ui.style import styleForm, getHighlightColor, getBackgroundColor, getBrightColor
 
@@ -139,15 +140,15 @@
         line.setFrameShape(QFrame.HLine)
         line.setFrameShadow(QFrame.Sunken)
         line.setStyleSheet("background: " + getBrightColor(asString = True))
         self.vlayout.addWidget(line)
         
         
         # settings for segmentation
-        self.SegmentationSettingslayout = QHBoxLayout()
+        self.SegmentationSettingslayout = QVBoxLayout()
         self.SegmentationSettingslayout.setContentsMargins(0, 0, 0, 0)
         layout0 = QVBoxLayout()
         self.Bautoseg = DCDButton(self.centralWidget)
         self.Bautoseg.setToolTip('press to perform auto segmentation')
         self.Bautoseg.setText('Auto Seg')
         self.Bautoseg.setIcon(QIcon('icons/magicwand.png'))
         
@@ -159,29 +160,111 @@
         layout0.addWidget(self.Bautoseg)
         layout0.addWidget(self.Bassist)
 
         layout = QVBoxLayout()
         self.CBSmartMode = QCheckBox("Smart Mode",self.centralWidget)
         self.CBSmartMode.setToolTip("Check to activate smart segmentation mode")
         self.CBSmartMode.setObjectName('SmartMode')
-        self.CBInner = QCheckBox("Inner Contours",self.centralWidget)
-        self.CBInner.setToolTip("Check to allow contours to have holes")
-        self.CBInner.setObjectName('InnerContours')
-        self.CBInner.setChecked(True)
+
+        self.CBSAM = QCheckBox("SAM",self.centralWidget)
+        self.CBSAM.setToolTip("Check to open segment anything (SAM)")
+        self.CBSAM.setObjectName('sam_activate')
+        self.CBSAM.setChecked(False)
         layout.addWidget(self.CBSmartMode)
-        layout.addWidget(self.CBInner)
+        layout.addWidget(self.CBSAM)
+
+        samlayout = QVBoxLayout()
+        samlayout.setContentsMargins(0, 0, 0, 0)
+
+        sam1layout = QHBoxLayout()
+        sam2layout = QHBoxLayout()
+        self.BsamTool = DCDButton(self.centralWidget)
+        self.BsamTool.setText('SAM')
+        self.BsamTool.setObjectName('sam')
+        self.BsamTool.setToolTip('Select to activate segment anything.')
+        self.BsamTool.setIcon(QIcon('icons/sam.png'))
+
+        self.RBsampos = QRadioButton(self.centralWidget)
+        self.RBsampos.setText('Pos')
+        self.RBsampos.setObjectName('sam_positive')
+        self.RBsampos.setToolTip('Select to assign positive object points for SAM.')
+ 
+        self.RBsamneg = QRadioButton(self.centralWidget)
+        self.RBsamneg.setText('Neg')
+        self.RBsamneg.setObjectName('sam_negative')
+        self.RBsamneg.setToolTip('Select to assign negative objects points for SAM.')
+
+        self.RBsambb = QRadioButton(self.centralWidget)
+        self.RBsambb.setText('Box')
+        self.RBsambb.setObjectName('sam_bbox')
+        self.RBsambb.setToolTip('Select to assign object bounding box for SAM.')
+
+        self.CBSamSettings = DCDButton(self.centralWidget)
+        self.CBSamSettings.setMaximumSize(bwidth, bheight)
+        self.CBSamSettings.setIcon(QIcon('icons/settings.png'))
+
+        self.SAMMenu = QMenu(self.centralWidget)
+        ag = QActionGroup(self.centralWidget, exclusive=True)
+
+        self.Asam_vit_b = QAction('vit_b', self.centralWidget, checkable=True)
+        self.Asam_vit_l = QAction('vit_l', self.centralWidget, checkable=True)
+        self.Asam_vit_h = QAction('vit_h', self.centralWidget, checkable=False)
+        ag.addAction(self.Asam_vit_b)
+        ag.addAction(self.Asam_vit_l)
+        ag.addAction(self.Asam_vit_h)
+        self.Asam_vit_b.setChecked(True)
+        self.SAMMenu.addAction(self.Asam_vit_b)
+        self.SAMMenu.addAction(self.Asam_vit_l)
+        self.SAMMenu.addAction(self.Asam_vit_h)
+        
+
+        self.CBSamSettings.setMenu(self.SAMMenu)
+
+
+        sam1layout.addWidget(self.BsamTool)
+        sam1layout.addWidget(self.CBSamSettings)
+
+        sam2layout.addWidget(self.RBsampos)
+        sam2layout.addWidget(self.RBsamneg)
+        sam2layout.addWidget(self.RBsambb)
+
+        line = QFrame(self.centralWidget)
+        line.setFrameShape(QFrame.HLine)
+        line.setFrameShadow(QFrame.Sunken)
+        line.setStyleSheet("background: " + getBrightColor(asString = True))
+        
+        samlayout.addWidget(line)
+        samlayout.addLayout(sam1layout)
+        samlayout.addLayout(sam2layout)
+
+        line = QFrame(self.centralWidget)
+        line.setFrameShape(QFrame.HLine)
+        line.setFrameShadow(QFrame.Sunken)
+        line.setStyleSheet("background: " + getBrightColor(asString = True))
+
+        samlayout.addWidget(line)
+
+        self.SAMSettings = QFrame()
+        self.SAMSettings.setContentsMargins(0, 0, 0, 0)
+        self.SAMSettings.setLayout(samlayout)
+        self.SAMSettings.hide()
+
+        layout3 = QHBoxLayout()
+        layout3.addLayout(layout)
+        layout3.addLayout(layout0)
+
+        self.SegmentationSettingslayout.addLayout(layout3)
+        self.SegmentationSettingslayout.addWidget(self.SAMSettings)
+
 
-        self.SegmentationSettingslayout.addLayout(layout)
-        self.SegmentationSettingslayout.addLayout(layout0)
         self.SegmentationSettings = QFrame()
         self.SegmentationSettings.setLayout(self.SegmentationSettingslayout)
         self.SegmentationSettings.hide()
         self.vlayout.addWidget(self.SegmentationSettings)
         
-        
         # settings for object detection
         self.DetectionSettingslayout = QHBoxLayout()
         self.DetectionSettingslayout.setContentsMargins(0, 0, 0, 0)
         self.Bautodect = DCDButton(self.centralWidget)
         self.Bautodect.setToolTip('press to perform auto detection')
         self.Bautodect.setText('Auto Detection')
         self.Bautodect.setIcon(QIcon('icons/magicwand.png'))
```

### Comparing `mianalyzer-0.2.6/mia/ui/classification/ui_ClassResults.py` & `mianalyzer-0.3.0/mia/ui/classification/ui_ClassResults.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/objectdetection/ui_ODPostProcessing.py` & `mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODPostProcessing.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/objectdetection/ui_ODResults.py` & `mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODResults.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/objectdetection/ui_ODSettings.py` & `mianalyzer-0.3.0/mia/ui/objectdetection/ui_ODSettings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/painter/ContourPainter.py` & `mianalyzer-0.3.0/mia/ui/painter/ContourPainter.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import copy 
 
 class ContourPainter(Painter):
     def __init__(self, canvas):
         super(ContourPainter,self).__init__(canvas)
         self.tools.append(canvasTool.assign)
         self.tools.append(canvasTool.assist)
+        self.tools.append(canvasTool.sam)
         self.tools.append(canvasTool.objectnumber)
         self.tools.append(canvasTool.objectcolor)
         self.tools.append(canvasTool.deleteobject)
         
         # self.mask = None
         self.smartmode = False
 
@@ -57,14 +58,15 @@
     def enableDrawBackgroundMode(self):
         super(ContourPainter, self).enableDrawBackgroundMode()
 
     def disableDrawBackgroundMode(self):
         super(ContourPainter, self).enableDrawBackgroundMode()
         self.tools.append(canvasTool.assign)
         self.tools.append(canvasTool.assist)
+        self.tools.append(canvasTool.sam)
         self.tools.append(canvasTool.objectnumber)
         self.tools.append(canvasTool.objectcolor)
         self.tools.append(canvasTool.deleteobject)
 
     def clear(self):
         super(ContourPainter, self).clear()
         self.shapes.clear()
@@ -135,14 +137,41 @@
             mask = self.canvas.getFieldOfViewImage(self.mask)
             prediction = self.canvas.parent.dl.SemiAutoSegment(image, mask)
             self.contours.deleteShapes(self.contours.getShapesOfClass_x(self.canvas.parent.activeClass()))
             smartcontours = Contour.extractContoursFromImage(prediction, not self.canvas.parent.allowInnerContours, offset = (int(fov.x()),int(fov.y())))
             Contour.drawContoursToImage(self.contoursketch, smartcontours)  
 
         super(ContourPainter, self).getFinalContours()
+        
+    def SegmentAnything(self, points, labels, bbox):
+        with self.canvas.parent.wait_cursor():
+            try:
+                if not bbox.any():
+                    bbox = None
+                if not points:
+                    points = None
+                    labels = None
+                else:
+                    points = np.asarray(points, dtype = np.int)
+                    labels = np.asarray(labels, dtype = np.int)
+                prediction = self.canvas.parent.dl.SAM(self.canvas.parent.getCurrentImage(), bbox, points, labels)
+
+            except:
+                self.canvas.parent.PopupWarning('SAM not working, try smaller image size (settings->Image Down Scaling)')
+                return
+            
+            if prediction is None:
+                self.canvas.redrawImage()
+                return
+            shapes = Contour.extractContoursFromLabel(prediction, not self.canvas.parent.allowInnerContours)
+            for s in shapes:
+                s.setClassLabel(self.canvas.parent.activeClass())
+            self.contours.addShapes(shapes)
+            self.checkForChanges()    
+    
 
     def assistedSegmentation(self, extremepoints):
         with self.canvas.parent.wait_cursor():
             # do not use fov here because the target image is cropped to network size
             prediction = self.canvas.parent.dl.AssistedSegmentation(self.canvas.parent.getCurrentImage(), np.asarray(extremepoints, dtype = np.int))
             if prediction is None:
                 self.canvas.redrawImage()
```

### Comparing `mianalyzer-0.2.6/mia/ui/painter/ImageLabelPainter.py` & `mianalyzer-0.3.0/mia/ui/painter/ImageLabelPainter.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/painter/ObjectPainter.py` & `mianalyzer-0.3.0/mia/ui/painter/ObjectPainter.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/painter/Painter.py` & `mianalyzer-0.3.0/mia/ui/painter/Painter.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,16 +172,18 @@
         p.setPen(QPen(Qt.NoPen))
         if erase:
             p.setBrush(QBrush(self.canvas.displayedimage.getImage()))
         p.drawEllipse(center, radius, radius)
         self.canvas.updateImage()
 
 
-    def addRectangle(self, x, y, width, height, color = None):
+    def addRectangle(self, x, y, width, height, color = None, filled = True):
         p = self.getPainter(color)
+        if not filled:
+            p.setBrush(Qt.NoBrush)
         p.drawRect(x, y, width, height)
         self.canvas.updateImage()
 
 
     #### contour drawing functions
     def drawcontour(self, contour):   
         painter = self.getPainter()
```

### Comparing `mianalyzer-0.2.6/mia/ui/segmentation/ui_SegPostProcessing.py` & `mianalyzer-0.3.0/mia/ui/segmentation/ui_SegPostProcessing.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/segmentation/ui_SegResults.py` & `mianalyzer-0.3.0/mia/ui/segmentation/ui_SegResults.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/segmentation/ui_SegSettings.py` & `mianalyzer-0.3.0/mia/ui/segmentation/ui_SegSettings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/settings.py` & `mianalyzer-0.3.0/mia/ui/settings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/style.py` & `mianalyzer-0.3.0/mia/ui/style.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Abstract.py` & `mianalyzer-0.3.0/mia/ui/ui_Abstract.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Augment.py` & `mianalyzer-0.3.0/mia/ui/ui_Augment.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Canvas.py` & `mianalyzer-0.3.0/mia/ui/ui_Canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,29 +309,31 @@
         return np.array([p.x(),p.y()])
     
     
     def setnewTool(self, tool):
         self.lasttool = self.tool  
         self.updateImage()
         self.tool.HideSettings()
-        
+
         if tool == canvasTool.drag.name:
             self.tool = Tools.DragTool(self)
         elif tool == canvasTool.draw.name:
             self.tool = Tools.DrawTool(self)
         elif tool == canvasTool.assign.name:
             self.tool = Tools.AssignTool(self)
         elif tool == canvasTool.extend.name:
             self.tool = Tools.ExtendTool(self)
         elif tool == canvasTool.delete.name:
             self.tool = Tools.DeleteTool(self)
         elif tool == canvasTool.poly.name:
             self.tool = Tools.PolygonTool(self)
         elif tool == canvasTool.assist.name:
             self.tool = Tools.DEXTRTool(self)
+        elif tool == canvasTool.sam.name:
+            self.tool = Tools.SAMTool(self)
         elif tool == canvasTool.scale.name:
             self.tool = Tools.ScaleTool(self)
         elif tool == canvasTool.point.name:
             self.tool = Tools.PointTool(self)
         elif tool == canvasTool.shift.name:
             self.tool = Tools.ShiftTool(self)
         elif tool == canvasTool.setimageclass.name:
```

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Log.py` & `mianalyzer-0.3.0/mia/ui/ui_Log.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Results.py` & `mianalyzer-0.3.0/mia/ui/ui_Results.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Settings.py` & `mianalyzer-0.3.0/mia/ui/ui_Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,16 +120,22 @@
         self.CBShapeNumbers.setToolTip('Select to show number below each shape')
         self.CBShapeNumbers.setObjectName('ShowShapeNumbers')
         vlayout.addWidget(self.CBShapeNumbers)
         
         self.CBFastDrawing = QCheckBox("Fast Drawing",self.centralWidget)
         self.CBFastDrawing.setToolTip('Reduces performance needs during drawing. Might be used for large images.')
         self.CBFastDrawing.setObjectName('FastDrawing')
+
+        self.CBInner = QCheckBox("Inner Contours",self.centralWidget)
+        self.CBInner.setToolTip("Check to allow contours to have holes")
+        self.CBInner.setObjectName('InnerContours')
+        self.CBInner.setChecked(True)
+
         vlayout.addWidget(self.CBFastDrawing)
-        
+        vlayout.addWidget(self.CBInner)
 
         self.SBFontSize = LabelledSpinBox('Font Size',self.centralWidget)
         self.SBFontSize.setToolTip('Set font size')
         self.SBFontSize.setObjectName('FontSize')
         self.SBFontSize.SpinBox.setRange(4,32)
         vlayout.addWidget(self.SBFontSize)
 
@@ -173,14 +179,15 @@
         self.SBBorderOverlap.SpinBox.setValue(self.parent.dl.borderremoval)
         self.CBWeightsonly.setChecked(self.parent.saveload_modelweights_only)
         self.CBMixedPrecision.setChecked(self.parent.dl.mixed_precision)
         
         
         self.CBShapeNumbers.stateChanged.connect(self.showContourNumbers)
         self.CBFastDrawing.stateChanged.connect(self.fastDrawing)
+        self.CBInner.stateChanged.connect(self.setInnerContours)
         self.CBSeparateLabels.stateChanged.connect(self.separateLabels)
         self.SBPenSize.SpinBox.valueChanged.connect(self.setPenSize)
         self.SBFontSize.SpinBox.valueChanged.connect(self.setFontSize)
         self.STransparency.valueChanged.connect(self.setTransparency)
         self.CBgpu.currentIndexChanged.connect(self.setGPU)
         self.SBThreads.SpinBox.valueChanged.connect(self.setNumThreads)
         self.SBScaleFactor.SpinBox.valueChanged.connect(self.ScaleFactorChanged)
@@ -255,14 +262,17 @@
     def setPenSize(self):
         self.parent.canvas.pen_size = self.SBPenSize.SpinBox.value()
         self.parent.canvas.redrawImage()
         
     def setFontSize(self):
         self.parent.canvas.FontSize = self.SBFontSize.SpinBox.value()
         self.parent.canvas.redrawImage()
+
+    def setInnerContours(self):
+        self.parent.updateImage()
         
     def setTransparency(self):
         self.parent.canvas.ContourTransparency = self.STransparency.value()
         self.parent.canvas.redrawImage()
         
     def closeEvent(self, event):
         self.parent.canvas.redrawImage()
```

### Comparing `mianalyzer-0.2.6/mia/ui/ui_TrainPlot.py` & `mianalyzer-0.3.0/mia/ui/ui_TrainPlot.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_TrainSettings.py` & `mianalyzer-0.3.0/mia/ui/ui_TrainSettings.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_Training.py` & `mianalyzer-0.3.0/mia/ui/ui_Training.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/ui/ui_utils.py` & `mianalyzer-0.3.0/mia/ui/ui_utils.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/FilesAndFolders.py` & `mianalyzer-0.3.0/mia/utils/FilesAndFolders.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/Image.py` & `mianalyzer-0.3.0/mia/utils/Image.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/Observer.py` & `mianalyzer-0.3.0/mia/utils/Observer.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/postprocessing/tracking.py` & `mianalyzer-0.3.0/mia/utils/postprocessing/tracking.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/shapes/Contour.py` & `mianalyzer-0.3.0/mia/utils/shapes/Contour.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/shapes/ImageLabel.py` & `mianalyzer-0.3.0/mia/utils/shapes/ImageLabel.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/shapes/Point.py` & `mianalyzer-0.3.0/mia/utils/shapes/Point.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/shapes/Shape.py` & `mianalyzer-0.3.0/mia/utils/shapes/Shape.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mia/utils/workerthread.py` & `mianalyzer-0.3.0/mia/utils/workerthread.py`

 * *Files identical despite different names*

### Comparing `mianalyzer-0.2.6/mianalyzer.egg-info/SOURCES.txt` & `mianalyzer-0.3.0/mianalyzer.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,30 @@
 mia/dl/machine_learning/hed.py
 mia/dl/machine_learning/dextr/__init__.py
 mia/dl/machine_learning/dextr/classifiers.py
 mia/dl/machine_learning/dextr/dextr.py
 mia/dl/machine_learning/dextr/dextr_segmentation.py
 mia/dl/machine_learning/dextr/helpers.py
 mia/dl/machine_learning/dextr/resnet.py
+mia/dl/machine_learning/segment_anything/__init__.py
+mia/dl/machine_learning/segment_anything/automatic_mask_generator.py
+mia/dl/machine_learning/segment_anything/build_sam.py
+mia/dl/machine_learning/segment_anything/predictor.py
+mia/dl/machine_learning/segment_anything/sam.py
+mia/dl/machine_learning/segment_anything/modeling/__init__.py
+mia/dl/machine_learning/segment_anything/modeling/common.py
+mia/dl/machine_learning/segment_anything/modeling/image_encoder.py
+mia/dl/machine_learning/segment_anything/modeling/mask_decoder.py
+mia/dl/machine_learning/segment_anything/modeling/prompt_encoder.py
+mia/dl/machine_learning/segment_anything/modeling/sam.py
+mia/dl/machine_learning/segment_anything/modeling/transformer.py
+mia/dl/machine_learning/segment_anything/utils/__init__.py
+mia/dl/machine_learning/segment_anything/utils/amg.py
+mia/dl/machine_learning/segment_anything/utils/onnx.py
+mia/dl/machine_learning/segment_anything/utils/transforms.py
 mia/dl/method/__init__.py
 mia/dl/method/classification.py
 mia/dl/method/mode.py
 mia/dl/method/objectcounting.py
 mia/dl/method/pixelbasedprediction.py
 mia/dl/method/segmentation.py
 mia/dl/method/undefinedmode.py
@@ -102,14 +118,15 @@
 mia/dl/training/augment.py
 mia/dl/training/datagenerator.py
 mia/dl/training/lrschedule.py
 mia/dl/training/training_record.py
 mia/dl/utils/__init__.py
 mia/dl/utils/dl_downloads.py
 mia/dl/utils/dl_utils.py
+mia/icons/__init__.py
 mia/icons/addobject.png
 mia/icons/assign.png
 mia/icons/assignclass.png
 mia/icons/augmentation.png
 mia/icons/clear.png
 mia/icons/delete.png
 mia/icons/dextr.png
@@ -130,16 +147,18 @@
 mia/icons/poly.png
 mia/icons/postprocessing.png
 mia/icons/predict.png
 mia/icons/predictall.png
 mia/icons/previous.png
 mia/icons/reset.png
 mia/icons/results.png
+mia/icons/sam.png
 mia/icons/saveall.png
 mia/icons/savemodel.png
+mia/icons/setallclass.png
 mia/icons/setclass.png
 mia/icons/settings.png
 mia/icons/shift.png
 mia/icons/tracking.png
 mia/icons/train.png
 mia/ui/Tools.py
 mia/ui/UI.py
```

### Comparing `mianalyzer-0.2.6/setup.py` & `mianalyzer-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 	'mia/icons/predictall.png', 
 	'mia/icons/previous.png',
 	'mia/icons/reset.png',
 	'mia/icons/results.png', 
 	'mia/icons/saveall.png',
 	'mia/icons/savemodel.png', 
 	'mia/icons/setclass.png',
+	'mia/icons/setallclass.png',
 	'mia/icons/settings.png', 
 	'mia/icons/shift.png',
 	'mia/icons/tracking.png', 
 	'mia/icons/train.png',
 	'mia/icons/logo.png', 
 	'mia/icons/loading.png', 
 	'mia/dl/machine_learning/deploy.prototxt',
```

