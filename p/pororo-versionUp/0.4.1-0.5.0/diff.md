# Comparing `tmp/pororo_versionUp-0.4.1.tar.gz` & `tmp/pororo_versionUp-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pororo_versionUp-0.4.1.tar", last modified: Fri Jul 21 10:58:29 2023, max compression
+gzip compressed data, was "pororo_versionUp-0.5.0.tar", last modified: Fri Jul 21 11:09:24 2023, max compression
```

## Comparing `pororo_versionUp-0.4.1.tar` & `pororo_versionUp-0.5.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.895573 pororo_versionUp-0.4.1/
--rw-rw-rw-   0        0        0     3156 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/INSTALL.md
--rw-rw-rw-   0        0        0    11368 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/LICENSE
--rw-rw-rw-   0        0        0    26965 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/LICENSE.3rd_party_library
--rw-rw-rw-   0        0        0      966 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/LICENSE.3rd_party_model
--rw-rw-rw-   0        0        0      118 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     8757 2023-07-21 10:58:29.895573 pororo_versionUp-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     7813 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.655343 pororo_versionUp-0.4.1/pororo/
--rw-rw-rw-   0        0        0      103 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/__init__.py
--rw-rw-rw-   0        0        0       18 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/__version__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.669217 pororo_versionUp-0.4.1/pororo/models/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.673109 pororo_versionUp-0.4.1/pororo/models/bart/
--rw-rw-rw-   0        0        0     6299 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/bart/KoBART.py
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/bart/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.688077 pororo_versionUp-0.4.1/pororo/models/brainOCR/
--rw-rw-rw-   0        0        0       37 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/__init__.py
--rw-rw-rw-   0        0        0     1022 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/_dataset.py
--rw-rw-rw-   0        0        0    20996 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/_modules.py
--rw-rw-rw-   0        0        0     8365 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/brainocr.py
--rw-rw-rw-   0        0        0     2938 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/craft.py
--rw-rw-rw-   0        0        0    10051 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/craft_utils.py
--rw-rw-rw-   0        0        0     2706 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/detection.py
--rw-rw-rw-   0        0        0     2421 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/imgproc.py
--rw-rw-rw-   0        0        0     3831 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/model.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.700966 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/__init__.py
--rw-rw-rw-   0        0        0     2897 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/basenet.py
--rw-rw-rw-   0        0        0    11445 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/feature_extraction.py
--rw-rw-rw-   0        0        0     4524 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/prediction.py
--rw-rw-rw-   0        0        0      859 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/sequence_modeling.py
--rw-rw-rw-   0        0        0     8768 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/transformation.py
--rw-rw-rw-   0        0        0     7845 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/recognition.py
--rw-rw-rw-   0        0        0    25982 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainOCR/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.712043 pororo_versionUp-0.4.1/pororo/models/brainbert/
--rw-rw-rw-   0        0        0    17950 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/BrainLaBERTa.py
--rw-rw-rw-   0        0        0     9854 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/BrainRoBERTa.py
--rw-rw-rw-   0        0        0     9064 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/CharBrainRoBERTa.py
--rw-rw-rw-   0        0        0     5628 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/EnBERTa.py
--rw-rw-rw-   0        0        0     6231 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/JaBERTa.py
--rw-rw-rw-   0        0        0    16989 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/PoSLaBERTa.py
--rw-rw-rw-   0        0        0     4052 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/PosRoBERTa.py
--rw-rw-rw-   0        0        0     5577 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/ZhBERTa.py
--rw-rw-rw-   0        0        0     1581 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.720071 pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/__init__.py
--rw-rw-rw-   0        0        0     5828 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/dependency_parse.py
--rw-rw-rw-   0        0        0     3733 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/sequence_tagging.py
--rw-rw-rw-   0        0        0     3801 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/sequence_tagging_label.py
--rw-rw-rw-   0        0        0     6545 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/span_prediction.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.728332 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/__init__.py
--rw-rw-rw-   0        0        0     7900 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/brain_roberta_task.py
--rw-rw-rw-   0        0        0    12935 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/dependency_parse.py
--rw-rw-rw-   0        0        0     8093 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/sequence_tagging.py
--rw-rw-rw-   0        0        0     8924 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/sequence_tagging_label.py
--rw-rw-rw-   0        0        0     9431 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/span_prediction.py
--rw-rw-rw-   0        0        0     1432 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainbert/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.728332 pororo_versionUp-0.4.1/pororo/models/brainsbert/
--rw-rw-rw-   0        0        0     6052 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainsbert/BrainRoBERTa.py
--rw-rw-rw-   0        0        0       71 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/brainsbert/__init__.py
--rw-rw-rw-   0        0        0    13799 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/caption.py
--rw-rw-rw-   0        0        0     3863 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/collocate.py
--rw-rw-rw-   0        0        0     5379 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/p2g.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.736386 pororo_versionUp-0.4.1/pororo/models/tts/
--rw-rw-rw-   0        0        0       80 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.736386 pororo_versionUp-0.4.1/pororo/models/tts/hifigan/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/hifigan/__init__.py
--rw-rw-rw-   0        0        0      470 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/hifigan/checkpoint.py
--rw-rw-rw-   0        0        0    12068 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/hifigan/model.py
--rw-rw-rw-   0        0        0     1712 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/synthesis.py
--rw-rw-rw-   0        0        0     5441 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/synthesizer.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.745633 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/__init__.py
--rw-rw-rw-   0        0        0     4188 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/attention.py
--rw-rw-rw-   0        0        0     3973 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/encoder.py
--rw-rw-rw-   0        0        0     4567 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/generated.py
--rw-rw-rw-   0        0        0     8097 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/layers.py
--rw-rw-rw-   0        0        0    12490 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/params.py
--rw-rw-rw-   0        0        0    18786 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/tacotron/tacotron2.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.754001 pororo_versionUp-0.4.1/pororo/models/tts/utils/
--rw-rw-rw-   0        0        0      614 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/utils/__init__.py
--rw-rw-rw-   0        0        0     3444 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/utils/audio.py
--rw-rw-rw-   0        0        0     1668 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/utils/display.py
--rw-rw-rw-   0        0        0     2988 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/utils/dsp.py
--rw-rw-rw-   0        0        0     4260 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/utils/numerical_pinyin_converter.py
--rw-rw-rw-   0        0        0     3003 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/utils/text.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.764757 pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/__init__.py
--rw-rw-rw-   0        0        0      686 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/gen_wavernn.py
--rw-rw-rw-   0        0        0     2550 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/params.py
--rw-rw-rw-   0        0        0    16817 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/waveRNN.py
--rw-rw-rw-   0        0        0     9211 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/vad.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.769063 pororo_versionUp-0.4.1/pororo/models/wav2vec2/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/wav2vec2/__init__.py
--rw-rw-rw-   0        0        0    10024 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/wav2vec2/recognizer.py
--rw-rw-rw-   0        0        0     7294 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/wav2vec2/submodules.py
--rw-rw-rw-   0        0        0     1067 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/wav2vec2/utils.py
--rw-rw-rw-   0        0        0     9092 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/models/wikipedia2vec.py
--rw-rw-rw-   0        0        0     7715 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/pororo.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.812748 pororo_versionUp-0.4.1/pororo/tasks/
--rw-rw-rw-   0        0        0     2795 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/__init__.py
--rw-rw-rw-   0        0        0    10175 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/age_suitability.py
--rw-rw-rw-   0        0        0     2139 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/automated_essay_scoring.py
--rw-rw-rw-   0        0        0     6960 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/automatic_speech_recognition.py
--rw-rw-rw-   0        0        0     4061 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/collocation.py
--rw-rw-rw-   0        0        0    17917 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/constituency_parsing.py
--rw-rw-rw-   0        0        0     4436 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/contextualized_embedding.py
--rw-rw-rw-   0        0        0     5021 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/dependency_parsing.py
--rw-rw-rw-   0        0        0     4660 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/fill_in_the_blank.py
--rw-rw-rw-   0        0        0    15752 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/grammatical_error_correction.py
--rw-rw-rw-   0        0        0     5554 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/grapheme_conversion.py
--rw-rw-rw-   0        0        0     6108 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/image_captioning.py
--rw-rw-rw-   0        0        0     2982 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/lemmatization.py
--rw-rw-rw-   0        0        0     4106 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/machine_reading_comprehension.py
--rw-rw-rw-   0        0        0    12237 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/machine_translation.py
--rw-rw-rw-   0        0        0     3902 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/morph_inflection.py
--rw-rw-rw-   0        0        0    20508 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/named_entity_recognition.py
--rw-rw-rw-   0        0        0     4555 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/natural_language_inference.py
--rw-rw-rw-   0        0        0     5400 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/optical_character_recognition.py
--rw-rw-rw-   0        0        0    11777 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/paraphrase_generation.py
--rw-rw-rw-   0        0        0     2756 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/paraphrase_identification.py
--rw-rw-rw-   0        0        0     8541 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/phoneme_conversion.py
--rw-rw-rw-   0        0        0    12285 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/pos_tagging.py
--rw-rw-rw-   0        0        0    24796 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/question_generation.py
--rw-rw-rw-   0        0        0     4523 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/review_scoring.py
--rw-rw-rw-   0        0        0     5615 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/semantic_role_labeling.py
--rw-rw-rw-   0        0        0     5746 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/semantic_textual_similarity.py
--rw-rw-rw-   0        0        0     6583 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/sentence_embedding.py
--rw-rw-rw-   0        0        0     4192 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/sentiment_analysis.py
--rw-rw-rw-   0        0        0     6884 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/speech_synthesis.py
--rw-rw-rw-   0        0        0     4269 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/speech_translation.py
--rw-rw-rw-   0        0        0    34847 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/text_summarization.py
--rw-rw-rw-   0        0        0    14269 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/tokenization.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.813870 pororo_versionUp-0.4.1/pororo/tasks/utils/
--rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/utils/__init__.py
--rw-rw-rw-   0        0        0     5011 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/utils/base.py
--rw-rw-rw-   0        0        0     3386 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/utils/config.py
--rw-rw-rw-   0        0        0     8101 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/utils/download_utils.py
--rw-rw-rw-   0        0        0     2804 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/utils/tokenizer.py
--rw-rw-rw-   0        0        0    27844 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/word_embedding.py
--rw-rw-rw-   0        0        0     8442 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/word_sense_disambiguation.py
--rw-rw-rw-   0        0        0     2318 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/word_translation.py
--rw-rw-rw-   0        0        0     6467 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/tasks/zero_shot_classification.py
--rw-rw-rw-   0        0        0     2222 2021-02-18 08:01:58.000000 pororo_versionUp-0.4.1/pororo/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-21 10:58:29.895573 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/
--rw-rw-rw-   0        0        0     8757 2023-07-21 10:58:29.000000 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4817 2023-07-21 10:58:29.000000 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 10:58:29.000000 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-21 10:58:29.000000 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      219 2023-07-21 10:58:29.000000 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-21 10:58:29.000000 pororo_versionUp-0.4.1/pororo_versionUp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      216 2023-07-21 10:58:29.912233 pororo_versionUp-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1629 2023-07-21 10:58:23.000000 pororo_versionUp-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.169554 pororo_versionUp-0.5.0/
+-rw-rw-rw-   0        0        0     3156 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/INSTALL.md
+-rw-rw-rw-   0        0        0    11368 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    26965 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/LICENSE.3rd_party_library
+-rw-rw-rw-   0        0        0      966 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/LICENSE.3rd_party_model
+-rw-rw-rw-   0        0        0      118 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     8757 2023-07-21 11:09:24.169554 pororo_versionUp-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7813 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.918343 pororo_versionUp-0.5.0/pororo/
+-rw-rw-rw-   0        0        0      103 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/__init__.py
+-rw-rw-rw-   0        0        0       18 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/__version__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.927390 pororo_versionUp-0.5.0/pororo/models/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.935499 pororo_versionUp-0.5.0/pororo/models/bart/
+-rw-rw-rw-   0        0        0     6299 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/bart/KoBART.py
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/bart/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.947001 pororo_versionUp-0.5.0/pororo/models/brainOCR/
+-rw-rw-rw-   0        0        0       37 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/__init__.py
+-rw-rw-rw-   0        0        0     1022 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/_dataset.py
+-rw-rw-rw-   0        0        0    20996 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/_modules.py
+-rw-rw-rw-   0        0        0     8365 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/brainocr.py
+-rw-rw-rw-   0        0        0     2938 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/craft.py
+-rw-rw-rw-   0        0        0    10051 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/craft_utils.py
+-rw-rw-rw-   0        0        0     2706 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/detection.py
+-rw-rw-rw-   0        0        0     2421 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/imgproc.py
+-rw-rw-rw-   0        0        0     3831 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/model.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.956026 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/__init__.py
+-rw-rw-rw-   0        0        0     2897 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/basenet.py
+-rw-rw-rw-   0        0        0    11445 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/feature_extraction.py
+-rw-rw-rw-   0        0        0     4524 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/prediction.py
+-rw-rw-rw-   0        0        0      859 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/sequence_modeling.py
+-rw-rw-rw-   0        0        0     8768 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/transformation.py
+-rw-rw-rw-   0        0        0     7845 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/recognition.py
+-rw-rw-rw-   0        0        0    25982 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainOCR/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.969226 pororo_versionUp-0.5.0/pororo/models/brainbert/
+-rw-rw-rw-   0        0        0    17950 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/BrainLaBERTa.py
+-rw-rw-rw-   0        0        0     9854 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/BrainRoBERTa.py
+-rw-rw-rw-   0        0        0     9064 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/CharBrainRoBERTa.py
+-rw-rw-rw-   0        0        0     5628 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/EnBERTa.py
+-rw-rw-rw-   0        0        0     6231 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/JaBERTa.py
+-rw-rw-rw-   0        0        0    16989 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/PoSLaBERTa.py
+-rw-rw-rw-   0        0        0     4052 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/PosRoBERTa.py
+-rw-rw-rw-   0        0        0     5577 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/ZhBERTa.py
+-rw-rw-rw-   0        0        0     1581 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.977753 pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/__init__.py
+-rw-rw-rw-   0        0        0     5828 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/dependency_parse.py
+-rw-rw-rw-   0        0        0     3733 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/sequence_tagging.py
+-rw-rw-rw-   0        0        0     3801 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/sequence_tagging_label.py
+-rw-rw-rw-   0        0        0     6545 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/span_prediction.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.986209 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/__init__.py
+-rw-rw-rw-   0        0        0     7900 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/brain_roberta_task.py
+-rw-rw-rw-   0        0        0    12935 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/dependency_parse.py
+-rw-rw-rw-   0        0        0     8093 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/sequence_tagging.py
+-rw-rw-rw-   0        0        0     8924 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/sequence_tagging_label.py
+-rw-rw-rw-   0        0        0     9431 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/span_prediction.py
+-rw-rw-rw-   0        0        0     1432 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainbert/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.986209 pororo_versionUp-0.5.0/pororo/models/brainsbert/
+-rw-rw-rw-   0        0        0     6052 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainsbert/BrainRoBERTa.py
+-rw-rw-rw-   0        0        0       71 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/brainsbert/__init__.py
+-rw-rw-rw-   0        0        0    13799 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/caption.py
+-rw-rw-rw-   0        0        0     3863 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/collocate.py
+-rw-rw-rw-   0        0        0     5379 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/p2g.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.995497 pororo_versionUp-0.5.0/pororo/models/tts/
+-rw-rw-rw-   0        0        0       80 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:23.995497 pororo_versionUp-0.5.0/pororo/models/tts/hifigan/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/hifigan/__init__.py
+-rw-rw-rw-   0        0        0      470 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/hifigan/checkpoint.py
+-rw-rw-rw-   0        0        0    12068 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/hifigan/model.py
+-rw-rw-rw-   0        0        0     1712 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/synthesis.py
+-rw-rw-rw-   0        0        0     5441 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/synthesizer.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.010630 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/__init__.py
+-rw-rw-rw-   0        0        0     4188 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/attention.py
+-rw-rw-rw-   0        0        0     3973 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/encoder.py
+-rw-rw-rw-   0        0        0     4567 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/generated.py
+-rw-rw-rw-   0        0        0     8097 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/layers.py
+-rw-rw-rw-   0        0        0    12490 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/params.py
+-rw-rw-rw-   0        0        0    18786 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/tacotron/tacotron2.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.019278 pororo_versionUp-0.5.0/pororo/models/tts/utils/
+-rw-rw-rw-   0        0        0      614 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/utils/__init__.py
+-rw-rw-rw-   0        0        0     3444 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/utils/audio.py
+-rw-rw-rw-   0        0        0     1668 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/utils/display.py
+-rw-rw-rw-   0        0        0     2988 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/utils/dsp.py
+-rw-rw-rw-   0        0        0     4260 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/utils/numerical_pinyin_converter.py
+-rw-rw-rw-   0        0        0     3003 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/utils/text.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.019278 pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/__init__.py
+-rw-rw-rw-   0        0        0      686 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/gen_wavernn.py
+-rw-rw-rw-   0        0        0     2550 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/params.py
+-rw-rw-rw-   0        0        0    16817 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/waveRNN.py
+-rw-rw-rw-   0        0        0     9211 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/vad.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.027817 pororo_versionUp-0.5.0/pororo/models/wav2vec2/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/wav2vec2/__init__.py
+-rw-rw-rw-   0        0        0    10024 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/wav2vec2/recognizer.py
+-rw-rw-rw-   0        0        0     7294 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/wav2vec2/submodules.py
+-rw-rw-rw-   0        0        0     1067 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/wav2vec2/utils.py
+-rw-rw-rw-   0        0        0     9092 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/models/wikipedia2vec.py
+-rw-rw-rw-   0        0        0     7715 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/pororo.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.077566 pororo_versionUp-0.5.0/pororo/tasks/
+-rw-rw-rw-   0        0        0     2795 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/__init__.py
+-rw-rw-rw-   0        0        0    10175 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/age_suitability.py
+-rw-rw-rw-   0        0        0     2139 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/automated_essay_scoring.py
+-rw-rw-rw-   0        0        0     6960 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/automatic_speech_recognition.py
+-rw-rw-rw-   0        0        0     4061 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/collocation.py
+-rw-rw-rw-   0        0        0    17917 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/constituency_parsing.py
+-rw-rw-rw-   0        0        0     4436 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/contextualized_embedding.py
+-rw-rw-rw-   0        0        0     5021 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/dependency_parsing.py
+-rw-rw-rw-   0        0        0     4660 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/fill_in_the_blank.py
+-rw-rw-rw-   0        0        0    15752 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/grammatical_error_correction.py
+-rw-rw-rw-   0        0        0     5554 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/grapheme_conversion.py
+-rw-rw-rw-   0        0        0     6108 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/image_captioning.py
+-rw-rw-rw-   0        0        0     2982 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/lemmatization.py
+-rw-rw-rw-   0        0        0     4106 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/machine_reading_comprehension.py
+-rw-rw-rw-   0        0        0    12237 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/machine_translation.py
+-rw-rw-rw-   0        0        0     3902 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/morph_inflection.py
+-rw-rw-rw-   0        0        0    20508 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/named_entity_recognition.py
+-rw-rw-rw-   0        0        0     4555 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/natural_language_inference.py
+-rw-rw-rw-   0        0        0     5400 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/optical_character_recognition.py
+-rw-rw-rw-   0        0        0    11777 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/paraphrase_generation.py
+-rw-rw-rw-   0        0        0     2756 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/paraphrase_identification.py
+-rw-rw-rw-   0        0        0     8541 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/phoneme_conversion.py
+-rw-rw-rw-   0        0        0    12285 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/pos_tagging.py
+-rw-rw-rw-   0        0        0    24796 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/question_generation.py
+-rw-rw-rw-   0        0        0     4523 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/review_scoring.py
+-rw-rw-rw-   0        0        0     5615 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/semantic_role_labeling.py
+-rw-rw-rw-   0        0        0     5746 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/semantic_textual_similarity.py
+-rw-rw-rw-   0        0        0     6583 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/sentence_embedding.py
+-rw-rw-rw-   0        0        0     4192 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/sentiment_analysis.py
+-rw-rw-rw-   0        0        0     6884 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/speech_synthesis.py
+-rw-rw-rw-   0        0        0     4269 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/speech_translation.py
+-rw-rw-rw-   0        0        0    34847 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/text_summarization.py
+-rw-rw-rw-   0        0        0    14269 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/tokenization.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.085694 pororo_versionUp-0.5.0/pororo/tasks/utils/
+-rw-rw-rw-   0        0        0        0 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/utils/__init__.py
+-rw-rw-rw-   0        0        0     5011 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/utils/base.py
+-rw-rw-rw-   0        0        0     3386 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/utils/config.py
+-rw-rw-rw-   0        0        0     8101 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/utils/download_utils.py
+-rw-rw-rw-   0        0        0     2804 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/utils/tokenizer.py
+-rw-rw-rw-   0        0        0    27844 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/word_embedding.py
+-rw-rw-rw-   0        0        0     8442 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/word_sense_disambiguation.py
+-rw-rw-rw-   0        0        0     2318 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/word_translation.py
+-rw-rw-rw-   0        0        0     6467 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/tasks/zero_shot_classification.py
+-rw-rw-rw-   0        0        0     2222 2021-02-18 08:01:58.000000 pororo_versionUp-0.5.0/pororo/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-21 11:09:24.169554 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/
+-rw-rw-rw-   0        0        0     8757 2023-07-21 11:09:23.000000 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4817 2023-07-21 11:09:23.000000 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-21 11:09:23.000000 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-21 10:58:29.000000 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      219 2023-07-21 11:09:23.000000 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-21 11:09:23.000000 pororo_versionUp-0.5.0/pororo_versionUp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      216 2023-07-21 11:09:24.186196 pororo_versionUp-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1618 2023-07-21 11:09:18.000000 pororo_versionUp-0.5.0/setup.py
```

### Comparing `pororo_versionUp-0.4.1/INSTALL.md` & `pororo_versionUp-0.5.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/LICENSE` & `pororo_versionUp-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/LICENSE.3rd_party_library` & `pororo_versionUp-0.5.0/LICENSE.3rd_party_library`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/LICENSE.3rd_party_model` & `pororo_versionUp-0.5.0/LICENSE.3rd_party_model`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/PKG-INFO` & `pororo_versionUp-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pororo_versionUp
-Version: 0.4.1
+Version: 0.5.0
 Summary: Pororo: A Deep Learning based Multilingual Natural Language Processing Library
 Home-page: https://github.com/kakaobrain/pororo
 Author: kakaobrain Team SIGNALS
 Author-email: contact@kakaobrain.com
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pororo_versionUp Version: 0.4.1 Summary: Pororo: A
+Metadata-Version: 2.1 Name: pororo_versionUp Version: 0.5.0 Summary: Pororo: A
 Deep Learning based Multilingual Natural Language Processing Library Home-page:
 https://github.com/kakaobrain/pororo Author: kakaobrain Team SIGNALS Author-
 email: contact@kakaobrain.com License: Apache-2.0 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
```

### Comparing `pororo_versionUp-0.4.1/README.md` & `pororo_versionUp-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/bart/KoBART.py` & `pororo_versionUp-0.5.0/pororo/models/bart/KoBART.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/_dataset.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/_dataset.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/_modules.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/_modules.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/brainocr.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/brainocr.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/craft.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/craft.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/craft_utils.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/craft_utils.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/detection.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/detection.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/imgproc.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/imgproc.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/model.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/model.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/basenet.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/basenet.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/feature_extraction.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/prediction.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/prediction.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/sequence_modeling.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/sequence_modeling.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/modules/transformation.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/modules/transformation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/recognition.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/recognition.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainOCR/utils.py` & `pororo_versionUp-0.5.0/pororo/models/brainOCR/utils.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/BrainLaBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/BrainLaBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/BrainRoBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/BrainRoBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/CharBrainRoBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/CharBrainRoBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/EnBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/EnBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/JaBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/JaBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/PoSLaBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/PoSLaBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/PosRoBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/PosRoBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/ZhBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/ZhBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/__init__.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/__init__.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/dependency_parse.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/dependency_parse.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/sequence_tagging.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/sequence_tagging.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/sequence_tagging_label.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/sequence_tagging_label.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/criterions/span_prediction.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/criterions/span_prediction.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/brain_roberta_task.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/brain_roberta_task.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/dependency_parse.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/dependency_parse.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/sequence_tagging.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/sequence_tagging.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/sequence_tagging_label.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/sequence_tagging_label.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/tasks/span_prediction.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/tasks/span_prediction.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainbert/utils.py` & `pororo_versionUp-0.5.0/pororo/models/brainbert/utils.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/brainsbert/BrainRoBERTa.py` & `pororo_versionUp-0.5.0/pororo/models/brainsbert/BrainRoBERTa.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/caption.py` & `pororo_versionUp-0.5.0/pororo/models/caption.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/collocate.py` & `pororo_versionUp-0.5.0/pororo/models/collocate.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/p2g.py` & `pororo_versionUp-0.5.0/pororo/models/p2g.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/hifigan/model.py` & `pororo_versionUp-0.5.0/pororo/models/tts/hifigan/model.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/synthesis.py` & `pororo_versionUp-0.5.0/pororo/models/tts/synthesis.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/synthesizer.py` & `pororo_versionUp-0.5.0/pororo/models/tts/synthesizer.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/tacotron/attention.py` & `pororo_versionUp-0.5.0/pororo/models/tts/tacotron/attention.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/tacotron/encoder.py` & `pororo_versionUp-0.5.0/pororo/models/tts/tacotron/encoder.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/tacotron/generated.py` & `pororo_versionUp-0.5.0/pororo/models/tts/tacotron/generated.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/tacotron/layers.py` & `pororo_versionUp-0.5.0/pororo/models/tts/tacotron/layers.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/tacotron/params.py` & `pororo_versionUp-0.5.0/pororo/models/tts/tacotron/params.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/tacotron/tacotron2.py` & `pororo_versionUp-0.5.0/pororo/models/tts/tacotron/tacotron2.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/utils/__init__.py` & `pororo_versionUp-0.5.0/pororo/models/tts/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/utils/audio.py` & `pororo_versionUp-0.5.0/pororo/models/tts/utils/audio.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/utils/display.py` & `pororo_versionUp-0.5.0/pororo/models/tts/utils/display.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/utils/dsp.py` & `pororo_versionUp-0.5.0/pororo/models/tts/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/utils/numerical_pinyin_converter.py` & `pororo_versionUp-0.5.0/pororo/models/tts/utils/numerical_pinyin_converter.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/utils/text.py` & `pororo_versionUp-0.5.0/pororo/models/tts/utils/text.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/gen_wavernn.py` & `pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/gen_wavernn.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/params.py` & `pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/params.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/tts/waveRNN/waveRNN.py` & `pororo_versionUp-0.5.0/pororo/models/tts/waveRNN/waveRNN.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/vad.py` & `pororo_versionUp-0.5.0/pororo/models/vad.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/wav2vec2/recognizer.py` & `pororo_versionUp-0.5.0/pororo/models/wav2vec2/recognizer.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/wav2vec2/submodules.py` & `pororo_versionUp-0.5.0/pororo/models/wav2vec2/submodules.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/wav2vec2/utils.py` & `pororo_versionUp-0.5.0/pororo/models/wav2vec2/utils.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/models/wikipedia2vec.py` & `pororo_versionUp-0.5.0/pororo/models/wikipedia2vec.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/pororo.py` & `pororo_versionUp-0.5.0/pororo/pororo.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/__init__.py` & `pororo_versionUp-0.5.0/pororo/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/age_suitability.py` & `pororo_versionUp-0.5.0/pororo/tasks/age_suitability.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/automated_essay_scoring.py` & `pororo_versionUp-0.5.0/pororo/tasks/automated_essay_scoring.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/automatic_speech_recognition.py` & `pororo_versionUp-0.5.0/pororo/tasks/automatic_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/collocation.py` & `pororo_versionUp-0.5.0/pororo/tasks/collocation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/constituency_parsing.py` & `pororo_versionUp-0.5.0/pororo/tasks/constituency_parsing.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/contextualized_embedding.py` & `pororo_versionUp-0.5.0/pororo/tasks/contextualized_embedding.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/dependency_parsing.py` & `pororo_versionUp-0.5.0/pororo/tasks/dependency_parsing.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/fill_in_the_blank.py` & `pororo_versionUp-0.5.0/pororo/tasks/fill_in_the_blank.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/grammatical_error_correction.py` & `pororo_versionUp-0.5.0/pororo/tasks/grammatical_error_correction.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/grapheme_conversion.py` & `pororo_versionUp-0.5.0/pororo/tasks/grapheme_conversion.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/image_captioning.py` & `pororo_versionUp-0.5.0/pororo/tasks/image_captioning.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/lemmatization.py` & `pororo_versionUp-0.5.0/pororo/tasks/lemmatization.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/machine_reading_comprehension.py` & `pororo_versionUp-0.5.0/pororo/tasks/machine_reading_comprehension.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/machine_translation.py` & `pororo_versionUp-0.5.0/pororo/tasks/machine_translation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/morph_inflection.py` & `pororo_versionUp-0.5.0/pororo/tasks/morph_inflection.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/named_entity_recognition.py` & `pororo_versionUp-0.5.0/pororo/tasks/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/natural_language_inference.py` & `pororo_versionUp-0.5.0/pororo/tasks/natural_language_inference.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/optical_character_recognition.py` & `pororo_versionUp-0.5.0/pororo/tasks/optical_character_recognition.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/paraphrase_generation.py` & `pororo_versionUp-0.5.0/pororo/tasks/paraphrase_generation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/paraphrase_identification.py` & `pororo_versionUp-0.5.0/pororo/tasks/paraphrase_identification.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/phoneme_conversion.py` & `pororo_versionUp-0.5.0/pororo/tasks/phoneme_conversion.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/pos_tagging.py` & `pororo_versionUp-0.5.0/pororo/tasks/pos_tagging.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/question_generation.py` & `pororo_versionUp-0.5.0/pororo/tasks/question_generation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/review_scoring.py` & `pororo_versionUp-0.5.0/pororo/tasks/review_scoring.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/semantic_role_labeling.py` & `pororo_versionUp-0.5.0/pororo/tasks/semantic_role_labeling.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/semantic_textual_similarity.py` & `pororo_versionUp-0.5.0/pororo/tasks/semantic_textual_similarity.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/sentence_embedding.py` & `pororo_versionUp-0.5.0/pororo/tasks/sentence_embedding.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/sentiment_analysis.py` & `pororo_versionUp-0.5.0/pororo/tasks/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/speech_synthesis.py` & `pororo_versionUp-0.5.0/pororo/tasks/speech_synthesis.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/speech_translation.py` & `pororo_versionUp-0.5.0/pororo/tasks/speech_translation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/text_summarization.py` & `pororo_versionUp-0.5.0/pororo/tasks/text_summarization.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/tokenization.py` & `pororo_versionUp-0.5.0/pororo/tasks/tokenization.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/utils/base.py` & `pororo_versionUp-0.5.0/pororo/tasks/utils/base.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/utils/config.py` & `pororo_versionUp-0.5.0/pororo/tasks/utils/config.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/utils/download_utils.py` & `pororo_versionUp-0.5.0/pororo/tasks/utils/download_utils.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/utils/tokenizer.py` & `pororo_versionUp-0.5.0/pororo/tasks/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/word_embedding.py` & `pororo_versionUp-0.5.0/pororo/tasks/word_embedding.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/word_sense_disambiguation.py` & `pororo_versionUp-0.5.0/pororo/tasks/word_sense_disambiguation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/word_translation.py` & `pororo_versionUp-0.5.0/pororo/tasks/word_translation.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/tasks/zero_shot_classification.py` & `pororo_versionUp-0.5.0/pororo/tasks/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo/utils.py` & `pororo_versionUp-0.5.0/pororo/utils.py`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/pororo_versionUp.egg-info/PKG-INFO` & `pororo_versionUp-0.5.0/pororo_versionUp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pororo-versionUp
-Version: 0.4.1
+Version: 0.5.0
 Summary: Pororo: A Deep Learning based Multilingual Natural Language Processing Library
 Home-page: https://github.com/kakaobrain/pororo
 Author: kakaobrain Team SIGNALS
 Author-email: contact@kakaobrain.com
 License: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pororo-versionUp Version: 0.4.1 Summary: Pororo: A
+Metadata-Version: 2.1 Name: pororo-versionUp Version: 0.5.0 Summary: Pororo: A
 Deep Learning based Multilingual Natural Language Processing Library Home-page:
 https://github.com/kakaobrain/pororo Author: kakaobrain Team SIGNALS Author-
 email: contact@kakaobrain.com License: Apache-2.0 Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 Development Status :: 3 - Alpha Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
```

### Comparing `pororo_versionUp-0.4.1/pororo_versionUp.egg-info/SOURCES.txt` & `pororo_versionUp-0.5.0/pororo_versionUp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pororo_versionUp-0.4.1/setup.py` & `pororo_versionUp-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # yapf: disable
 
 from setuptools import setup, find_packages
 
 packages = find_packages()
 requirements = [
-    "torch==1.7.1",
+    "torch==1.8.0",
     "torchvision==0.9.0",
     "pillow>=4.1.1",
     "fairseq>=0.10.2",
     "transformers>=4.0.0",
     "sentence_transformers>=0.4.1.2",
     "nltk>=3.5",
     "word2word",
@@ -24,15 +24,15 @@
 
 VERSION = {}  # type: ignore
 with open("pororo/__version__.py", "r") as version_file:
     exec(version_file.read(), VERSION)
 
 setup(
     name="pororo_versionUp",
-    version=VERSION["version"],
+    version='0.5.0',
     description="Pororo: A Deep Learning based Multilingual Natural Language Processing Library",
     long_description=open("README.md", encoding='UTF8').read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Development Status :: 3 - Alpha",
```

