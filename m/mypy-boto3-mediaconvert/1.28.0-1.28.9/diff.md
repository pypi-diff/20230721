# Comparing `tmp/mypy-boto3-mediaconvert-1.28.0.tar.gz` & `tmp/mypy-boto3-mediaconvert-1.28.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediaconvert-1.28.0.tar", last modified: Thu Jul  6 21:00:05 2023, max compression
+gzip compressed data, was "mypy-boto3-mediaconvert-1.28.9.tar", last modified: Fri Jul 21 20:32:58 2023, max compression
```

## Comparing `mypy-boto3-mediaconvert-1.28.0.tar` & `mypy-boto3-mediaconvert-1.28.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.042365 mypy-boto3-mediaconvert-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-06 21:00:05.038365 mypy-boto3-mediaconvert-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31706 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.026365 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55528 2023-07-06 20:46:55.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-07-06 20:46:55.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   103367 2023-07-06 20:47:00.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   103342 2023-07-06 20:46:59.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:46:54.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 21:00:05.038365 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33211 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-06 21:00:04.000000 mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 21:00:05.042365 mypy-boto3-mediaconvert-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-06 20:46:53.000000 mypy-boto3-mediaconvert-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.227903 mypy-boto3-mediaconvert-1.28.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37598 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22513 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22473 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    55551 2023-07-21 20:32:30.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55549 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   171396 2023-07-21 20:32:34.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171379 2023-07-21 20:32:31.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 20:32:28.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 20:32:58.223902 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    39103 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-21 20:32:58.000000 mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 20:32:58.227903 mypy-boto3-mediaconvert-1.28.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-07-21 20:32:27.000000 mypy-boto3-mediaconvert-1.28.9/setup.py
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/LICENSE` & `mypy-boto3-mediaconvert-1.28.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.0/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-mediaconvert
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaConvert 1.28.0 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -743,245 +711,401 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediaconvert.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
+    AccelerationSettingsOutputTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsOutputTypeDef,
     AdvancedInputFilterSettingsTypeDef,
+    AiffSettingsOutputTypeDef,
     AiffSettingsTypeDef,
+    AllowedRenditionSizeOutputTypeDef,
     AllowedRenditionSizeTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
+    AudioChannelTaggingSettingsOutputTypeDef,
     AudioChannelTaggingSettingsTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    Mp3SettingsOutputTypeDef,
+    OpusSettingsOutputTypeDef,
+    VorbisSettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
+    HlsRenditionGroupSettingsOutputTypeDef,
     HlsRenditionGroupSettingsTypeDef,
+    ForceIncludeRenditionSizeOutputTypeDef,
+    MinBottomRenditionSizeOutputTypeDef,
+    MinTopRenditionSizeOutputTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
+    Av1QvbrSettingsOutputTypeDef,
     Av1QvbrSettingsTypeDef,
+    AvailBlankingOutputTypeDef,
     AvailBlankingTypeDef,
+    AvcIntraUhdSettingsOutputTypeDef,
     AvcIntraUhdSettingsTypeDef,
+    BandwidthReductionFilterOutputTypeDef,
     BandwidthReductionFilterTypeDef,
+    BurninDestinationSettingsOutputTypeDef,
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    EmbeddedDestinationSettingsOutputTypeDef,
+    ImscDestinationSettingsOutputTypeDef,
+    SccDestinationSettingsOutputTypeDef,
+    SrtDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
     TeletextDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    CaptionSourceFramerateOutputTypeDef,
     CaptionSourceFramerateTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
+    TrackSourceSettingsOutputTypeDef,
+    WebvttHlsSourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
+    OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
+    ClipLimitsOutputTypeDef,
     ClipLimitsTypeDef,
+    CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
+    SpekeKeyProviderCmafOutputTypeDef,
+    StaticKeyProviderOutputTypeDef,
     SpekeKeyProviderCmafTypeDef,
     StaticKeyProviderTypeDef,
+    CmafImageBasedTrickPlaySettingsOutputTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
+    CmfcSettingsOutputTypeDef,
     CmfcSettingsTypeDef,
+    Hdr10MetadataOutputTypeDef,
     Hdr10MetadataTypeDef,
+    F4vSettingsOutputTypeDef,
+    M3u8SettingsOutputTypeDef,
+    MovSettingsOutputTypeDef,
+    Mp4SettingsOutputTypeDef,
+    MpdSettingsOutputTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
+    DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
+    DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
+    DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
+    DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
+    DvbSdtSettingsOutputTypeDef,
     DvbSdtSettingsTypeDef,
+    DvbTdtSettingsOutputTypeDef,
     DvbTdtSettingsTypeDef,
+    EsamManifestConfirmConditionNotificationOutputTypeDef,
     EsamManifestConfirmConditionNotificationTypeDef,
+    EsamSignalProcessingNotificationOutputTypeDef,
     EsamSignalProcessingNotificationTypeDef,
+    ExtendedDataServicesOutputTypeDef,
     ExtendedDataServicesTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobTemplateRequestRequestTypeDef,
-    PolicyTypeDef,
+    PolicyOutputTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
+    H264QvbrSettingsOutputTypeDef,
     H264QvbrSettingsTypeDef,
+    H265QvbrSettingsOutputTypeDef,
     H265QvbrSettingsTypeDef,
+    Hdr10PlusOutputTypeDef,
     Hdr10PlusTypeDef,
+    HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
+    HlsCaptionLanguageMappingOutputTypeDef,
     HlsCaptionLanguageMappingTypeDef,
+    HlsImageBasedTrickPlaySettingsOutputTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
+    HopDestinationOutputTypeDef,
+    Id3InsertionOutputTypeDef,
     Id3InsertionTypeDef,
+    InsertableImageOutputTypeDef,
     InsertableImageTypeDef,
+    InputClippingOutputTypeDef,
     InputClippingTypeDef,
+    InputDecryptionSettingsOutputTypeDef,
     InputDecryptionSettingsTypeDef,
+    InputVideoGeneratorOutputTypeDef,
+    RectangleOutputTypeDef,
     RectangleTypeDef,
     InputVideoGeneratorTypeDef,
     JobMessagesTypeDef,
+    KantarWatermarkSettingsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    NielsenNonLinearWatermarkSettingsOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
+    M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
+    MotionImageInsertionFramerateOutputTypeDef,
+    MotionImageInsertionOffsetOutputTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     Mpeg2SettingsTypeDef,
+    MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
+    MxfXavcProfileSettingsOutputTypeDef,
     MxfXavcProfileSettingsTypeDef,
+    NexGuardFileMarkerSettingsOutputTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
+    NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
+    NoiseReducerSpatialFilterSettingsOutputTypeDef,
+    NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
+    PolicyTypeDef,
+    ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
+    S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
+    S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
+    Vc3SettingsOutputTypeDef,
     Vc3SettingsTypeDef,
+    Vp8SettingsOutputTypeDef,
+    Vp9SettingsOutputTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
+    Xavc4kIntraCbgProfileSettingsOutputTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
+    Xavc4kIntraVbrProfileSettingsOutputTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
+    Xavc4kProfileSettingsOutputTypeDef,
     Xavc4kProfileSettingsTypeDef,
+    XavcHdIntraCbgProfileSettingsOutputTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
+    XavcHdProfileSettingsOutputTypeDef,
     XavcHdProfileSettingsTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
+    AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
+    Av1SettingsOutputTypeDef,
     Av1SettingsTypeDef,
+    AvcIntraSettingsOutputTypeDef,
     AvcIntraSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
+    FileSourceSettingsOutputTypeDef,
     FileSourceSettingsTypeDef,
+    ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
+    CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
+    ColorCorrectorOutputTypeDef,
+    VideoSelectorOutputTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
+    DashIsoEncryptionSettingsOutputTypeDef,
+    HlsEncryptionSettingsOutputTypeDef,
+    MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
+    DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
+    EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    H264SettingsOutputTypeDef,
     H264SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
+    TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
+    ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
+    M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
+    MotionImageInserterOutputTypeDef,
     MotionImageInserterTypeDef,
+    MxfSettingsOutputTypeDef,
     MxfSettingsTypeDef,
+    PartnerWatermarkingOutputTypeDef,
     PartnerWatermarkingTypeDef,
+    NoiseReducerOutputTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
+    PutPolicyRequestRequestTypeDef,
     QueueTypeDef,
+    S3DestinationSettingsOutputTypeDef,
     S3DestinationSettingsTypeDef,
+    XavcSettingsOutputTypeDef,
     XavcSettingsTypeDef,
+    AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionOutputTypeDef,
+    CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
-    CaptionDescriptionTypeDef,
+    CaptionSourceSettingsOutputTypeDef,
     CaptionSourceSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
+    VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
+    DestinationSettingsOutputTypeDef,
     DestinationSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
+    AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
+    AudioDescriptionOutputTypeDef,
+    AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
+    CmafGroupSettingsOutputTypeDef,
+    DashIsoGroupSettingsOutputTypeDef,
+    FileGroupSettingsOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
     CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
     HlsGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
+    InputOutputTypeDef,
+    InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     OutputTypeDef,
+    PresetSettingsOutputTypeDef,
     PresetSettingsTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
+    CreatePresetRequestRequestTypeDef,
     UpdatePresetRequestRequestTypeDef,
+    JobSettingsOutputTypeDef,
+    JobTemplateSettingsOutputTypeDef,
     JobSettingsTypeDef,
     JobTemplateSettingsTypeDef,
     CreatePresetResponseTypeDef,
     GetPresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     UpdatePresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobRequestRequestTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/README.md` & `mypy-boto3-mediaconvert-1.28.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-mediaconvert
+Version: 1.28.9
+Summary: Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder 7.15.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 mediaconvert type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-mediaconvert"></a>
 
 # mypy-boto3-mediaconvert
 
 [![PyPI - mypy-boto3-mediaconvert](https://img.shields.io/pypi/v/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -711,245 +743,401 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediaconvert.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
+    AccelerationSettingsOutputTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsOutputTypeDef,
     AdvancedInputFilterSettingsTypeDef,
+    AiffSettingsOutputTypeDef,
     AiffSettingsTypeDef,
+    AllowedRenditionSizeOutputTypeDef,
     AllowedRenditionSizeTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
+    AudioChannelTaggingSettingsOutputTypeDef,
     AudioChannelTaggingSettingsTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    Mp3SettingsOutputTypeDef,
+    OpusSettingsOutputTypeDef,
+    VorbisSettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
+    HlsRenditionGroupSettingsOutputTypeDef,
     HlsRenditionGroupSettingsTypeDef,
+    ForceIncludeRenditionSizeOutputTypeDef,
+    MinBottomRenditionSizeOutputTypeDef,
+    MinTopRenditionSizeOutputTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
+    Av1QvbrSettingsOutputTypeDef,
     Av1QvbrSettingsTypeDef,
+    AvailBlankingOutputTypeDef,
     AvailBlankingTypeDef,
+    AvcIntraUhdSettingsOutputTypeDef,
     AvcIntraUhdSettingsTypeDef,
+    BandwidthReductionFilterOutputTypeDef,
     BandwidthReductionFilterTypeDef,
+    BurninDestinationSettingsOutputTypeDef,
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    EmbeddedDestinationSettingsOutputTypeDef,
+    ImscDestinationSettingsOutputTypeDef,
+    SccDestinationSettingsOutputTypeDef,
+    SrtDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
     TeletextDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    CaptionSourceFramerateOutputTypeDef,
     CaptionSourceFramerateTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
+    TrackSourceSettingsOutputTypeDef,
+    WebvttHlsSourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
+    OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
+    ClipLimitsOutputTypeDef,
     ClipLimitsTypeDef,
+    CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
+    SpekeKeyProviderCmafOutputTypeDef,
+    StaticKeyProviderOutputTypeDef,
     SpekeKeyProviderCmafTypeDef,
     StaticKeyProviderTypeDef,
+    CmafImageBasedTrickPlaySettingsOutputTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
+    CmfcSettingsOutputTypeDef,
     CmfcSettingsTypeDef,
+    Hdr10MetadataOutputTypeDef,
     Hdr10MetadataTypeDef,
+    F4vSettingsOutputTypeDef,
+    M3u8SettingsOutputTypeDef,
+    MovSettingsOutputTypeDef,
+    Mp4SettingsOutputTypeDef,
+    MpdSettingsOutputTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
+    DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
+    DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
+    DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
+    DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
+    DvbSdtSettingsOutputTypeDef,
     DvbSdtSettingsTypeDef,
+    DvbTdtSettingsOutputTypeDef,
     DvbTdtSettingsTypeDef,
+    EsamManifestConfirmConditionNotificationOutputTypeDef,
     EsamManifestConfirmConditionNotificationTypeDef,
+    EsamSignalProcessingNotificationOutputTypeDef,
     EsamSignalProcessingNotificationTypeDef,
+    ExtendedDataServicesOutputTypeDef,
     ExtendedDataServicesTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobTemplateRequestRequestTypeDef,
-    PolicyTypeDef,
+    PolicyOutputTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
+    H264QvbrSettingsOutputTypeDef,
     H264QvbrSettingsTypeDef,
+    H265QvbrSettingsOutputTypeDef,
     H265QvbrSettingsTypeDef,
+    Hdr10PlusOutputTypeDef,
     Hdr10PlusTypeDef,
+    HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
+    HlsCaptionLanguageMappingOutputTypeDef,
     HlsCaptionLanguageMappingTypeDef,
+    HlsImageBasedTrickPlaySettingsOutputTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
+    HopDestinationOutputTypeDef,
+    Id3InsertionOutputTypeDef,
     Id3InsertionTypeDef,
+    InsertableImageOutputTypeDef,
     InsertableImageTypeDef,
+    InputClippingOutputTypeDef,
     InputClippingTypeDef,
+    InputDecryptionSettingsOutputTypeDef,
     InputDecryptionSettingsTypeDef,
+    InputVideoGeneratorOutputTypeDef,
+    RectangleOutputTypeDef,
     RectangleTypeDef,
     InputVideoGeneratorTypeDef,
     JobMessagesTypeDef,
+    KantarWatermarkSettingsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    NielsenNonLinearWatermarkSettingsOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
+    M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
+    MotionImageInsertionFramerateOutputTypeDef,
+    MotionImageInsertionOffsetOutputTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     Mpeg2SettingsTypeDef,
+    MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
+    MxfXavcProfileSettingsOutputTypeDef,
     MxfXavcProfileSettingsTypeDef,
+    NexGuardFileMarkerSettingsOutputTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
+    NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
+    NoiseReducerSpatialFilterSettingsOutputTypeDef,
+    NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
+    PolicyTypeDef,
+    ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
+    S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
+    S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
+    Vc3SettingsOutputTypeDef,
     Vc3SettingsTypeDef,
+    Vp8SettingsOutputTypeDef,
+    Vp9SettingsOutputTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
+    Xavc4kIntraCbgProfileSettingsOutputTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
+    Xavc4kIntraVbrProfileSettingsOutputTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
+    Xavc4kProfileSettingsOutputTypeDef,
     Xavc4kProfileSettingsTypeDef,
+    XavcHdIntraCbgProfileSettingsOutputTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
+    XavcHdProfileSettingsOutputTypeDef,
     XavcHdProfileSettingsTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
+    AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
+    Av1SettingsOutputTypeDef,
     Av1SettingsTypeDef,
+    AvcIntraSettingsOutputTypeDef,
     AvcIntraSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
+    FileSourceSettingsOutputTypeDef,
     FileSourceSettingsTypeDef,
+    ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
+    CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
+    ColorCorrectorOutputTypeDef,
+    VideoSelectorOutputTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
+    DashIsoEncryptionSettingsOutputTypeDef,
+    HlsEncryptionSettingsOutputTypeDef,
+    MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
+    DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
+    EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    H264SettingsOutputTypeDef,
     H264SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
+    TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
+    ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
+    M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
+    MotionImageInserterOutputTypeDef,
     MotionImageInserterTypeDef,
+    MxfSettingsOutputTypeDef,
     MxfSettingsTypeDef,
+    PartnerWatermarkingOutputTypeDef,
     PartnerWatermarkingTypeDef,
+    NoiseReducerOutputTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
+    PutPolicyRequestRequestTypeDef,
     QueueTypeDef,
+    S3DestinationSettingsOutputTypeDef,
     S3DestinationSettingsTypeDef,
+    XavcSettingsOutputTypeDef,
     XavcSettingsTypeDef,
+    AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionOutputTypeDef,
+    CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
-    CaptionDescriptionTypeDef,
+    CaptionSourceSettingsOutputTypeDef,
     CaptionSourceSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
+    VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
+    DestinationSettingsOutputTypeDef,
     DestinationSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
+    AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
+    AudioDescriptionOutputTypeDef,
+    AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
+    CmafGroupSettingsOutputTypeDef,
+    DashIsoGroupSettingsOutputTypeDef,
+    FileGroupSettingsOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
     CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
     HlsGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
+    InputOutputTypeDef,
+    InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     OutputTypeDef,
+    PresetSettingsOutputTypeDef,
     PresetSettingsTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
+    CreatePresetRequestRequestTypeDef,
     UpdatePresetRequestRequestTypeDef,
+    JobSettingsOutputTypeDef,
+    JobTemplateSettingsOutputTypeDef,
     JobSettingsTypeDef,
     JobTemplateSettingsTypeDef,
     CreatePresetResponseTypeDef,
     GetPresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     UpdatePresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobRequestRequestTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__init__.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/__main__.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaConvert 1.28.0\nVersion:         1.28.0\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.MediaConvert 1.28.9\nVersion:         1.28.9\nBuilder version:"
+        " 7.15.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/client.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1511,14 +1511,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/literals.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1509,14 +1509,15 @@
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 
@@ -93,15 +93,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -113,15 +113,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobspaginator)
         """
 
 
@@ -133,15 +133,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listpresetspaginator)
         """
 
 
@@ -152,13 +152,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/paginator.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
     """
 
     def paginate(
         self,
         *,
         Mode: DescribeEndpointsModeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEndpointsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#describeendpointspaginator)
         """
 
 class ListJobTemplatesPaginator(Paginator):
@@ -89,15 +89,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: JobTemplateListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -108,15 +108,15 @@
 
     def paginate(
         self,
         *,
         Order: OrderType = ...,
         Queue: str = ...,
         Status: JobStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listjobspaginator)
         """
 
 class ListPresetsPaginator(Paginator):
@@ -127,15 +127,15 @@
 
     def paginate(
         self,
         *,
         Category: str = ...,
         ListBy: PresetListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listpresetspaginator)
         """
 
 class ListQueuesPaginator(Paginator):
@@ -145,13 +145,13 @@
     """
 
     def paginate(
         self,
         *,
         ListBy: QueueListByType = ...,
         Order: OrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.py` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediaconvert service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediaconvert.type_defs import AacSettingsTypeDef
+    from mypy_boto3_mediaconvert.type_defs import AacSettingsOutputTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -428,243 +428,414 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
+    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
+    "AccelerationSettingsOutputTypeDef",
     "AccelerationSettingsTypeDef",
+    "AdvancedInputFilterSettingsOutputTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
+    "AiffSettingsOutputTypeDef",
     "AiffSettingsTypeDef",
+    "AllowedRenditionSizeOutputTypeDef",
     "AllowedRenditionSizeTypeDef",
+    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
     "AssociateCertificateRequestRequestTypeDef",
+    "AudioChannelTaggingSettingsOutputTypeDef",
     "AudioChannelTaggingSettingsTypeDef",
+    "Eac3AtmosSettingsOutputTypeDef",
+    "Eac3SettingsOutputTypeDef",
+    "Mp2SettingsOutputTypeDef",
+    "Mp3SettingsOutputTypeDef",
+    "OpusSettingsOutputTypeDef",
+    "VorbisSettingsOutputTypeDef",
+    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
+    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
+    "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
+    "HlsRenditionGroupSettingsOutputTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    "MinBottomRenditionSizeOutputTypeDef",
+    "MinTopRenditionSizeOutputTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
+    "Av1QvbrSettingsOutputTypeDef",
     "Av1QvbrSettingsTypeDef",
+    "AvailBlankingOutputTypeDef",
     "AvailBlankingTypeDef",
+    "AvcIntraUhdSettingsOutputTypeDef",
     "AvcIntraUhdSettingsTypeDef",
+    "BandwidthReductionFilterOutputTypeDef",
     "BandwidthReductionFilterTypeDef",
+    "BurninDestinationSettingsOutputTypeDef",
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
+    "DvbSubDestinationSettingsOutputTypeDef",
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    "ImscDestinationSettingsOutputTypeDef",
+    "SccDestinationSettingsOutputTypeDef",
+    "SrtDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsOutputTypeDef",
+    "TtmlDestinationSettingsOutputTypeDef",
+    "WebvttDestinationSettingsOutputTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
     "TeletextDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
+    "CaptionSourceFramerateOutputTypeDef",
     "CaptionSourceFramerateTypeDef",
+    "DvbSubSourceSettingsOutputTypeDef",
+    "EmbeddedSourceSettingsOutputTypeDef",
+    "TeletextSourceSettingsOutputTypeDef",
+    "TrackSourceSettingsOutputTypeDef",
+    "WebvttHlsSourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
+    "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
+    "ClipLimitsOutputTypeDef",
     "ClipLimitsTypeDef",
+    "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
+    "SpekeKeyProviderCmafOutputTypeDef",
+    "StaticKeyProviderOutputTypeDef",
     "SpekeKeyProviderCmafTypeDef",
     "StaticKeyProviderTypeDef",
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
+    "CmfcSettingsOutputTypeDef",
     "CmfcSettingsTypeDef",
+    "Hdr10MetadataOutputTypeDef",
     "Hdr10MetadataTypeDef",
+    "F4vSettingsOutputTypeDef",
+    "M3u8SettingsOutputTypeDef",
+    "MovSettingsOutputTypeDef",
+    "Mp4SettingsOutputTypeDef",
+    "MpdSettingsOutputTypeDef",
     "F4vSettingsTypeDef",
     "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
     "HopDestinationTypeDef",
+    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
+    "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
+    "DeinterlacerOutputTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
+    "DolbyVisionLevel6MetadataOutputTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
+    "DvbNitSettingsOutputTypeDef",
     "DvbNitSettingsTypeDef",
+    "DvbSdtSettingsOutputTypeDef",
     "DvbSdtSettingsTypeDef",
+    "DvbTdtSettingsOutputTypeDef",
     "DvbTdtSettingsTypeDef",
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
     "EsamManifestConfirmConditionNotificationTypeDef",
+    "EsamSignalProcessingNotificationOutputTypeDef",
     "EsamSignalProcessingNotificationTypeDef",
+    "ExtendedDataServicesOutputTypeDef",
     "ExtendedDataServicesTypeDef",
+    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetJobTemplateRequestRequestTypeDef",
-    "PolicyTypeDef",
+    "PolicyOutputTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
+    "H264QvbrSettingsOutputTypeDef",
     "H264QvbrSettingsTypeDef",
+    "H265QvbrSettingsOutputTypeDef",
     "H265QvbrSettingsTypeDef",
+    "Hdr10PlusOutputTypeDef",
     "Hdr10PlusTypeDef",
+    "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
+    "HlsCaptionLanguageMappingOutputTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
-    "HlsSettingsTypeDef",
+    "HlsSettingsOutputTypeDef",
+    "HopDestinationOutputTypeDef",
+    "Id3InsertionOutputTypeDef",
     "Id3InsertionTypeDef",
+    "InsertableImageOutputTypeDef",
     "InsertableImageTypeDef",
+    "InputClippingOutputTypeDef",
     "InputClippingTypeDef",
+    "InputDecryptionSettingsOutputTypeDef",
     "InputDecryptionSettingsTypeDef",
+    "InputVideoGeneratorOutputTypeDef",
+    "RectangleOutputTypeDef",
     "RectangleTypeDef",
     "InputVideoGeneratorTypeDef",
     "JobMessagesTypeDef",
+    "KantarWatermarkSettingsOutputTypeDef",
+    "NielsenConfigurationOutputTypeDef",
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    "TimecodeConfigOutputTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
+    "M2tsScte35EsamOutputTypeDef",
     "M2tsScte35EsamTypeDef",
+    "MotionImageInsertionFramerateOutputTypeDef",
+    "MotionImageInsertionOffsetOutputTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
+    "Mpeg2SettingsOutputTypeDef",
     "Mpeg2SettingsTypeDef",
+    "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
+    "MxfXavcProfileSettingsOutputTypeDef",
     "MxfXavcProfileSettingsTypeDef",
+    "NexGuardFileMarkerSettingsOutputTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
+    "NoiseReducerFilterSettingsOutputTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
-    "PaginatorConfigTypeDef",
+    "PolicyTypeDef",
+    "ProresSettingsOutputTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3DestinationAccessControlOutputTypeDef",
     "S3DestinationAccessControlTypeDef",
+    "S3EncryptionSettingsOutputTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TimecodeBurninOutputTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "Vc3SettingsOutputTypeDef",
     "Vc3SettingsTypeDef",
+    "Vp8SettingsOutputTypeDef",
+    "Vp9SettingsOutputTypeDef",
     "Vp8SettingsTypeDef",
     "Vp9SettingsTypeDef",
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
+    "Xavc4kProfileSettingsOutputTypeDef",
     "Xavc4kProfileSettingsTypeDef",
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
+    "XavcHdProfileSettingsOutputTypeDef",
     "XavcHdProfileSettingsTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
+    "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
+    "Av1SettingsOutputTypeDef",
     "Av1SettingsTypeDef",
+    "AvcIntraSettingsOutputTypeDef",
     "AvcIntraSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
+    "FileSourceSettingsOutputTypeDef",
     "FileSourceSettingsTypeDef",
+    "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
+    "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
+    "ColorCorrectorOutputTypeDef",
+    "VideoSelectorOutputTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    "HlsEncryptionSettingsOutputTypeDef",
+    "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "DolbyVisionOutputTypeDef",
     "DolbyVisionTypeDef",
+    "EsamSettingsOutputTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "OutputSettingsTypeDef",
+    "OutputSettingsOutputTypeDef",
+    "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
+    "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
+    "MotionImageInserterOutputTypeDef",
     "MotionImageInserterTypeDef",
+    "MxfSettingsOutputTypeDef",
     "MxfSettingsTypeDef",
+    "PartnerWatermarkingOutputTypeDef",
     "PartnerWatermarkingTypeDef",
+    "NoiseReducerOutputTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "QueueTypeDef",
+    "S3DestinationSettingsOutputTypeDef",
     "S3DestinationSettingsTypeDef",
+    "XavcSettingsOutputTypeDef",
     "XavcSettingsTypeDef",
+    "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
+    "CaptionDescriptionOutputTypeDef",
+    "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
-    "CaptionDescriptionTypeDef",
+    "CaptionSourceSettingsOutputTypeDef",
     "CaptionSourceSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
+    "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
+    "DestinationSettingsOutputTypeDef",
     "DestinationSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
+    "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
+    "AudioDescriptionOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
+    "CmafGroupSettingsOutputTypeDef",
+    "DashIsoGroupSettingsOutputTypeDef",
+    "FileGroupSettingsOutputTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
     "CmafGroupSettingsTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
     "HlsGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
+    "InputOutputTypeDef",
+    "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
     "OutputTypeDef",
+    "PresetSettingsOutputTypeDef",
     "PresetSettingsTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
-    "CreatePresetRequestRequestTypeDef",
     "PresetTypeDef",
+    "CreatePresetRequestRequestTypeDef",
     "UpdatePresetRequestRequestTypeDef",
+    "JobSettingsOutputTypeDef",
+    "JobTemplateSettingsOutputTypeDef",
     "JobSettingsTypeDef",
     "JobTemplateSettingsTypeDef",
     "CreatePresetResponseTypeDef",
     "GetPresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "UpdatePresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "UpdateJobTemplateResponseTypeDef",
 )
 
+AacSettingsOutputTypeDef = TypedDict(
+    "AacSettingsOutputTypeDef",
+    {
+        "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
+        "Bitrate": int,
+        "CodecProfile": AacCodecProfileType,
+        "CodingMode": AacCodingModeType,
+        "RateControlMode": AacRateControlModeType,
+        "RawFormat": AacRawFormatType,
+        "SampleRate": int,
+        "Specification": AacSpecificationType,
+        "VbrQuality": AacVbrQualityType,
+    },
+)
+
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
         "Bitrate": int,
         "CodecProfile": AacCodecProfileType,
         "CodingMode": AacCodingModeType,
@@ -673,14 +844,30 @@
         "SampleRate": int,
         "Specification": AacSpecificationType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
+Ac3SettingsOutputTypeDef = TypedDict(
+    "Ac3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Ac3BitstreamModeType,
+        "CodingMode": Ac3CodingModeType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Ac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionProfile": Ac3DynamicRangeCompressionProfileType,
+        "DynamicRangeCompressionRf": Ac3DynamicRangeCompressionRfType,
+        "LfeFilter": Ac3LfeFilterType,
+        "MetadataControl": Ac3MetadataControlType,
+        "SampleRate": int,
+    },
+)
+
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -690,50 +877,92 @@
         "LfeFilter": Ac3LfeFilterType,
         "MetadataControl": Ac3MetadataControlType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AccelerationSettingsOutputTypeDef = TypedDict(
+    "AccelerationSettingsOutputTypeDef",
+    {
+        "Mode": AccelerationModeType,
+    },
+)
+
 AccelerationSettingsTypeDef = TypedDict(
     "AccelerationSettingsTypeDef",
     {
         "Mode": AccelerationModeType,
     },
 )
 
+AdvancedInputFilterSettingsOutputTypeDef = TypedDict(
+    "AdvancedInputFilterSettingsOutputTypeDef",
+    {
+        "AddTexture": AdvancedInputFilterAddTextureType,
+        "Sharpening": AdvancedInputFilterSharpenType,
+    },
+)
+
 AdvancedInputFilterSettingsTypeDef = TypedDict(
     "AdvancedInputFilterSettingsTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
     },
     total=False,
 )
 
+AiffSettingsOutputTypeDef = TypedDict(
+    "AiffSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
     total=False,
 )
 
+AllowedRenditionSizeOutputTypeDef = TypedDict(
+    "AllowedRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Required": RequiredFlagType,
+        "Width": int,
+    },
+)
+
 AllowedRenditionSizeTypeDef = TypedDict(
     "AllowedRenditionSizeTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
         "Width": int,
     },
     total=False,
 )
 
+AncillarySourceSettingsOutputTypeDef = TypedDict(
+    "AncillarySourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": AncillaryConvert608To708Type,
+        "SourceAncillaryChannelNumber": int,
+        "TerminateCaptions": AncillaryTerminateCaptionsType,
+    },
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
         "TerminateCaptions": AncillaryTerminateCaptionsType,
     },
@@ -743,22 +972,127 @@
 AssociateCertificateRequestRequestTypeDef = TypedDict(
     "AssociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+AudioChannelTaggingSettingsOutputTypeDef = TypedDict(
+    "AudioChannelTaggingSettingsOutputTypeDef",
+    {
+        "ChannelTag": AudioChannelTagType,
+    },
+)
+
 AudioChannelTaggingSettingsTypeDef = TypedDict(
     "AudioChannelTaggingSettingsTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
     total=False,
 )
 
+Eac3AtmosSettingsOutputTypeDef = TypedDict(
+    "Eac3AtmosSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Literal["COMPLETE_MAIN"],
+        "CodingMode": Eac3AtmosCodingModeType,
+        "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
+        "DownmixControl": Eac3AtmosDownmixControlType,
+        "DynamicRangeCompressionLine": Eac3AtmosDynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3AtmosDynamicRangeCompressionRfType,
+        "DynamicRangeControl": Eac3AtmosDynamicRangeControlType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MeteringMode": Eac3AtmosMeteringModeType,
+        "SampleRate": int,
+        "SpeechThreshold": int,
+        "StereoDownmix": Eac3AtmosStereoDownmixType,
+        "SurroundExMode": Eac3AtmosSurroundExModeType,
+    },
+)
+
+Eac3SettingsOutputTypeDef = TypedDict(
+    "Eac3SettingsOutputTypeDef",
+    {
+        "AttenuationControl": Eac3AttenuationControlType,
+        "Bitrate": int,
+        "BitstreamMode": Eac3BitstreamModeType,
+        "CodingMode": Eac3CodingModeType,
+        "DcFilter": Eac3DcFilterType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Eac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3DynamicRangeCompressionRfType,
+        "LfeControl": Eac3LfeControlType,
+        "LfeFilter": Eac3LfeFilterType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MetadataControl": Eac3MetadataControlType,
+        "PassthroughControl": Eac3PassthroughControlType,
+        "PhaseControl": Eac3PhaseControlType,
+        "SampleRate": int,
+        "StereoDownmix": Eac3StereoDownmixType,
+        "SurroundExMode": Eac3SurroundExModeType,
+        "SurroundMode": Eac3SurroundModeType,
+    },
+)
+
+Mp2SettingsOutputTypeDef = TypedDict(
+    "Mp2SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+Mp3SettingsOutputTypeDef = TypedDict(
+    "Mp3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "RateControlMode": Mp3RateControlModeType,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+OpusSettingsOutputTypeDef = TypedDict(
+    "OpusSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+VorbisSettingsOutputTypeDef = TypedDict(
+    "VorbisSettingsOutputTypeDef",
+    {
+        "Channels": int,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+WavSettingsOutputTypeDef = TypedDict(
+    "WavSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "Format": WavFormatType,
+        "SampleRate": int,
+    },
+)
+
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Literal["COMPLETE_MAIN"],
         "CodingMode": Eac3AtmosCodingModeType,
         "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
@@ -856,46 +1190,99 @@
         "Channels": int,
         "Format": WavFormatType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AudioNormalizationSettingsOutputTypeDef = TypedDict(
+    "AudioNormalizationSettingsOutputTypeDef",
+    {
+        "Algorithm": AudioNormalizationAlgorithmType,
+        "AlgorithmControl": AudioNormalizationAlgorithmControlType,
+        "CorrectionGateLevel": int,
+        "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
+        "PeakCalculation": AudioNormalizationPeakCalculationType,
+        "TargetLkfs": float,
+        "TruePeakLimiterThreshold": float,
+    },
+)
+
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
         "CorrectionGateLevel": int,
         "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
     total=False,
 )
 
+AudioSelectorGroupOutputTypeDef = TypedDict(
+    "AudioSelectorGroupOutputTypeDef",
+    {
+        "AudioSelectorNames": List[str],
+    },
+)
+
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
 
+HlsRenditionGroupSettingsOutputTypeDef = TypedDict(
+    "HlsRenditionGroupSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 HlsRenditionGroupSettingsTypeDef = TypedDict(
     "HlsRenditionGroupSettingsTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+ForceIncludeRenditionSizeOutputTypeDef = TypedDict(
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinBottomRenditionSizeOutputTypeDef = TypedDict(
+    "MinBottomRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinTopRenditionSizeOutputTypeDef = TypedDict(
+    "MinTopRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
 ForceIncludeRenditionSizeTypeDef = TypedDict(
     "ForceIncludeRenditionSizeTypeDef",
     {
         "Height": int,
         "Width": int,
     },
     total=False,
@@ -915,48 +1302,105 @@
     {
         "Height": int,
         "Width": int,
     },
     total=False,
 )
 
+Av1QvbrSettingsOutputTypeDef = TypedDict(
+    "Av1QvbrSettingsOutputTypeDef",
+    {
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 Av1QvbrSettingsTypeDef = TypedDict(
     "Av1QvbrSettingsTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+AvailBlankingOutputTypeDef = TypedDict(
+    "AvailBlankingOutputTypeDef",
+    {
+        "AvailBlankingImage": str,
+    },
+)
+
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": str,
     },
     total=False,
 )
 
+AvcIntraUhdSettingsOutputTypeDef = TypedDict(
+    "AvcIntraUhdSettingsOutputTypeDef",
+    {
+        "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
+    },
+)
+
 AvcIntraUhdSettingsTypeDef = TypedDict(
     "AvcIntraUhdSettingsTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
     total=False,
 )
 
+BandwidthReductionFilterOutputTypeDef = TypedDict(
+    "BandwidthReductionFilterOutputTypeDef",
+    {
+        "Sharpening": BandwidthReductionFilterSharpeningType,
+        "Strength": BandwidthReductionFilterStrengthType,
+    },
+)
+
 BandwidthReductionFilterTypeDef = TypedDict(
     "BandwidthReductionFilterTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
     },
     total=False,
 )
 
+BurninDestinationSettingsOutputTypeDef = TypedDict(
+    "BurninDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": BurninSubtitleAlignmentType,
+        "ApplyFontColor": BurninSubtitleApplyFontColorType,
+        "BackgroundColor": BurninSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "FallbackFont": BurninSubtitleFallbackFontType,
+        "FontColor": BurninSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "HexFontColor": str,
+        "OutlineColor": BurninSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": BurninSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": BurnInSubtitleStylePassthroughType,
+        "TeletextSpacing": BurninSubtitleTeletextSpacingType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
 BurninDestinationSettingsTypeDef = TypedDict(
     "BurninDestinationSettingsTypeDef",
     {
         "Alignment": BurninSubtitleAlignmentType,
         "ApplyFontColor": BurninSubtitleApplyFontColorType,
         "BackgroundColor": BurninSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -984,14 +1428,100 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DvbSubDestinationSettingsOutputTypeDef = TypedDict(
+    "DvbSubDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": DvbSubtitleAlignmentType,
+        "ApplyFontColor": DvbSubtitleApplyFontColorType,
+        "BackgroundColor": DvbSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "DdsHandling": DvbddsHandlingType,
+        "DdsXCoordinate": int,
+        "DdsYCoordinate": int,
+        "FallbackFont": DvbSubSubtitleFallbackFontType,
+        "FontColor": DvbSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "Height": int,
+        "HexFontColor": str,
+        "OutlineColor": DvbSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": DvbSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": DvbSubtitleStylePassthroughType,
+        "SubtitlingType": DvbSubtitlingTypeType,
+        "TeletextSpacing": DvbSubtitleTeletextSpacingType,
+        "Width": int,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
+EmbeddedDestinationSettingsOutputTypeDef = TypedDict(
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    {
+        "Destination608ChannelNumber": int,
+        "Destination708ServiceNumber": int,
+    },
+)
+
+ImscDestinationSettingsOutputTypeDef = TypedDict(
+    "ImscDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": ImscAccessibilitySubsType,
+        "StylePassthrough": ImscStylePassthroughType,
+    },
+)
+
+SccDestinationSettingsOutputTypeDef = TypedDict(
+    "SccDestinationSettingsOutputTypeDef",
+    {
+        "Framerate": SccDestinationFramerateType,
+    },
+)
+
+SrtDestinationSettingsOutputTypeDef = TypedDict(
+    "SrtDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": SrtStylePassthroughType,
+    },
+)
+
+TeletextDestinationSettingsOutputTypeDef = TypedDict(
+    "TeletextDestinationSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+        "PageTypes": List[TeletextPageTypeType],
+    },
+)
+
+TtmlDestinationSettingsOutputTypeDef = TypedDict(
+    "TtmlDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": TtmlStylePassthroughType,
+    },
+)
+
+WebvttDestinationSettingsOutputTypeDef = TypedDict(
+    "WebvttDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": WebvttAccessibilitySubsType,
+        "StylePassthrough": WebvttStylePassthroughType,
+    },
+)
+
 DvbSubDestinationSettingsTypeDef = TypedDict(
     "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubtitleAlignmentType,
         "ApplyFontColor": DvbSubtitleApplyFontColorType,
         "BackgroundColor": DvbSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -1078,23 +1608,71 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
+CaptionSourceFramerateOutputTypeDef = TypedDict(
+    "CaptionSourceFramerateOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
 )
 
+DvbSubSourceSettingsOutputTypeDef = TypedDict(
+    "DvbSubSourceSettingsOutputTypeDef",
+    {
+        "Pid": int,
+    },
+)
+
+EmbeddedSourceSettingsOutputTypeDef = TypedDict(
+    "EmbeddedSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": EmbeddedConvert608To708Type,
+        "Source608ChannelNumber": int,
+        "Source608TrackNumber": int,
+        "TerminateCaptions": EmbeddedTerminateCaptionsType,
+    },
+)
+
+TeletextSourceSettingsOutputTypeDef = TypedDict(
+    "TeletextSourceSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+    },
+)
+
+TrackSourceSettingsOutputTypeDef = TypedDict(
+    "TrackSourceSettingsOutputTypeDef",
+    {
+        "TrackNumber": int,
+    },
+)
+
+WebvttHlsSourceSettingsOutputTypeDef = TypedDict(
+    "WebvttHlsSourceSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
@@ -1132,43 +1710,90 @@
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+OutputChannelMappingOutputTypeDef = TypedDict(
+    "OutputChannelMappingOutputTypeDef",
+    {
+        "InputChannels": List[int],
+        "InputChannelsFineTune": List[float],
+    },
+)
+
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
 )
 
+ClipLimitsOutputTypeDef = TypedDict(
+    "ClipLimitsOutputTypeDef",
+    {
+        "MaximumRGBTolerance": int,
+        "MaximumYUV": int,
+        "MinimumRGBTolerance": int,
+        "MinimumYUV": int,
+    },
+)
+
 ClipLimitsTypeDef = TypedDict(
     "ClipLimitsTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
     total=False,
 )
 
+CmafAdditionalManifestOutputTypeDef = TypedDict(
+    "CmafAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+SpekeKeyProviderCmafOutputTypeDef = TypedDict(
+    "SpekeKeyProviderCmafOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "DashSignaledSystemIds": List[str],
+        "HlsSignaledSystemIds": List[str],
+        "ResourceId": str,
+        "Url": str,
+    },
+)
+
+StaticKeyProviderOutputTypeDef = TypedDict(
+    "StaticKeyProviderOutputTypeDef",
+    {
+        "KeyFormat": str,
+        "KeyFormatVersions": str,
+        "StaticKeyValue": str,
+        "Url": str,
+    },
+)
+
 SpekeKeyProviderCmafTypeDef = TypedDict(
     "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": Sequence[str],
         "HlsSignaledSystemIds": Sequence[str],
         "ResourceId": str,
@@ -1184,27 +1809,59 @@
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
     total=False,
 )
 
+CmafImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": CmafIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+CmfcSettingsOutputTypeDef = TypedDict(
+    "CmfcSettingsOutputTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "AudioGroupId": str,
+        "AudioRenditionSets": str,
+        "AudioTrackType": CmfcAudioTrackTypeType,
+        "DescriptiveVideoServiceFlag": CmfcDescriptiveVideoServiceFlagType,
+        "IFrameOnlyManifest": CmfcIFrameOnlyManifestType,
+        "KlvMetadata": CmfcKlvMetadataType,
+        "ManifestMetadataSignaling": CmfcManifestMetadataSignalingType,
+        "Scte35Esam": CmfcScte35EsamType,
+        "Scte35Source": CmfcScte35SourceType,
+        "TimedMetadata": CmfcTimedMetadataType,
+        "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+)
+
 CmfcSettingsTypeDef = TypedDict(
     "CmfcSettingsTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "AudioGroupId": str,
         "AudioRenditionSets": str,
         "AudioTrackType": CmfcAudioTrackTypeType,
@@ -1218,14 +1875,32 @@
         "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
+Hdr10MetadataOutputTypeDef = TypedDict(
+    "Hdr10MetadataOutputTypeDef",
+    {
+        "BluePrimaryX": int,
+        "BluePrimaryY": int,
+        "GreenPrimaryX": int,
+        "GreenPrimaryY": int,
+        "MaxContentLightLevel": int,
+        "MaxFrameAverageLightLevel": int,
+        "MaxLuminance": int,
+        "MinLuminance": int,
+        "RedPrimaryX": int,
+        "RedPrimaryY": int,
+        "WhitePointX": int,
+        "WhitePointY": int,
+    },
+)
+
 Hdr10MetadataTypeDef = TypedDict(
     "Hdr10MetadataTypeDef",
     {
         "BluePrimaryX": int,
         "BluePrimaryY": int,
         "GreenPrimaryX": int,
         "GreenPrimaryY": int,
@@ -1237,14 +1912,86 @@
         "RedPrimaryY": int,
         "WhitePointX": int,
         "WhitePointY": int,
     },
     total=False,
 )
 
+F4vSettingsOutputTypeDef = TypedDict(
+    "F4vSettingsOutputTypeDef",
+    {
+        "MoovPlacement": F4vMoovPlacementType,
+    },
+)
+
+M3u8SettingsOutputTypeDef = TypedDict(
+    "M3u8SettingsOutputTypeDef",
+    {
+        "AudioDuration": M3u8AudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": List[int],
+        "DataPTSControl": M3u8DataPtsControlType,
+        "MaxPcrInterval": int,
+        "NielsenId3": M3u8NielsenId3Type,
+        "PatInterval": int,
+        "PcrControl": M3u8PcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "Scte35Pid": int,
+        "Scte35Source": M3u8Scte35SourceType,
+        "TimedMetadata": TimedMetadataType,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
+    },
+)
+
+MovSettingsOutputTypeDef = TypedDict(
+    "MovSettingsOutputTypeDef",
+    {
+        "ClapAtom": MovClapAtomType,
+        "CslgAtom": MovCslgAtomType,
+        "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
+        "PaddingControl": MovPaddingControlType,
+        "Reference": MovReferenceType,
+    },
+)
+
+Mp4SettingsOutputTypeDef = TypedDict(
+    "Mp4SettingsOutputTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "CslgAtom": Mp4CslgAtomType,
+        "CttsVersion": int,
+        "FreeSpaceBox": Mp4FreeSpaceBoxType,
+        "MoovPlacement": Mp4MoovPlacementType,
+        "Mp4MajorBrand": str,
+    },
+)
+
+MpdSettingsOutputTypeDef = TypedDict(
+    "MpdSettingsOutputTypeDef",
+    {
+        "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
+        "AudioDuration": MpdAudioDurationType,
+        "CaptionContainerType": MpdCaptionContainerTypeType,
+        "KlvMetadata": MpdKlvMetadataType,
+        "ManifestMetadataSignaling": MpdManifestMetadataSignalingType,
+        "Scte35Esam": MpdScte35EsamType,
+        "Scte35Source": MpdScte35SourceType,
+        "TimedMetadata": MpdTimedMetadataType,
+        "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+)
+
 F4vSettingsTypeDef = TypedDict(
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
     total=False,
 )
@@ -1324,56 +2071,106 @@
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
 )
 
+DashAdditionalManifestOutputTypeDef = TypedDict(
+    "DashAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "ResourceId": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+)
+
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
     total=False,
 )
 
+DashIsoImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": DashIsoIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 DashIsoImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+DeinterlacerOutputTypeDef = TypedDict(
+    "DeinterlacerOutputTypeDef",
+    {
+        "Algorithm": DeinterlaceAlgorithmType,
+        "Control": DeinterlacerControlType,
+        "Mode": DeinterlacerModeType,
+    },
+)
+
 DeinterlacerTypeDef = TypedDict(
     "DeinterlacerTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
         "Mode": DeinterlacerModeType,
     },
@@ -1397,19 +2194,20 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -1421,87 +2219,152 @@
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Url": str,
     },
-    total=False,
 )
 
 DisassociateCertificateRequestRequestTypeDef = TypedDict(
     "DisassociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DolbyVisionLevel6MetadataOutputTypeDef = TypedDict(
+    "DolbyVisionLevel6MetadataOutputTypeDef",
+    {
+        "MaxCll": int,
+        "MaxFall": int,
+    },
+)
+
 DolbyVisionLevel6MetadataTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
+DvbNitSettingsOutputTypeDef = TypedDict(
+    "DvbNitSettingsOutputTypeDef",
+    {
+        "NetworkId": int,
+        "NetworkName": str,
+        "NitInterval": int,
+    },
+)
+
 DvbNitSettingsTypeDef = TypedDict(
     "DvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
         "NitInterval": int,
     },
     total=False,
 )
 
+DvbSdtSettingsOutputTypeDef = TypedDict(
+    "DvbSdtSettingsOutputTypeDef",
+    {
+        "OutputSdt": OutputSdtType,
+        "SdtInterval": int,
+        "ServiceName": str,
+        "ServiceProviderName": str,
+    },
+)
+
 DvbSdtSettingsTypeDef = TypedDict(
     "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
+DvbTdtSettingsOutputTypeDef = TypedDict(
+    "DvbTdtSettingsOutputTypeDef",
+    {
+        "TdtInterval": int,
+    },
+)
+
 DvbTdtSettingsTypeDef = TypedDict(
     "DvbTdtSettingsTypeDef",
     {
         "TdtInterval": int,
     },
     total=False,
 )
 
+EsamManifestConfirmConditionNotificationOutputTypeDef = TypedDict(
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
+    {
+        "MccXml": str,
+    },
+)
+
 EsamManifestConfirmConditionNotificationTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationTypeDef",
     {
         "MccXml": str,
     },
     total=False,
 )
 
+EsamSignalProcessingNotificationOutputTypeDef = TypedDict(
+    "EsamSignalProcessingNotificationOutputTypeDef",
+    {
+        "SccXml": str,
+    },
+)
+
 EsamSignalProcessingNotificationTypeDef = TypedDict(
     "EsamSignalProcessingNotificationTypeDef",
     {
         "SccXml": str,
     },
     total=False,
 )
 
+ExtendedDataServicesOutputTypeDef = TypedDict(
+    "ExtendedDataServicesOutputTypeDef",
+    {
+        "CopyProtectionAction": CopyProtectionActionType,
+        "VchipAction": VchipActionType,
+    },
+)
+
 ExtendedDataServicesTypeDef = TypedDict(
     "ExtendedDataServicesTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
     },
     total=False,
 )
 
+FrameCaptureSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureSettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "MaxCaptures": int,
+        "Quality": int,
+    },
+)
+
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "MaxCaptures": int,
         "Quality": int,
@@ -1519,22 +2382,21 @@
 GetJobTemplateRequestRequestTypeDef = TypedDict(
     "GetJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
         "S3Inputs": InputPolicyType,
     },
-    total=False,
 )
 
 GetPresetRequestRequestTypeDef = TypedDict(
     "GetPresetRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1543,99 +2405,188 @@
 GetQueueRequestRequestTypeDef = TypedDict(
     "GetQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+H264QvbrSettingsOutputTypeDef = TypedDict(
+    "H264QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H264QvbrSettingsTypeDef = TypedDict(
     "H264QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+H265QvbrSettingsOutputTypeDef = TypedDict(
+    "H265QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H265QvbrSettingsTypeDef = TypedDict(
     "H265QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+Hdr10PlusOutputTypeDef = TypedDict(
+    "Hdr10PlusOutputTypeDef",
+    {
+        "MasteringMonitorNits": int,
+        "TargetMonitorNits": int,
+    },
+)
+
 Hdr10PlusTypeDef = TypedDict(
     "Hdr10PlusTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
 )
 
+HlsAdditionalManifestOutputTypeDef = TypedDict(
+    "HlsAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+HlsCaptionLanguageMappingOutputTypeDef = TypedDict(
+    "HlsCaptionLanguageMappingOutputTypeDef",
+    {
+        "CaptionChannel": int,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
 HlsCaptionLanguageMappingTypeDef = TypedDict(
     "HlsCaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+HlsImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": HlsIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 HlsImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "HlsImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
-HlsSettingsTypeDef = TypedDict(
-    "HlsSettingsTypeDef",
+HlsSettingsOutputTypeDef = TypedDict(
+    "HlsSettingsOutputTypeDef",
     {
         "AudioGroupId": str,
         "AudioOnlyContainer": HlsAudioOnlyContainerType,
         "AudioRenditionSets": str,
         "AudioTrackType": HlsAudioTrackTypeType,
         "DescriptiveVideoServiceFlag": HlsDescriptiveVideoServiceFlagType,
         "IFrameOnlyManifest": HlsIFrameOnlyManifestType,
         "SegmentModifier": str,
     },
-    total=False,
+)
+
+HopDestinationOutputTypeDef = TypedDict(
+    "HopDestinationOutputTypeDef",
+    {
+        "Priority": int,
+        "Queue": str,
+        "WaitMinutes": int,
+    },
+)
+
+Id3InsertionOutputTypeDef = TypedDict(
+    "Id3InsertionOutputTypeDef",
+    {
+        "Id3": str,
+        "Timecode": str,
+    },
 )
 
 Id3InsertionTypeDef = TypedDict(
     "Id3InsertionTypeDef",
     {
         "Id3": str,
         "Timecode": str,
     },
     total=False,
 )
 
+InsertableImageOutputTypeDef = TypedDict(
+    "InsertableImageOutputTypeDef",
+    {
+        "Duration": int,
+        "FadeIn": int,
+        "FadeOut": int,
+        "Height": int,
+        "ImageInserterInput": str,
+        "ImageX": int,
+        "ImageY": int,
+        "Layer": int,
+        "Opacity": int,
+        "StartTime": str,
+        "Width": int,
+    },
+)
+
 InsertableImageTypeDef = TypedDict(
     "InsertableImageTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
         "FadeOut": int,
         "Height": int,
@@ -1646,34 +2597,69 @@
         "Opacity": int,
         "StartTime": str,
         "Width": int,
     },
     total=False,
 )
 
+InputClippingOutputTypeDef = TypedDict(
+    "InputClippingOutputTypeDef",
+    {
+        "EndTimecode": str,
+        "StartTimecode": str,
+    },
+)
+
 InputClippingTypeDef = TypedDict(
     "InputClippingTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
     },
     total=False,
 )
 
+InputDecryptionSettingsOutputTypeDef = TypedDict(
+    "InputDecryptionSettingsOutputTypeDef",
+    {
+        "DecryptionMode": DecryptionModeType,
+        "EncryptedDecryptionKey": str,
+        "InitializationVector": str,
+        "KmsKeyRegion": str,
+    },
+)
+
 InputDecryptionSettingsTypeDef = TypedDict(
     "InputDecryptionSettingsTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
+InputVideoGeneratorOutputTypeDef = TypedDict(
+    "InputVideoGeneratorOutputTypeDef",
+    {
+        "Duration": int,
+    },
+)
+
+RectangleOutputTypeDef = TypedDict(
+    "RectangleOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+        "X": int,
+        "Y": int,
+    },
+)
+
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
@@ -1691,15 +2677,68 @@
 
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
-    total=False,
+)
+
+KantarWatermarkSettingsOutputTypeDef = TypedDict(
+    "KantarWatermarkSettingsOutputTypeDef",
+    {
+        "ChannelName": str,
+        "ContentReference": str,
+        "CredentialsSecretName": str,
+        "FileOffset": float,
+        "KantarLicenseId": int,
+        "KantarServerUrl": str,
+        "LogDestination": str,
+        "Metadata3": str,
+        "Metadata4": str,
+        "Metadata5": str,
+        "Metadata6": str,
+        "Metadata7": str,
+        "Metadata8": str,
+    },
+)
+
+NielsenConfigurationOutputTypeDef = TypedDict(
+    "NielsenConfigurationOutputTypeDef",
+    {
+        "BreakoutCode": int,
+        "DistributorId": str,
+    },
+)
+
+NielsenNonLinearWatermarkSettingsOutputTypeDef = TypedDict(
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    {
+        "ActiveWatermarkProcess": NielsenActiveWatermarkProcessTypeType,
+        "AdiFilename": str,
+        "AssetId": str,
+        "AssetName": str,
+        "CbetSourceId": str,
+        "EpisodeId": str,
+        "MetadataDestination": str,
+        "SourceId": int,
+        "SourceWatermarkStatus": NielsenSourceWatermarkStatusTypeType,
+        "TicServerUrl": str,
+        "UniqueTicPerAudioTrack": NielsenUniqueTicPerAudioTrackTypeType,
+    },
+)
+
+TimecodeConfigOutputTypeDef = TypedDict(
+    "TimecodeConfigOutputTypeDef",
+    {
+        "Anchor": str,
+        "Source": TimecodeSourceType,
+        "Start": str,
+        "TimestampOffset": str,
+    },
 )
 
 KantarWatermarkSettingsTypeDef = TypedDict(
     "KantarWatermarkSettingsTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -1759,114 +2798,69 @@
 QueueTransitionTypeDef = TypedDict(
     "QueueTransitionTypeDef",
     {
         "DestinationQueue": str,
         "SourceQueue": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
-    total=False,
 )
 
 WarningGroupTypeDef = TypedDict(
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
     },
 )
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -1883,25 +2877,47 @@
 
 ResourceTagsTypeDef = TypedDict(
     "ResourceTagsTypeDef",
     {
         "Arn": str,
         "Tags": Dict[str, str],
     },
-    total=False,
+)
+
+M2tsScte35EsamOutputTypeDef = TypedDict(
+    "M2tsScte35EsamOutputTypeDef",
+    {
+        "Scte35EsamPid": int,
+    },
 )
 
 M2tsScte35EsamTypeDef = TypedDict(
     "M2tsScte35EsamTypeDef",
     {
         "Scte35EsamPid": int,
     },
     total=False,
 )
 
+MotionImageInsertionFramerateOutputTypeDef = TypedDict(
+    "MotionImageInsertionFramerateOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+
+MotionImageInsertionOffsetOutputTypeDef = TypedDict(
+    "MotionImageInsertionOffsetOutputTypeDef",
+    {
+        "ImageX": int,
+        "ImageY": int,
+    },
+)
+
 MotionImageInsertionFramerateTypeDef = TypedDict(
     "MotionImageInsertionFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -1912,14 +2928,53 @@
     {
         "ImageX": int,
         "ImageY": int,
     },
     total=False,
 )
 
+Mpeg2SettingsOutputTypeDef = TypedDict(
+    "Mpeg2SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
+        "Bitrate": int,
+        "CodecLevel": Mpeg2CodecLevelType,
+        "CodecProfile": Mpeg2CodecProfileType,
+        "DynamicSubGop": Mpeg2DynamicSubGopType,
+        "FramerateControl": Mpeg2FramerateControlType,
+        "FramerateConversionAlgorithm": Mpeg2FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": Mpeg2GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": Mpeg2InterlaceModeType,
+        "IntraDcPrecision": Mpeg2IntraDcPrecisionType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "ParControl": Mpeg2ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Mpeg2QualityTuningLevelType,
+        "RateControlMode": Mpeg2RateControlModeType,
+        "ScanTypeConversionMode": Mpeg2ScanTypeConversionModeType,
+        "SceneChangeDetect": Mpeg2SceneChangeDetectType,
+        "SlowPal": Mpeg2SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": Mpeg2SpatialAdaptiveQuantizationType,
+        "Syntax": Mpeg2SyntaxType,
+        "Telecine": Mpeg2TelecineType,
+        "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
+    },
+)
+
 Mpeg2SettingsTypeDef = TypedDict(
     "Mpeg2SettingsTypeDef",
     {
         "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
         "Bitrate": int,
         "CodecLevel": Mpeg2CodecLevelType,
         "CodecProfile": Mpeg2CodecProfileType,
@@ -1952,51 +3007,104 @@
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
     total=False,
 )
 
+MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
+    "MsSmoothAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+MxfXavcProfileSettingsOutputTypeDef = TypedDict(
+    "MxfXavcProfileSettingsOutputTypeDef",
+    {
+        "DurationMode": MxfXavcDurationModeType,
+        "MaxAncDataSize": int,
+    },
+)
+
 MxfXavcProfileSettingsTypeDef = TypedDict(
     "MxfXavcProfileSettingsTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
     },
     total=False,
 )
 
+NexGuardFileMarkerSettingsOutputTypeDef = TypedDict(
+    "NexGuardFileMarkerSettingsOutputTypeDef",
+    {
+        "License": str,
+        "Payload": int,
+        "Preset": str,
+        "Strength": WatermarkingStrengthType,
+    },
+)
+
 NexGuardFileMarkerSettingsTypeDef = TypedDict(
     "NexGuardFileMarkerSettingsTypeDef",
     {
         "License": str,
         "Payload": int,
         "Preset": str,
         "Strength": WatermarkingStrengthType,
     },
     total=False,
 )
 
+NoiseReducerFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerFilterSettingsOutputTypeDef",
+    {
+        "Strength": int,
+    },
+)
+
 NoiseReducerFilterSettingsTypeDef = TypedDict(
     "NoiseReducerFilterSettingsTypeDef",
     {
         "Strength": int,
     },
     total=False,
 )
 
+NoiseReducerSpatialFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    {
+        "PostFilterSharpenStrength": int,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
+NoiseReducerTemporalFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
+    {
+        "AggressiveMode": int,
+        "PostTemporalSharpening": NoiseFilterPostTemporalSharpeningType,
+        "PostTemporalSharpeningStrength": NoiseFilterPostTemporalSharpeningStrengthType,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
 NoiseReducerSpatialFilterSettingsTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
         "Strength": int,
     },
@@ -2017,27 +3125,45 @@
 
 VideoDetailTypeDef = TypedDict(
     "VideoDetailTypeDef",
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HttpInputs": InputPolicyType,
+        "HttpsInputs": InputPolicyType,
+        "S3Inputs": InputPolicyType,
     },
     total=False,
 )
 
+ProresSettingsOutputTypeDef = TypedDict(
+    "ProresSettingsOutputTypeDef",
+    {
+        "ChromaSampling": ProresChromaSamplingType,
+        "CodecProfile": ProresCodecProfileType,
+        "FramerateControl": ProresFramerateControlType,
+        "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": ProresInterlaceModeType,
+        "ParControl": ProresParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "ScanTypeConversionMode": ProresScanTypeConversionModeType,
+        "SlowPal": ProresSlowPalType,
+        "Telecine": ProresTelecineType,
+    },
+)
+
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -2060,36 +3186,40 @@
         "Commitment": Literal["ONE_YEAR"],
         "ExpiresAt": datetime,
         "PurchasedAt": datetime,
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3DestinationAccessControlOutputTypeDef = TypedDict(
+    "S3DestinationAccessControlOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CannedAcl": S3ObjectCannedAclType,
     },
 )
 
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
 
+S3EncryptionSettingsOutputTypeDef = TypedDict(
+    "S3EncryptionSettingsOutputTypeDef",
+    {
+        "EncryptionType": S3ServerSideEncryptionTypeType,
+        "KmsEncryptionContext": str,
+        "KmsKeyArn": str,
+    },
+)
+
 S3EncryptionSettingsTypeDef = TypedDict(
     "S3EncryptionSettingsTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
         "KmsKeyArn": str,
     },
@@ -2100,14 +3230,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TimecodeBurninOutputTypeDef = TypedDict(
+    "TimecodeBurninOutputTypeDef",
+    {
+        "FontSize": int,
+        "Position": TimecodeBurninPositionType,
+        "Prefix": str,
+    },
+)
+
 TimecodeBurninTypeDef = TypedDict(
     "TimecodeBurninTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
         "Prefix": str,
     },
@@ -2131,14 +3270,29 @@
 
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
 
+Vc3SettingsOutputTypeDef = TypedDict(
+    "Vc3SettingsOutputTypeDef",
+    {
+        "FramerateControl": Vc3FramerateControlType,
+        "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": Vc3InterlaceModeType,
+        "ScanTypeConversionMode": Vc3ScanTypeConversionModeType,
+        "SlowPal": Vc3SlowPalType,
+        "Telecine": Vc3TelecineType,
+        "Vc3Class": Vc3ClassType,
+    },
+)
+
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2147,14 +3301,52 @@
         "SlowPal": Vc3SlowPalType,
         "Telecine": Vc3TelecineType,
         "Vc3Class": Vc3ClassType,
     },
     total=False,
 )
 
+Vp8SettingsOutputTypeDef = TypedDict(
+    "Vp8SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp8FramerateControlType,
+        "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp8ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp8QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
+Vp9SettingsOutputTypeDef = TypedDict(
+    "Vp9SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp9FramerateControlType,
+        "FramerateConversionAlgorithm": Vp9FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp9ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp9QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
 Vp8SettingsTypeDef = TypedDict(
     "Vp8SettingsTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp8FramerateControlType,
         "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
@@ -2187,30 +3379,58 @@
         "ParNumerator": int,
         "QualityTuningLevel": Vp9QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
     total=False,
 )
 
+Xavc4kIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraCbgProfileClassType,
+    },
+)
+
 Xavc4kIntraCbgProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
     total=False,
 )
 
+Xavc4kIntraVbrProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraVbrProfileClassType,
+    },
+)
+
 Xavc4kIntraVbrProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
     total=False,
 )
 
+Xavc4kProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": Xavc4kProfileBitrateClassType,
+        "CodecProfile": Xavc4kProfileCodecProfileType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
+        "Slices": int,
+    },
+)
+
 Xavc4kProfileSettingsTypeDef = TypedDict(
     "Xavc4kProfileSettingsTypeDef",
     {
         "BitrateClass": Xavc4kProfileBitrateClassType,
         "CodecProfile": Xavc4kProfileCodecProfileType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
@@ -2218,22 +3438,44 @@
         "HrdBufferSize": int,
         "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
         "Slices": int,
     },
     total=False,
 )
 
+XavcHdIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": XavcHdIntraCbgProfileClassType,
+    },
+)
+
 XavcHdIntraCbgProfileSettingsTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
     total=False,
 )
 
+XavcHdProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": XavcHdProfileBitrateClassType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": XavcInterlaceModeType,
+        "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
+        "Slices": int,
+        "Telecine": XavcHdProfileTelecineType,
+    },
+)
+
 XavcHdProfileSettingsTypeDef = TypedDict(
     "XavcHdProfileSettingsTypeDef",
     {
         "BitrateClass": XavcHdProfileBitrateClassType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
         "GopClosedCadence": int,
@@ -2242,14 +3484,31 @@
         "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
         "Slices": int,
         "Telecine": XavcHdProfileTelecineType,
     },
     total=False,
 )
 
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": AacSettingsOutputTypeDef,
+        "Ac3Settings": Ac3SettingsOutputTypeDef,
+        "AiffSettings": AiffSettingsOutputTypeDef,
+        "Codec": AudioCodecType,
+        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
+        "Eac3Settings": Eac3SettingsOutputTypeDef,
+        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "Mp3Settings": Mp3SettingsOutputTypeDef,
+        "OpusSettings": OpusSettingsOutputTypeDef,
+        "VorbisSettings": VorbisSettingsOutputTypeDef,
+        "WavSettings": WavSettingsOutputTypeDef,
+    },
+)
+
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "AiffSettings": AiffSettingsTypeDef,
         "Codec": AudioCodecType,
@@ -2260,26 +3519,56 @@
         "OpusSettings": OpusSettingsTypeDef,
         "VorbisSettings": VorbisSettingsTypeDef,
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrRuleOutputTypeDef = TypedDict(
+    "AutomatedAbrRuleOutputTypeDef",
+    {
+        "AllowedRenditions": List[AllowedRenditionSizeOutputTypeDef],
+        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeOutputTypeDef],
+        "MinBottomRenditionSize": MinBottomRenditionSizeOutputTypeDef,
+        "MinTopRenditionSize": MinTopRenditionSizeOutputTypeDef,
+        "Type": RuleTypeType,
+    },
+)
+
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
         "Type": RuleTypeType,
     },
     total=False,
 )
 
+Av1SettingsOutputTypeDef = TypedDict(
+    "Av1SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Av1AdaptiveQuantizationType,
+        "BitDepth": Av1BitDepthType,
+        "FramerateControl": Av1FramerateControlType,
+        "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "MaxBitrate": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "QvbrSettings": Av1QvbrSettingsOutputTypeDef,
+        "RateControlMode": Literal["QVBR"],
+        "Slices": int,
+        "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
+    },
+)
+
 Av1SettingsTypeDef = TypedDict(
     "Av1SettingsTypeDef",
     {
         "AdaptiveQuantization": Av1AdaptiveQuantizationType,
         "BitDepth": Av1BitDepthType,
         "FramerateControl": Av1FramerateControlType,
         "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
@@ -2292,14 +3581,30 @@
         "RateControlMode": Literal["QVBR"],
         "Slices": int,
         "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
     },
     total=False,
 )
 
+AvcIntraSettingsOutputTypeDef = TypedDict(
+    "AvcIntraSettingsOutputTypeDef",
+    {
+        "AvcIntraClass": AvcIntraClassType,
+        "AvcIntraUhdSettings": AvcIntraUhdSettingsOutputTypeDef,
+        "FramerateControl": AvcIntraFramerateControlType,
+        "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": AvcIntraInterlaceModeType,
+        "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
+        "SlowPal": AvcIntraSlowPalType,
+        "Telecine": AvcIntraTelecineType,
+    },
+)
+
 AvcIntraSettingsTypeDef = TypedDict(
     "AvcIntraSettingsTypeDef",
     {
         "AvcIntraClass": AvcIntraClassType,
         "AvcIntraUhdSettings": AvcIntraUhdSettingsTypeDef,
         "FramerateControl": AvcIntraFramerateControlType,
         "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
@@ -2309,14 +3614,30 @@
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
     total=False,
 )
 
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "BurninDestinationSettings": BurninDestinationSettingsOutputTypeDef,
+        "DestinationType": CaptionDestinationTypeType,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
+        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsOutputTypeDef,
+        "ImscDestinationSettings": ImscDestinationSettingsOutputTypeDef,
+        "SccDestinationSettings": SccDestinationSettingsOutputTypeDef,
+        "SrtDestinationSettings": SrtDestinationSettingsOutputTypeDef,
+        "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
+    },
+)
+
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
@@ -2326,48 +3647,111 @@
         "TeletextDestinationSettings": TeletextDestinationSettingsTypeDef,
         "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
         "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
     },
     total=False,
 )
 
+FileSourceSettingsOutputTypeDef = TypedDict(
+    "FileSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": FileSourceConvert608To708Type,
+        "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
+        "Framerate": CaptionSourceFramerateOutputTypeDef,
+        "SourceFile": str,
+        "TimeDelta": int,
+        "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
+    },
+)
+
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateTypeDef,
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
 
+ChannelMappingOutputTypeDef = TypedDict(
+    "ChannelMappingOutputTypeDef",
+    {
+        "OutputChannels": List[OutputChannelMappingOutputTypeDef],
+    },
+)
+
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
     total=False,
 )
 
+CmafEncryptionSettingsOutputTypeDef = TypedDict(
+    "CmafEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": CmafEncryptionTypeType,
+        "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
+        "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
+        "Type": CmafKeyProviderTypeType,
+    },
+)
+
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
         "StaticKeyProvider": StaticKeyProviderTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
     total=False,
 )
 
+ColorCorrectorOutputTypeDef = TypedDict(
+    "ColorCorrectorOutputTypeDef",
+    {
+        "Brightness": int,
+        "ClipLimits": ClipLimitsOutputTypeDef,
+        "ColorSpaceConversion": ColorSpaceConversionType,
+        "Contrast": int,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "HdrToSdrToneMapper": HDRToSDRToneMapperType,
+        "Hue": int,
+        "SampleRangeConversion": SampleRangeConversionType,
+        "Saturation": int,
+        "SdrReferenceWhiteLevel": int,
+    },
+)
+
+VideoSelectorOutputTypeDef = TypedDict(
+    "VideoSelectorOutputTypeDef",
+    {
+        "AlphaBehavior": AlphaBehaviorType,
+        "ColorSpace": ColorSpaceType,
+        "ColorSpaceUsage": ColorSpaceUsageType,
+        "EmbeddedTimecodeOverride": EmbeddedTimecodeOverrideType,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "PadVideo": PadVideoType,
+        "Pid": int,
+        "ProgramNumber": int,
+        "Rotate": InputRotateType,
+        "SampleRange": InputSampleRangeType,
+    },
+)
+
 ColorCorrectorTypeDef = TypedDict(
     "ColorCorrectorTypeDef",
     {
         "Brightness": int,
         "ClipLimits": ClipLimitsTypeDef,
         "ColorSpaceConversion": ColorSpaceConversionType,
         "Contrast": int,
@@ -2442,14 +3826,42 @@
 
 class UpdateQueueRequestRequestTypeDef(
     _RequiredUpdateQueueRequestRequestTypeDef, _OptionalUpdateQueueRequestRequestTypeDef
 ):
     pass
 
 
+DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    {
+        "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+
+HlsEncryptionSettingsOutputTypeDef = TypedDict(
+    "HlsEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": HlsEncryptionTypeType,
+        "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
+        "OfflineEncrypted": HlsOfflineEncryptedType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
+        "Type": HlsKeyProviderTypeType,
+    },
+)
+
+MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
+    "MsSmoothEncryptionSettingsOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
@@ -2473,64 +3885,178 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    {
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DolbyVisionOutputTypeDef = TypedDict(
+    "DolbyVisionOutputTypeDef",
+    {
+        "L6Metadata": DolbyVisionLevel6MetadataOutputTypeDef,
+        "L6Mode": DolbyVisionLevel6ModeType,
+        "Mapping": DolbyVisionMappingType,
+        "Profile": DolbyVisionProfileType,
     },
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
         "Mapping": DolbyVisionMappingType,
         "Profile": DolbyVisionProfileType,
     },
     total=False,
 )
 
+EsamSettingsOutputTypeDef = TypedDict(
+    "EsamSettingsOutputTypeDef",
+    {
+        "ManifestConfirmConditionNotification": (
+            EsamManifestConfirmConditionNotificationOutputTypeDef
+        ),
+        "ResponseSignalPreroll": int,
+        "SignalProcessingNotification": EsamSignalProcessingNotificationOutputTypeDef,
+    },
+)
+
 EsamSettingsTypeDef = TypedDict(
     "EsamSettingsTypeDef",
     {
         "ManifestConfirmConditionNotification": EsamManifestConfirmConditionNotificationTypeDef,
         "ResponseSignalPreroll": int,
         "SignalProcessingNotification": EsamSignalProcessingNotificationTypeDef,
     },
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Policy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyRequestRequestTypeDef = TypedDict(
-    "PutPolicyRequestRequestTypeDef",
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AdaptiveQuantization": H264AdaptiveQuantizationType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H264CodecLevelType,
+        "CodecProfile": H264CodecProfileType,
+        "DynamicSubGop": H264DynamicSubGopType,
+        "EntropyEncoding": H264EntropyEncodingType,
+        "FieldEncoding": H264FieldEncodingType,
+        "FlickerAdaptiveQuantization": H264FlickerAdaptiveQuantizationType,
+        "FramerateControl": H264FramerateControlType,
+        "FramerateConversionAlgorithm": H264FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H264GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H264GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H264InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H264ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H264QualityTuningLevelType,
+        "QvbrSettings": H264QvbrSettingsOutputTypeDef,
+        "RateControlMode": H264RateControlModeType,
+        "RepeatPps": H264RepeatPpsType,
+        "ScanTypeConversionMode": H264ScanTypeConversionModeType,
+        "SceneChangeDetect": H264SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H264SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": H264SpatialAdaptiveQuantizationType,
+        "Syntax": H264SyntaxType,
+        "Telecine": H264TelecineType,
+        "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
+        "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2575,14 +4101,62 @@
         "Telecine": H264TelecineType,
         "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
         "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
     total=False,
 )
 
+H265SettingsOutputTypeDef = TypedDict(
+    "H265SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H265AdaptiveQuantizationType,
+        "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H265CodecLevelType,
+        "CodecProfile": H265CodecProfileType,
+        "DynamicSubGop": H265DynamicSubGopType,
+        "FlickerAdaptiveQuantization": H265FlickerAdaptiveQuantizationType,
+        "FramerateControl": H265FramerateControlType,
+        "FramerateConversionAlgorithm": H265FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H265GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H265GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H265InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H265ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H265QualityTuningLevelType,
+        "QvbrSettings": H265QvbrSettingsOutputTypeDef,
+        "RateControlMode": H265RateControlModeType,
+        "SampleAdaptiveOffsetFilterMode": H265SampleAdaptiveOffsetFilterModeType,
+        "ScanTypeConversionMode": H265ScanTypeConversionModeType,
+        "SceneChangeDetect": H265SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H265SlowPalType,
+        "SpatialAdaptiveQuantization": H265SpatialAdaptiveQuantizationType,
+        "Telecine": H265TelecineType,
+        "TemporalAdaptiveQuantization": H265TemporalAdaptiveQuantizationType,
+        "TemporalIds": H265TemporalIdsType,
+        "Tiles": H265TilesType,
+        "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
+        "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
+    },
+)
+
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
         "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
         "Bitrate": int,
@@ -2624,44 +4198,103 @@
         "Tiles": H265TilesType,
         "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
         "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
     },
     total=False,
 )
 
-OutputSettingsTypeDef = TypedDict(
-    "OutputSettingsTypeDef",
+OutputSettingsOutputTypeDef = TypedDict(
+    "OutputSettingsOutputTypeDef",
     {
-        "HlsSettings": HlsSettingsTypeDef,
+        "HlsSettings": HlsSettingsOutputTypeDef,
+    },
+)
+
+TimedMetadataInsertionOutputTypeDef = TypedDict(
+    "TimedMetadataInsertionOutputTypeDef",
+    {
+        "Id3Insertions": List[Id3InsertionOutputTypeDef],
     },
-    total=False,
 )
 
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
+ImageInserterOutputTypeDef = TypedDict(
+    "ImageInserterOutputTypeDef",
+    {
+        "InsertableImages": List[InsertableImageOutputTypeDef],
+        "SdrReferenceWhiteLevel": int,
+    },
+)
+
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+M2tsSettingsOutputTypeDef = TypedDict(
+    "M2tsSettingsOutputTypeDef",
+    {
+        "AudioBufferModel": M2tsAudioBufferModelType,
+        "AudioDuration": M2tsAudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": List[int],
+        "Bitrate": int,
+        "BufferModel": M2tsBufferModelType,
+        "DataPTSControl": M2tsDataPtsControlType,
+        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
+        "DvbSubPids": List[int],
+        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
+        "DvbTeletextPid": int,
+        "EbpAudioInterval": M2tsEbpAudioIntervalType,
+        "EbpPlacement": M2tsEbpPlacementType,
+        "EsRateInPes": M2tsEsRateInPesType,
+        "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
+        "FragmentTime": float,
+        "KlvMetadata": M2tsKlvMetadataType,
+        "MaxPcrInterval": int,
+        "MinEbpInterval": int,
+        "NielsenId3": M2tsNielsenId3Type,
+        "NullPacketBitrate": float,
+        "PatInterval": int,
+        "PcrControl": M2tsPcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "RateMode": M2tsRateModeType,
+        "Scte35Esam": M2tsScte35EsamOutputTypeDef,
+        "Scte35Pid": int,
+        "Scte35Source": M2tsScte35SourceType,
+        "SegmentationMarkers": M2tsSegmentationMarkersType,
+        "SegmentationStyle": M2tsSegmentationStyleType,
+        "SegmentationTime": float,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
     },
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
@@ -2703,45 +4336,83 @@
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
     total=False,
 )
 
+MotionImageInserterOutputTypeDef = TypedDict(
+    "MotionImageInserterOutputTypeDef",
+    {
+        "Framerate": MotionImageInsertionFramerateOutputTypeDef,
+        "Input": str,
+        "InsertionMode": MotionImageInsertionModeType,
+        "Offset": MotionImageInsertionOffsetOutputTypeDef,
+        "Playback": MotionImagePlaybackType,
+        "StartTime": str,
+    },
+)
+
 MotionImageInserterTypeDef = TypedDict(
     "MotionImageInserterTypeDef",
     {
         "Framerate": MotionImageInsertionFramerateTypeDef,
         "Input": str,
         "InsertionMode": MotionImageInsertionModeType,
         "Offset": MotionImageInsertionOffsetTypeDef,
         "Playback": MotionImagePlaybackType,
         "StartTime": str,
     },
     total=False,
 )
 
+MxfSettingsOutputTypeDef = TypedDict(
+    "MxfSettingsOutputTypeDef",
+    {
+        "AfdSignaling": MxfAfdSignalingType,
+        "Profile": MxfProfileType,
+        "XavcProfileSettings": MxfXavcProfileSettingsOutputTypeDef,
+    },
+)
+
 MxfSettingsTypeDef = TypedDict(
     "MxfSettingsTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
         "XavcProfileSettings": MxfXavcProfileSettingsTypeDef,
     },
     total=False,
 )
 
+PartnerWatermarkingOutputTypeDef = TypedDict(
+    "PartnerWatermarkingOutputTypeDef",
+    {
+        "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsOutputTypeDef,
+    },
+)
+
 PartnerWatermarkingTypeDef = TypedDict(
     "PartnerWatermarkingTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsTypeDef,
     },
     total=False,
 )
 
+NoiseReducerOutputTypeDef = TypedDict(
+    "NoiseReducerOutputTypeDef",
+    {
+        "Filter": NoiseReducerFilterType,
+        "FilterSettings": NoiseReducerFilterSettingsOutputTypeDef,
+        "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsOutputTypeDef,
+        "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsOutputTypeDef,
+    },
+)
+
 NoiseReducerTypeDef = TypedDict(
     "NoiseReducerTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsTypeDef,
         "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsTypeDef,
         "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsTypeDef,
@@ -2751,54 +4422,79 @@
 
 OutputDetailTypeDef = TypedDict(
     "OutputDetailTypeDef",
     {
         "DurationInMs": int,
         "VideoDetails": VideoDetailTypeDef,
     },
-    total=False,
 )
 
-_RequiredQueueTypeDef = TypedDict(
-    "_RequiredQueueTypeDef",
+PutPolicyRequestRequestTypeDef = TypedDict(
+    "PutPolicyRequestRequestTypeDef",
     {
-        "Name": str,
+        "Policy": PolicyTypeDef,
     },
 )
-_OptionalQueueTypeDef = TypedDict(
-    "_OptionalQueueTypeDef",
+
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
         "PricingPlan": PricingPlanType,
         "ProgressingJobsCount": int,
         "ReservationPlan": ReservationPlanTypeDef,
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
-    total=False,
 )
 
-
-class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
-    pass
-
+S3DestinationSettingsOutputTypeDef = TypedDict(
+    "S3DestinationSettingsOutputTypeDef",
+    {
+        "AccessControl": S3DestinationAccessControlOutputTypeDef,
+        "Encryption": S3EncryptionSettingsOutputTypeDef,
+    },
+)
 
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
     },
     total=False,
 )
 
+XavcSettingsOutputTypeDef = TypedDict(
+    "XavcSettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": XavcAdaptiveQuantizationType,
+        "EntropyEncoding": XavcEntropyEncodingType,
+        "FramerateControl": XavcFramerateControlType,
+        "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "Profile": XavcProfileType,
+        "SlowPal": XavcSlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": XavcSpatialAdaptiveQuantizationType,
+        "TemporalAdaptiveQuantization": XavcTemporalAdaptiveQuantizationType,
+        "Xavc4kIntraCbgProfileSettings": Xavc4kIntraCbgProfileSettingsOutputTypeDef,
+        "Xavc4kIntraVbrProfileSettings": Xavc4kIntraVbrProfileSettingsOutputTypeDef,
+        "Xavc4kProfileSettings": Xavc4kProfileSettingsOutputTypeDef,
+        "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsOutputTypeDef,
+        "XavcHdProfileSettings": XavcHdProfileSettingsOutputTypeDef,
+    },
+)
+
 XavcSettingsTypeDef = TypedDict(
     "XavcSettingsTypeDef",
     {
         "AdaptiveQuantization": XavcAdaptiveQuantizationType,
         "EntropyEncoding": XavcEntropyEncodingType,
         "FramerateControl": XavcFramerateControlType,
         "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
@@ -2814,48 +4510,81 @@
         "Xavc4kProfileSettings": Xavc4kProfileSettingsTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrSettingsOutputTypeDef = TypedDict(
+    "AutomatedAbrSettingsOutputTypeDef",
+    {
+        "MaxAbrBitrate": int,
+        "MaxRenditions": int,
+        "MinAbrBitrate": int,
+        "Rules": List[AutomatedAbrRuleOutputTypeDef],
+    },
+)
+
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
-CaptionDescriptionPresetTypeDef = TypedDict(
-    "CaptionDescriptionPresetTypeDef",
+CaptionDescriptionOutputTypeDef = TypedDict(
+    "CaptionDescriptionOutputTypeDef",
     {
+        "CaptionSelectorName": str,
         "CustomLanguageCode": str,
-        "DestinationSettings": CaptionDestinationSettingsTypeDef,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
-CaptionDescriptionTypeDef = TypedDict(
-    "CaptionDescriptionTypeDef",
+CaptionDescriptionPresetOutputTypeDef = TypedDict(
+    "CaptionDescriptionPresetOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
+CaptionDescriptionPresetTypeDef = TypedDict(
+    "CaptionDescriptionPresetTypeDef",
     {
-        "CaptionSelectorName": str,
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+CaptionSourceSettingsOutputTypeDef = TypedDict(
+    "CaptionSourceSettingsOutputTypeDef",
+    {
+        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
+        "FileSourceSettings": FileSourceSettingsOutputTypeDef,
+        "SourceType": CaptionSourceTypeType,
+        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+        "TrackSourceSettings": TrackSourceSettingsOutputTypeDef,
+        "WebvttHlsSourceSettings": WebvttHlsSourceSettingsOutputTypeDef,
+    },
+)
+
 CaptionSourceSettingsTypeDef = TypedDict(
     "CaptionSourceSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
         "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
         "FileSourceSettings": FileSourceSettingsTypeDef,
@@ -2863,24 +4592,48 @@
         "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
         "TrackSourceSettings": TrackSourceSettingsTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsTypeDef,
     },
     total=False,
 )
 
+RemixSettingsOutputTypeDef = TypedDict(
+    "RemixSettingsOutputTypeDef",
+    {
+        "ChannelMapping": ChannelMappingOutputTypeDef,
+        "ChannelsIn": int,
+        "ChannelsOut": int,
+    },
+)
+
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
+ContainerSettingsOutputTypeDef = TypedDict(
+    "ContainerSettingsOutputTypeDef",
+    {
+        "CmfcSettings": CmfcSettingsOutputTypeDef,
+        "Container": ContainerTypeType,
+        "F4vSettings": F4vSettingsOutputTypeDef,
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "M3u8Settings": M3u8SettingsOutputTypeDef,
+        "MovSettings": MovSettingsOutputTypeDef,
+        "Mp4Settings": Mp4SettingsOutputTypeDef,
+        "MpdSettings": MpdSettingsOutputTypeDef,
+        "MxfSettings": MxfSettingsOutputTypeDef,
+    },
+)
+
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
         "F4vSettings": F4vSettingsTypeDef,
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -2889,14 +4642,28 @@
         "Mp4Settings": Mp4SettingsTypeDef,
         "MpdSettings": MpdSettingsTypeDef,
         "MxfSettings": MxfSettingsTypeDef,
     },
     total=False,
 )
 
+VideoPreprocessorOutputTypeDef = TypedDict(
+    "VideoPreprocessorOutputTypeDef",
+    {
+        "ColorCorrector": ColorCorrectorOutputTypeDef,
+        "Deinterlacer": DeinterlacerOutputTypeDef,
+        "DolbyVision": DolbyVisionOutputTypeDef,
+        "Hdr10Plus": Hdr10PlusOutputTypeDef,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "NoiseReducer": NoiseReducerOutputTypeDef,
+        "PartnerWatermarking": PartnerWatermarkingOutputTypeDef,
+        "TimecodeBurnin": TimecodeBurninOutputTypeDef,
+    },
+)
+
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
         "DolbyVision": DolbyVisionTypeDef,
         "Hdr10Plus": Hdr10PlusTypeDef,
@@ -2909,58 +4676,82 @@
 )
 
 OutputGroupDetailTypeDef = TypedDict(
     "OutputGroupDetailTypeDef",
     {
         "OutputDetails": List[OutputDetailTypeDef],
     },
-    total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationSettingsOutputTypeDef = TypedDict(
+    "DestinationSettingsOutputTypeDef",
+    {
+        "S3Settings": S3DestinationSettingsOutputTypeDef,
     },
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
     },
     total=False,
 )
 
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "Av1Settings": Av1SettingsOutputTypeDef,
+        "AvcIntraSettings": AvcIntraSettingsOutputTypeDef,
+        "Codec": VideoCodecType,
+        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "H264Settings": H264SettingsOutputTypeDef,
+        "H265Settings": H265SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+        "ProresSettings": ProresSettingsOutputTypeDef,
+        "Vc3Settings": Vc3SettingsOutputTypeDef,
+        "Vp8Settings": Vp8SettingsOutputTypeDef,
+        "Vp9Settings": Vp9SettingsOutputTypeDef,
+        "XavcSettings": XavcSettingsOutputTypeDef,
+    },
+)
+
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "Av1Settings": Av1SettingsTypeDef,
         "AvcIntraSettings": AvcIntraSettingsTypeDef,
         "Codec": VideoCodecType,
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
@@ -2972,32 +4763,83 @@
         "Vp8Settings": Vp8SettingsTypeDef,
         "Vp9Settings": Vp9SettingsTypeDef,
         "XavcSettings": XavcSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedEncodingSettingsOutputTypeDef = TypedDict(
+    "AutomatedEncodingSettingsOutputTypeDef",
+    {
+        "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
+    },
+)
+
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
 
+CaptionSelectorOutputTypeDef = TypedDict(
+    "CaptionSelectorOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "SourceSettings": CaptionSourceSettingsOutputTypeDef,
+    },
+)
+
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
+AudioDescriptionOutputTypeDef = TypedDict(
+    "AudioDescriptionOutputTypeDef",
+    {
+        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsOutputTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
+        "AudioSourceName": str,
+        "AudioType": int,
+        "AudioTypeControl": AudioTypeControlType,
+        "CodecSettings": AudioCodecSettingsOutputTypeDef,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageCodeControl": AudioLanguageCodeControlType,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "StreamName": str,
+    },
+)
+
+AudioSelectorOutputTypeDef = TypedDict(
+    "AudioSelectorOutputTypeDef",
+    {
+        "AudioDurationCorrection": AudioDurationCorrectionType,
+        "CustomLanguageCode": str,
+        "DefaultSelection": AudioDefaultSelectionType,
+        "ExternalAudioFileInput": str,
+        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "Offset": int,
+        "Pids": List[int],
+        "ProgramSelection": int,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "SelectorType": AudioSelectorTypeType,
+        "Tracks": List[int],
+    },
+)
+
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
@@ -3027,14 +4869,134 @@
         "RemixSettings": RemixSettingsTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": Sequence[int],
     },
     total=False,
 )
 
+CmafGroupSettingsOutputTypeDef = TypedDict(
+    "CmafGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
+        "BaseUrl": str,
+        "ClientCache": CmafClientCacheType,
+        "CodecSpecification": CmafCodecSpecificationType,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": CmafEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsOutputTypeDef,
+        "ManifestCompression": CmafManifestCompressionType,
+        "ManifestDurationFormat": CmafManifestDurationFormatType,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
+        "MpdProfile": CmafMpdProfileType,
+        "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
+        "SegmentControl": CmafSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": CmafSegmentLengthControlType,
+        "StreamInfResolution": CmafStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
+        "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
+        "WriteDashManifest": CmafWriteDASHManifestType,
+        "WriteHlsManifest": CmafWriteHLSManifestType,
+        "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
+    },
+)
+
+DashIsoGroupSettingsOutputTypeDef = TypedDict(
+    "DashIsoGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
+        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
+        "BaseUrl": str,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "HbbtvCompliance": DashIsoHbbtvComplianceType,
+        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
+        "MpdProfile": DashIsoMpdProfileType,
+        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
+        "SegmentControl": DashIsoSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": DashIsoSegmentLengthControlType,
+        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
+        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
+    },
+)
+
+FileGroupSettingsOutputTypeDef = TypedDict(
+    "FileGroupSettingsOutputTypeDef",
+    {
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+    },
+)
+
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
+        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
+        "BaseUrl": str,
+        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "Encryption": HlsEncryptionSettingsOutputTypeDef,
+        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsOutputTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinFinalSegmentLength": float,
+        "MinSegmentLength": int,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
+        "SegmentControl": HlsSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": HlsSegmentLengthControlType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+    },
+)
+
+MsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "MsSmoothGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
+        "AudioDeduplication": MsSmoothAudioDeduplicationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
+        "ManifestEncoding": MsSmoothManifestEncodingType,
+    },
+)
+
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
@@ -3152,14 +5114,35 @@
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
     total=False,
 )
 
+VideoDescriptionOutputTypeDef = TypedDict(
+    "VideoDescriptionOutputTypeDef",
+    {
+        "AfdSignaling": AfdSignalingType,
+        "AntiAlias": AntiAliasType,
+        "CodecSettings": VideoCodecSettingsOutputTypeDef,
+        "ColorMetadata": ColorMetadataType,
+        "Crop": RectangleOutputTypeDef,
+        "DropFrameTimecode": DropFrameTimecodeType,
+        "FixedAfd": int,
+        "Height": int,
+        "Position": RectangleOutputTypeDef,
+        "RespondToAfd": RespondToAfdType,
+        "ScalingBehavior": ScalingBehaviorType,
+        "Sharpness": int,
+        "TimecodeInsertion": VideoTimecodeInsertionType,
+        "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
+        "Width": int,
+    },
+)
+
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
         "CodecSettings": VideoCodecSettingsTypeDef,
         "ColorMetadata": ColorMetadataType,
@@ -3174,14 +5157,70 @@
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorTypeDef,
         "Width": int,
     },
     total=False,
 )
 
+InputOutputTypeDef = TypedDict(
+    "InputOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DecryptionSettings": InputDecryptionSettingsOutputTypeDef,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FileInput": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingOutputTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleOutputTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "SupplementalImps": List[str],
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoGenerator": InputVideoGeneratorOutputTypeDef,
+        "VideoSelector": VideoSelectorOutputTypeDef,
+    },
+)
+
+InputTemplateOutputTypeDef = TypedDict(
+    "InputTemplateOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingOutputTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleOutputTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoSelector": VideoSelectorOutputTypeDef,
+    },
+)
+
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
@@ -3232,14 +5271,26 @@
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorTypeDef,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
+        "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
+        "FileGroupSettings": FileGroupSettingsOutputTypeDef,
+        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "Type": OutputGroupTypeType,
+    },
+)
+
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
         "FileGroupSettings": FileGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
@@ -3248,49 +5299,83 @@
     },
     total=False,
 )
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
-        "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
-        "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
-        "ContainerSettings": ContainerSettingsTypeDef,
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
         "Extension": str,
         "NameModifier": str,
-        "OutputSettings": OutputSettingsTypeDef,
+        "OutputSettings": OutputSettingsOutputTypeDef,
         "Preset": str,
-        "VideoDescription": VideoDescriptionTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
+    },
+)
+
+PresetSettingsOutputTypeDef = TypedDict(
+    "PresetSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsTypeDef = TypedDict(
     "PresetSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
+OutputGroupOutputTypeDef = TypedDict(
+    "OutputGroupOutputTypeDef",
+    {
+        "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
+        "CustomName": str,
+        "Name": str,
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
+    },
+)
+
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
     total=False,
 )
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
+        "Type": TypeType,
+    },
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": PresetSettingsTypeDef,
     },
 )
@@ -3307,39 +5392,14 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
-    {
-        "Arn": str,
-        "Category": str,
-        "CreatedAt": datetime,
-        "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
-
 _RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
@@ -3355,14 +5415,50 @@
 
 class UpdatePresetRequestRequestTypeDef(
     _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
 ):
     pass
 
 
+JobSettingsOutputTypeDef = TypedDict(
+    "JobSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
+        "Inputs": List[InputOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+)
+
+JobTemplateSettingsOutputTypeDef = TypedDict(
+    "JobTemplateSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
+        "Inputs": List[InputTemplateOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+)
+
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
         "Esam": EsamSettingsTypeDef,
         "ExtendedDataServices": ExtendedDataServicesTypeDef,
@@ -3397,175 +5493,153 @@
     total=False,
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPresetResponseTypeDef = TypedDict(
     "GetPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "NextToken": str,
         "Presets": List[PresetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePresetResponseTypeDef = TypedDict(
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
-        "BillingTagsSource": BillingTagsSourceType,
-        "ClientRequestToken": str,
-        "HopDestinations": Sequence[HopDestinationTypeDef],
-        "JobTemplate": str,
-        "Priority": int,
-        "Queue": str,
-        "SimulateReservedQueue": SimulateReservedQueueType,
-        "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Tags": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+JobTypeDef = TypedDict(
+    "JobTypeDef",
     {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
         "ClientRequestToken": str,
         "CreatedAt": datetime,
         "CurrentPhase": JobPhaseType,
         "ErrorCode": int,
         "ErrorMessage": str,
-        "HopDestinations": List[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationOutputTypeDef],
         "Id": str,
         "JobPercentComplete": int,
         "JobTemplate": str,
         "Messages": JobMessagesTypeDef,
         "OutputGroupDetails": List[OutputGroupDetailTypeDef],
         "Priority": int,
         "Queue": str,
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
+        "Role": str,
+        "Settings": JobSettingsOutputTypeDef,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
-    total=False,
 )
 
-
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+JobTemplateTypeDef = TypedDict(
+    "JobTemplateTypeDef",
     {
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "HopDestinations": List[HopDestinationOutputTypeDef],
+        "LastUpdated": datetime,
         "Name": str,
-        "Settings": JobTemplateSettingsTypeDef,
+        "Priority": int,
+        "Queue": str,
+        "Settings": JobTemplateSettingsOutputTypeDef,
+        "StatusUpdateInterval": StatusUpdateIntervalType,
+        "Type": TypeType,
     },
 )
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "Role": str,
+        "Settings": JobSettingsTypeDef,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Category": str,
-        "Description": str,
+        "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
         "HopDestinations": Sequence[HopDestinationTypeDef],
+        "JobTemplate": str,
         "Priority": int,
         "Queue": str,
+        "SimulateReservedQueue": SimulateReservedQueueType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Tags": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
 
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
-        "LastUpdated": datetime,
+        "HopDestinations": Sequence[HopDestinationTypeDef],
         "Priority": int,
         "Queue": str,
         "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Type": TypeType,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
     pass
 
 
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
@@ -3593,60 +5667,60 @@
     pass
 
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert/type_defs.pyi` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert/type_defs.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for mediaconvert service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_mediaconvert.type_defs import AacSettingsTypeDef
+    from mypy_boto3_mediaconvert.type_defs import AacSettingsOutputTypeDef
 
-    data: AacSettingsTypeDef = {...}
+    data: AacSettingsOutputTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -427,243 +427,414 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AacSettingsOutputTypeDef",
     "AacSettingsTypeDef",
+    "Ac3SettingsOutputTypeDef",
     "Ac3SettingsTypeDef",
+    "AccelerationSettingsOutputTypeDef",
     "AccelerationSettingsTypeDef",
+    "AdvancedInputFilterSettingsOutputTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
+    "AiffSettingsOutputTypeDef",
     "AiffSettingsTypeDef",
+    "AllowedRenditionSizeOutputTypeDef",
     "AllowedRenditionSizeTypeDef",
+    "AncillarySourceSettingsOutputTypeDef",
     "AncillarySourceSettingsTypeDef",
     "AssociateCertificateRequestRequestTypeDef",
+    "AudioChannelTaggingSettingsOutputTypeDef",
     "AudioChannelTaggingSettingsTypeDef",
+    "Eac3AtmosSettingsOutputTypeDef",
+    "Eac3SettingsOutputTypeDef",
+    "Mp2SettingsOutputTypeDef",
+    "Mp3SettingsOutputTypeDef",
+    "OpusSettingsOutputTypeDef",
+    "VorbisSettingsOutputTypeDef",
+    "WavSettingsOutputTypeDef",
     "Eac3AtmosSettingsTypeDef",
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
+    "AudioNormalizationSettingsOutputTypeDef",
     "AudioNormalizationSettingsTypeDef",
+    "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
+    "HlsRenditionGroupSettingsOutputTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    "MinBottomRenditionSizeOutputTypeDef",
+    "MinTopRenditionSizeOutputTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
+    "Av1QvbrSettingsOutputTypeDef",
     "Av1QvbrSettingsTypeDef",
+    "AvailBlankingOutputTypeDef",
     "AvailBlankingTypeDef",
+    "AvcIntraUhdSettingsOutputTypeDef",
     "AvcIntraUhdSettingsTypeDef",
+    "BandwidthReductionFilterOutputTypeDef",
     "BandwidthReductionFilterTypeDef",
+    "BurninDestinationSettingsOutputTypeDef",
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
+    "DvbSubDestinationSettingsOutputTypeDef",
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    "ImscDestinationSettingsOutputTypeDef",
+    "SccDestinationSettingsOutputTypeDef",
+    "SrtDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsOutputTypeDef",
+    "TtmlDestinationSettingsOutputTypeDef",
+    "WebvttDestinationSettingsOutputTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
     "TeletextDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
+    "CaptionSourceFramerateOutputTypeDef",
     "CaptionSourceFramerateTypeDef",
+    "DvbSubSourceSettingsOutputTypeDef",
+    "EmbeddedSourceSettingsOutputTypeDef",
+    "TeletextSourceSettingsOutputTypeDef",
+    "TrackSourceSettingsOutputTypeDef",
+    "WebvttHlsSourceSettingsOutputTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
+    "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
+    "ClipLimitsOutputTypeDef",
     "ClipLimitsTypeDef",
+    "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
+    "SpekeKeyProviderCmafOutputTypeDef",
+    "StaticKeyProviderOutputTypeDef",
     "SpekeKeyProviderCmafTypeDef",
     "StaticKeyProviderTypeDef",
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
+    "CmfcSettingsOutputTypeDef",
     "CmfcSettingsTypeDef",
+    "Hdr10MetadataOutputTypeDef",
     "Hdr10MetadataTypeDef",
+    "F4vSettingsOutputTypeDef",
+    "M3u8SettingsOutputTypeDef",
+    "MovSettingsOutputTypeDef",
+    "Mp4SettingsOutputTypeDef",
+    "MpdSettingsOutputTypeDef",
     "F4vSettingsTypeDef",
     "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
     "HopDestinationTypeDef",
+    "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
+    "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
+    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
+    "DeinterlacerOutputTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEndpointsRequestRequestTypeDef",
     "EndpointTypeDef",
     "DisassociateCertificateRequestRequestTypeDef",
+    "DolbyVisionLevel6MetadataOutputTypeDef",
     "DolbyVisionLevel6MetadataTypeDef",
+    "DvbNitSettingsOutputTypeDef",
     "DvbNitSettingsTypeDef",
+    "DvbSdtSettingsOutputTypeDef",
     "DvbSdtSettingsTypeDef",
+    "DvbTdtSettingsOutputTypeDef",
     "DvbTdtSettingsTypeDef",
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
     "EsamManifestConfirmConditionNotificationTypeDef",
+    "EsamSignalProcessingNotificationOutputTypeDef",
     "EsamSignalProcessingNotificationTypeDef",
+    "ExtendedDataServicesOutputTypeDef",
     "ExtendedDataServicesTypeDef",
+    "FrameCaptureSettingsOutputTypeDef",
     "FrameCaptureSettingsTypeDef",
     "GetJobRequestRequestTypeDef",
     "GetJobTemplateRequestRequestTypeDef",
-    "PolicyTypeDef",
+    "PolicyOutputTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
+    "H264QvbrSettingsOutputTypeDef",
     "H264QvbrSettingsTypeDef",
+    "H265QvbrSettingsOutputTypeDef",
     "H265QvbrSettingsTypeDef",
+    "Hdr10PlusOutputTypeDef",
     "Hdr10PlusTypeDef",
+    "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
+    "HlsCaptionLanguageMappingOutputTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
-    "HlsSettingsTypeDef",
+    "HlsSettingsOutputTypeDef",
+    "HopDestinationOutputTypeDef",
+    "Id3InsertionOutputTypeDef",
     "Id3InsertionTypeDef",
+    "InsertableImageOutputTypeDef",
     "InsertableImageTypeDef",
+    "InputClippingOutputTypeDef",
     "InputClippingTypeDef",
+    "InputDecryptionSettingsOutputTypeDef",
     "InputDecryptionSettingsTypeDef",
+    "InputVideoGeneratorOutputTypeDef",
+    "RectangleOutputTypeDef",
     "RectangleTypeDef",
     "InputVideoGeneratorTypeDef",
     "JobMessagesTypeDef",
+    "KantarWatermarkSettingsOutputTypeDef",
+    "NielsenConfigurationOutputTypeDef",
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    "TimecodeConfigOutputTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
     "WarningGroupTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
+    "M2tsScte35EsamOutputTypeDef",
     "M2tsScte35EsamTypeDef",
+    "MotionImageInsertionFramerateOutputTypeDef",
+    "MotionImageInsertionOffsetOutputTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
+    "Mpeg2SettingsOutputTypeDef",
     "Mpeg2SettingsTypeDef",
+    "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
+    "MxfXavcProfileSettingsOutputTypeDef",
     "MxfXavcProfileSettingsTypeDef",
+    "NexGuardFileMarkerSettingsOutputTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
+    "NoiseReducerFilterSettingsOutputTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
-    "PaginatorConfigTypeDef",
+    "PolicyTypeDef",
+    "ProresSettingsOutputTypeDef",
     "ProresSettingsTypeDef",
     "ReservationPlanTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3DestinationAccessControlOutputTypeDef",
     "S3DestinationAccessControlTypeDef",
+    "S3EncryptionSettingsOutputTypeDef",
     "S3EncryptionSettingsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "TimecodeBurninOutputTypeDef",
     "TimecodeBurninTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "Vc3SettingsOutputTypeDef",
     "Vc3SettingsTypeDef",
+    "Vp8SettingsOutputTypeDef",
+    "Vp9SettingsOutputTypeDef",
     "Vp8SettingsTypeDef",
     "Vp9SettingsTypeDef",
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
+    "Xavc4kProfileSettingsOutputTypeDef",
     "Xavc4kProfileSettingsTypeDef",
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
+    "XavcHdProfileSettingsOutputTypeDef",
     "XavcHdProfileSettingsTypeDef",
+    "AudioCodecSettingsOutputTypeDef",
     "AudioCodecSettingsTypeDef",
+    "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
+    "Av1SettingsOutputTypeDef",
     "Av1SettingsTypeDef",
+    "AvcIntraSettingsOutputTypeDef",
     "AvcIntraSettingsTypeDef",
+    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
+    "FileSourceSettingsOutputTypeDef",
     "FileSourceSettingsTypeDef",
+    "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
+    "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
+    "ColorCorrectorOutputTypeDef",
+    "VideoSelectorOutputTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    "HlsEncryptionSettingsOutputTypeDef",
+    "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "DescribeEndpointsResponseTypeDef",
+    "DolbyVisionOutputTypeDef",
     "DolbyVisionTypeDef",
+    "EsamSettingsOutputTypeDef",
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "H264SettingsOutputTypeDef",
     "H264SettingsTypeDef",
+    "H265SettingsOutputTypeDef",
     "H265SettingsTypeDef",
-    "OutputSettingsTypeDef",
+    "OutputSettingsOutputTypeDef",
+    "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
+    "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
+    "MotionImageInserterOutputTypeDef",
     "MotionImageInserterTypeDef",
+    "MxfSettingsOutputTypeDef",
     "MxfSettingsTypeDef",
+    "PartnerWatermarkingOutputTypeDef",
     "PartnerWatermarkingTypeDef",
+    "NoiseReducerOutputTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "QueueTypeDef",
+    "S3DestinationSettingsOutputTypeDef",
     "S3DestinationSettingsTypeDef",
+    "XavcSettingsOutputTypeDef",
     "XavcSettingsTypeDef",
+    "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
+    "CaptionDescriptionOutputTypeDef",
+    "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
-    "CaptionDescriptionTypeDef",
+    "CaptionSourceSettingsOutputTypeDef",
     "CaptionSourceSettingsTypeDef",
+    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
+    "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
+    "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
+    "DestinationSettingsOutputTypeDef",
     "DestinationSettingsTypeDef",
+    "VideoCodecSettingsOutputTypeDef",
     "VideoCodecSettingsTypeDef",
+    "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
+    "CaptionSelectorOutputTypeDef",
     "CaptionSelectorTypeDef",
+    "AudioDescriptionOutputTypeDef",
+    "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
+    "CmafGroupSettingsOutputTypeDef",
+    "DashIsoGroupSettingsOutputTypeDef",
+    "FileGroupSettingsOutputTypeDef",
+    "HlsGroupSettingsOutputTypeDef",
+    "MsSmoothGroupSettingsOutputTypeDef",
     "CmafGroupSettingsTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
     "HlsGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
+    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
+    "InputOutputTypeDef",
+    "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
+    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
     "OutputTypeDef",
+    "PresetSettingsOutputTypeDef",
     "PresetSettingsTypeDef",
+    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
-    "CreatePresetRequestRequestTypeDef",
     "PresetTypeDef",
+    "CreatePresetRequestRequestTypeDef",
     "UpdatePresetRequestRequestTypeDef",
+    "JobSettingsOutputTypeDef",
+    "JobTemplateSettingsOutputTypeDef",
     "JobSettingsTypeDef",
     "JobTemplateSettingsTypeDef",
     "CreatePresetResponseTypeDef",
     "GetPresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "UpdatePresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
-    "CreateJobTemplateRequestRequestTypeDef",
     "JobTemplateTypeDef",
+    "CreateJobRequestRequestTypeDef",
+    "CreateJobTemplateRequestRequestTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
     "UpdateJobTemplateResponseTypeDef",
 )
 
+AacSettingsOutputTypeDef = TypedDict(
+    "AacSettingsOutputTypeDef",
+    {
+        "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
+        "Bitrate": int,
+        "CodecProfile": AacCodecProfileType,
+        "CodingMode": AacCodingModeType,
+        "RateControlMode": AacRateControlModeType,
+        "RawFormat": AacRawFormatType,
+        "SampleRate": int,
+        "Specification": AacSpecificationType,
+        "VbrQuality": AacVbrQualityType,
+    },
+)
+
 AacSettingsTypeDef = TypedDict(
     "AacSettingsTypeDef",
     {
         "AudioDescriptionBroadcasterMix": AacAudioDescriptionBroadcasterMixType,
         "Bitrate": int,
         "CodecProfile": AacCodecProfileType,
         "CodingMode": AacCodingModeType,
@@ -672,14 +843,30 @@
         "SampleRate": int,
         "Specification": AacSpecificationType,
         "VbrQuality": AacVbrQualityType,
     },
     total=False,
 )
 
+Ac3SettingsOutputTypeDef = TypedDict(
+    "Ac3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Ac3BitstreamModeType,
+        "CodingMode": Ac3CodingModeType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Ac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionProfile": Ac3DynamicRangeCompressionProfileType,
+        "DynamicRangeCompressionRf": Ac3DynamicRangeCompressionRfType,
+        "LfeFilter": Ac3LfeFilterType,
+        "MetadataControl": Ac3MetadataControlType,
+        "SampleRate": int,
+    },
+)
+
 Ac3SettingsTypeDef = TypedDict(
     "Ac3SettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Ac3BitstreamModeType,
         "CodingMode": Ac3CodingModeType,
         "Dialnorm": int,
@@ -689,50 +876,92 @@
         "LfeFilter": Ac3LfeFilterType,
         "MetadataControl": Ac3MetadataControlType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AccelerationSettingsOutputTypeDef = TypedDict(
+    "AccelerationSettingsOutputTypeDef",
+    {
+        "Mode": AccelerationModeType,
+    },
+)
+
 AccelerationSettingsTypeDef = TypedDict(
     "AccelerationSettingsTypeDef",
     {
         "Mode": AccelerationModeType,
     },
 )
 
+AdvancedInputFilterSettingsOutputTypeDef = TypedDict(
+    "AdvancedInputFilterSettingsOutputTypeDef",
+    {
+        "AddTexture": AdvancedInputFilterAddTextureType,
+        "Sharpening": AdvancedInputFilterSharpenType,
+    },
+)
+
 AdvancedInputFilterSettingsTypeDef = TypedDict(
     "AdvancedInputFilterSettingsTypeDef",
     {
         "AddTexture": AdvancedInputFilterAddTextureType,
         "Sharpening": AdvancedInputFilterSharpenType,
     },
     total=False,
 )
 
+AiffSettingsOutputTypeDef = TypedDict(
+    "AiffSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
 AiffSettingsTypeDef = TypedDict(
     "AiffSettingsTypeDef",
     {
         "BitDepth": int,
         "Channels": int,
         "SampleRate": int,
     },
     total=False,
 )
 
+AllowedRenditionSizeOutputTypeDef = TypedDict(
+    "AllowedRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Required": RequiredFlagType,
+        "Width": int,
+    },
+)
+
 AllowedRenditionSizeTypeDef = TypedDict(
     "AllowedRenditionSizeTypeDef",
     {
         "Height": int,
         "Required": RequiredFlagType,
         "Width": int,
     },
     total=False,
 )
 
+AncillarySourceSettingsOutputTypeDef = TypedDict(
+    "AncillarySourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": AncillaryConvert608To708Type,
+        "SourceAncillaryChannelNumber": int,
+        "TerminateCaptions": AncillaryTerminateCaptionsType,
+    },
+)
+
 AncillarySourceSettingsTypeDef = TypedDict(
     "AncillarySourceSettingsTypeDef",
     {
         "Convert608To708": AncillaryConvert608To708Type,
         "SourceAncillaryChannelNumber": int,
         "TerminateCaptions": AncillaryTerminateCaptionsType,
     },
@@ -742,22 +971,127 @@
 AssociateCertificateRequestRequestTypeDef = TypedDict(
     "AssociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+AudioChannelTaggingSettingsOutputTypeDef = TypedDict(
+    "AudioChannelTaggingSettingsOutputTypeDef",
+    {
+        "ChannelTag": AudioChannelTagType,
+    },
+)
+
 AudioChannelTaggingSettingsTypeDef = TypedDict(
     "AudioChannelTaggingSettingsTypeDef",
     {
         "ChannelTag": AudioChannelTagType,
     },
     total=False,
 )
 
+Eac3AtmosSettingsOutputTypeDef = TypedDict(
+    "Eac3AtmosSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "BitstreamMode": Literal["COMPLETE_MAIN"],
+        "CodingMode": Eac3AtmosCodingModeType,
+        "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
+        "DownmixControl": Eac3AtmosDownmixControlType,
+        "DynamicRangeCompressionLine": Eac3AtmosDynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3AtmosDynamicRangeCompressionRfType,
+        "DynamicRangeControl": Eac3AtmosDynamicRangeControlType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MeteringMode": Eac3AtmosMeteringModeType,
+        "SampleRate": int,
+        "SpeechThreshold": int,
+        "StereoDownmix": Eac3AtmosStereoDownmixType,
+        "SurroundExMode": Eac3AtmosSurroundExModeType,
+    },
+)
+
+Eac3SettingsOutputTypeDef = TypedDict(
+    "Eac3SettingsOutputTypeDef",
+    {
+        "AttenuationControl": Eac3AttenuationControlType,
+        "Bitrate": int,
+        "BitstreamMode": Eac3BitstreamModeType,
+        "CodingMode": Eac3CodingModeType,
+        "DcFilter": Eac3DcFilterType,
+        "Dialnorm": int,
+        "DynamicRangeCompressionLine": Eac3DynamicRangeCompressionLineType,
+        "DynamicRangeCompressionRf": Eac3DynamicRangeCompressionRfType,
+        "LfeControl": Eac3LfeControlType,
+        "LfeFilter": Eac3LfeFilterType,
+        "LoRoCenterMixLevel": float,
+        "LoRoSurroundMixLevel": float,
+        "LtRtCenterMixLevel": float,
+        "LtRtSurroundMixLevel": float,
+        "MetadataControl": Eac3MetadataControlType,
+        "PassthroughControl": Eac3PassthroughControlType,
+        "PhaseControl": Eac3PhaseControlType,
+        "SampleRate": int,
+        "StereoDownmix": Eac3StereoDownmixType,
+        "SurroundExMode": Eac3SurroundExModeType,
+        "SurroundMode": Eac3SurroundModeType,
+    },
+)
+
+Mp2SettingsOutputTypeDef = TypedDict(
+    "Mp2SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+Mp3SettingsOutputTypeDef = TypedDict(
+    "Mp3SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "RateControlMode": Mp3RateControlModeType,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+OpusSettingsOutputTypeDef = TypedDict(
+    "OpusSettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "Channels": int,
+        "SampleRate": int,
+    },
+)
+
+VorbisSettingsOutputTypeDef = TypedDict(
+    "VorbisSettingsOutputTypeDef",
+    {
+        "Channels": int,
+        "SampleRate": int,
+        "VbrQuality": int,
+    },
+)
+
+WavSettingsOutputTypeDef = TypedDict(
+    "WavSettingsOutputTypeDef",
+    {
+        "BitDepth": int,
+        "Channels": int,
+        "Format": WavFormatType,
+        "SampleRate": int,
+    },
+)
+
 Eac3AtmosSettingsTypeDef = TypedDict(
     "Eac3AtmosSettingsTypeDef",
     {
         "Bitrate": int,
         "BitstreamMode": Literal["COMPLETE_MAIN"],
         "CodingMode": Eac3AtmosCodingModeType,
         "DialogueIntelligence": Eac3AtmosDialogueIntelligenceType,
@@ -855,46 +1189,99 @@
         "Channels": int,
         "Format": WavFormatType,
         "SampleRate": int,
     },
     total=False,
 )
 
+AudioNormalizationSettingsOutputTypeDef = TypedDict(
+    "AudioNormalizationSettingsOutputTypeDef",
+    {
+        "Algorithm": AudioNormalizationAlgorithmType,
+        "AlgorithmControl": AudioNormalizationAlgorithmControlType,
+        "CorrectionGateLevel": int,
+        "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
+        "PeakCalculation": AudioNormalizationPeakCalculationType,
+        "TargetLkfs": float,
+        "TruePeakLimiterThreshold": float,
+    },
+)
+
 AudioNormalizationSettingsTypeDef = TypedDict(
     "AudioNormalizationSettingsTypeDef",
     {
         "Algorithm": AudioNormalizationAlgorithmType,
         "AlgorithmControl": AudioNormalizationAlgorithmControlType,
         "CorrectionGateLevel": int,
         "LoudnessLogging": AudioNormalizationLoudnessLoggingType,
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
     total=False,
 )
 
+AudioSelectorGroupOutputTypeDef = TypedDict(
+    "AudioSelectorGroupOutputTypeDef",
+    {
+        "AudioSelectorNames": List[str],
+    },
+)
+
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
 
+HlsRenditionGroupSettingsOutputTypeDef = TypedDict(
+    "HlsRenditionGroupSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 HlsRenditionGroupSettingsTypeDef = TypedDict(
     "HlsRenditionGroupSettingsTypeDef",
     {
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+ForceIncludeRenditionSizeOutputTypeDef = TypedDict(
+    "ForceIncludeRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinBottomRenditionSizeOutputTypeDef = TypedDict(
+    "MinBottomRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
+MinTopRenditionSizeOutputTypeDef = TypedDict(
+    "MinTopRenditionSizeOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+    },
+)
+
 ForceIncludeRenditionSizeTypeDef = TypedDict(
     "ForceIncludeRenditionSizeTypeDef",
     {
         "Height": int,
         "Width": int,
     },
     total=False,
@@ -914,48 +1301,105 @@
     {
         "Height": int,
         "Width": int,
     },
     total=False,
 )
 
+Av1QvbrSettingsOutputTypeDef = TypedDict(
+    "Av1QvbrSettingsOutputTypeDef",
+    {
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 Av1QvbrSettingsTypeDef = TypedDict(
     "Av1QvbrSettingsTypeDef",
     {
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+AvailBlankingOutputTypeDef = TypedDict(
+    "AvailBlankingOutputTypeDef",
+    {
+        "AvailBlankingImage": str,
+    },
+)
+
 AvailBlankingTypeDef = TypedDict(
     "AvailBlankingTypeDef",
     {
         "AvailBlankingImage": str,
     },
     total=False,
 )
 
+AvcIntraUhdSettingsOutputTypeDef = TypedDict(
+    "AvcIntraUhdSettingsOutputTypeDef",
+    {
+        "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
+    },
+)
+
 AvcIntraUhdSettingsTypeDef = TypedDict(
     "AvcIntraUhdSettingsTypeDef",
     {
         "QualityTuningLevel": AvcIntraUhdQualityTuningLevelType,
     },
     total=False,
 )
 
+BandwidthReductionFilterOutputTypeDef = TypedDict(
+    "BandwidthReductionFilterOutputTypeDef",
+    {
+        "Sharpening": BandwidthReductionFilterSharpeningType,
+        "Strength": BandwidthReductionFilterStrengthType,
+    },
+)
+
 BandwidthReductionFilterTypeDef = TypedDict(
     "BandwidthReductionFilterTypeDef",
     {
         "Sharpening": BandwidthReductionFilterSharpeningType,
         "Strength": BandwidthReductionFilterStrengthType,
     },
     total=False,
 )
 
+BurninDestinationSettingsOutputTypeDef = TypedDict(
+    "BurninDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": BurninSubtitleAlignmentType,
+        "ApplyFontColor": BurninSubtitleApplyFontColorType,
+        "BackgroundColor": BurninSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "FallbackFont": BurninSubtitleFallbackFontType,
+        "FontColor": BurninSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "HexFontColor": str,
+        "OutlineColor": BurninSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": BurninSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": BurnInSubtitleStylePassthroughType,
+        "TeletextSpacing": BurninSubtitleTeletextSpacingType,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
 BurninDestinationSettingsTypeDef = TypedDict(
     "BurninDestinationSettingsTypeDef",
     {
         "Alignment": BurninSubtitleAlignmentType,
         "ApplyFontColor": BurninSubtitleApplyFontColorType,
         "BackgroundColor": BurninSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -983,14 +1427,100 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
+DvbSubDestinationSettingsOutputTypeDef = TypedDict(
+    "DvbSubDestinationSettingsOutputTypeDef",
+    {
+        "Alignment": DvbSubtitleAlignmentType,
+        "ApplyFontColor": DvbSubtitleApplyFontColorType,
+        "BackgroundColor": DvbSubtitleBackgroundColorType,
+        "BackgroundOpacity": int,
+        "DdsHandling": DvbddsHandlingType,
+        "DdsXCoordinate": int,
+        "DdsYCoordinate": int,
+        "FallbackFont": DvbSubSubtitleFallbackFontType,
+        "FontColor": DvbSubtitleFontColorType,
+        "FontOpacity": int,
+        "FontResolution": int,
+        "FontScript": FontScriptType,
+        "FontSize": int,
+        "Height": int,
+        "HexFontColor": str,
+        "OutlineColor": DvbSubtitleOutlineColorType,
+        "OutlineSize": int,
+        "ShadowColor": DvbSubtitleShadowColorType,
+        "ShadowOpacity": int,
+        "ShadowXOffset": int,
+        "ShadowYOffset": int,
+        "StylePassthrough": DvbSubtitleStylePassthroughType,
+        "SubtitlingType": DvbSubtitlingTypeType,
+        "TeletextSpacing": DvbSubtitleTeletextSpacingType,
+        "Width": int,
+        "XPosition": int,
+        "YPosition": int,
+    },
+)
+
+EmbeddedDestinationSettingsOutputTypeDef = TypedDict(
+    "EmbeddedDestinationSettingsOutputTypeDef",
+    {
+        "Destination608ChannelNumber": int,
+        "Destination708ServiceNumber": int,
+    },
+)
+
+ImscDestinationSettingsOutputTypeDef = TypedDict(
+    "ImscDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": ImscAccessibilitySubsType,
+        "StylePassthrough": ImscStylePassthroughType,
+    },
+)
+
+SccDestinationSettingsOutputTypeDef = TypedDict(
+    "SccDestinationSettingsOutputTypeDef",
+    {
+        "Framerate": SccDestinationFramerateType,
+    },
+)
+
+SrtDestinationSettingsOutputTypeDef = TypedDict(
+    "SrtDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": SrtStylePassthroughType,
+    },
+)
+
+TeletextDestinationSettingsOutputTypeDef = TypedDict(
+    "TeletextDestinationSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+        "PageTypes": List[TeletextPageTypeType],
+    },
+)
+
+TtmlDestinationSettingsOutputTypeDef = TypedDict(
+    "TtmlDestinationSettingsOutputTypeDef",
+    {
+        "StylePassthrough": TtmlStylePassthroughType,
+    },
+)
+
+WebvttDestinationSettingsOutputTypeDef = TypedDict(
+    "WebvttDestinationSettingsOutputTypeDef",
+    {
+        "Accessibility": WebvttAccessibilitySubsType,
+        "StylePassthrough": WebvttStylePassthroughType,
+    },
+)
+
 DvbSubDestinationSettingsTypeDef = TypedDict(
     "DvbSubDestinationSettingsTypeDef",
     {
         "Alignment": DvbSubtitleAlignmentType,
         "ApplyFontColor": DvbSubtitleApplyFontColorType,
         "BackgroundColor": DvbSubtitleBackgroundColorType,
         "BackgroundOpacity": int,
@@ -1077,23 +1607,71 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
+CaptionSourceFramerateOutputTypeDef = TypedDict(
+    "CaptionSourceFramerateOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
 )
 
+DvbSubSourceSettingsOutputTypeDef = TypedDict(
+    "DvbSubSourceSettingsOutputTypeDef",
+    {
+        "Pid": int,
+    },
+)
+
+EmbeddedSourceSettingsOutputTypeDef = TypedDict(
+    "EmbeddedSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": EmbeddedConvert608To708Type,
+        "Source608ChannelNumber": int,
+        "Source608TrackNumber": int,
+        "TerminateCaptions": EmbeddedTerminateCaptionsType,
+    },
+)
+
+TeletextSourceSettingsOutputTypeDef = TypedDict(
+    "TeletextSourceSettingsOutputTypeDef",
+    {
+        "PageNumber": str,
+    },
+)
+
+TrackSourceSettingsOutputTypeDef = TypedDict(
+    "TrackSourceSettingsOutputTypeDef",
+    {
+        "TrackNumber": int,
+    },
+)
+
+WebvttHlsSourceSettingsOutputTypeDef = TypedDict(
+    "WebvttHlsSourceSettingsOutputTypeDef",
+    {
+        "RenditionGroupId": str,
+        "RenditionLanguageCode": LanguageCodeType,
+        "RenditionName": str,
+    },
+)
+
 DvbSubSourceSettingsTypeDef = TypedDict(
     "DvbSubSourceSettingsTypeDef",
     {
         "Pid": int,
     },
     total=False,
 )
@@ -1131,43 +1709,90 @@
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
+OutputChannelMappingOutputTypeDef = TypedDict(
+    "OutputChannelMappingOutputTypeDef",
+    {
+        "InputChannels": List[int],
+        "InputChannelsFineTune": List[float],
+    },
+)
+
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
 )
 
+ClipLimitsOutputTypeDef = TypedDict(
+    "ClipLimitsOutputTypeDef",
+    {
+        "MaximumRGBTolerance": int,
+        "MaximumYUV": int,
+        "MinimumRGBTolerance": int,
+        "MinimumYUV": int,
+    },
+)
+
 ClipLimitsTypeDef = TypedDict(
     "ClipLimitsTypeDef",
     {
         "MaximumRGBTolerance": int,
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
     total=False,
 )
 
+CmafAdditionalManifestOutputTypeDef = TypedDict(
+    "CmafAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+SpekeKeyProviderCmafOutputTypeDef = TypedDict(
+    "SpekeKeyProviderCmafOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "DashSignaledSystemIds": List[str],
+        "HlsSignaledSystemIds": List[str],
+        "ResourceId": str,
+        "Url": str,
+    },
+)
+
+StaticKeyProviderOutputTypeDef = TypedDict(
+    "StaticKeyProviderOutputTypeDef",
+    {
+        "KeyFormat": str,
+        "KeyFormatVersions": str,
+        "StaticKeyValue": str,
+        "Url": str,
+    },
+)
+
 SpekeKeyProviderCmafTypeDef = TypedDict(
     "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
         "DashSignaledSystemIds": Sequence[str],
         "HlsSignaledSystemIds": Sequence[str],
         "ResourceId": str,
@@ -1183,27 +1808,59 @@
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
     total=False,
 )
 
+CmafImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "CmafImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": CmafIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+CmfcSettingsOutputTypeDef = TypedDict(
+    "CmfcSettingsOutputTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "AudioGroupId": str,
+        "AudioRenditionSets": str,
+        "AudioTrackType": CmfcAudioTrackTypeType,
+        "DescriptiveVideoServiceFlag": CmfcDescriptiveVideoServiceFlagType,
+        "IFrameOnlyManifest": CmfcIFrameOnlyManifestType,
+        "KlvMetadata": CmfcKlvMetadataType,
+        "ManifestMetadataSignaling": CmfcManifestMetadataSignalingType,
+        "Scte35Esam": CmfcScte35EsamType,
+        "Scte35Source": CmfcScte35SourceType,
+        "TimedMetadata": CmfcTimedMetadataType,
+        "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+)
+
 CmfcSettingsTypeDef = TypedDict(
     "CmfcSettingsTypeDef",
     {
         "AudioDuration": CmfcAudioDurationType,
         "AudioGroupId": str,
         "AudioRenditionSets": str,
         "AudioTrackType": CmfcAudioTrackTypeType,
@@ -1217,14 +1874,32 @@
         "TimedMetadataBoxVersion": CmfcTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
+Hdr10MetadataOutputTypeDef = TypedDict(
+    "Hdr10MetadataOutputTypeDef",
+    {
+        "BluePrimaryX": int,
+        "BluePrimaryY": int,
+        "GreenPrimaryX": int,
+        "GreenPrimaryY": int,
+        "MaxContentLightLevel": int,
+        "MaxFrameAverageLightLevel": int,
+        "MaxLuminance": int,
+        "MinLuminance": int,
+        "RedPrimaryX": int,
+        "RedPrimaryY": int,
+        "WhitePointX": int,
+        "WhitePointY": int,
+    },
+)
+
 Hdr10MetadataTypeDef = TypedDict(
     "Hdr10MetadataTypeDef",
     {
         "BluePrimaryX": int,
         "BluePrimaryY": int,
         "GreenPrimaryX": int,
         "GreenPrimaryY": int,
@@ -1236,14 +1911,86 @@
         "RedPrimaryY": int,
         "WhitePointX": int,
         "WhitePointY": int,
     },
     total=False,
 )
 
+F4vSettingsOutputTypeDef = TypedDict(
+    "F4vSettingsOutputTypeDef",
+    {
+        "MoovPlacement": F4vMoovPlacementType,
+    },
+)
+
+M3u8SettingsOutputTypeDef = TypedDict(
+    "M3u8SettingsOutputTypeDef",
+    {
+        "AudioDuration": M3u8AudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": List[int],
+        "DataPTSControl": M3u8DataPtsControlType,
+        "MaxPcrInterval": int,
+        "NielsenId3": M3u8NielsenId3Type,
+        "PatInterval": int,
+        "PcrControl": M3u8PcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "Scte35Pid": int,
+        "Scte35Source": M3u8Scte35SourceType,
+        "TimedMetadata": TimedMetadataType,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
+    },
+)
+
+MovSettingsOutputTypeDef = TypedDict(
+    "MovSettingsOutputTypeDef",
+    {
+        "ClapAtom": MovClapAtomType,
+        "CslgAtom": MovCslgAtomType,
+        "Mpeg2FourCCControl": MovMpeg2FourCCControlType,
+        "PaddingControl": MovPaddingControlType,
+        "Reference": MovReferenceType,
+    },
+)
+
+Mp4SettingsOutputTypeDef = TypedDict(
+    "Mp4SettingsOutputTypeDef",
+    {
+        "AudioDuration": CmfcAudioDurationType,
+        "CslgAtom": Mp4CslgAtomType,
+        "CttsVersion": int,
+        "FreeSpaceBox": Mp4FreeSpaceBoxType,
+        "MoovPlacement": Mp4MoovPlacementType,
+        "Mp4MajorBrand": str,
+    },
+)
+
+MpdSettingsOutputTypeDef = TypedDict(
+    "MpdSettingsOutputTypeDef",
+    {
+        "AccessibilityCaptionHints": MpdAccessibilityCaptionHintsType,
+        "AudioDuration": MpdAudioDurationType,
+        "CaptionContainerType": MpdCaptionContainerTypeType,
+        "KlvMetadata": MpdKlvMetadataType,
+        "ManifestMetadataSignaling": MpdManifestMetadataSignalingType,
+        "Scte35Esam": MpdScte35EsamType,
+        "Scte35Source": MpdScte35SourceType,
+        "TimedMetadata": MpdTimedMetadataType,
+        "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
+        "TimedMetadataSchemeIdUri": str,
+        "TimedMetadataValue": str,
+    },
+)
+
 F4vSettingsTypeDef = TypedDict(
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
     total=False,
 )
@@ -1323,56 +2070,106 @@
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 ReservationPlanSettingsTypeDef = TypedDict(
     "ReservationPlanSettingsTypeDef",
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
 )
 
+DashAdditionalManifestOutputTypeDef = TypedDict(
+    "DashAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+SpekeKeyProviderOutputTypeDef = TypedDict(
+    "SpekeKeyProviderOutputTypeDef",
+    {
+        "CertificateArn": str,
+        "ResourceId": str,
+        "SystemIds": List[str],
+        "Url": str,
+    },
+)
+
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
     },
     total=False,
 )
 
+DashIsoImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "DashIsoImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": DashIsoIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 DashIsoImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": DashIsoIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
+DeinterlacerOutputTypeDef = TypedDict(
+    "DeinterlacerOutputTypeDef",
+    {
+        "Algorithm": DeinterlaceAlgorithmType,
+        "Control": DeinterlacerControlType,
+        "Mode": DeinterlacerModeType,
+    },
+)
+
 DeinterlacerTypeDef = TypedDict(
     "DeinterlacerTypeDef",
     {
         "Algorithm": DeinterlaceAlgorithmType,
         "Control": DeinterlacerControlType,
         "Mode": DeinterlacerModeType,
     },
@@ -1396,19 +2193,20 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
-    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Mode": DescribeEndpointsModeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEndpointsRequestRequestTypeDef = TypedDict(
     "DescribeEndpointsRequestRequestTypeDef",
     {
@@ -1420,87 +2218,152 @@
 )
 
 EndpointTypeDef = TypedDict(
     "EndpointTypeDef",
     {
         "Url": str,
     },
-    total=False,
 )
 
 DisassociateCertificateRequestRequestTypeDef = TypedDict(
     "DisassociateCertificateRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
+DolbyVisionLevel6MetadataOutputTypeDef = TypedDict(
+    "DolbyVisionLevel6MetadataOutputTypeDef",
+    {
+        "MaxCll": int,
+        "MaxFall": int,
+    },
+)
+
 DolbyVisionLevel6MetadataTypeDef = TypedDict(
     "DolbyVisionLevel6MetadataTypeDef",
     {
         "MaxCll": int,
         "MaxFall": int,
     },
     total=False,
 )
 
+DvbNitSettingsOutputTypeDef = TypedDict(
+    "DvbNitSettingsOutputTypeDef",
+    {
+        "NetworkId": int,
+        "NetworkName": str,
+        "NitInterval": int,
+    },
+)
+
 DvbNitSettingsTypeDef = TypedDict(
     "DvbNitSettingsTypeDef",
     {
         "NetworkId": int,
         "NetworkName": str,
         "NitInterval": int,
     },
     total=False,
 )
 
+DvbSdtSettingsOutputTypeDef = TypedDict(
+    "DvbSdtSettingsOutputTypeDef",
+    {
+        "OutputSdt": OutputSdtType,
+        "SdtInterval": int,
+        "ServiceName": str,
+        "ServiceProviderName": str,
+    },
+)
+
 DvbSdtSettingsTypeDef = TypedDict(
     "DvbSdtSettingsTypeDef",
     {
         "OutputSdt": OutputSdtType,
         "SdtInterval": int,
         "ServiceName": str,
         "ServiceProviderName": str,
     },
     total=False,
 )
 
+DvbTdtSettingsOutputTypeDef = TypedDict(
+    "DvbTdtSettingsOutputTypeDef",
+    {
+        "TdtInterval": int,
+    },
+)
+
 DvbTdtSettingsTypeDef = TypedDict(
     "DvbTdtSettingsTypeDef",
     {
         "TdtInterval": int,
     },
     total=False,
 )
 
+EsamManifestConfirmConditionNotificationOutputTypeDef = TypedDict(
+    "EsamManifestConfirmConditionNotificationOutputTypeDef",
+    {
+        "MccXml": str,
+    },
+)
+
 EsamManifestConfirmConditionNotificationTypeDef = TypedDict(
     "EsamManifestConfirmConditionNotificationTypeDef",
     {
         "MccXml": str,
     },
     total=False,
 )
 
+EsamSignalProcessingNotificationOutputTypeDef = TypedDict(
+    "EsamSignalProcessingNotificationOutputTypeDef",
+    {
+        "SccXml": str,
+    },
+)
+
 EsamSignalProcessingNotificationTypeDef = TypedDict(
     "EsamSignalProcessingNotificationTypeDef",
     {
         "SccXml": str,
     },
     total=False,
 )
 
+ExtendedDataServicesOutputTypeDef = TypedDict(
+    "ExtendedDataServicesOutputTypeDef",
+    {
+        "CopyProtectionAction": CopyProtectionActionType,
+        "VchipAction": VchipActionType,
+    },
+)
+
 ExtendedDataServicesTypeDef = TypedDict(
     "ExtendedDataServicesTypeDef",
     {
         "CopyProtectionAction": CopyProtectionActionType,
         "VchipAction": VchipActionType,
     },
     total=False,
 )
 
+FrameCaptureSettingsOutputTypeDef = TypedDict(
+    "FrameCaptureSettingsOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "MaxCaptures": int,
+        "Quality": int,
+    },
+)
+
 FrameCaptureSettingsTypeDef = TypedDict(
     "FrameCaptureSettingsTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
         "MaxCaptures": int,
         "Quality": int,
@@ -1518,22 +2381,21 @@
 GetJobTemplateRequestRequestTypeDef = TypedDict(
     "GetJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-PolicyTypeDef = TypedDict(
-    "PolicyTypeDef",
+PolicyOutputTypeDef = TypedDict(
+    "PolicyOutputTypeDef",
     {
         "HttpInputs": InputPolicyType,
         "HttpsInputs": InputPolicyType,
         "S3Inputs": InputPolicyType,
     },
-    total=False,
 )
 
 GetPresetRequestRequestTypeDef = TypedDict(
     "GetPresetRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -1542,99 +2404,188 @@
 GetQueueRequestRequestTypeDef = TypedDict(
     "GetQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
+H264QvbrSettingsOutputTypeDef = TypedDict(
+    "H264QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H264QvbrSettingsTypeDef = TypedDict(
     "H264QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+H265QvbrSettingsOutputTypeDef = TypedDict(
+    "H265QvbrSettingsOutputTypeDef",
+    {
+        "MaxAverageBitrate": int,
+        "QvbrQualityLevel": int,
+        "QvbrQualityLevelFineTune": float,
+    },
+)
+
 H265QvbrSettingsTypeDef = TypedDict(
     "H265QvbrSettingsTypeDef",
     {
         "MaxAverageBitrate": int,
         "QvbrQualityLevel": int,
         "QvbrQualityLevelFineTune": float,
     },
     total=False,
 )
 
+Hdr10PlusOutputTypeDef = TypedDict(
+    "Hdr10PlusOutputTypeDef",
+    {
+        "MasteringMonitorNits": int,
+        "TargetMonitorNits": int,
+    },
+)
+
 Hdr10PlusTypeDef = TypedDict(
     "Hdr10PlusTypeDef",
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
 )
 
+HlsAdditionalManifestOutputTypeDef = TypedDict(
+    "HlsAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+HlsCaptionLanguageMappingOutputTypeDef = TypedDict(
+    "HlsCaptionLanguageMappingOutputTypeDef",
+    {
+        "CaptionChannel": int,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
 HlsCaptionLanguageMappingTypeDef = TypedDict(
     "HlsCaptionLanguageMappingTypeDef",
     {
         "CaptionChannel": int,
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+HlsImageBasedTrickPlaySettingsOutputTypeDef = TypedDict(
+    "HlsImageBasedTrickPlaySettingsOutputTypeDef",
+    {
+        "IntervalCadence": HlsIntervalCadenceType,
+        "ThumbnailHeight": int,
+        "ThumbnailInterval": float,
+        "ThumbnailWidth": int,
+        "TileHeight": int,
+        "TileWidth": int,
+    },
+)
+
 HlsImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "HlsImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": HlsIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
         "TileHeight": int,
         "TileWidth": int,
     },
     total=False,
 )
 
-HlsSettingsTypeDef = TypedDict(
-    "HlsSettingsTypeDef",
+HlsSettingsOutputTypeDef = TypedDict(
+    "HlsSettingsOutputTypeDef",
     {
         "AudioGroupId": str,
         "AudioOnlyContainer": HlsAudioOnlyContainerType,
         "AudioRenditionSets": str,
         "AudioTrackType": HlsAudioTrackTypeType,
         "DescriptiveVideoServiceFlag": HlsDescriptiveVideoServiceFlagType,
         "IFrameOnlyManifest": HlsIFrameOnlyManifestType,
         "SegmentModifier": str,
     },
-    total=False,
+)
+
+HopDestinationOutputTypeDef = TypedDict(
+    "HopDestinationOutputTypeDef",
+    {
+        "Priority": int,
+        "Queue": str,
+        "WaitMinutes": int,
+    },
+)
+
+Id3InsertionOutputTypeDef = TypedDict(
+    "Id3InsertionOutputTypeDef",
+    {
+        "Id3": str,
+        "Timecode": str,
+    },
 )
 
 Id3InsertionTypeDef = TypedDict(
     "Id3InsertionTypeDef",
     {
         "Id3": str,
         "Timecode": str,
     },
     total=False,
 )
 
+InsertableImageOutputTypeDef = TypedDict(
+    "InsertableImageOutputTypeDef",
+    {
+        "Duration": int,
+        "FadeIn": int,
+        "FadeOut": int,
+        "Height": int,
+        "ImageInserterInput": str,
+        "ImageX": int,
+        "ImageY": int,
+        "Layer": int,
+        "Opacity": int,
+        "StartTime": str,
+        "Width": int,
+    },
+)
+
 InsertableImageTypeDef = TypedDict(
     "InsertableImageTypeDef",
     {
         "Duration": int,
         "FadeIn": int,
         "FadeOut": int,
         "Height": int,
@@ -1645,34 +2596,69 @@
         "Opacity": int,
         "StartTime": str,
         "Width": int,
     },
     total=False,
 )
 
+InputClippingOutputTypeDef = TypedDict(
+    "InputClippingOutputTypeDef",
+    {
+        "EndTimecode": str,
+        "StartTimecode": str,
+    },
+)
+
 InputClippingTypeDef = TypedDict(
     "InputClippingTypeDef",
     {
         "EndTimecode": str,
         "StartTimecode": str,
     },
     total=False,
 )
 
+InputDecryptionSettingsOutputTypeDef = TypedDict(
+    "InputDecryptionSettingsOutputTypeDef",
+    {
+        "DecryptionMode": DecryptionModeType,
+        "EncryptedDecryptionKey": str,
+        "InitializationVector": str,
+        "KmsKeyRegion": str,
+    },
+)
+
 InputDecryptionSettingsTypeDef = TypedDict(
     "InputDecryptionSettingsTypeDef",
     {
         "DecryptionMode": DecryptionModeType,
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
+InputVideoGeneratorOutputTypeDef = TypedDict(
+    "InputVideoGeneratorOutputTypeDef",
+    {
+        "Duration": int,
+    },
+)
+
+RectangleOutputTypeDef = TypedDict(
+    "RectangleOutputTypeDef",
+    {
+        "Height": int,
+        "Width": int,
+        "X": int,
+        "Y": int,
+    },
+)
+
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
@@ -1690,15 +2676,68 @@
 
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
-    total=False,
+)
+
+KantarWatermarkSettingsOutputTypeDef = TypedDict(
+    "KantarWatermarkSettingsOutputTypeDef",
+    {
+        "ChannelName": str,
+        "ContentReference": str,
+        "CredentialsSecretName": str,
+        "FileOffset": float,
+        "KantarLicenseId": int,
+        "KantarServerUrl": str,
+        "LogDestination": str,
+        "Metadata3": str,
+        "Metadata4": str,
+        "Metadata5": str,
+        "Metadata6": str,
+        "Metadata7": str,
+        "Metadata8": str,
+    },
+)
+
+NielsenConfigurationOutputTypeDef = TypedDict(
+    "NielsenConfigurationOutputTypeDef",
+    {
+        "BreakoutCode": int,
+        "DistributorId": str,
+    },
+)
+
+NielsenNonLinearWatermarkSettingsOutputTypeDef = TypedDict(
+    "NielsenNonLinearWatermarkSettingsOutputTypeDef",
+    {
+        "ActiveWatermarkProcess": NielsenActiveWatermarkProcessTypeType,
+        "AdiFilename": str,
+        "AssetId": str,
+        "AssetName": str,
+        "CbetSourceId": str,
+        "EpisodeId": str,
+        "MetadataDestination": str,
+        "SourceId": int,
+        "SourceWatermarkStatus": NielsenSourceWatermarkStatusTypeType,
+        "TicServerUrl": str,
+        "UniqueTicPerAudioTrack": NielsenUniqueTicPerAudioTrackTypeType,
+    },
+)
+
+TimecodeConfigOutputTypeDef = TypedDict(
+    "TimecodeConfigOutputTypeDef",
+    {
+        "Anchor": str,
+        "Source": TimecodeSourceType,
+        "Start": str,
+        "TimestampOffset": str,
+    },
 )
 
 KantarWatermarkSettingsTypeDef = TypedDict(
     "KantarWatermarkSettingsTypeDef",
     {
         "ChannelName": str,
         "ContentReference": str,
@@ -1758,114 +2797,69 @@
 QueueTransitionTypeDef = TypedDict(
     "QueueTransitionTypeDef",
     {
         "DestinationQueue": str,
         "SourceQueue": str,
         "Timestamp": datetime,
     },
-    total=False,
 )
 
 TimingTypeDef = TypedDict(
     "TimingTypeDef",
     {
         "FinishTime": datetime,
         "StartTime": datetime,
         "SubmitTime": datetime,
     },
-    total=False,
 )
 
 WarningGroupTypeDef = TypedDict(
     "WarningGroupTypeDef",
     {
         "Code": int,
         "Count": int,
     },
 )
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": JobTemplateListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": JobTemplateListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "Order": OrderType,
-        "Queue": str,
-        "Status": JobStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
         "Queue": str,
         "Status": JobStatusType,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Category": str,
-        "ListBy": PresetListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Category": str,
         "ListBy": PresetListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
     },
     total=False,
 )
 
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "ListBy": QueueListByType,
-        "Order": OrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "ListBy": QueueListByType,
         "MaxResults": int,
         "NextToken": str,
         "Order": OrderType,
@@ -1882,25 +2876,47 @@
 
 ResourceTagsTypeDef = TypedDict(
     "ResourceTagsTypeDef",
     {
         "Arn": str,
         "Tags": Dict[str, str],
     },
-    total=False,
+)
+
+M2tsScte35EsamOutputTypeDef = TypedDict(
+    "M2tsScte35EsamOutputTypeDef",
+    {
+        "Scte35EsamPid": int,
+    },
 )
 
 M2tsScte35EsamTypeDef = TypedDict(
     "M2tsScte35EsamTypeDef",
     {
         "Scte35EsamPid": int,
     },
     total=False,
 )
 
+MotionImageInsertionFramerateOutputTypeDef = TypedDict(
+    "MotionImageInsertionFramerateOutputTypeDef",
+    {
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+    },
+)
+
+MotionImageInsertionOffsetOutputTypeDef = TypedDict(
+    "MotionImageInsertionOffsetOutputTypeDef",
+    {
+        "ImageX": int,
+        "ImageY": int,
+    },
+)
+
 MotionImageInsertionFramerateTypeDef = TypedDict(
     "MotionImageInsertionFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -1911,14 +2927,53 @@
     {
         "ImageX": int,
         "ImageY": int,
     },
     total=False,
 )
 
+Mpeg2SettingsOutputTypeDef = TypedDict(
+    "Mpeg2SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
+        "Bitrate": int,
+        "CodecLevel": Mpeg2CodecLevelType,
+        "CodecProfile": Mpeg2CodecProfileType,
+        "DynamicSubGop": Mpeg2DynamicSubGopType,
+        "FramerateControl": Mpeg2FramerateControlType,
+        "FramerateConversionAlgorithm": Mpeg2FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": Mpeg2GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": Mpeg2InterlaceModeType,
+        "IntraDcPrecision": Mpeg2IntraDcPrecisionType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "ParControl": Mpeg2ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Mpeg2QualityTuningLevelType,
+        "RateControlMode": Mpeg2RateControlModeType,
+        "ScanTypeConversionMode": Mpeg2ScanTypeConversionModeType,
+        "SceneChangeDetect": Mpeg2SceneChangeDetectType,
+        "SlowPal": Mpeg2SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": Mpeg2SpatialAdaptiveQuantizationType,
+        "Syntax": Mpeg2SyntaxType,
+        "Telecine": Mpeg2TelecineType,
+        "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
+    },
+)
+
 Mpeg2SettingsTypeDef = TypedDict(
     "Mpeg2SettingsTypeDef",
     {
         "AdaptiveQuantization": Mpeg2AdaptiveQuantizationType,
         "Bitrate": int,
         "CodecLevel": Mpeg2CodecLevelType,
         "CodecProfile": Mpeg2CodecProfileType,
@@ -1951,51 +3006,104 @@
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
     total=False,
 )
 
+MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
+    "MsSmoothAdditionalManifestOutputTypeDef",
+    {
+        "ManifestNameModifier": str,
+        "SelectedOutputs": List[str],
+    },
+)
+
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
+MxfXavcProfileSettingsOutputTypeDef = TypedDict(
+    "MxfXavcProfileSettingsOutputTypeDef",
+    {
+        "DurationMode": MxfXavcDurationModeType,
+        "MaxAncDataSize": int,
+    },
+)
+
 MxfXavcProfileSettingsTypeDef = TypedDict(
     "MxfXavcProfileSettingsTypeDef",
     {
         "DurationMode": MxfXavcDurationModeType,
         "MaxAncDataSize": int,
     },
     total=False,
 )
 
+NexGuardFileMarkerSettingsOutputTypeDef = TypedDict(
+    "NexGuardFileMarkerSettingsOutputTypeDef",
+    {
+        "License": str,
+        "Payload": int,
+        "Preset": str,
+        "Strength": WatermarkingStrengthType,
+    },
+)
+
 NexGuardFileMarkerSettingsTypeDef = TypedDict(
     "NexGuardFileMarkerSettingsTypeDef",
     {
         "License": str,
         "Payload": int,
         "Preset": str,
         "Strength": WatermarkingStrengthType,
     },
     total=False,
 )
 
+NoiseReducerFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerFilterSettingsOutputTypeDef",
+    {
+        "Strength": int,
+    },
+)
+
 NoiseReducerFilterSettingsTypeDef = TypedDict(
     "NoiseReducerFilterSettingsTypeDef",
     {
         "Strength": int,
     },
     total=False,
 )
 
+NoiseReducerSpatialFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerSpatialFilterSettingsOutputTypeDef",
+    {
+        "PostFilterSharpenStrength": int,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
+NoiseReducerTemporalFilterSettingsOutputTypeDef = TypedDict(
+    "NoiseReducerTemporalFilterSettingsOutputTypeDef",
+    {
+        "AggressiveMode": int,
+        "PostTemporalSharpening": NoiseFilterPostTemporalSharpeningType,
+        "PostTemporalSharpeningStrength": NoiseFilterPostTemporalSharpeningStrengthType,
+        "Speed": int,
+        "Strength": int,
+    },
+)
+
 NoiseReducerSpatialFilterSettingsTypeDef = TypedDict(
     "NoiseReducerSpatialFilterSettingsTypeDef",
     {
         "PostFilterSharpenStrength": int,
         "Speed": int,
         "Strength": int,
     },
@@ -2016,27 +3124,45 @@
 
 VideoDetailTypeDef = TypedDict(
     "VideoDetailTypeDef",
     {
         "HeightInPx": int,
         "WidthInPx": int,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PolicyTypeDef = TypedDict(
+    "PolicyTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "HttpInputs": InputPolicyType,
+        "HttpsInputs": InputPolicyType,
+        "S3Inputs": InputPolicyType,
     },
     total=False,
 )
 
+ProresSettingsOutputTypeDef = TypedDict(
+    "ProresSettingsOutputTypeDef",
+    {
+        "ChromaSampling": ProresChromaSamplingType,
+        "CodecProfile": ProresCodecProfileType,
+        "FramerateControl": ProresFramerateControlType,
+        "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": ProresInterlaceModeType,
+        "ParControl": ProresParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "ScanTypeConversionMode": ProresScanTypeConversionModeType,
+        "SlowPal": ProresSlowPalType,
+        "Telecine": ProresTelecineType,
+    },
+)
+
 ProresSettingsTypeDef = TypedDict(
     "ProresSettingsTypeDef",
     {
         "ChromaSampling": ProresChromaSamplingType,
         "CodecProfile": ProresCodecProfileType,
         "FramerateControl": ProresFramerateControlType,
         "FramerateConversionAlgorithm": ProresFramerateConversionAlgorithmType,
@@ -2059,36 +3185,40 @@
         "Commitment": Literal["ONE_YEAR"],
         "ExpiresAt": datetime,
         "PurchasedAt": datetime,
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
         "Status": ReservationPlanStatusType,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3DestinationAccessControlOutputTypeDef = TypedDict(
+    "S3DestinationAccessControlOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "CannedAcl": S3ObjectCannedAclType,
     },
 )
 
 S3DestinationAccessControlTypeDef = TypedDict(
     "S3DestinationAccessControlTypeDef",
     {
         "CannedAcl": S3ObjectCannedAclType,
     },
     total=False,
 )
 
+S3EncryptionSettingsOutputTypeDef = TypedDict(
+    "S3EncryptionSettingsOutputTypeDef",
+    {
+        "EncryptionType": S3ServerSideEncryptionTypeType,
+        "KmsEncryptionContext": str,
+        "KmsKeyArn": str,
+    },
+)
+
 S3EncryptionSettingsTypeDef = TypedDict(
     "S3EncryptionSettingsTypeDef",
     {
         "EncryptionType": S3ServerSideEncryptionTypeType,
         "KmsEncryptionContext": str,
         "KmsKeyArn": str,
     },
@@ -2099,14 +3229,23 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Mapping[str, str],
     },
 )
 
+TimecodeBurninOutputTypeDef = TypedDict(
+    "TimecodeBurninOutputTypeDef",
+    {
+        "FontSize": int,
+        "Position": TimecodeBurninPositionType,
+        "Prefix": str,
+    },
+)
+
 TimecodeBurninTypeDef = TypedDict(
     "TimecodeBurninTypeDef",
     {
         "FontSize": int,
         "Position": TimecodeBurninPositionType,
         "Prefix": str,
     },
@@ -2128,14 +3267,29 @@
 )
 
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
+Vc3SettingsOutputTypeDef = TypedDict(
+    "Vc3SettingsOutputTypeDef",
+    {
+        "FramerateControl": Vc3FramerateControlType,
+        "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": Vc3InterlaceModeType,
+        "ScanTypeConversionMode": Vc3ScanTypeConversionModeType,
+        "SlowPal": Vc3SlowPalType,
+        "Telecine": Vc3TelecineType,
+        "Vc3Class": Vc3ClassType,
+    },
+)
+
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2144,14 +3298,52 @@
         "SlowPal": Vc3SlowPalType,
         "Telecine": Vc3TelecineType,
         "Vc3Class": Vc3ClassType,
     },
     total=False,
 )
 
+Vp8SettingsOutputTypeDef = TypedDict(
+    "Vp8SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp8FramerateControlType,
+        "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp8ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp8QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
+Vp9SettingsOutputTypeDef = TypedDict(
+    "Vp9SettingsOutputTypeDef",
+    {
+        "Bitrate": int,
+        "FramerateControl": Vp9FramerateControlType,
+        "FramerateConversionAlgorithm": Vp9FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "HrdBufferSize": int,
+        "MaxBitrate": int,
+        "ParControl": Vp9ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": Vp9QualityTuningLevelType,
+        "RateControlMode": Literal["VBR"],
+    },
+)
+
 Vp8SettingsTypeDef = TypedDict(
     "Vp8SettingsTypeDef",
     {
         "Bitrate": int,
         "FramerateControl": Vp8FramerateControlType,
         "FramerateConversionAlgorithm": Vp8FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
@@ -2184,30 +3376,58 @@
         "ParNumerator": int,
         "QualityTuningLevel": Vp9QualityTuningLevelType,
         "RateControlMode": Literal["VBR"],
     },
     total=False,
 )
 
+Xavc4kIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraCbgProfileClassType,
+    },
+)
+
 Xavc4kIntraCbgProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraCbgProfileClassType,
     },
     total=False,
 )
 
+Xavc4kIntraVbrProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kIntraVbrProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": Xavc4kIntraVbrProfileClassType,
+    },
+)
+
 Xavc4kIntraVbrProfileSettingsTypeDef = TypedDict(
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     {
         "XavcClass": Xavc4kIntraVbrProfileClassType,
     },
     total=False,
 )
 
+Xavc4kProfileSettingsOutputTypeDef = TypedDict(
+    "Xavc4kProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": Xavc4kProfileBitrateClassType,
+        "CodecProfile": Xavc4kProfileCodecProfileType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
+        "Slices": int,
+    },
+)
+
 Xavc4kProfileSettingsTypeDef = TypedDict(
     "Xavc4kProfileSettingsTypeDef",
     {
         "BitrateClass": Xavc4kProfileBitrateClassType,
         "CodecProfile": Xavc4kProfileCodecProfileType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
@@ -2215,22 +3435,44 @@
         "HrdBufferSize": int,
         "QualityTuningLevel": Xavc4kProfileQualityTuningLevelType,
         "Slices": int,
     },
     total=False,
 )
 
+XavcHdIntraCbgProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdIntraCbgProfileSettingsOutputTypeDef",
+    {
+        "XavcClass": XavcHdIntraCbgProfileClassType,
+    },
+)
+
 XavcHdIntraCbgProfileSettingsTypeDef = TypedDict(
     "XavcHdIntraCbgProfileSettingsTypeDef",
     {
         "XavcClass": XavcHdIntraCbgProfileClassType,
     },
     total=False,
 )
 
+XavcHdProfileSettingsOutputTypeDef = TypedDict(
+    "XavcHdProfileSettingsOutputTypeDef",
+    {
+        "BitrateClass": XavcHdProfileBitrateClassType,
+        "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
+        "GopBReference": XavcGopBReferenceType,
+        "GopClosedCadence": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": XavcInterlaceModeType,
+        "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
+        "Slices": int,
+        "Telecine": XavcHdProfileTelecineType,
+    },
+)
+
 XavcHdProfileSettingsTypeDef = TypedDict(
     "XavcHdProfileSettingsTypeDef",
     {
         "BitrateClass": XavcHdProfileBitrateClassType,
         "FlickerAdaptiveQuantization": XavcFlickerAdaptiveQuantizationType,
         "GopBReference": XavcGopBReferenceType,
         "GopClosedCadence": int,
@@ -2239,14 +3481,31 @@
         "QualityTuningLevel": XavcHdProfileQualityTuningLevelType,
         "Slices": int,
         "Telecine": XavcHdProfileTelecineType,
     },
     total=False,
 )
 
+AudioCodecSettingsOutputTypeDef = TypedDict(
+    "AudioCodecSettingsOutputTypeDef",
+    {
+        "AacSettings": AacSettingsOutputTypeDef,
+        "Ac3Settings": Ac3SettingsOutputTypeDef,
+        "AiffSettings": AiffSettingsOutputTypeDef,
+        "Codec": AudioCodecType,
+        "Eac3AtmosSettings": Eac3AtmosSettingsOutputTypeDef,
+        "Eac3Settings": Eac3SettingsOutputTypeDef,
+        "Mp2Settings": Mp2SettingsOutputTypeDef,
+        "Mp3Settings": Mp3SettingsOutputTypeDef,
+        "OpusSettings": OpusSettingsOutputTypeDef,
+        "VorbisSettings": VorbisSettingsOutputTypeDef,
+        "WavSettings": WavSettingsOutputTypeDef,
+    },
+)
+
 AudioCodecSettingsTypeDef = TypedDict(
     "AudioCodecSettingsTypeDef",
     {
         "AacSettings": AacSettingsTypeDef,
         "Ac3Settings": Ac3SettingsTypeDef,
         "AiffSettings": AiffSettingsTypeDef,
         "Codec": AudioCodecType,
@@ -2257,26 +3516,56 @@
         "OpusSettings": OpusSettingsTypeDef,
         "VorbisSettings": VorbisSettingsTypeDef,
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrRuleOutputTypeDef = TypedDict(
+    "AutomatedAbrRuleOutputTypeDef",
+    {
+        "AllowedRenditions": List[AllowedRenditionSizeOutputTypeDef],
+        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeOutputTypeDef],
+        "MinBottomRenditionSize": MinBottomRenditionSizeOutputTypeDef,
+        "MinTopRenditionSize": MinTopRenditionSizeOutputTypeDef,
+        "Type": RuleTypeType,
+    },
+)
+
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
         "Type": RuleTypeType,
     },
     total=False,
 )
 
+Av1SettingsOutputTypeDef = TypedDict(
+    "Av1SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": Av1AdaptiveQuantizationType,
+        "BitDepth": Av1BitDepthType,
+        "FramerateControl": Av1FramerateControlType,
+        "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopSize": float,
+        "MaxBitrate": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "QvbrSettings": Av1QvbrSettingsOutputTypeDef,
+        "RateControlMode": Literal["QVBR"],
+        "Slices": int,
+        "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
+    },
+)
+
 Av1SettingsTypeDef = TypedDict(
     "Av1SettingsTypeDef",
     {
         "AdaptiveQuantization": Av1AdaptiveQuantizationType,
         "BitDepth": Av1BitDepthType,
         "FramerateControl": Av1FramerateControlType,
         "FramerateConversionAlgorithm": Av1FramerateConversionAlgorithmType,
@@ -2289,14 +3578,30 @@
         "RateControlMode": Literal["QVBR"],
         "Slices": int,
         "SpatialAdaptiveQuantization": Av1SpatialAdaptiveQuantizationType,
     },
     total=False,
 )
 
+AvcIntraSettingsOutputTypeDef = TypedDict(
+    "AvcIntraSettingsOutputTypeDef",
+    {
+        "AvcIntraClass": AvcIntraClassType,
+        "AvcIntraUhdSettings": AvcIntraUhdSettingsOutputTypeDef,
+        "FramerateControl": AvcIntraFramerateControlType,
+        "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "InterlaceMode": AvcIntraInterlaceModeType,
+        "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
+        "SlowPal": AvcIntraSlowPalType,
+        "Telecine": AvcIntraTelecineType,
+    },
+)
+
 AvcIntraSettingsTypeDef = TypedDict(
     "AvcIntraSettingsTypeDef",
     {
         "AvcIntraClass": AvcIntraClassType,
         "AvcIntraUhdSettings": AvcIntraUhdSettingsTypeDef,
         "FramerateControl": AvcIntraFramerateControlType,
         "FramerateConversionAlgorithm": AvcIntraFramerateConversionAlgorithmType,
@@ -2306,14 +3611,30 @@
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
     total=False,
 )
 
+CaptionDestinationSettingsOutputTypeDef = TypedDict(
+    "CaptionDestinationSettingsOutputTypeDef",
+    {
+        "BurninDestinationSettings": BurninDestinationSettingsOutputTypeDef,
+        "DestinationType": CaptionDestinationTypeType,
+        "DvbSubDestinationSettings": DvbSubDestinationSettingsOutputTypeDef,
+        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsOutputTypeDef,
+        "ImscDestinationSettings": ImscDestinationSettingsOutputTypeDef,
+        "SccDestinationSettings": SccDestinationSettingsOutputTypeDef,
+        "SrtDestinationSettings": SrtDestinationSettingsOutputTypeDef,
+        "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
+        "TtmlDestinationSettings": TtmlDestinationSettingsOutputTypeDef,
+        "WebvttDestinationSettings": WebvttDestinationSettingsOutputTypeDef,
+    },
+)
+
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
@@ -2323,48 +3644,111 @@
         "TeletextDestinationSettings": TeletextDestinationSettingsTypeDef,
         "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
         "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
     },
     total=False,
 )
 
+FileSourceSettingsOutputTypeDef = TypedDict(
+    "FileSourceSettingsOutputTypeDef",
+    {
+        "Convert608To708": FileSourceConvert608To708Type,
+        "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
+        "Framerate": CaptionSourceFramerateOutputTypeDef,
+        "SourceFile": str,
+        "TimeDelta": int,
+        "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
+    },
+)
+
 FileSourceSettingsTypeDef = TypedDict(
     "FileSourceSettingsTypeDef",
     {
         "Convert608To708": FileSourceConvert608To708Type,
         "ConvertPaintToPop": CaptionSourceConvertPaintOnToPopOnType,
         "Framerate": CaptionSourceFramerateTypeDef,
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
 
+ChannelMappingOutputTypeDef = TypedDict(
+    "ChannelMappingOutputTypeDef",
+    {
+        "OutputChannels": List[OutputChannelMappingOutputTypeDef],
+    },
+)
+
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
     total=False,
 )
 
+CmafEncryptionSettingsOutputTypeDef = TypedDict(
+    "CmafEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": CmafEncryptionTypeType,
+        "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
+        "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
+        "Type": CmafKeyProviderTypeType,
+    },
+)
+
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
         "StaticKeyProvider": StaticKeyProviderTypeDef,
         "Type": CmafKeyProviderTypeType,
     },
     total=False,
 )
 
+ColorCorrectorOutputTypeDef = TypedDict(
+    "ColorCorrectorOutputTypeDef",
+    {
+        "Brightness": int,
+        "ClipLimits": ClipLimitsOutputTypeDef,
+        "ColorSpaceConversion": ColorSpaceConversionType,
+        "Contrast": int,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "HdrToSdrToneMapper": HDRToSDRToneMapperType,
+        "Hue": int,
+        "SampleRangeConversion": SampleRangeConversionType,
+        "Saturation": int,
+        "SdrReferenceWhiteLevel": int,
+    },
+)
+
+VideoSelectorOutputTypeDef = TypedDict(
+    "VideoSelectorOutputTypeDef",
+    {
+        "AlphaBehavior": AlphaBehaviorType,
+        "ColorSpace": ColorSpaceType,
+        "ColorSpaceUsage": ColorSpaceUsageType,
+        "EmbeddedTimecodeOverride": EmbeddedTimecodeOverrideType,
+        "Hdr10Metadata": Hdr10MetadataOutputTypeDef,
+        "PadVideo": PadVideoType,
+        "Pid": int,
+        "ProgramNumber": int,
+        "Rotate": InputRotateType,
+        "SampleRange": InputSampleRangeType,
+    },
+)
+
 ColorCorrectorTypeDef = TypedDict(
     "ColorCorrectorTypeDef",
     {
         "Brightness": int,
         "ClipLimits": ClipLimitsTypeDef,
         "ColorSpaceConversion": ColorSpaceConversionType,
         "Contrast": int,
@@ -2435,14 +3819,42 @@
 )
 
 class UpdateQueueRequestRequestTypeDef(
     _RequiredUpdateQueueRequestRequestTypeDef, _OptionalUpdateQueueRequestRequestTypeDef
 ):
     pass
 
+DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
+    "DashIsoEncryptionSettingsOutputTypeDef",
+    {
+        "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+
+HlsEncryptionSettingsOutputTypeDef = TypedDict(
+    "HlsEncryptionSettingsOutputTypeDef",
+    {
+        "ConstantInitializationVector": str,
+        "EncryptionMethod": HlsEncryptionTypeType,
+        "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
+        "OfflineEncrypted": HlsOfflineEncryptedType,
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+        "StaticKeyProvider": StaticKeyProviderOutputTypeDef,
+        "Type": HlsKeyProviderTypeType,
+    },
+)
+
+MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
+    "MsSmoothEncryptionSettingsOutputTypeDef",
+    {
+        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
+    },
+)
+
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
@@ -2466,64 +3878,178 @@
     "MsSmoothEncryptionSettingsTypeDef",
     {
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
 )
 
+DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = TypedDict(
+    "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
+    {
+        "Mode": DescribeEndpointsModeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": JobTemplateListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "Order": OrderType,
+        "Queue": str,
+        "Status": JobStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Category": str,
+        "ListBy": PresetListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "ListBy": QueueListByType,
+        "Order": OrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DolbyVisionOutputTypeDef = TypedDict(
+    "DolbyVisionOutputTypeDef",
+    {
+        "L6Metadata": DolbyVisionLevel6MetadataOutputTypeDef,
+        "L6Mode": DolbyVisionLevel6ModeType,
+        "Mapping": DolbyVisionMappingType,
+        "Profile": DolbyVisionProfileType,
     },
 )
 
 DolbyVisionTypeDef = TypedDict(
     "DolbyVisionTypeDef",
     {
         "L6Metadata": DolbyVisionLevel6MetadataTypeDef,
         "L6Mode": DolbyVisionLevel6ModeType,
         "Mapping": DolbyVisionMappingType,
         "Profile": DolbyVisionProfileType,
     },
     total=False,
 )
 
+EsamSettingsOutputTypeDef = TypedDict(
+    "EsamSettingsOutputTypeDef",
+    {
+        "ManifestConfirmConditionNotification": (
+            EsamManifestConfirmConditionNotificationOutputTypeDef
+        ),
+        "ResponseSignalPreroll": int,
+        "SignalProcessingNotification": EsamSignalProcessingNotificationOutputTypeDef,
+    },
+)
+
 EsamSettingsTypeDef = TypedDict(
     "EsamSettingsTypeDef",
     {
         "ManifestConfirmConditionNotification": EsamManifestConfirmConditionNotificationTypeDef,
         "ResponseSignalPreroll": int,
         "SignalProcessingNotification": EsamSignalProcessingNotificationTypeDef,
     },
     total=False,
 )
 
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Policy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyRequestRequestTypeDef = TypedDict(
-    "PutPolicyRequestRequestTypeDef",
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
+H264SettingsOutputTypeDef = TypedDict(
+    "H264SettingsOutputTypeDef",
     {
-        "Policy": PolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AdaptiveQuantization": H264AdaptiveQuantizationType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H264CodecLevelType,
+        "CodecProfile": H264CodecProfileType,
+        "DynamicSubGop": H264DynamicSubGopType,
+        "EntropyEncoding": H264EntropyEncodingType,
+        "FieldEncoding": H264FieldEncodingType,
+        "FlickerAdaptiveQuantization": H264FlickerAdaptiveQuantizationType,
+        "FramerateControl": H264FramerateControlType,
+        "FramerateConversionAlgorithm": H264FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H264GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H264GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H264InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H264ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H264QualityTuningLevelType,
+        "QvbrSettings": H264QvbrSettingsOutputTypeDef,
+        "RateControlMode": H264RateControlModeType,
+        "RepeatPps": H264RepeatPpsType,
+        "ScanTypeConversionMode": H264ScanTypeConversionModeType,
+        "SceneChangeDetect": H264SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H264SlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": H264SpatialAdaptiveQuantizationType,
+        "Syntax": H264SyntaxType,
+        "Telecine": H264TelecineType,
+        "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
+        "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
 )
 
 H264SettingsTypeDef = TypedDict(
     "H264SettingsTypeDef",
     {
         "AdaptiveQuantization": H264AdaptiveQuantizationType,
@@ -2568,14 +4094,62 @@
         "Telecine": H264TelecineType,
         "TemporalAdaptiveQuantization": H264TemporalAdaptiveQuantizationType,
         "UnregisteredSeiTimecode": H264UnregisteredSeiTimecodeType,
     },
     total=False,
 )
 
+H265SettingsOutputTypeDef = TypedDict(
+    "H265SettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": H265AdaptiveQuantizationType,
+        "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
+        "BandwidthReductionFilter": BandwidthReductionFilterOutputTypeDef,
+        "Bitrate": int,
+        "CodecLevel": H265CodecLevelType,
+        "CodecProfile": H265CodecProfileType,
+        "DynamicSubGop": H265DynamicSubGopType,
+        "FlickerAdaptiveQuantization": H265FlickerAdaptiveQuantizationType,
+        "FramerateControl": H265FramerateControlType,
+        "FramerateConversionAlgorithm": H265FramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "GopBReference": H265GopBReferenceType,
+        "GopClosedCadence": int,
+        "GopSize": float,
+        "GopSizeUnits": H265GopSizeUnitsType,
+        "HrdBufferFinalFillPercentage": int,
+        "HrdBufferInitialFillPercentage": int,
+        "HrdBufferSize": int,
+        "InterlaceMode": H265InterlaceModeType,
+        "MaxBitrate": int,
+        "MinIInterval": int,
+        "NumberBFramesBetweenReferenceFrames": int,
+        "NumberReferenceFrames": int,
+        "ParControl": H265ParControlType,
+        "ParDenominator": int,
+        "ParNumerator": int,
+        "QualityTuningLevel": H265QualityTuningLevelType,
+        "QvbrSettings": H265QvbrSettingsOutputTypeDef,
+        "RateControlMode": H265RateControlModeType,
+        "SampleAdaptiveOffsetFilterMode": H265SampleAdaptiveOffsetFilterModeType,
+        "ScanTypeConversionMode": H265ScanTypeConversionModeType,
+        "SceneChangeDetect": H265SceneChangeDetectType,
+        "Slices": int,
+        "SlowPal": H265SlowPalType,
+        "SpatialAdaptiveQuantization": H265SpatialAdaptiveQuantizationType,
+        "Telecine": H265TelecineType,
+        "TemporalAdaptiveQuantization": H265TemporalAdaptiveQuantizationType,
+        "TemporalIds": H265TemporalIdsType,
+        "Tiles": H265TilesType,
+        "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
+        "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
+    },
+)
+
 H265SettingsTypeDef = TypedDict(
     "H265SettingsTypeDef",
     {
         "AdaptiveQuantization": H265AdaptiveQuantizationType,
         "AlternateTransferFunctionSei": H265AlternateTransferFunctionSeiType,
         "BandwidthReductionFilter": BandwidthReductionFilterTypeDef,
         "Bitrate": int,
@@ -2617,44 +4191,103 @@
         "Tiles": H265TilesType,
         "UnregisteredSeiTimecode": H265UnregisteredSeiTimecodeType,
         "WriteMp4PackagingType": H265WriteMp4PackagingTypeType,
     },
     total=False,
 )
 
-OutputSettingsTypeDef = TypedDict(
-    "OutputSettingsTypeDef",
+OutputSettingsOutputTypeDef = TypedDict(
+    "OutputSettingsOutputTypeDef",
     {
-        "HlsSettings": HlsSettingsTypeDef,
+        "HlsSettings": HlsSettingsOutputTypeDef,
+    },
+)
+
+TimedMetadataInsertionOutputTypeDef = TypedDict(
+    "TimedMetadataInsertionOutputTypeDef",
+    {
+        "Id3Insertions": List[Id3InsertionOutputTypeDef],
     },
-    total=False,
 )
 
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
+ImageInserterOutputTypeDef = TypedDict(
+    "ImageInserterOutputTypeDef",
+    {
+        "InsertableImages": List[InsertableImageOutputTypeDef],
+        "SdrReferenceWhiteLevel": int,
+    },
+)
+
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+M2tsSettingsOutputTypeDef = TypedDict(
+    "M2tsSettingsOutputTypeDef",
+    {
+        "AudioBufferModel": M2tsAudioBufferModelType,
+        "AudioDuration": M2tsAudioDurationType,
+        "AudioFramesPerPes": int,
+        "AudioPids": List[int],
+        "Bitrate": int,
+        "BufferModel": M2tsBufferModelType,
+        "DataPTSControl": M2tsDataPtsControlType,
+        "DvbNitSettings": DvbNitSettingsOutputTypeDef,
+        "DvbSdtSettings": DvbSdtSettingsOutputTypeDef,
+        "DvbSubPids": List[int],
+        "DvbTdtSettings": DvbTdtSettingsOutputTypeDef,
+        "DvbTeletextPid": int,
+        "EbpAudioInterval": M2tsEbpAudioIntervalType,
+        "EbpPlacement": M2tsEbpPlacementType,
+        "EsRateInPes": M2tsEsRateInPesType,
+        "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
+        "FragmentTime": float,
+        "KlvMetadata": M2tsKlvMetadataType,
+        "MaxPcrInterval": int,
+        "MinEbpInterval": int,
+        "NielsenId3": M2tsNielsenId3Type,
+        "NullPacketBitrate": float,
+        "PatInterval": int,
+        "PcrControl": M2tsPcrControlType,
+        "PcrPid": int,
+        "PmtInterval": int,
+        "PmtPid": int,
+        "PrivateMetadataPid": int,
+        "ProgramNumber": int,
+        "RateMode": M2tsRateModeType,
+        "Scte35Esam": M2tsScte35EsamOutputTypeDef,
+        "Scte35Pid": int,
+        "Scte35Source": M2tsScte35SourceType,
+        "SegmentationMarkers": M2tsSegmentationMarkersType,
+        "SegmentationStyle": M2tsSegmentationStyleType,
+        "SegmentationTime": float,
+        "TimedMetadataPid": int,
+        "TransportStreamId": int,
+        "VideoPid": int,
     },
 )
 
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
@@ -2696,45 +4329,83 @@
         "TimedMetadataPid": int,
         "TransportStreamId": int,
         "VideoPid": int,
     },
     total=False,
 )
 
+MotionImageInserterOutputTypeDef = TypedDict(
+    "MotionImageInserterOutputTypeDef",
+    {
+        "Framerate": MotionImageInsertionFramerateOutputTypeDef,
+        "Input": str,
+        "InsertionMode": MotionImageInsertionModeType,
+        "Offset": MotionImageInsertionOffsetOutputTypeDef,
+        "Playback": MotionImagePlaybackType,
+        "StartTime": str,
+    },
+)
+
 MotionImageInserterTypeDef = TypedDict(
     "MotionImageInserterTypeDef",
     {
         "Framerate": MotionImageInsertionFramerateTypeDef,
         "Input": str,
         "InsertionMode": MotionImageInsertionModeType,
         "Offset": MotionImageInsertionOffsetTypeDef,
         "Playback": MotionImagePlaybackType,
         "StartTime": str,
     },
     total=False,
 )
 
+MxfSettingsOutputTypeDef = TypedDict(
+    "MxfSettingsOutputTypeDef",
+    {
+        "AfdSignaling": MxfAfdSignalingType,
+        "Profile": MxfProfileType,
+        "XavcProfileSettings": MxfXavcProfileSettingsOutputTypeDef,
+    },
+)
+
 MxfSettingsTypeDef = TypedDict(
     "MxfSettingsTypeDef",
     {
         "AfdSignaling": MxfAfdSignalingType,
         "Profile": MxfProfileType,
         "XavcProfileSettings": MxfXavcProfileSettingsTypeDef,
     },
     total=False,
 )
 
+PartnerWatermarkingOutputTypeDef = TypedDict(
+    "PartnerWatermarkingOutputTypeDef",
+    {
+        "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsOutputTypeDef,
+    },
+)
+
 PartnerWatermarkingTypeDef = TypedDict(
     "PartnerWatermarkingTypeDef",
     {
         "NexguardFileMarkerSettings": NexGuardFileMarkerSettingsTypeDef,
     },
     total=False,
 )
 
+NoiseReducerOutputTypeDef = TypedDict(
+    "NoiseReducerOutputTypeDef",
+    {
+        "Filter": NoiseReducerFilterType,
+        "FilterSettings": NoiseReducerFilterSettingsOutputTypeDef,
+        "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsOutputTypeDef,
+        "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsOutputTypeDef,
+    },
+)
+
 NoiseReducerTypeDef = TypedDict(
     "NoiseReducerTypeDef",
     {
         "Filter": NoiseReducerFilterType,
         "FilterSettings": NoiseReducerFilterSettingsTypeDef,
         "SpatialFilterSettings": NoiseReducerSpatialFilterSettingsTypeDef,
         "TemporalFilterSettings": NoiseReducerTemporalFilterSettingsTypeDef,
@@ -2744,52 +4415,79 @@
 
 OutputDetailTypeDef = TypedDict(
     "OutputDetailTypeDef",
     {
         "DurationInMs": int,
         "VideoDetails": VideoDetailTypeDef,
     },
-    total=False,
 )
 
-_RequiredQueueTypeDef = TypedDict(
-    "_RequiredQueueTypeDef",
+PutPolicyRequestRequestTypeDef = TypedDict(
+    "PutPolicyRequestRequestTypeDef",
     {
-        "Name": str,
+        "Policy": PolicyTypeDef,
     },
 )
-_OptionalQueueTypeDef = TypedDict(
-    "_OptionalQueueTypeDef",
+
+QueueTypeDef = TypedDict(
+    "QueueTypeDef",
     {
         "Arn": str,
         "CreatedAt": datetime,
         "Description": str,
         "LastUpdated": datetime,
+        "Name": str,
         "PricingPlan": PricingPlanType,
         "ProgressingJobsCount": int,
         "ReservationPlan": ReservationPlanTypeDef,
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
-    total=False,
 )
 
-class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
-    pass
+S3DestinationSettingsOutputTypeDef = TypedDict(
+    "S3DestinationSettingsOutputTypeDef",
+    {
+        "AccessControl": S3DestinationAccessControlOutputTypeDef,
+        "Encryption": S3EncryptionSettingsOutputTypeDef,
+    },
+)
 
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
     },
     total=False,
 )
 
+XavcSettingsOutputTypeDef = TypedDict(
+    "XavcSettingsOutputTypeDef",
+    {
+        "AdaptiveQuantization": XavcAdaptiveQuantizationType,
+        "EntropyEncoding": XavcEntropyEncodingType,
+        "FramerateControl": XavcFramerateControlType,
+        "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
+        "FramerateDenominator": int,
+        "FramerateNumerator": int,
+        "Profile": XavcProfileType,
+        "SlowPal": XavcSlowPalType,
+        "Softness": int,
+        "SpatialAdaptiveQuantization": XavcSpatialAdaptiveQuantizationType,
+        "TemporalAdaptiveQuantization": XavcTemporalAdaptiveQuantizationType,
+        "Xavc4kIntraCbgProfileSettings": Xavc4kIntraCbgProfileSettingsOutputTypeDef,
+        "Xavc4kIntraVbrProfileSettings": Xavc4kIntraVbrProfileSettingsOutputTypeDef,
+        "Xavc4kProfileSettings": Xavc4kProfileSettingsOutputTypeDef,
+        "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsOutputTypeDef,
+        "XavcHdProfileSettings": XavcHdProfileSettingsOutputTypeDef,
+    },
+)
+
 XavcSettingsTypeDef = TypedDict(
     "XavcSettingsTypeDef",
     {
         "AdaptiveQuantization": XavcAdaptiveQuantizationType,
         "EntropyEncoding": XavcEntropyEncodingType,
         "FramerateControl": XavcFramerateControlType,
         "FramerateConversionAlgorithm": XavcFramerateConversionAlgorithmType,
@@ -2805,48 +4503,81 @@
         "Xavc4kProfileSettings": Xavc4kProfileSettingsTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedAbrSettingsOutputTypeDef = TypedDict(
+    "AutomatedAbrSettingsOutputTypeDef",
+    {
+        "MaxAbrBitrate": int,
+        "MaxRenditions": int,
+        "MinAbrBitrate": int,
+        "Rules": List[AutomatedAbrRuleOutputTypeDef],
+    },
+)
+
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
-CaptionDescriptionPresetTypeDef = TypedDict(
-    "CaptionDescriptionPresetTypeDef",
+CaptionDescriptionOutputTypeDef = TypedDict(
+    "CaptionDescriptionOutputTypeDef",
     {
+        "CaptionSelectorName": str,
         "CustomLanguageCode": str,
-        "DestinationSettings": CaptionDestinationSettingsTypeDef,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
-    total=False,
 )
 
-CaptionDescriptionTypeDef = TypedDict(
-    "CaptionDescriptionTypeDef",
+CaptionDescriptionPresetOutputTypeDef = TypedDict(
+    "CaptionDescriptionPresetOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "LanguageDescription": str,
+    },
+)
+
+CaptionDescriptionPresetTypeDef = TypedDict(
+    "CaptionDescriptionPresetTypeDef",
     {
-        "CaptionSelectorName": str,
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
     },
     total=False,
 )
 
+CaptionSourceSettingsOutputTypeDef = TypedDict(
+    "CaptionSourceSettingsOutputTypeDef",
+    {
+        "AncillarySourceSettings": AncillarySourceSettingsOutputTypeDef,
+        "DvbSubSourceSettings": DvbSubSourceSettingsOutputTypeDef,
+        "EmbeddedSourceSettings": EmbeddedSourceSettingsOutputTypeDef,
+        "FileSourceSettings": FileSourceSettingsOutputTypeDef,
+        "SourceType": CaptionSourceTypeType,
+        "TeletextSourceSettings": TeletextSourceSettingsOutputTypeDef,
+        "TrackSourceSettings": TrackSourceSettingsOutputTypeDef,
+        "WebvttHlsSourceSettings": WebvttHlsSourceSettingsOutputTypeDef,
+    },
+)
+
 CaptionSourceSettingsTypeDef = TypedDict(
     "CaptionSourceSettingsTypeDef",
     {
         "AncillarySourceSettings": AncillarySourceSettingsTypeDef,
         "DvbSubSourceSettings": DvbSubSourceSettingsTypeDef,
         "EmbeddedSourceSettings": EmbeddedSourceSettingsTypeDef,
         "FileSourceSettings": FileSourceSettingsTypeDef,
@@ -2854,24 +4585,48 @@
         "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
         "TrackSourceSettings": TrackSourceSettingsTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsTypeDef,
     },
     total=False,
 )
 
+RemixSettingsOutputTypeDef = TypedDict(
+    "RemixSettingsOutputTypeDef",
+    {
+        "ChannelMapping": ChannelMappingOutputTypeDef,
+        "ChannelsIn": int,
+        "ChannelsOut": int,
+    },
+)
+
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
+ContainerSettingsOutputTypeDef = TypedDict(
+    "ContainerSettingsOutputTypeDef",
+    {
+        "CmfcSettings": CmfcSettingsOutputTypeDef,
+        "Container": ContainerTypeType,
+        "F4vSettings": F4vSettingsOutputTypeDef,
+        "M2tsSettings": M2tsSettingsOutputTypeDef,
+        "M3u8Settings": M3u8SettingsOutputTypeDef,
+        "MovSettings": MovSettingsOutputTypeDef,
+        "Mp4Settings": Mp4SettingsOutputTypeDef,
+        "MpdSettings": MpdSettingsOutputTypeDef,
+        "MxfSettings": MxfSettingsOutputTypeDef,
+    },
+)
+
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
         "F4vSettings": F4vSettingsTypeDef,
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -2880,14 +4635,28 @@
         "Mp4Settings": Mp4SettingsTypeDef,
         "MpdSettings": MpdSettingsTypeDef,
         "MxfSettings": MxfSettingsTypeDef,
     },
     total=False,
 )
 
+VideoPreprocessorOutputTypeDef = TypedDict(
+    "VideoPreprocessorOutputTypeDef",
+    {
+        "ColorCorrector": ColorCorrectorOutputTypeDef,
+        "Deinterlacer": DeinterlacerOutputTypeDef,
+        "DolbyVision": DolbyVisionOutputTypeDef,
+        "Hdr10Plus": Hdr10PlusOutputTypeDef,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "NoiseReducer": NoiseReducerOutputTypeDef,
+        "PartnerWatermarking": PartnerWatermarkingOutputTypeDef,
+        "TimecodeBurnin": TimecodeBurninOutputTypeDef,
+    },
+)
+
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
         "DolbyVision": DolbyVisionTypeDef,
         "Hdr10Plus": Hdr10PlusTypeDef,
@@ -2900,58 +4669,82 @@
 )
 
 OutputGroupDetailTypeDef = TypedDict(
     "OutputGroupDetailTypeDef",
     {
         "OutputDetails": List[OutputDetailTypeDef],
     },
-    total=False,
 )
 
 CreateQueueResponseTypeDef = TypedDict(
     "CreateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueueResponseTypeDef = TypedDict(
     "GetQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueuesResponseTypeDef = TypedDict(
     "ListQueuesResponseTypeDef",
     {
         "NextToken": str,
         "Queues": List[QueueTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateQueueResponseTypeDef = TypedDict(
     "UpdateQueueResponseTypeDef",
     {
         "Queue": QueueTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DestinationSettingsOutputTypeDef = TypedDict(
+    "DestinationSettingsOutputTypeDef",
+    {
+        "S3Settings": S3DestinationSettingsOutputTypeDef,
     },
 )
 
 DestinationSettingsTypeDef = TypedDict(
     "DestinationSettingsTypeDef",
     {
         "S3Settings": S3DestinationSettingsTypeDef,
     },
     total=False,
 )
 
+VideoCodecSettingsOutputTypeDef = TypedDict(
+    "VideoCodecSettingsOutputTypeDef",
+    {
+        "Av1Settings": Av1SettingsOutputTypeDef,
+        "AvcIntraSettings": AvcIntraSettingsOutputTypeDef,
+        "Codec": VideoCodecType,
+        "FrameCaptureSettings": FrameCaptureSettingsOutputTypeDef,
+        "H264Settings": H264SettingsOutputTypeDef,
+        "H265Settings": H265SettingsOutputTypeDef,
+        "Mpeg2Settings": Mpeg2SettingsOutputTypeDef,
+        "ProresSettings": ProresSettingsOutputTypeDef,
+        "Vc3Settings": Vc3SettingsOutputTypeDef,
+        "Vp8Settings": Vp8SettingsOutputTypeDef,
+        "Vp9Settings": Vp9SettingsOutputTypeDef,
+        "XavcSettings": XavcSettingsOutputTypeDef,
+    },
+)
+
 VideoCodecSettingsTypeDef = TypedDict(
     "VideoCodecSettingsTypeDef",
     {
         "Av1Settings": Av1SettingsTypeDef,
         "AvcIntraSettings": AvcIntraSettingsTypeDef,
         "Codec": VideoCodecType,
         "FrameCaptureSettings": FrameCaptureSettingsTypeDef,
@@ -2963,32 +4756,83 @@
         "Vp8Settings": Vp8SettingsTypeDef,
         "Vp9Settings": Vp9SettingsTypeDef,
         "XavcSettings": XavcSettingsTypeDef,
     },
     total=False,
 )
 
+AutomatedEncodingSettingsOutputTypeDef = TypedDict(
+    "AutomatedEncodingSettingsOutputTypeDef",
+    {
+        "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
+    },
+)
+
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
 
+CaptionSelectorOutputTypeDef = TypedDict(
+    "CaptionSelectorOutputTypeDef",
+    {
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "SourceSettings": CaptionSourceSettingsOutputTypeDef,
+    },
+)
+
 CaptionSelectorTypeDef = TypedDict(
     "CaptionSelectorTypeDef",
     {
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
+AudioDescriptionOutputTypeDef = TypedDict(
+    "AudioDescriptionOutputTypeDef",
+    {
+        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsOutputTypeDef,
+        "AudioNormalizationSettings": AudioNormalizationSettingsOutputTypeDef,
+        "AudioSourceName": str,
+        "AudioType": int,
+        "AudioTypeControl": AudioTypeControlType,
+        "CodecSettings": AudioCodecSettingsOutputTypeDef,
+        "CustomLanguageCode": str,
+        "LanguageCode": LanguageCodeType,
+        "LanguageCodeControl": AudioLanguageCodeControlType,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "StreamName": str,
+    },
+)
+
+AudioSelectorOutputTypeDef = TypedDict(
+    "AudioSelectorOutputTypeDef",
+    {
+        "AudioDurationCorrection": AudioDurationCorrectionType,
+        "CustomLanguageCode": str,
+        "DefaultSelection": AudioDefaultSelectionType,
+        "ExternalAudioFileInput": str,
+        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsOutputTypeDef,
+        "LanguageCode": LanguageCodeType,
+        "Offset": int,
+        "Pids": List[int],
+        "ProgramSelection": int,
+        "RemixSettings": RemixSettingsOutputTypeDef,
+        "SelectorType": AudioSelectorTypeType,
+        "Tracks": List[int],
+    },
+)
+
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
@@ -3018,14 +4862,134 @@
         "RemixSettings": RemixSettingsTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": Sequence[int],
     },
     total=False,
 )
 
+CmafGroupSettingsOutputTypeDef = TypedDict(
+    "CmafGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
+        "BaseUrl": str,
+        "ClientCache": CmafClientCacheType,
+        "CodecSpecification": CmafCodecSpecificationType,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": CmafEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsOutputTypeDef,
+        "ManifestCompression": CmafManifestCompressionType,
+        "ManifestDurationFormat": CmafManifestDurationFormatType,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
+        "MpdProfile": CmafMpdProfileType,
+        "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
+        "SegmentControl": CmafSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": CmafSegmentLengthControlType,
+        "StreamInfResolution": CmafStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
+        "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
+        "WriteDashManifest": CmafWriteDASHManifestType,
+        "WriteHlsManifest": CmafWriteHLSManifestType,
+        "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
+    },
+)
+
+DashIsoGroupSettingsOutputTypeDef = TypedDict(
+    "DashIsoGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
+        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
+        "BaseUrl": str,
+        "DashManifestStyle": DashManifestStyleType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "HbbtvCompliance": DashIsoHbbtvComplianceType,
+        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
+        "MinBufferTime": int,
+        "MinFinalSegmentLength": float,
+        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
+        "MpdProfile": DashIsoMpdProfileType,
+        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
+        "SegmentControl": DashIsoSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": DashIsoSegmentLengthControlType,
+        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
+        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
+    },
+)
+
+FileGroupSettingsOutputTypeDef = TypedDict(
+    "FileGroupSettingsOutputTypeDef",
+    {
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+    },
+)
+
+HlsGroupSettingsOutputTypeDef = TypedDict(
+    "HlsGroupSettingsOutputTypeDef",
+    {
+        "AdMarkers": List[HlsAdMarkersType],
+        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
+        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
+        "BaseUrl": str,
+        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingOutputTypeDef],
+        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
+        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
+        "ClientCache": HlsClientCacheType,
+        "CodecSpecification": HlsCodecSpecificationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "DirectoryStructure": HlsDirectoryStructureType,
+        "Encryption": HlsEncryptionSettingsOutputTypeDef,
+        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
+        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsOutputTypeDef,
+        "ManifestCompression": HlsManifestCompressionType,
+        "ManifestDurationFormat": HlsManifestDurationFormatType,
+        "MinFinalSegmentLength": float,
+        "MinSegmentLength": int,
+        "OutputSelection": HlsOutputSelectionType,
+        "ProgramDateTime": HlsProgramDateTimeType,
+        "ProgramDateTimePeriod": int,
+        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
+        "SegmentControl": HlsSegmentControlType,
+        "SegmentLength": int,
+        "SegmentLengthControl": HlsSegmentLengthControlType,
+        "SegmentsPerSubdirectory": int,
+        "StreamInfResolution": HlsStreamInfResolutionType,
+        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
+        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
+        "TimedMetadataId3Period": int,
+        "TimestampDeltaMilliseconds": int,
+    },
+)
+
+MsSmoothGroupSettingsOutputTypeDef = TypedDict(
+    "MsSmoothGroupSettingsOutputTypeDef",
+    {
+        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
+        "AudioDeduplication": MsSmoothAudioDeduplicationType,
+        "Destination": str,
+        "DestinationSettings": DestinationSettingsOutputTypeDef,
+        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
+        "FragmentLength": int,
+        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
+        "ManifestEncoding": MsSmoothManifestEncodingType,
+    },
+)
+
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
@@ -3143,14 +5107,35 @@
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
     total=False,
 )
 
+VideoDescriptionOutputTypeDef = TypedDict(
+    "VideoDescriptionOutputTypeDef",
+    {
+        "AfdSignaling": AfdSignalingType,
+        "AntiAlias": AntiAliasType,
+        "CodecSettings": VideoCodecSettingsOutputTypeDef,
+        "ColorMetadata": ColorMetadataType,
+        "Crop": RectangleOutputTypeDef,
+        "DropFrameTimecode": DropFrameTimecodeType,
+        "FixedAfd": int,
+        "Height": int,
+        "Position": RectangleOutputTypeDef,
+        "RespondToAfd": RespondToAfdType,
+        "ScalingBehavior": ScalingBehaviorType,
+        "Sharpness": int,
+        "TimecodeInsertion": VideoTimecodeInsertionType,
+        "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
+        "Width": int,
+    },
+)
+
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
         "CodecSettings": VideoCodecSettingsTypeDef,
         "ColorMetadata": ColorMetadataType,
@@ -3165,14 +5150,70 @@
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorTypeDef,
         "Width": int,
     },
     total=False,
 )
 
+InputOutputTypeDef = TypedDict(
+    "InputOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DecryptionSettings": InputDecryptionSettingsOutputTypeDef,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FileInput": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingOutputTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleOutputTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "SupplementalImps": List[str],
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoGenerator": InputVideoGeneratorOutputTypeDef,
+        "VideoSelector": VideoSelectorOutputTypeDef,
+    },
+)
+
+InputTemplateOutputTypeDef = TypedDict(
+    "InputTemplateOutputTypeDef",
+    {
+        "AdvancedInputFilter": AdvancedInputFilterType,
+        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsOutputTypeDef,
+        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
+        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
+        "CaptionSelectors": Dict[str, CaptionSelectorOutputTypeDef],
+        "Crop": RectangleOutputTypeDef,
+        "DeblockFilter": InputDeblockFilterType,
+        "DenoiseFilter": InputDenoiseFilterType,
+        "DolbyVisionMetadataXml": str,
+        "FilterEnable": InputFilterEnableType,
+        "FilterStrength": int,
+        "ImageInserter": ImageInserterOutputTypeDef,
+        "InputClippings": List[InputClippingOutputTypeDef],
+        "InputScanType": InputScanTypeType,
+        "Position": RectangleOutputTypeDef,
+        "ProgramNumber": int,
+        "PsiControl": InputPsiControlType,
+        "TimecodeSource": InputTimecodeSourceType,
+        "TimecodeStart": str,
+        "VideoSelector": VideoSelectorOutputTypeDef,
+    },
+)
+
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
@@ -3223,14 +5264,26 @@
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorTypeDef,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
+OutputGroupSettingsOutputTypeDef = TypedDict(
+    "OutputGroupSettingsOutputTypeDef",
+    {
+        "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
+        "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
+        "FileGroupSettings": FileGroupSettingsOutputTypeDef,
+        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
+        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
+        "Type": OutputGroupTypeType,
+    },
+)
+
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
         "FileGroupSettings": FileGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
@@ -3239,49 +5292,83 @@
     },
     total=False,
 )
 
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
-        "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
-        "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
-        "ContainerSettings": ContainerSettingsTypeDef,
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
         "Extension": str,
         "NameModifier": str,
-        "OutputSettings": OutputSettingsTypeDef,
+        "OutputSettings": OutputSettingsOutputTypeDef,
         "Preset": str,
-        "VideoDescription": VideoDescriptionTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
+    },
+)
+
+PresetSettingsOutputTypeDef = TypedDict(
+    "PresetSettingsOutputTypeDef",
+    {
+        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
+        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
+        "ContainerSettings": ContainerSettingsOutputTypeDef,
+        "VideoDescription": VideoDescriptionOutputTypeDef,
     },
-    total=False,
 )
 
 PresetSettingsTypeDef = TypedDict(
     "PresetSettingsTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
+OutputGroupOutputTypeDef = TypedDict(
+    "OutputGroupOutputTypeDef",
+    {
+        "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
+        "CustomName": str,
+        "Name": str,
+        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
+        "Outputs": List[OutputTypeDef],
+    },
+)
+
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
         "Outputs": Sequence[OutputTypeDef],
     },
     total=False,
 )
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Name": str,
+        "Settings": PresetSettingsOutputTypeDef,
+        "Type": TypeType,
+    },
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": PresetSettingsTypeDef,
     },
 )
@@ -3296,37 +5383,14 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
-    {
-        "Arn": str,
-        "Category": str,
-        "CreatedAt": datetime,
-        "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
 _RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
@@ -3340,14 +5404,50 @@
 )
 
 class UpdatePresetRequestRequestTypeDef(
     _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
 ):
     pass
 
+JobSettingsOutputTypeDef = TypedDict(
+    "JobSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
+        "Inputs": List[InputOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+)
+
+JobTemplateSettingsOutputTypeDef = TypedDict(
+    "JobTemplateSettingsOutputTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingOutputTypeDef,
+        "Esam": EsamSettingsOutputTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesOutputTypeDef,
+        "Inputs": List[InputTemplateOutputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsOutputTypeDef,
+        "MotionImageInserter": MotionImageInserterOutputTypeDef,
+        "NielsenConfiguration": NielsenConfigurationOutputTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsOutputTypeDef,
+        "OutputGroups": List[OutputGroupOutputTypeDef],
+        "TimecodeConfig": TimecodeConfigOutputTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+    },
+)
+
 JobSettingsTypeDef = TypedDict(
     "JobSettingsTypeDef",
     {
         "AdAvailOffset": int,
         "AvailBlanking": AvailBlankingTypeDef,
         "Esam": EsamSettingsTypeDef,
         "ExtendedDataServices": ExtendedDataServicesTypeDef,
@@ -3382,168 +5482,150 @@
     total=False,
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPresetResponseTypeDef = TypedDict(
     "GetPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "NextToken": str,
         "Presets": List[PresetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePresetResponseTypeDef = TypedDict(
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
-        "BillingTagsSource": BillingTagsSourceType,
-        "ClientRequestToken": str,
-        "HopDestinations": Sequence[HopDestinationTypeDef],
-        "JobTemplate": str,
-        "Priority": int,
-        "Queue": str,
-        "SimulateReservedQueue": SimulateReservedQueueType,
-        "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Tags": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
-_RequiredJobTypeDef = TypedDict(
-    "_RequiredJobTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalJobTypeDef = TypedDict(
-    "_OptionalJobTypeDef",
+JobTypeDef = TypedDict(
+    "JobTypeDef",
     {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
         "AccelerationStatus": AccelerationStatusType,
         "Arn": str,
         "BillingTagsSource": BillingTagsSourceType,
         "ClientRequestToken": str,
         "CreatedAt": datetime,
         "CurrentPhase": JobPhaseType,
         "ErrorCode": int,
         "ErrorMessage": str,
-        "HopDestinations": List[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationOutputTypeDef],
         "Id": str,
         "JobPercentComplete": int,
         "JobTemplate": str,
         "Messages": JobMessagesTypeDef,
         "OutputGroupDetails": List[OutputGroupDetailTypeDef],
         "Priority": int,
         "Queue": str,
         "QueueTransitions": List[QueueTransitionTypeDef],
         "RetryCount": int,
+        "Role": str,
+        "Settings": JobSettingsOutputTypeDef,
         "SimulateReservedQueue": SimulateReservedQueueType,
         "Status": JobStatusType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
-    total=False,
 )
 
-class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
-    pass
-
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+JobTemplateTypeDef = TypedDict(
+    "JobTemplateTypeDef",
     {
+        "AccelerationSettings": AccelerationSettingsOutputTypeDef,
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "HopDestinations": List[HopDestinationOutputTypeDef],
+        "LastUpdated": datetime,
         "Name": str,
-        "Settings": JobTemplateSettingsTypeDef,
+        "Priority": int,
+        "Queue": str,
+        "Settings": JobTemplateSettingsOutputTypeDef,
+        "StatusUpdateInterval": StatusUpdateIntervalType,
+        "Type": TypeType,
     },
 )
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "Role": str,
+        "Settings": JobSettingsTypeDef,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Category": str,
-        "Description": str,
+        "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
         "HopDestinations": Sequence[HopDestinationTypeDef],
+        "JobTemplate": str,
         "Priority": int,
         "Queue": str,
+        "SimulateReservedQueue": SimulateReservedQueueType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Tags": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
 
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
-        "LastUpdated": datetime,
+        "HopDestinations": Sequence[HopDestinationTypeDef],
         "Priority": int,
         "Queue": str,
         "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Type": TypeType,
+        "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
+):
     pass
 
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -3568,60 +5650,60 @@
 ):
     pass
 
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobResponseTypeDef = TypedDict(
     "GetJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateJobTemplateResponseTypeDef = TypedDict(
     "CreateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetJobTemplateResponseTypeDef = TypedDict(
     "GetJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "JobTemplates": List[JobTemplateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobTemplateResponseTypeDef = TypedDict(
     "UpdateJobTemplateResponseTypeDef",
     {
         "JobTemplate": JobTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/PKG-INFO` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediaconvert
-Version: 1.28.0
-Summary: Type annotations for boto3.MediaConvert 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.9
+Summary: Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder 7.15.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediaconvert.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediaconvert)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-mediaconvert?color=blue)](https://pypistats.org/packages/mypy-boto3-mediaconvert)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaConvert 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
+[boto3.MediaConvert 1.28.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.15.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mediaconvert docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediaconvert/).
 
 See how it helps to find and fix potential bugs:
 
@@ -743,245 +743,401 @@
 ### Typed dictionaries
 
 `mypy_boto3_mediaconvert.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediaconvert.type_defs import (
+    AacSettingsOutputTypeDef,
     AacSettingsTypeDef,
+    Ac3SettingsOutputTypeDef,
     Ac3SettingsTypeDef,
+    AccelerationSettingsOutputTypeDef,
     AccelerationSettingsTypeDef,
+    AdvancedInputFilterSettingsOutputTypeDef,
     AdvancedInputFilterSettingsTypeDef,
+    AiffSettingsOutputTypeDef,
     AiffSettingsTypeDef,
+    AllowedRenditionSizeOutputTypeDef,
     AllowedRenditionSizeTypeDef,
+    AncillarySourceSettingsOutputTypeDef,
     AncillarySourceSettingsTypeDef,
     AssociateCertificateRequestRequestTypeDef,
+    AudioChannelTaggingSettingsOutputTypeDef,
     AudioChannelTaggingSettingsTypeDef,
+    Eac3AtmosSettingsOutputTypeDef,
+    Eac3SettingsOutputTypeDef,
+    Mp2SettingsOutputTypeDef,
+    Mp3SettingsOutputTypeDef,
+    OpusSettingsOutputTypeDef,
+    VorbisSettingsOutputTypeDef,
+    WavSettingsOutputTypeDef,
     Eac3AtmosSettingsTypeDef,
     Eac3SettingsTypeDef,
     Mp2SettingsTypeDef,
     Mp3SettingsTypeDef,
     OpusSettingsTypeDef,
     VorbisSettingsTypeDef,
     WavSettingsTypeDef,
+    AudioNormalizationSettingsOutputTypeDef,
     AudioNormalizationSettingsTypeDef,
+    AudioSelectorGroupOutputTypeDef,
     AudioSelectorGroupTypeDef,
+    HlsRenditionGroupSettingsOutputTypeDef,
     HlsRenditionGroupSettingsTypeDef,
+    ForceIncludeRenditionSizeOutputTypeDef,
+    MinBottomRenditionSizeOutputTypeDef,
+    MinTopRenditionSizeOutputTypeDef,
     ForceIncludeRenditionSizeTypeDef,
     MinBottomRenditionSizeTypeDef,
     MinTopRenditionSizeTypeDef,
+    Av1QvbrSettingsOutputTypeDef,
     Av1QvbrSettingsTypeDef,
+    AvailBlankingOutputTypeDef,
     AvailBlankingTypeDef,
+    AvcIntraUhdSettingsOutputTypeDef,
     AvcIntraUhdSettingsTypeDef,
+    BandwidthReductionFilterOutputTypeDef,
     BandwidthReductionFilterTypeDef,
+    BurninDestinationSettingsOutputTypeDef,
     BurninDestinationSettingsTypeDef,
     CancelJobRequestRequestTypeDef,
+    DvbSubDestinationSettingsOutputTypeDef,
+    EmbeddedDestinationSettingsOutputTypeDef,
+    ImscDestinationSettingsOutputTypeDef,
+    SccDestinationSettingsOutputTypeDef,
+    SrtDestinationSettingsOutputTypeDef,
+    TeletextDestinationSettingsOutputTypeDef,
+    TtmlDestinationSettingsOutputTypeDef,
+    WebvttDestinationSettingsOutputTypeDef,
     DvbSubDestinationSettingsTypeDef,
     EmbeddedDestinationSettingsTypeDef,
     ImscDestinationSettingsTypeDef,
     SccDestinationSettingsTypeDef,
     SrtDestinationSettingsTypeDef,
     TeletextDestinationSettingsTypeDef,
     TtmlDestinationSettingsTypeDef,
     WebvttDestinationSettingsTypeDef,
+    CaptionSourceFramerateOutputTypeDef,
     CaptionSourceFramerateTypeDef,
+    DvbSubSourceSettingsOutputTypeDef,
+    EmbeddedSourceSettingsOutputTypeDef,
+    TeletextSourceSettingsOutputTypeDef,
+    TrackSourceSettingsOutputTypeDef,
+    WebvttHlsSourceSettingsOutputTypeDef,
     DvbSubSourceSettingsTypeDef,
     EmbeddedSourceSettingsTypeDef,
     TeletextSourceSettingsTypeDef,
     TrackSourceSettingsTypeDef,
     WebvttHlsSourceSettingsTypeDef,
+    OutputChannelMappingOutputTypeDef,
     OutputChannelMappingTypeDef,
+    ClipLimitsOutputTypeDef,
     ClipLimitsTypeDef,
+    CmafAdditionalManifestOutputTypeDef,
     CmafAdditionalManifestTypeDef,
+    SpekeKeyProviderCmafOutputTypeDef,
+    StaticKeyProviderOutputTypeDef,
     SpekeKeyProviderCmafTypeDef,
     StaticKeyProviderTypeDef,
+    CmafImageBasedTrickPlaySettingsOutputTypeDef,
     CmafImageBasedTrickPlaySettingsTypeDef,
+    CmfcSettingsOutputTypeDef,
     CmfcSettingsTypeDef,
+    Hdr10MetadataOutputTypeDef,
     Hdr10MetadataTypeDef,
+    F4vSettingsOutputTypeDef,
+    M3u8SettingsOutputTypeDef,
+    MovSettingsOutputTypeDef,
+    Mp4SettingsOutputTypeDef,
+    MpdSettingsOutputTypeDef,
     F4vSettingsTypeDef,
     M3u8SettingsTypeDef,
     MovSettingsTypeDef,
     Mp4SettingsTypeDef,
     MpdSettingsTypeDef,
     HopDestinationTypeDef,
+    ResponseMetadataTypeDef,
     ReservationPlanSettingsTypeDef,
+    DashAdditionalManifestOutputTypeDef,
     DashAdditionalManifestTypeDef,
+    SpekeKeyProviderOutputTypeDef,
     SpekeKeyProviderTypeDef,
+    DashIsoImageBasedTrickPlaySettingsOutputTypeDef,
     DashIsoImageBasedTrickPlaySettingsTypeDef,
+    DeinterlacerOutputTypeDef,
     DeinterlacerTypeDef,
     DeleteJobTemplateRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
-    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEndpointsRequestRequestTypeDef,
     EndpointTypeDef,
     DisassociateCertificateRequestRequestTypeDef,
+    DolbyVisionLevel6MetadataOutputTypeDef,
     DolbyVisionLevel6MetadataTypeDef,
+    DvbNitSettingsOutputTypeDef,
     DvbNitSettingsTypeDef,
+    DvbSdtSettingsOutputTypeDef,
     DvbSdtSettingsTypeDef,
+    DvbTdtSettingsOutputTypeDef,
     DvbTdtSettingsTypeDef,
+    EsamManifestConfirmConditionNotificationOutputTypeDef,
     EsamManifestConfirmConditionNotificationTypeDef,
+    EsamSignalProcessingNotificationOutputTypeDef,
     EsamSignalProcessingNotificationTypeDef,
+    ExtendedDataServicesOutputTypeDef,
     ExtendedDataServicesTypeDef,
+    FrameCaptureSettingsOutputTypeDef,
     FrameCaptureSettingsTypeDef,
     GetJobRequestRequestTypeDef,
     GetJobTemplateRequestRequestTypeDef,
-    PolicyTypeDef,
+    PolicyOutputTypeDef,
     GetPresetRequestRequestTypeDef,
     GetQueueRequestRequestTypeDef,
+    H264QvbrSettingsOutputTypeDef,
     H264QvbrSettingsTypeDef,
+    H265QvbrSettingsOutputTypeDef,
     H265QvbrSettingsTypeDef,
+    Hdr10PlusOutputTypeDef,
     Hdr10PlusTypeDef,
+    HlsAdditionalManifestOutputTypeDef,
     HlsAdditionalManifestTypeDef,
+    HlsCaptionLanguageMappingOutputTypeDef,
     HlsCaptionLanguageMappingTypeDef,
+    HlsImageBasedTrickPlaySettingsOutputTypeDef,
     HlsImageBasedTrickPlaySettingsTypeDef,
-    HlsSettingsTypeDef,
+    HlsSettingsOutputTypeDef,
+    HopDestinationOutputTypeDef,
+    Id3InsertionOutputTypeDef,
     Id3InsertionTypeDef,
+    InsertableImageOutputTypeDef,
     InsertableImageTypeDef,
+    InputClippingOutputTypeDef,
     InputClippingTypeDef,
+    InputDecryptionSettingsOutputTypeDef,
     InputDecryptionSettingsTypeDef,
+    InputVideoGeneratorOutputTypeDef,
+    RectangleOutputTypeDef,
     RectangleTypeDef,
     InputVideoGeneratorTypeDef,
     JobMessagesTypeDef,
+    KantarWatermarkSettingsOutputTypeDef,
+    NielsenConfigurationOutputTypeDef,
+    NielsenNonLinearWatermarkSettingsOutputTypeDef,
+    TimecodeConfigOutputTypeDef,
     KantarWatermarkSettingsTypeDef,
     NielsenConfigurationTypeDef,
     NielsenNonLinearWatermarkSettingsTypeDef,
     TimecodeConfigTypeDef,
     QueueTransitionTypeDef,
     TimingTypeDef,
     WarningGroupTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ResourceTagsTypeDef,
+    M2tsScte35EsamOutputTypeDef,
     M2tsScte35EsamTypeDef,
+    MotionImageInsertionFramerateOutputTypeDef,
+    MotionImageInsertionOffsetOutputTypeDef,
     MotionImageInsertionFramerateTypeDef,
     MotionImageInsertionOffsetTypeDef,
+    Mpeg2SettingsOutputTypeDef,
     Mpeg2SettingsTypeDef,
+    MsSmoothAdditionalManifestOutputTypeDef,
     MsSmoothAdditionalManifestTypeDef,
+    MxfXavcProfileSettingsOutputTypeDef,
     MxfXavcProfileSettingsTypeDef,
+    NexGuardFileMarkerSettingsOutputTypeDef,
     NexGuardFileMarkerSettingsTypeDef,
+    NoiseReducerFilterSettingsOutputTypeDef,
     NoiseReducerFilterSettingsTypeDef,
+    NoiseReducerSpatialFilterSettingsOutputTypeDef,
+    NoiseReducerTemporalFilterSettingsOutputTypeDef,
     NoiseReducerSpatialFilterSettingsTypeDef,
     NoiseReducerTemporalFilterSettingsTypeDef,
     VideoDetailTypeDef,
-    PaginatorConfigTypeDef,
+    PolicyTypeDef,
+    ProresSettingsOutputTypeDef,
     ProresSettingsTypeDef,
     ReservationPlanTypeDef,
-    ResponseMetadataTypeDef,
+    S3DestinationAccessControlOutputTypeDef,
     S3DestinationAccessControlTypeDef,
+    S3EncryptionSettingsOutputTypeDef,
     S3EncryptionSettingsTypeDef,
     TagResourceRequestRequestTypeDef,
+    TimecodeBurninOutputTypeDef,
     TimecodeBurninTypeDef,
     UntagResourceRequestRequestTypeDef,
+    Vc3SettingsOutputTypeDef,
     Vc3SettingsTypeDef,
+    Vp8SettingsOutputTypeDef,
+    Vp9SettingsOutputTypeDef,
     Vp8SettingsTypeDef,
     Vp9SettingsTypeDef,
+    Xavc4kIntraCbgProfileSettingsOutputTypeDef,
     Xavc4kIntraCbgProfileSettingsTypeDef,
+    Xavc4kIntraVbrProfileSettingsOutputTypeDef,
     Xavc4kIntraVbrProfileSettingsTypeDef,
+    Xavc4kProfileSettingsOutputTypeDef,
     Xavc4kProfileSettingsTypeDef,
+    XavcHdIntraCbgProfileSettingsOutputTypeDef,
     XavcHdIntraCbgProfileSettingsTypeDef,
+    XavcHdProfileSettingsOutputTypeDef,
     XavcHdProfileSettingsTypeDef,
+    AudioCodecSettingsOutputTypeDef,
     AudioCodecSettingsTypeDef,
+    AutomatedAbrRuleOutputTypeDef,
     AutomatedAbrRuleTypeDef,
+    Av1SettingsOutputTypeDef,
     Av1SettingsTypeDef,
+    AvcIntraSettingsOutputTypeDef,
     AvcIntraSettingsTypeDef,
+    CaptionDestinationSettingsOutputTypeDef,
     CaptionDestinationSettingsTypeDef,
+    FileSourceSettingsOutputTypeDef,
     FileSourceSettingsTypeDef,
+    ChannelMappingOutputTypeDef,
     ChannelMappingTypeDef,
+    CmafEncryptionSettingsOutputTypeDef,
     CmafEncryptionSettingsTypeDef,
+    ColorCorrectorOutputTypeDef,
+    VideoSelectorOutputTypeDef,
     ColorCorrectorTypeDef,
     VideoSelectorTypeDef,
     CreateQueueRequestRequestTypeDef,
     UpdateQueueRequestRequestTypeDef,
+    DashIsoEncryptionSettingsOutputTypeDef,
+    HlsEncryptionSettingsOutputTypeDef,
+    MsSmoothEncryptionSettingsOutputTypeDef,
     DashIsoEncryptionSettingsTypeDef,
     HlsEncryptionSettingsTypeDef,
     MsSmoothEncryptionSettingsTypeDef,
+    DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     DescribeEndpointsResponseTypeDef,
+    DolbyVisionOutputTypeDef,
     DolbyVisionTypeDef,
+    EsamSettingsOutputTypeDef,
     EsamSettingsTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    H264SettingsOutputTypeDef,
     H264SettingsTypeDef,
+    H265SettingsOutputTypeDef,
     H265SettingsTypeDef,
-    OutputSettingsTypeDef,
+    OutputSettingsOutputTypeDef,
+    TimedMetadataInsertionOutputTypeDef,
     TimedMetadataInsertionTypeDef,
+    ImageInserterOutputTypeDef,
     ImageInserterTypeDef,
     ListTagsForResourceResponseTypeDef,
+    M2tsSettingsOutputTypeDef,
     M2tsSettingsTypeDef,
+    MotionImageInserterOutputTypeDef,
     MotionImageInserterTypeDef,
+    MxfSettingsOutputTypeDef,
     MxfSettingsTypeDef,
+    PartnerWatermarkingOutputTypeDef,
     PartnerWatermarkingTypeDef,
+    NoiseReducerOutputTypeDef,
     NoiseReducerTypeDef,
     OutputDetailTypeDef,
+    PutPolicyRequestRequestTypeDef,
     QueueTypeDef,
+    S3DestinationSettingsOutputTypeDef,
     S3DestinationSettingsTypeDef,
+    XavcSettingsOutputTypeDef,
     XavcSettingsTypeDef,
+    AutomatedAbrSettingsOutputTypeDef,
     AutomatedAbrSettingsTypeDef,
+    CaptionDescriptionOutputTypeDef,
+    CaptionDescriptionPresetOutputTypeDef,
     CaptionDescriptionPresetTypeDef,
-    CaptionDescriptionTypeDef,
+    CaptionSourceSettingsOutputTypeDef,
     CaptionSourceSettingsTypeDef,
+    RemixSettingsOutputTypeDef,
     RemixSettingsTypeDef,
+    ContainerSettingsOutputTypeDef,
     ContainerSettingsTypeDef,
+    VideoPreprocessorOutputTypeDef,
     VideoPreprocessorTypeDef,
     OutputGroupDetailTypeDef,
     CreateQueueResponseTypeDef,
     GetQueueResponseTypeDef,
     ListQueuesResponseTypeDef,
     UpdateQueueResponseTypeDef,
+    DestinationSettingsOutputTypeDef,
     DestinationSettingsTypeDef,
+    VideoCodecSettingsOutputTypeDef,
     VideoCodecSettingsTypeDef,
+    AutomatedEncodingSettingsOutputTypeDef,
     AutomatedEncodingSettingsTypeDef,
+    CaptionSelectorOutputTypeDef,
     CaptionSelectorTypeDef,
+    AudioDescriptionOutputTypeDef,
+    AudioSelectorOutputTypeDef,
     AudioDescriptionTypeDef,
     AudioSelectorTypeDef,
+    CmafGroupSettingsOutputTypeDef,
+    DashIsoGroupSettingsOutputTypeDef,
+    FileGroupSettingsOutputTypeDef,
+    HlsGroupSettingsOutputTypeDef,
+    MsSmoothGroupSettingsOutputTypeDef,
     CmafGroupSettingsTypeDef,
     DashIsoGroupSettingsTypeDef,
     FileGroupSettingsTypeDef,
     HlsGroupSettingsTypeDef,
     MsSmoothGroupSettingsTypeDef,
+    VideoDescriptionOutputTypeDef,
     VideoDescriptionTypeDef,
+    InputOutputTypeDef,
+    InputTemplateOutputTypeDef,
     InputTemplateTypeDef,
     InputTypeDef,
+    OutputGroupSettingsOutputTypeDef,
     OutputGroupSettingsTypeDef,
     OutputTypeDef,
+    PresetSettingsOutputTypeDef,
     PresetSettingsTypeDef,
+    OutputGroupOutputTypeDef,
     OutputGroupTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
+    CreatePresetRequestRequestTypeDef,
     UpdatePresetRequestRequestTypeDef,
+    JobSettingsOutputTypeDef,
+    JobTemplateSettingsOutputTypeDef,
     JobSettingsTypeDef,
     JobTemplateSettingsTypeDef,
     CreatePresetResponseTypeDef,
     GetPresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     UpdatePresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
-    CreateJobTemplateRequestRequestTypeDef,
     JobTemplateTypeDef,
+    CreateJobRequestRequestTypeDef,
+    CreateJobTemplateRequestRequestTypeDef,
     UpdateJobTemplateRequestRequestTypeDef,
     CreateJobResponseTypeDef,
     GetJobResponseTypeDef,
     ListJobsResponseTypeDef,
     CreateJobTemplateResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     UpdateJobTemplateResponseTypeDef,
 )
 
 
-def get_structure() -> AacSettingsTypeDef:
+def get_structure() -> AacSettingsOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-mediaconvert-1.28.0/mypy_boto3_mediaconvert.egg-info/SOURCES.txt` & `mypy-boto3-mediaconvert-1.28.9/mypy_boto3_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediaconvert-1.28.0/setup.py` & `mypy-boto3-mediaconvert-1.28.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediaconvert",
-    version="1.28.0",
+    version="1.28.9",
     packages=["mypy_boto3_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaConvert 1.28.0 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        "Type annotations for boto3.MediaConvert 1.28.9 service generated with mypy-boto3-builder"
+        " 7.15.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

