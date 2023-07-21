# Comparing `tmp/spacy-curated-transformers-0.1.1.tar.gz` & `tmp/spacy-curated-transformers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-curated-transformers-0.1.1.tar", last modified: Wed May 24 06:33:00 2023, max compression
+gzip compressed data, was "spacy-curated-transformers-0.2.0.tar", last modified: Fri Jul 21 11:39:07 2023, max compression
```

## Comparing `spacy-curated-transformers-0.1.1.tar` & `spacy-curated-transformers-0.2.0.tar`

### file list

```diff
@@ -1,82 +1,81 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      960 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     4241 2023-05-24 06:33:00.629343 spacy-curated-transformers-0.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.617343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4050 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/debug_pieces.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4697 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/quantize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3433 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/errors.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24806 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1225 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19182 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2704 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/output.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/remove_eos_bos.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4669 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       37 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17299 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/pipeline/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_hf_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2644 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_listeners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4556 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_pooling.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_scalar_weight.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6191 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4325 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_strided_spans.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.621343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18102 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/test_transformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
--rw-r--r--   0 vsts      (1001) docker     (122)      418 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2513 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_torchscript_wrapper.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4090 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2716 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7943 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4907 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-chars.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.model
--rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (122)      482 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.625343 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/
--rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3623 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/bbpe_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/char_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/hf_loader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3834 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/types.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5901 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/wordpiece_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2711 2023-05-24 06:32:46.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-24 06:33:00.617343 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1285 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3494 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     3466 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-24 06:33:00.000000 spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.605195 spacy-curated-transformers-0.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1088 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     2562 2023-07-21 11:39:07.605195 spacy-curated-transformers-0.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2217 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     4174 2023-07-21 11:39:07.605195 spacy-curated-transformers-0.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      210 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.593195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       41 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      570 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.593195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4113 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/cli/debug_pieces.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3188 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/errors.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.597195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      438 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    27177 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1225 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24358 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2704 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/output.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2192 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/remove_eos_bos.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4669 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2666 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7876 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10279 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.597195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       44 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17713 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/pipeline/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.597195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2340 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.601195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_hf_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2653 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_listeners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4556 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_pooling.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1425 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_scalar_weight.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6191 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3194 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4325 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_with_strided_spans.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.601195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22713 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/pipeline/test_transformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2703 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy
+-rw-r--r--   0 vsts      (1001) docker     (122)      241 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2513 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      794 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/test_torchscript_wrapper.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.601195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3393 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4090 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2716 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7943 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4907 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      138 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy-chars.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     4690 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)    14493 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (122)   253270 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (122)     4968 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (122)      907 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.605195 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/
+-rw-r--r--   0 vsts      (1001) docker     (122)      568 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3623 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/bbpe_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3713 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/char_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5394 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/hf_loader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2500 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3834 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      557 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/types.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5901 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/wordpiece_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2743 2023-07-21 11:38:56.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-21 11:39:07.593195 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2562 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3451 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     3375 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      107 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-21 11:39:07.000000 spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/zip-safe
```

### Comparing `spacy-curated-transformers-0.1.1/LICENSE` & `spacy-curated-transformers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/setup.cfg` & `spacy-curated-transformers-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-version = 0.1.1
-description = Curated transformer models
+version = 0.2.0
+description = Curated transformer models for spaCy pipelines
 url = https://github.com/explosion/spacy-curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -12,15 +12,15 @@
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	curated-transformers>=0.1.0,<0.2.0
 	curated-tokenizers>=0.0.7,<0.1.0
-	spacy>=3.5.0,<4.0.0
+	spacy>=3.7.0.dev0,<4.0.0
 	torch>=1.12.0
 
 [options.entry_points]
 spacy_factories = 
 	curated_transformer = spacy_curated_transformers.pipeline.transformer:make_transformer
 spacy_architectures = 
 	spacy-curated-transformers.AlbertTransformer.v1 = spacy_curated_transformers.models:build_albert_transformer_model_v1
@@ -40,15 +40,14 @@
 	spacy-curated-transformers.SentencepieceEncoder.v1 = spacy_curated_transformers.tokenization:build_sentencepiece_encoder_v1
 	spacy-curated-transformers.WordpieceEncoder.v1 = spacy_curated_transformers.tokenization:build_wordpiece_encoder_v1
 	spacy-curated-transformers.XlmrSentencepieceEncoder.v1 = spacy_curated_transformers.tokenization:build_xlmr_sentencepiece_encoder_v1
 spacy_callbacks = 
 	spacy-curated-transformers.gradual_transformer_unfreezing.v1 = spacy_curated_transformers.util:create_gradual_transformer_unfreezing
 spacy_cli = 
 	spacy-curated-transformers.debug_pieces = spacy_curated_transformers.cli.debug_pieces:debug_pieces_cli
-	spacy-curated-transformers.quantize = spacy_curated_transformers.cli.quantize:quantize_cli
 thinc_model_loaders = 
 	spacy-curated-transformers.ByteBpeLoader.v1 = spacy_curated_transformers.tokenization:build_byte_bpe_encoder_loader_v1
 	spacy-curated-transformers.CharEncoderLoader.v1 = spacy_curated_transformers.tokenization:build_char_encoder_loader_v1
 	spacy-curated-transformers.HFTransformerEncoderLoader.v1 = spacy_curated_transformers.models:build_hf_transformer_encoder_loader_v1
 	spacy-curated-transformers.HFPieceEncoderLoader.v1 = spacy_curated_transformers.tokenization:build_hf_piece_encoder_loader_v1
 	spacy-curated-transformers.PyTorchCheckpointLoader.v1 = spacy_curated_transformers.models:build_pytorch_checkpoint_loader_v1
 	spacy-curated-transformers.SentencepieceLoader.v1 = spacy_curated_transformers.tokenization:build_sentencepiece_encoder_loader_v1
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/_compat.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/cli/debug_pieces.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/cli/debug_pieces.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from pathlib import Path
 from typing import Any, Dict, List, Optional, cast
+
 import numpy
-from pathlib import Path
 from spacy import util
 from spacy.cli._util import (
     debug_cli,
     import_code,
     parse_config_overrides,
     show_validation_error,
 )
 from spacy.schemas import ConfigSchemaTraining
 from spacy.tokens import Doc
 from spacy.util import registry, resolve_dot_names
-from typer import Argument as Arg, Context, Option as Opt
+from typer import Argument as Arg
+from typer import Context
+from typer import Option as Opt
 from wasabi import Printer, msg
 
+from ..pipeline.transformer import CuratedTransformer
 from ..tokenization.types import Tok2PiecesModelT
-from ..pipeline.transformer import Transformer
 
 
 @debug_cli.command(
     "pieces",
     context_settings={"allow_extra_args": True, "ignore_unknown_options": True},
 )
 def debug_pieces_cli(
@@ -60,15 +63,15 @@
     dot_names = [T["train_corpus"], T["dev_corpus"]]
     train_corpus, dev_corpus = resolve_dot_names(config, dot_names)
 
     nlp.initialize(lambda: train_corpus(nlp))
 
     if transformer_name is None:
         transformers = [
-            pipe for _, pipe in nlp.pipeline if isinstance(pipe, Transformer)
+            pipe for _, pipe in nlp.pipeline if isinstance(pipe, CuratedTransformer)
         ]
         if not transformers:
             msg.fail("Pipeline does not contain transformer", exits=1)
         transformer_pipe = transformers[0]
     else:
         # We have to dance a bit around that MyPy cannot infer that we are
         # exiting if the invariants don't hold and that get_pipe returns
@@ -76,17 +79,17 @@
         try:
             transformer_pipe_callable = nlp.get_pipe(transformer_name)
         except KeyError:
             transformer_pipe_callable = None
             msg.fail(
                 f"Pipeline does not contain a pipe named '{transformer_name}'", exits=1
             )
-        if not isinstance(transformer_pipe_callable, Transformer):
+        if not isinstance(transformer_pipe_callable, CuratedTransformer):
             msg.fail(f"Pipe named '{transformer_name}' is not a transformer", exits=1)
-        transformer_pipe = cast(Transformer, transformer_pipe_callable)
+        transformer_pipe = cast(CuratedTransformer, transformer_pipe_callable)
 
     piece_encoder = transformer_pipe.model.get_ref("piece_encoder")
     msg.info(f"Found piece encoder: {piece_encoder.name}")
 
     train_docs = [eg.predicted for eg in train_corpus(nlp)]
     dev_docs = [eg.predicted for eg in dev_corpus(nlp)]
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/errors.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,24 +7,15 @@
             return "(spacy-curated-transformers) [{code}] {msg}".format(
                 code=code, msg=msg
             )
 
 
 # fmt: off
 
-class Warnings(metaclass=ErrorsWithCodes):
-    W001 = ("Skipping transfomer pipe with TorchScript model - Model "
-            "is likely already quantized")
-
-
 class Errors(metaclass=ErrorsWithCodes):
-    E001 = ("Attempting to quantize a transformer pipe with a "
-            "non-PyTorch model ('{model_name}'). Quantization "
-            "is only supported by PyTorch-specific curated "
-            "transformer models")
     E009 = ("At least one sequence in the transformer's input has a length "
             "of {seq_len}, which is larger than the model's maximum sequence "
             "length of {max_seq_len} tokens")
     E010 = ("Curated transformers do not currently support listener replacement")
     E011 = ("`{loader_name}` requires the Hugging Face `transformers` package to be installed")
     E012 = ("`{listener_name}` requires the upstream transformer pipe to output "
             "all hidden layer outputs. This can be enabled by setting the pipe's "
@@ -52,9 +43,11 @@
             "{supported_tokenizers}")
     E023 = ("Japanese BERT models currently only support character subword encoding")
     E024 = ("Attempting to initialize an incompatible piece encoder ('{model_name}') "
             "with the Hugging Face Japanese BERT tokenizer. It can only be used with the "
             "`CharEncoder` piece encoder")
     E025 = ("Attempting to perform gradual unfreezing of a non-transformer pipe "
             "('{pipe_name}'}. Only transformer pipes support this feature")
+    E026 = ("Attempting to register a model ('{model_name}') with the transformer pipe"
+            "that isn't a transformer listener")
 
 # fmt: on
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/architectures.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/architectures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-from typing import List, Optional, Tuple, Callable, Any, cast
+from functools import partial
+from pathlib import Path
+from typing import Any, Callable, List, Optional, Tuple, Union, cast
+
+import torch
 from curated_transformers.models.albert import AlbertConfig, AlbertEncoder
 from curated_transformers.models.bert import BertConfig, BertEncoder
 from curated_transformers.models.curated_transformer import (
-    CuratedTransformer,
     CuratedEncoderT,
+    CuratedTransformer,
 )
 from curated_transformers.models.hf_util import convert_pretrained_model_for_encoder
 from curated_transformers.models.output import PyTorchTransformerOutput
 from curated_transformers.models.roberta import RobertaConfig, RobertaEncoder
-from pathlib import Path
-from functools import partial
 from spacy.tokens import Doc
 from spacy.util import SimpleFrozenDict
+
 from thinc.api import (
     Model,
     PyTorchWrapper_v2,
-    xp2torch,
-    torch2xp,
-    get_torch_default_device,
     TorchScriptWrapper_v1,
+    get_torch_default_device,
+    torch2xp,
+    xp2torch,
 )
 from thinc.layers import chain
 from thinc.model import Model
 from thinc.shims.pytorch_grad_scaler import PyTorchGradScaler
 from thinc.types import ArgsKwargs, Floats2d, Ints1d
-import torch
-
 
+from ..errors import Errors
+from ..tokenization.types import Tok2PiecesModelT
+from .listeners import (
+    WrappedTransformerAndListener,
+    replace_listener_callback,
+    replace_listener_cfg_callback,
+)
 from .output import TransformerModelOutput
 from .remove_eos_bos import remove_bos_eos
-from .with_non_ws_tokens import with_non_ws_tokens
-from ..tokenization.types import Tok2PiecesModelT
 from .types import (
+    SpanExtractorModelT,
     TorchTransformerInT,
     TorchTransformerModelT,
     TorchTransformerOutT,
     TransformerBackpropT,
     TransformerInT,
-    TransformerOutT,
+    TransformerListenerModelT,
     TransformerModelT,
-    SpanExtractorModelT,
+    TransformerOutT,
+    WrappedTransformerAndListenerModelT,
 )
-from ..errors import Errors
+from .with_non_ws_tokens import with_non_ws_tokens
 
 
 def build_albert_transformer_model_v1(
     *,
     vocab_size: int,
     with_spans: Callable[
         [TorchTransformerModelT],
@@ -65,15 +73,16 @@
     num_hidden_groups: int = 1,
     num_hidden_layers: int = 12,
     padding_idx: int = 0,
     type_vocab_size: int = 2,
     torchscript: bool = False,
     mixed_precision: bool = False,
     grad_scaler_config: dict = SimpleFrozenDict(),
-) -> TransformerModelT:
+    wrapped_listener: Optional[TransformerListenerModelT] = None,
+) -> Union[TransformerModelT, WrappedTransformerAndListenerModelT]:
     """Construct an ALBERT transformer model.
 
     vocab_size (int):
         Vocabulary size.
     with_spans (Callable):
         Callback that constructs a span generator model.
     piece_encoder (Model)
@@ -110,14 +119,17 @@
         Type vocabulary size.
     torchscript (bool):
         Set to `True` when loading TorchScript models, `False` otherwise.
     mixed_precision (bool):
         Use mixed-precision training.
     grad_scaler_config (dict):
         Configuration passed to the PyTorch gradient scaler.
+    wrapped_listener (Optional[TransformerListenerModelT]):
+        Optional listener to wrap. Only used when replacing listeners
+        in downstream components.
     """
     config = AlbertConfig(
         embedding_width=embedding_width,
         hidden_width=hidden_width,
         intermediate_width=intermediate_width,
         num_attention_heads=num_attention_heads,
         num_hidden_groups=num_hidden_groups,
@@ -142,18 +154,19 @@
         transformer = _pytorch_encoder(
             encoder,
             hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
-    return build_transformer_model_v1(
+    return build_transformer_or_listener_wrapper_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
         transformer=transformer,
+        wrapped_listener=wrapped_listener,
     )
 
 
 def build_bert_transformer_model_v1(
     *,
     vocab_size: int,
     with_spans: Callable[
@@ -172,15 +185,16 @@
     num_attention_heads: int = 12,
     num_hidden_layers: int = 12,
     padding_idx: int = 0,
     type_vocab_size: int = 2,
     torchscript: bool = False,
     mixed_precision: bool = False,
     grad_scaler_config: dict = SimpleFrozenDict(),
-) -> TransformerModelT:
+    wrapped_listener: Optional[TransformerListenerModelT] = None,
+) -> Union[TransformerModelT, WrappedTransformerAndListenerModelT]:
     """Construct a BERT transformer model.
 
     vocab_size (int):
         Vocabulary size.
     with_spans (Callable):
         Callback that constructs a span generator model.
     piece_encoder (Model)
@@ -213,14 +227,17 @@
         Type vocabulary size.
     torchscript (bool):
         Set to `True` when loading TorchScript models, `False` otherwise.
     mixed_precision (bool):
         Use mixed-precision training.
     grad_scaler_config (dict):
         Configuration passed to the PyTorch gradient scaler.
+    wrapped_listener (Optional[TransformerListenerModelT]):
+        Optional listener to wrap. Only used when replacing listeners
+        in downstream components.
     """
     config = BertConfig(
         hidden_width=hidden_width,
         intermediate_width=intermediate_width,
         num_attention_heads=num_attention_heads,
         num_hidden_layers=num_hidden_layers,
         attention_probs_dropout_prob=attention_probs_dropout_prob,
@@ -243,18 +260,19 @@
         transformer = _pytorch_encoder(
             encoder,
             hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
-    return build_transformer_model_v1(
+    return build_transformer_or_listener_wrapper_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
         transformer=transformer,
+        wrapped_listener=wrapped_listener,
     )
 
 
 def build_camembert_transformer_model_v1(
     *,
     vocab_size: int,
     with_spans: Callable[
@@ -273,15 +291,16 @@
     num_attention_heads: int = 12,
     num_hidden_layers: int = 12,
     padding_idx: int = 1,
     type_vocab_size: int = 1,
     mixed_precision: bool = False,
     torchscript=False,
     grad_scaler_config: dict = SimpleFrozenDict(),
-) -> TransformerModelT:
+    wrapped_listener: Optional[TransformerListenerModelT] = None,
+) -> Union[TransformerModelT, WrappedTransformerAndListenerModelT]:
     """Construct a CamemBERT transformer model.
 
     vocab_size (int):
         Vocabulary size.
     with_spans (Callable):
         Callback that constructs a span generator model.
     piece_encoder (Model)
@@ -314,14 +333,17 @@
         Type vocabulary size.
     torchscript (bool):
         Set to `True` when loading TorchScript models, `False` otherwise.
     mixed_precision (bool):
         Use mixed-precision training.
     grad_scaler_config (dict):
         Configuration passed to the PyTorch gradient scaler.
+    wrapped_listener (Optional[TransformerListenerModelT]):
+        Optional listener to wrap. Only used when replacing listeners
+        in downstream components.
     """
     config = RobertaConfig(
         hidden_width=hidden_width,
         intermediate_width=intermediate_width,
         num_attention_heads=num_attention_heads,
         num_hidden_layers=num_hidden_layers,
         attention_probs_dropout_prob=attention_probs_dropout_prob,
@@ -344,18 +366,19 @@
         transformer = _pytorch_encoder(
             encoder,
             hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
-    return build_transformer_model_v1(
+    return build_transformer_or_listener_wrapper_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
         transformer=transformer,
+        wrapped_listener=wrapped_listener,
     )
 
 
 def build_roberta_transformer_model_v1(
     *,
     vocab_size: int,
     with_spans: Callable[
@@ -374,15 +397,16 @@
     num_attention_heads: int = 12,
     num_hidden_layers: int = 12,
     padding_idx: int = 1,
     type_vocab_size: int = 1,
     torchscript: bool = False,
     mixed_precision: bool = False,
     grad_scaler_config: dict = SimpleFrozenDict(),
-) -> TransformerModelT:
+    wrapped_listener: Optional[TransformerListenerModelT] = None,
+) -> Union[TransformerModelT, WrappedTransformerAndListenerModelT]:
     """Construct a RoBERTa transformer model.
 
     vocab_size (int):
         Vocabulary size.
     with_spans (Callable):
         Callback that constructs a span generator model.
     piece_encoder (Model)
@@ -415,14 +439,17 @@
         Type vocabulary size.
     torchscript (bool):
         Set to `True` when loading TorchScript models, `False` otherwise.
     mixed_precision (bool):
         Use mixed-precision training.
     grad_scaler_config (dict):
         Configuration passed to the PyTorch gradient scaler.
+    wrapped_listener (Optional[TransformerListenerModelT]):
+        Optional listener to wrap. Only used when replacing listeners
+        in downstream components.
     """
     config = RobertaConfig(
         hidden_width=hidden_width,
         intermediate_width=intermediate_width,
         num_attention_heads=num_attention_heads,
         num_hidden_layers=num_hidden_layers,
         attention_probs_dropout_prob=attention_probs_dropout_prob,
@@ -445,18 +472,19 @@
         transformer = _pytorch_encoder(
             encoder,
             hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
-    return build_transformer_model_v1(
+    return build_transformer_or_listener_wrapper_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
         transformer=transformer,
+        wrapped_listener=wrapped_listener,
     )
 
 
 def build_xlmr_transformer_model_v1(
     *,
     vocab_size: int,
     with_spans: Callable[
@@ -475,15 +503,16 @@
     num_attention_heads: int = 12,
     num_hidden_layers: int = 12,
     padding_idx: int = 1,
     type_vocab_size: int = 1,
     torchscript: bool = False,
     mixed_precision: bool = False,
     grad_scaler_config: dict = SimpleFrozenDict(),
-) -> TransformerModelT:
+    wrapped_listener: Optional[TransformerListenerModelT] = None,
+) -> Union[TransformerModelT, WrappedTransformerAndListenerModelT]:
     """Construct a XLM-RoBERTa transformer model.
 
     vocab_size (int):
         Vocabulary size.
     with_spans (Callable):
         Callback that constructs a span generator model.
     piece_encoder (Model)
@@ -516,14 +545,17 @@
         Type vocabulary size.
     torchscript (bool):
         Set to `True` when loading TorchScript models, `False` otherwise.
     mixed_precision (bool):
         Use mixed-precision training.
     grad_scaler_config (dict):
         Configuration passed to the PyTorch gradient scaler.
+    wrapped_listener (Optional[TransformerListenerModelT]):
+        Optional listener to wrap. Only used when replacing listeners
+        in downstream components.
     """
     config = RobertaConfig(
         hidden_width=hidden_width,
         intermediate_width=intermediate_width,
         num_attention_heads=num_attention_heads,
         num_hidden_layers=num_hidden_layers,
         attention_probs_dropout_prob=attention_probs_dropout_prob,
@@ -546,19 +578,39 @@
         transformer = _pytorch_encoder(
             encoder,
             hidden_width=hidden_width,
             mixed_precision=mixed_precision,
             grad_scaler_config=grad_scaler_config,
         )
 
-    return build_transformer_model_v1(
+    return build_transformer_or_listener_wrapper_v1(
         with_spans=with_spans,
         piece_encoder=piece_encoder,
         transformer=transformer,
+        wrapped_listener=wrapped_listener,
+    )
+
+
+def build_transformer_or_listener_wrapper_v1(
+    *,
+    with_spans: Callable[
+        [TorchTransformerModelT],
+        SpanExtractorModelT,
+    ],
+    transformer: TorchTransformerModelT,
+    piece_encoder: Tok2PiecesModelT,
+    wrapped_listener: Optional[TransformerListenerModelT],
+) -> Union[TransformerModelT, WrappedTransformerAndListenerModelT]:
+    thinc_transformer = build_transformer_model_v1(
+        with_spans=with_spans, transformer=transformer, piece_encoder=piece_encoder
     )
+    if wrapped_listener is not None:
+        return WrappedTransformerAndListener(thinc_transformer, wrapped_listener)
+    else:
+        return thinc_transformer
 
 
 def build_transformer_model_v1(
     *,
     with_spans: Callable[
         [TorchTransformerModelT],
         SpanExtractorModelT,
@@ -580,16 +632,16 @@
     return Model(
         "transformer_model",
         transformer_model_forward,
         init=transformer_model_init,
         layers=layers,
         refs=refs,  # type: ignore
         attrs={
-            "replace_listener": _replace_listener,
-            "replace_listener_cfg": _replace_listener_cfg,
+            "replace_listener": replace_listener_callback,
+            "replace_listener_cfg": replace_listener_cfg_callback,
         },
         dims={"nO": transformer.get_dim("nO")},
     )
 
 
 def transformer_model_forward(
     model: TransformerModelT, docs: TransformerInT, is_train: bool
@@ -725,22 +777,14 @@
             args=(Yt_flat,),
             kwargs={"grad_tensors": dYt_flat},
         )
 
     return output, convert_for_torch_backward
 
 
-def _replace_listener(trf_model):
-    raise ValueError(Errors.E010)
-
-
-def _replace_listener_cfg(trf_model_cfg, listener_model_cfg):
-    raise ValueError(Errors.E010)
-
-
 def build_pytorch_checkpoint_loader_v1(
     *, path: Path
 ) -> Callable[
     [TorchTransformerModelT, Optional[List[Doc]], Optional[List[Doc]]],
     TorchTransformerModelT,
 ]:
     """Construct a callback that initializes a supported transformer
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/hf_loader.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/listeners.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/pipeline/transformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,509 +1,459 @@
+from itertools import islice
 from typing import (
     Any,
     Callable,
+    Dict,
     Iterable,
+    Iterator,
     List,
     Optional,
+    Sequence,
     Tuple,
 )
 
 from spacy import Errors as SpacyErrors
+from spacy import Language, Vocab
+from spacy.pipeline import TrainablePipe
 from spacy.tokens import Doc
+from spacy.training import Example, validate_examples, validate_get_examples
+from spacy.util import minibatch
+
+from thinc.api import Config, Optimizer, set_dropout_rate
 from thinc.model import Model
-from thinc.types import Ragged, Floats2d
+from thinc.types import Ragged
 
-from .output import TransformerModelOutput
-from .pooling import with_ragged_layers, with_ragged_last_layer
-from .types import (
-    WithRaggedLayersModelT,
-    WithRaggedLastLayerModelT,
-    PoolingModelT,
-    ScalarWeightOutT,
-    ScalarWeightModelT,
-)
-from .output import TransformerModelOutput
-from .pooling import with_ragged_layers, with_ragged_last_layer
-from .types import (
-    WithRaggedLayersModelT,
-    WithRaggedLastLayerModelT,
-    PoolingModelT,
-)
 from ..errors import Errors
+from ..models.listeners import ListenerStateUtils
+from ..models.output import DocTransformerOutput, TransformerModelOutput
+from ..models.types import TransformerListenerModelT
 
+DEFAULT_CONFIG_STR = """
+    [transformer]
 
-def build_transformer_layers_listener_v1(
-    layers: int,
-    width: int,
-    pooling: PoolingModelT,
-    upstream: str = "*",
-    grad_factor: float = 1.0,
-) -> Model[List[Doc], List[Floats2d]]:
-    """Construct a listener layer that communicates with one or more upstream Transformer
-    components. This layer extracts the output of all transformer layers and performs
-    pooling over the individual pieces of each Doc token, returning their corresponding
-    representations.
-
-    layers (int):
-        The the number of layers produced by the upstream transformer component,
-        excluding the embedding layer.
-    width (int):
-        The width of the vectors produced by the upstream transformer component.
-    pooling (PoolingModelT):
-        Model that is used to perform pooling over the piece representations.
-    upstream_name (str):
-        A string to identify the 'upstream' Transformer component
-        to communicate with. The upstream name should either be the wildcard
-        string '*', or the name of the Transformer component.
-
-        In almost all cases, the wildcard string will suffice as there'll only be one
-        upstream Transformer component. But in certain situations, e.g: you have disjoint
-        datasets for certain tasks, or you'd like to use a pre-trained pipeline but a
-        downstream task requires its own token representations, you could end up with
-        more than one Transformer component in the pipeline.
-    grad_factor (float):
-        Factor to multiply gradients with.
-    """
-    transformer = TransformerLayersListener(
-        upstream_name=upstream,
-        pooling=pooling,
-        layers=layers,
-        width=width,
-        grad_factor=grad_factor,
-    )
-    return transformer
+    [transformer.model]
+    @architectures = "spacy-curated-transformers.XlmrTransformer.v1"
 
+    [transformer.model.piece_encoder]
+    @architectures = "spacy-curated-transformers.XlmrSentencepieceEncoder.v1"
+
+    [transformer.model.with_spans]
+    @architectures = "spacy-curated-transformers.WithStridedSpans.v1"
+"""
 
-def build_last_transformer_layer_listener_v1(
-    width: int,
-    pooling: PoolingModelT,
-    upstream: str = "*",
-    grad_factor: float = 1.0,
-) -> Model[List[Doc], List[Floats2d]]:
-    """Construct a listener layer that communicates with one or more upstream Transformer
-    components. This layer extracts the output of the last transformer layer and performs
-    pooling over the individual pieces of each Doc token, returning their corresponding
-    representations.
-
-    width (int):
-        The width of the vectors produced by the upstream transformer component.
-    pooling (Model):
-        Model that is used to perform pooling over the piece representations.
-    upstream_name (str):
-        A string to identify the 'upstream' Transformer component
-        to communicate with. The upstream name should either be the wildcard
-        string '*', or the name of the Transformer component.
-
-        In almost all cases, the wildcard string will suffice as there'll only be one
-        upstream Transformer component. But in certain situations, e.g: you have disjoint
-        datasets for certain tasks, or you'd like to use a pre-trained pipeline but a
-        downstream task requires its own token representations, you could end up with
-        more than one Transformer component in the pipeline.
-    grad_factor (float):
-        Factor to multiply gradients with.
-    """
-    transformer = LastTransformerLayerListener(
-        upstream_name=upstream, pooling=pooling, width=width, grad_factor=grad_factor
-    )
-    return transformer
 
+DEFAULT_CONFIG = Config().from_str(DEFAULT_CONFIG_STR)
+DOC_EXT_ATTR = "trf_data"
 
-def build_scalar_weighting_listener_v1(
-    width: int,
-    weighting: ScalarWeightModelT,
-    pooling: PoolingModelT,
-    upstream: str = "*",
-    grad_factor: float = 1.0,
-) -> Model[List[Doc], List[Floats2d]]:
-    """Construct a listener layer that communicates with one or more upstream Transformer
-    components. This layer calculates a weighted representation of all transformer layer
-    outputs and performs pooling over the individual pieces of each Doc token, returning
-    their corresponding representations.
-
-    Requires its upstream Transformer components to return all layer outputs from
-    their models.
-
-    width (int):
-        The width of the vectors produced by the upstream transformer component.
-    weighting (Model):
-        Model that is used to perform the weighting of the different layer outputs.
-    pooling (Model):
-        Model that is used to perform pooling over the piece representations.
-    upstream_name (str):
-        A string to identify the 'upstream' Transformer component
-        to communicate with. The upstream name should either be the wildcard
-        string '*', or the name of the Transformer component.
-
-        In almost all cases, the wildcard string will suffice as there'll only be one
-        upstream Transformer component. But in certain situations, e.g: you have disjoint
-        datasets for certain tasks, or you'd like to use a pre-trained pipeline but a
-        downstream task requires its own token representations, you could end up with
-        more than one Transformer component in the pipeline.
-    grad_factor (float):
-        Factor to multiply gradients with.
+
+@Language.factory(
+    "curated_transformer",
+    assigns=["doc._.trf_data"],
+    default_config=DEFAULT_CONFIG["transformer"],
+)
+def make_transformer(
+    nlp: Language,
+    name: str,
+    model: Model,
+    *,
+    frozen: bool = False,
+    all_layer_outputs: bool = False,
+) -> "CuratedTransformer":
+    """Construct a CuratedTransformer component, which lets you plug a pre-trained
+    transformer model into spaCy so you can use it in your pipeline. One or
+    more subsequent spaCy components can use the transformer outputs as features
+    in its model, with gradients backpropagated to the single shared weights.
+
+    nlp (Language):
+        The pipeline.
+    name (str):
+        The component instance name.
+    model (Model):
+        One of the supported pre-trained transformer models.
+    frozen (bool):
+        If `True`, the model's weights are frozen and no backpropagation is performed.
+    all_layer_outputs (bool):
+        If `True`, the model returns the outputs of all the layers. Otherwise, only the
+        output of the last layer is returned. This must be set to `True` if any of the pipe's
+        downstream listeners require the outputs of all transformer layers.
     """
-    transformer = ScalarWeightingListener(
-        upstream_name=upstream,
-        weighting=weighting,
-        pooling=pooling,
-        width=width,
-        grad_factor=grad_factor,
+    return CuratedTransformer(
+        nlp.vocab,
+        model,
+        name=name,
+        frozen=frozen,
+        all_layer_outputs=all_layer_outputs,
     )
-    return transformer
 
 
-class TransformerListener(Model):
-    """A layer that gets fed its answers from an upstream Transformer component.
+class CuratedTransformer(TrainablePipe):
+    """spaCy pipeline component that provides access to a pre-trained transformer
+    model from. Downstream components are connected to this pip using transformer
+    listener layers. This works similarly to spaCy's Transformer component and
+    TransformerListener sublayer.
 
-    The TransformerListener layer is used as a sublayer within a component such
-    as a parser, NER or text categorizer. Usually you'll have multiple listeners
-    connecting to a single upstream Transformer component that's earlier in the
-    pipeline. These layers act as proxies, passing the predictions
-    from the Transformer component into downstream components and communicating
-    gradients back upstream.
+    The activations from the transformer are saved in the doc._.trf_data extension
+    attribute.
     """
 
-    upstream_name: str
-    _batch_id: Optional[int]
-    _outputs: Optional[TransformerModelOutput]
-    _backprop: Optional[Callable[[List[List[Ragged]], Tuple[int]], Any]]
-
-    @classmethod
-    def get_batch_id(cls, inputs: Iterable[Doc]) -> int:
-        """Calculate a content-sensitive hash of the batch of documents, to check
-        whether the next batch of documents is unexpected.
-        """
-        return sum(sum(token.orth for token in doc) for doc in inputs)
-
-    def receive(
+    def __init__(
         self,
-        batch_id: int,
-        outputs: TransformerModelOutput,
-        backprop: Callable[[List[List[Ragged]], Tuple[int]], Any],
+        vocab: Vocab,
+        model: Model,
+        *,
+        name: str = "transformer",
+        frozen: bool = False,
+        all_layer_outputs: bool = False,
     ) -> None:
-        """Store a batch of training predictions and a backprop callback. The
-        predictions and callback are produced by the upstream Transformer component,
-        and later will be used when the listener's component's model is called.
-        """
-        self._batch_id = batch_id
-        self._outputs = outputs
-        self._backprop = backprop
-
-    def verify_inputs(self, inputs: Iterable[Doc]) -> bool:
-        """Check that the batch of Doc objects matches the ones we have a
-        prediction for.
         """
-        if self._batch_id is None and self._outputs is None:
-            raise ValueError(SpacyErrors.E954)
-        else:
-            batch_id = self.get_batch_id(inputs)
-            if batch_id != self._batch_id:
-                raise ValueError(
-                    SpacyErrors.E953.format(id1=batch_id, id2=self._batch_id)
-                )
-            else:
-                return True
+        vocab (Vocab):
+            The shared vocabulary.
+        model (Model):
+            One of the supported pre-trained transformer models.
+        name (str):
+            The component instance name.
+        frozen (bool):
+            If `True`, the model's weights are frozen and no backpropagation is performed.
+        all_layer_outputs (bool):
+            If `True`, the model returns the outputs of all the layers. Otherwise, only the
+            output of the last layer is returned. This must be set to `True` if any of the pipe's
+            downstream listeners require the outputs of all transformer layers.
+        """
+        self.vocab = vocab
+        self.model = model
+        self.name = name
+        self.listener_map: Dict[str, List[TransformerListenerModelT]] = {}
+        self.cfg: Dict[str, Any] = {}
+
+        _install_extensions()
+        self.frozen = frozen
+        self.all_layer_outputs = all_layer_outputs
+        self._set_model_all_layer_outputs(all_layer_outputs)
 
+    @property
+    def listeners(self) -> List[TransformerListenerModelT]:
+        """
+        RETURNS (List[TransformerListenerModelT]):
+            The listener models listening to this component. Usually internals.
+        """
+        return [m for c in self.listening_components for m in self.listener_map[c]]
 
-class TransformerLayersListener(TransformerListener):
-    """Passes through the pooled representations of all transformer layers.
+    @property
+    def listening_components(self) -> List[str]:
+        """
+        RETURNS (List[str]):
+            The downstream components listening to this component. Usually internals.
+        """
+        return list(self.listener_map.keys())
 
-    Requires its upstream Transformer component to return all layer outputs from
-    its model.
-    """
+    def add_listener(
+        self, listener: TransformerListenerModelT, component_name: str
+    ) -> None:
+        """Add a listener for a downstream component. Usually internals."""
+        if not ListenerStateUtils.is_listener(listener):
+            raise ValueError(Errors.E026.format(model_name=listener.name))
+
+        self.listener_map.setdefault(component_name, [])
+        if listener not in self.listener_map[component_name]:
+            self.listener_map[component_name].append(listener)
+
+    def remove_listener(
+        self, listener: TransformerListenerModelT, component_name: str
+    ) -> bool:
+        """Remove a listener for a downstream component. Usually internals.
 
-    name = "transformer_layers_listener"
+        RETURNS (bool):
+            `True` if successful, `False` otherwise.
+        """
+        if component_name in self.listener_map:
+            if listener in self.listener_map[component_name]:
+                self.listener_map[component_name].remove(listener)
+                # If no listeners are left, remove entry
+                if not self.listener_map[component_name]:
+                    del self.listener_map[component_name]
+                return True
+        return False
 
-    def __init__(
-        self,
-        upstream_name: str,
-        pooling: PoolingModelT,
-        width: int,
-        layers: int,
-        grad_factor: float,
-    ) -> None:
+    def find_listeners(self, component: Any) -> None:
+        """Walk over a model of a processing component, looking for layers that
+        are transformer listeners that have an upstream_name that matches
+        this component. Listeners can also set their upstream_name attribute to
+        the wildcard string '*' to match any `Transformer`.
+        You're unlikely to ever need multiple `Transformer` components, so it's
+        fine to leave your listeners upstream_name on '*'.
         """
-        upstream_name (str):
-            A string to identify the 'upstream' Transformer component
-            to communicate with. The upstream name should either be the wildcard
-            string '*', or the name of the Transformer component.
-
-            In almost all cases, the wildcard string will suffice as there'll only be one
-            upstream Transformer component. But in certain situations, e.g: you have disjoint
-            datasets for certain tasks, or you'd like to use a pre-trained pipeline but a
-            downstream task requires its own token representations, you could end up with
-            more than one Transformer component in the pipeline.
-        pooling (PoolingModelT):
-            Model that is used to perform pooling over the piece representations.
-        width (int):
-            The width of the vectors produced by the upstream transformer component.
-        layers (int):
-            The the number of layers produced by the upstream transformer component,
-            excluding the embedding layer.
-        grad_factor (float):
-            Factor to multiply gradients with.
-        """
-        Model.__init__(
-            self,
-            name=self.name,
-            forward=tranformer_layers_listener_forward,
-            dims={"nO": width},
-            layers=[with_ragged_layers(pooling)],
-            attrs={
-                "grad_factor": grad_factor,
-                "layers": layers + 1,
-            },
-            refs={"pooling": pooling},
-        )
-        self.upstream_name = upstream_name
-        self._batch_id = None
-        self._outputs = None
-        self._backprop = None
-
-
-def tranformer_layers_listener_forward(
-    model: TransformerLayersListener, docs: Iterable[Doc], is_train: bool
-) -> Tuple[List[List[Floats2d]], Callable[[Any], Any]]:
-    pooling: WithRaggedLayersModelT = model.layers[0]
-    grad_factor: float = model.attrs["grad_factor"]
-    n_layers: int = model.attrs["layers"]
-
-    if is_train:
-        assert model._outputs is not None
-        if model._outputs.last_layer_only:
-            raise ValueError(
-                Errors.E012.format(listener_name="TransformerLayersListener")
-            )
+        names = ("*", self.name)
+        if isinstance(getattr(component, "model", None), Model):
+            for node in component.model.walk():
+                if (
+                    ListenerStateUtils.is_listener(node)
+                    and ListenerStateUtils.get_upstream_name(node) in names
+                ):
+                    self.add_listener(node, component.name)
+
+    def pipe(self, stream: Iterable[Doc], *, batch_size: int = 128) -> Iterator[Doc]:
+        """Apply the pipe to a stream of documents. This usually happens under
+        the hood when the nlp object is called on a text and all components are
+        applied to the Doc.
+
+        stream (Iterable[Doc]):
+            A stream of documents.
+        batch_size (int):
+            The number of documents to buffer.
 
-        model.verify_inputs(docs)
+        YIELDS (Doc):
+            Processed documents in order.
+        """
+        _install_extensions()
+        for batch in minibatch(stream, batch_size):
+            preds = self.predict(batch)
+            self.set_annotations(batch, preds)
+            yield from batch
 
-        Y, backprop_pooling = pooling(model._outputs.all_outputs, is_train)
+    def predict(self, docs: Iterable[Doc]) -> TransformerModelOutput:
+        """Apply the pipeline's model to a batch of docs, without modifying them.
 
-        def backprop(dY):
-            dX = backprop_pooling(dY)
+        docs (Iterable[Doc]):
+            The documents to predict.
 
-            if grad_factor != 1.0:
-                for dX_doc in dX:
-                    for dX_layer in dX_doc:
-                        dX_layer.data *= grad_factor
-
-            outputs_to_backprop = tuple(i for i in range(0, model._outputs.num_outputs))
-            dX = model._backprop(dX, outputs_to_backprop=outputs_to_backprop)
-
-            model._batch_id = None
-            model._outputs = None
-            model._backprop = None
-
-            return dX
-
-        return Y, backprop
-    else:
-        width = model.get_dim("nO")
-
-        no_trf_data = [doc._.trf_data is None for doc in docs]
-        if any(no_trf_data):
-            assert all(no_trf_data)
-            return [
-                [model.ops.alloc2f(len(doc), width) for _ in range(n_layers)]
-                for doc in docs
-            ], lambda dY: []
-
-        if any(doc._.trf_data.last_layer_only for doc in docs):
-            raise ValueError(
-                Errors.E012.format(listener_name="TransformerLayersListener")
+        RETURNS (TransformerModelOutput):
+            The extracted features of each document.
+        """
+        _install_extensions()
+        if not any(len(doc) for doc in docs):
+            # Handle cases where there are no tokens in any docs.
+            width = self.model.get_dim("nO")
+            return TransformerModelOutput(
+                outputs=[
+                    [
+                        Ragged(
+                            data=self.model.ops.alloc2f(0, width),
+                            lengths=self.model.ops.alloc1i(0),
+                        )
+                    ]
+                    for _ in docs
+                ],
+                last_layer_only=True,
             )
 
-        return pooling.predict(docs), lambda dY: []
+        # To ensure that the model's internal state is always consistent with the pipe's.
+        self._set_model_all_layer_outputs(self.all_layer_outputs)
+        return self.model.predict(docs)
 
+    def set_annotations(
+        self, docs: Sequence[Doc], trf_output: TransformerModelOutput
+    ) -> None:
+        """Assign the extracted features to the Doc objects. By default, a
+        DocTransformerOutput object is written to the doc._.trf_data attribute.
 
-class LastTransformerLayerListener(TransformerListener):
-    """Extracts the output of the last transformer layer and performs pooling over the
-    individual pieces of each Doc token, returning their corresponding representations.
-    """
-
-    name = "last_transformer_layer_listener"
+        docs (Iterable[Doc]):
+            The documents to modify.
+        trf_output (TransformerModelOutput):
+            The outputs of the transformer model.
+        """
+        for doc, tokvecs in zip(docs, trf_output.all_outputs):
+            doc._.trf_data = DocTransformerOutput(
+                all_outputs=tokvecs, last_layer_only=trf_output.last_layer_only
+            )
 
-    def __init__(
+    def update(
         self,
-        upstream_name: str,
-        pooling: PoolingModelT,
-        width: int,
-        grad_factor: float,
-    ) -> None:
+        examples: Iterable[Example],
+        *,
+        drop: float = 0.0,
+        sgd: Optional[Optimizer] = None,
+        losses: Optional[Dict[str, float]] = None,
+    ) -> Dict[str, float]:
+        """Prepare for an update to the transformer.
+
+        Like the `Tok2Vec` component, the `Transformer` component is unusual
+        in that it does not receive "gold standard" annotations to calculate
+        a weight update. The optimal output of the transformer data is unknown;
+        it's a hidden layer inside the network that is updated by backpropagating
+        from output layers.
+
+        The `Transformer` component therefore does not perform a weight update
+        during its own `update` method. Instead, it runs its transformer model
+        and communicates the output and the backpropagation callback to any
+        downstream components that have been connected to it via the
+        transformer listener sublayer. If there are multiple listeners, the last
+        layer will actually backprop to the transformer and call the optimizer,
+        while the others simply increment the gradients.
+
+        examples (Iterable[Example]):
+            A batch of Example objects. Only the `predicted` doc object is used,
+            the reference doc is ignored.
+        drop (float):
+            The dropout rate.
+        sgd (thinc.api.Optimizer):
+            The optimizer.
+        losses (Dict[str, float]):
+            Optional record of the loss during training. Updated using the component
+            name as the key.
+
+        RETURNS (Dict[str, float]):
+            The updated losses dictionary.
         """
-        upstream_name (str):
-            A string to identify the 'upstream' Transformer component
-            to communicate with. The upstream name should either be the wildcard
-            string '*', or the name of the Transformer component.
-
-            In almost all cases, the wildcard string will suffice as there'll only be one
-            upstream Transformer component. But in certain situations, e.g: you have disjoint
-            datasets for certain tasks, or you'd like to use a pre-trained pipeline but a
-            downstream task requires its own token representations, you could end up with
-            more than one Transformer component in the pipeline.
-        width (int):
-            The width of the vectors produced by the upstream transformer component.
-        pooling (Model):
-            Model that is used to perform pooling over the piece representations.
-        grad_factor (float):
-            Factor to multiply gradients with.
-        """
-        Model.__init__(
-            self,
-            name=self.name,
-            forward=last_transformer_layer_listener_forward,
-            dims={"nO": width},
-            layers=[with_ragged_last_layer(pooling)],
-            attrs={"grad_factor": grad_factor},
-            refs={"pooling": pooling},
+        if losses is None:
+            losses = {}
+        validate_examples(examples, "Transformer.update")
+        docs = [eg.predicted for eg in examples]
+        set_dropout_rate(self.model, drop)
+        losses.setdefault(self.name, 0.0)
+
+        # To ensure that the model's internal state is always consistent with the pipe's.
+        self._set_model_all_layer_outputs(self.all_layer_outputs)
+
+        outputs, accum_func, backprop_func = self._create_backprops(
+            docs, losses, sgd=sgd
         )
-        self.upstream_name = upstream_name
-        self._batch_id = None
-        self._outputs = None
-        self._backprop = None
-
-
-def last_transformer_layer_listener_forward(
-    model: LastTransformerLayerListener, docs: Iterable[Doc], is_train: bool
-) -> Tuple[List[Floats2d], Callable[[Any], Any]]:
-    pooling: WithRaggedLastLayerModelT = model.layers[0]
-    grad_factor: float = model.attrs["grad_factor"]
-
-    if is_train:
-        model.verify_inputs(docs)
-        assert model._outputs is not None
-        Y, backprop_pooling = pooling(model._outputs.last_hidden_layer_states, is_train)
-
-        def backprop(dY):
-            dX_pooling = backprop_pooling(dY)
-            if grad_factor != 1.0:
-                for dx in dX_pooling:
-                    dx.data *= grad_factor
-            dX = model._backprop([[d] for d in dX_pooling], outputs_to_backprop=(-1,))
-            model._batch_id = None
-            model._outputs = None
-            model._backprop = None
-            return dX
-
-        return Y, backprop
-    else:
-        width = model.get_dim("nO")
-
-        no_trf_data = [doc._.trf_data is None for doc in docs]
-        if any(no_trf_data):
-            assert all(no_trf_data)
-            return [model.ops.alloc2f(len(doc), width) for doc in docs], lambda dY: []
-
-        return pooling.predict(docs), lambda dY: []
-
-
-class ScalarWeightingListener(TransformerListener):
-    """Calculates a weighted representation of all transformer layer outputs and
-    performs pooling over the individual pieces of each Doc token, returning their
-    corresponding representations.
 
-    Requires its upstream Transformer component to return all layer outputs from
-    its model.
-    """
+        batch_id = ListenerStateUtils.calculate_batch_id(docs)
+        for listener in self.listeners[:-1]:
+            ListenerStateUtils.receive(listener, batch_id, outputs, accum_func)
+        if self.listeners:
+            ListenerStateUtils.receive(
+                self.listeners[-1], batch_id, outputs, backprop_func
+            )
+        return losses
 
-    name = "scalar_weighting_listener"
+    def get_loss(self, examples: Iterable[Example], scores: Any) -> None:
+        """A noop function, for compatibility with the Pipe API. See the `update`
+        method for an explanation of the loss mechanics of the component.
+        """
+        pass
 
-    def __init__(
+    def initialize(
         self,
-        upstream_name: str,
-        weighting: ScalarWeightModelT,
-        pooling: PoolingModelT,
-        width: int,
-        grad_factor: float,
-    ) -> None:
+        get_examples: Callable[[], Iterable[Example]],
+        *,
+        nlp: Optional[Language] = None,
+        encoder_loader: Optional[Callable] = None,
+        piecer_loader: Optional[Callable] = None,
+    ):
+        """Initialize the pipe for training, using data examples if available.
+
+        get_examples (Callable[[], Iterable[Example]]):
+            Optional function that returns gold-standard Example objects.
+        nlp (Language):
+            The current nlp object.
+        encoder_loader (Optional[Callable]):
+            Initialization callback for the transformer model.
+        piece_loader (Optional[Callable]):
+            Initialization callback for the input piece encoder.
         """
-        upstream_name (str):
-            A string to identify the 'upstream' Transformer component
-            to communicate with. The upstream name should either be the wildcard
-            string '*', or the name of the Transformer component.
-
-            In almost all cases, the wildcard string will suffice as there'll only be one
-            upstream Transformer component. But in certain situations, e.g: you have disjoint
-            datasets for certain tasks, or you'd like to use a pre-trained pipeline but a
-            downstream task requires its own token representations, you could end up with
-            more than one Transformer component in the pipeline.
-        weighting (Model):
-            Model that is used to perform the weighting of the different layer outputs.
-        pooling (Model):
-            Model that is used to perform pooling over the piece representations.
-        width (int):
-            The width of the vectors produced by the upstream transformer component.
-        grad_factor (float):
-            Factor to multiply gradients with.
-        """
-        Model.__init__(
-            self,
-            name=self.name,
-            forward=scalar_weighting_listener_forward,
-            dims={"nO": width},
-            layers=[weighting, with_ragged_last_layer(pooling)],
-            attrs={
-                "grad_factor": grad_factor,
-            },
-        )
-        self.upstream_name = upstream_name
-        self._batch_id = None
-        self._outputs = None
-        self._backprop = None
-
-
-def scalar_weighting_listener_forward(
-    model: ScalarWeightingListener, docs: Iterable[Doc], is_train: bool
-) -> Tuple[List[Floats2d], Callable[[Any], Any]]:
-    weighting: ScalarWeightModelT = model.layers[0]
-    pooling: WithRaggedLastLayerModelT = model.layers[1]
-    grad_factor: float = model.attrs["grad_factor"]
-
-    if is_train:
-        assert model._outputs is not None
-        if model._outputs.last_layer_only:
-            raise ValueError(
-                Errors.E012.format(listener_name="ScalarWeightingListener")
-            )
+        validate_get_examples(get_examples, "Transformer.initialize")
 
-        model.verify_inputs(docs)
+        if encoder_loader:
+            self.model.get_ref("transformer").init = encoder_loader  # type: ignore
+        if piecer_loader:
+            self.model.get_ref("piece_encoder").init = piecer_loader  # type: ignore
 
-        Y_weighting: ScalarWeightOutT = []
-        weighting_inputs = model._outputs.all_outputs
-        outputs_to_backprop = tuple(i for i in range(model._outputs.num_outputs))
-
-        Y_weighting, backprop_weighting = weighting(weighting_inputs, is_train)
-        Y, backprop_pooling = pooling(Y_weighting, is_train)
-
-        def backprop(dYs):
-            dX_pooling = backprop_pooling(dYs)
-            dX_weighting = backprop_weighting(dX_pooling)
-
-            if grad_factor != 1.0:
-                for dx_inner in dX_weighting:
-                    for dx in dx_inner:
-                        dx.data *= grad_factor
-
-            dX = model._backprop(dX_weighting, outputs_to_backprop=outputs_to_backprop)
-            model._batch_id = None
-            model._outputs = None
-            model._backprop = None
-            return dX
-
-        return Y, backprop
-    else:
-        width = model.get_dim("nO")
-
-        no_trf_data = [doc._.trf_data is None for doc in docs]
-        if any(no_trf_data):
-            assert all(no_trf_data)
-            return [model.ops.alloc2f(len(doc), width) for doc in docs], lambda dY: []
-
-        if any(doc._.trf_data.last_layer_only for doc in docs):
-            raise ValueError(
-                Errors.E012.format(listener_name="ScalarWeightingListener")
-            )
+        doc_sample = []
+        for example in islice(get_examples(), 10):
+            doc_sample.append(example.x)
+        assert doc_sample, SpacyErrors.E923.format(name=self.name)
+        self.model.initialize(X=doc_sample)
+
+    def add_label(self, label: Any):
+        raise NotImplementedError
 
-        Y_weigthing = weighting.predict([doc._.trf_data.all_outputs for doc in docs])
-        Y = pooling.predict(Y_weigthing)
+    def finish_update(self, sgd: Optimizer) -> None:
+        """Update parameters using the current parameter gradients.
+        The Optimizer instance contains the functionality to perform
+        the stochastic gradient descent.
+
+        This method is a noop when the pipe is frozen.
+
+        sgd (thinc.api.Optimizer): The optimizer.
+
+        DOCS: https://spacy.io/api/pipe#finish_update
+        """
+        if not self.frozen:
+            self.model.finish_update(sgd)
+
+    def _create_backprops(
+        self,
+        docs: Iterable[Doc],
+        losses: Dict[str, float],
+        *,
+        sgd: Optional[Optimizer] = None,
+    ) -> Tuple[TransformerModelOutput, Callable, Callable]:
+        ops = self.model.ops
+        # Accumulate the pipe's loss on the GPU at first.
+        cum_loss = ops.xp.full(1, losses[self.name])
+
+        if self.frozen:
+            # Ensures that the inner torch model is executed in a `no_grad` context.
+            outputs = self.model.predict(docs)
+            bp_outputs = None
+        else:
+            outputs, bp_outputs = self.model.begin_update(docs)
 
-        return Y, lambda dX: []
+        # We'll use this as a buffer for loss accumulation over individual gradients.
+        d_outputs = [
+            [Ragged(ops.alloc_f(t2v.dataXd.shape), t2v.lengths) for t2v in doc_layers]
+            for doc_layers in outputs.all_outputs
+        ]
+
+        # The loss of the transformer is calculated in a different manner than that of the
+        # tok2vec component. Instead of updating the loss value with each downstream component's
+        # gradient, we accumulate the gradients and and update it just once. This reduces the overhead
+        # of launching the associated kernels on the GPU as this operation would otherwise be
+        # performed on a per-document, per-layer basis. The resultant loss value, while potentially
+        # (slightly) different, still communicates the same information as before w.r.t the training
+        # progress: how large were the gradients of the downstream components in this step compared
+        # to the previous steps.
+
+        def accumulate_gradient(
+            one_d_outputs: List[List[Ragged]], outputs_to_backprop: Tuple[int, ...]
+        ) -> None:
+            """Accumulate transformer loss and gradient. This is passed as a callback
+            to all but the last listener. Only the last one does the backprop.
+
+            `outputs_to_backprop` is a tuple of indices indicating to which layers/outputs
+            the gradients are to be propagated.
+            """
+            nonlocal d_outputs
+            for i in range(len(one_d_outputs)):
+                for j in outputs_to_backprop:
+                    d_outputs[i][j].data += one_d_outputs[i][j].data
+
+        def update_loss():
+            """Reduce the gradient buffer and update the losses dict."""
+            nonlocal cum_loss
+            for i in range(len(d_outputs)):
+                for j in range(len(d_outputs[i])):
+                    cum_loss += (d_outputs[i][j].data ** 2).sum()
+            losses[self.name] = float(cum_loss)
+
+        def backprop(
+            one_d_outputs: List[List[Ragged]], outputs_to_backprop: Tuple[int, ...]
+        ) -> Any:
+            """Callback to actually do the backprop. Passed to last listener."""
+            nonlocal d_outputs
+            assert bp_outputs is not None
+            accumulate_gradient(one_d_outputs, outputs_to_backprop=outputs_to_backprop)
+            update_loss()
+            d_docs = bp_outputs(d_outputs)
+            if sgd is not None:
+                self.finish_update(sgd)
+            return d_docs
+
+        def backprop_noop(
+            one_d_outputs: List[List[Ragged]], outputs_to_backprop: Tuple[int, ...]
+        ) -> Any:
+            accumulate_gradient(one_d_outputs, outputs_to_backprop=outputs_to_backprop)
+            update_loss()
+            if sgd is not None:
+                self.finish_update(sgd)
+            return []
+
+        return outputs, accumulate_gradient, backprop_noop if self.frozen else backprop
+
+    def _set_model_all_layer_outputs(self, new_value: bool):
+        self.model.get_ref("transformer").attrs["_all_layer_outputs"] = new_value
+
+
+def _install_extensions() -> None:
+    if not Doc.has_extension(DOC_EXT_ATTR):
+        Doc.set_extension(DOC_EXT_ATTR, default=None)
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/output.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/pooling.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/remove_eos_bos.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/remove_eos_bos.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/scalar_weight.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/types.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Any, Callable, Iterable, List, Union
 
 from spacy.tokens.doc import Doc
+
 from thinc.model import Model
 from thinc.types import Floats2d, Ints1d, Ragged
 
 from .output import TransformerModelOutput
 
 PoolingModelT = Model[Ragged, Floats2d]
+TransformerListenerModelT = Model[List[Doc], List[Floats2d]]
 
 WithRaggedLayersInT = Union[Iterable[Doc], Iterable[Iterable[Ragged]]]
 WithRaggedLayersOutT = List[List[Floats2d]]  # Doc -> Layer -> Representation
 WithRaggedLayersModelT = Model[WithRaggedLayersInT, WithRaggedLayersOutT]
 
 WithRaggedLastLayerInT = Union[Iterable[Doc], Iterable[Ragged]]
 WithRaggedLastLayerOutT = List[Floats2d]  # Doc -> Last Layer Representation
@@ -47,7 +49,15 @@
 TransformerOutT = TransformerModelOutput
 TransformerBackpropT = Callable[[List[List[Floats2d]]], Any]
 TransformerModelT = Model[TransformerInT, TransformerOutT]
 
 ScalarWeightInT = List[List[Ragged]]  # Doc -> Layer -> Representation
 ScalarWeightOutT = List[Ragged]  # Doc -> Weighted Representation
 ScalarWeightModelT = Model[ScalarWeightInT, ScalarWeightOutT]
+
+# Only used when replacing listeners.
+WrappedTransformerAndListenerInT = List[Doc]
+WrappedTransformerAndListenerOutT = List[Floats2d]
+WrappedTransformerAndListenerBackpropT = Callable[[List[List[Floats2d]]], Any]
+WrappedTransformerAndListenerModelT = Model[
+    WrappedTransformerAndListenerInT, WrappedTransformerAndListenerOutT
+]
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_non_ws_tokens.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/models/with_strided_spans.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/models/with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/conftest.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_hf_model.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_hf_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_listeners.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_listeners.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import pytest
 from spacy import util
 from spacy.training import Example
-from thinc.api import Config, reduce_mean
-
-from spacy_curated_transformers.models.listeners import build_transformer_layers_listener_v1
 from spacy_curated_transformers._compat import has_hf_transformers
+from spacy_curated_transformers.models.listeners import (
+    build_transformer_layers_listener_v1,
+)
+
+from thinc.api import Config, reduce_mean
 
 cfg_string_transformer_layers_listener = """
     # TransformerLayersListener
 
     [nlp]
     lang = "en"
     pipeline = ["transformer"]
@@ -44,23 +46,23 @@
     config = Config().from_str(cfg_string_transformer_layers_listener)
     nlp = util.load_model_from_config(config, auto_fill=True, validate=True)
 
     transformer = nlp.get_pipe("transformer")
     listener = build_transformer_layers_listener_v1(
         layers=2, width=60, pooling=reduce_mean()
     )
-    transformer.add_listener(listener, "test")
 
     docs = [
         nlp.make_doc("Let's test a transformer."),
         nlp.make_doc("Can it handle more than one doc?"),
     ]
     examples = [Example.from_dict(doc, {}) for doc in docs]
 
     nlp.initialize(lambda: examples)
+    transformer.add_listener(listener, "test")
 
     # Check prediction.
     transformer.pipe(docs)
     Y = listener.predict(docs)
 
     hidden_size = 60
     layers = 3  # embed + hidden layers
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_pooling.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_pooling.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_scalar_weight.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_scalar_weight.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_transformer_model.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_with_non_ws_tokens.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/models/test_with_strided_spans.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/models/test_with_strided_spans.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/test_transformer.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/pipeline/test_transformer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-from typing import Dict, Any
 from functools import partial
+from typing import Any, Dict
+
+import numpy
 import pytest
 import spacy
+import torch
 from spacy import Config, util
+from spacy.language import Language
 from spacy.training import Example
 from spacy.training.initialize import init_nlp
 from spacy.training.loop import train
-from spacy.language import Language
 from spacy.util import registry as spacy_registry
-import torch
-
+from spacy_curated_transformers._compat import has_hf_transformers, transformers
 from spacy_curated_transformers.models.architectures import (
-    build_camembert_transformer_model_v1,
-    build_xlmr_transformer_model_v1,
     build_bert_transformer_model_v1,
+    build_camembert_transformer_model_v1,
     build_roberta_transformer_model_v1,
+    build_xlmr_transformer_model_v1,
 )
 from spacy_curated_transformers.models.hf_loader import (
     build_hf_transformer_encoder_loader_v1,
 )
+from spacy_curated_transformers.models.listeners import (
+    ListenerStateUtils,
+    WrappedTransformerAndListener,
+)
 from spacy_curated_transformers.models.with_strided_spans import (
     build_with_strided_spans_v1,
 )
+from spacy_curated_transformers.pipeline.transformer import make_transformer
 from spacy_curated_transformers.tokenization import (
     build_bert_wordpiece_encoder_v1,
     build_byte_bpe_encoder_v1,
     build_camembert_sentencepiece_encoder_v1,
     build_hf_piece_encoder_loader_v1,
     build_xlmr_sentencepiece_encoder_v1,
 )
-from spacy_curated_transformers.pipeline.transformer import make_transformer
 from spacy_curated_transformers.tokenization.sentencepiece_encoder import (
     build_sentencepiece_encoder_loader_v1,
 )
 from spacy_curated_transformers.util import create_gradual_transformer_unfreezing
-from spacy_curated_transformers._compat import has_hf_transformers, transformers
 
-from ..util import torch_assertclose
+from thinc.model import Model
 
+from ..util import make_tempdir, torch_assertclose, xp_assert_array_equal
 
 cfg_string_last_layer_listener = """
     # LastTransformerLayerListener
 
     [nlp]
     lang = "en"
     pipeline = ["transformer","tagger"]
@@ -555,7 +561,123 @@
 
     nlp = init_nlp(config)
     train(nlp)
     assert nlp.get_pipe("transformer").frozen == False
 
     with pytest.raises(ValueError):
         create_gradual_transformer_unfreezing({"transformer": 5, "*": 4})
+
+
+@pytest.mark.skipif(not has_hf_transformers, reason="requires huggingface transformers")
+@pytest.mark.parametrize(
+    ["cfg_string", "listener_name", "listener_entrypoint"],
+    [
+        (
+            cfg_string_last_layer_listener,
+            "last_transformer_layer_listener",
+            "spacy-curated-transformers.LastTransformerLayerListener.v1",
+        ),
+        (
+            cfg_string_scalar_weighting_layer_listener,
+            "scalar_weighting_listener",
+            "spacy-curated-transformers.ScalarWeightingListener.v1",
+        ),
+    ],
+)
+def test_replace_listeners(cfg_string, listener_name, listener_entrypoint):
+    orig_config = Config().from_str(cfg_string)
+    nlp = util.load_model_from_config(orig_config, auto_fill=True, validate=True)
+    text = "This is awesome"
+    examples = [Example.from_dict(nlp.make_doc(text), {"tags": ["A", "B", "C"]})]
+    optimizer = nlp.initialize(lambda: examples)
+
+    # verify correct configuration with transformer listener
+    transformer = nlp.get_pipe("transformer")
+    tagger = nlp.get_pipe("tagger")
+
+    tagger_tok2vec = tagger.model.get_ref("tok2vec")
+
+    assert ListenerStateUtils.is_listener(tagger_tok2vec)
+    assert transformer.listener_map["tagger"][0] == tagger_tok2vec
+    assert isinstance(transformer.model, Model)
+    assert transformer.model.name == "transformer_model"
+    assert (
+        nlp.config["components"]["transformer"]["model"]["@architectures"]
+        == "spacy-curated-transformers.BertTransformer.v1"
+    )
+    assert (
+        nlp.config["components"]["tagger"]["model"]["tok2vec"]["@architectures"]
+        == listener_entrypoint
+    )
+
+    # train pipe before replacing listeners
+    for i in range(5):
+        losses = {}
+        nlp.update(examples, sgd=optimizer, losses=losses)
+        doc = nlp(text)
+
+    preds = [t.tag_ for t in doc]
+    doc_tensor = tagger_tok2vec.predict([doc])
+
+    # replace listener and verify predictions are still the same
+    transformer.frozen = True
+    nlp.replace_listeners("transformer", "tagger", ["model.tok2vec"])
+    tagger = nlp.get_pipe("tagger")
+    tagger_tok2vec = tagger.model.get_ref("tok2vec")
+    assert isinstance(tagger_tok2vec, WrappedTransformerAndListener)
+    assert tagger_tok2vec.frozen_transformer
+    assert tagger_tok2vec.layers[0].name == "transformer_model"
+    assert tagger_tok2vec.layers[1].name == listener_name
+    assert (
+        nlp.config["components"]["tagger"]["model"]["tok2vec"]["@architectures"]
+        == "spacy-curated-transformers.BertTransformer.v1"
+    )
+    assert (
+        nlp.config["components"]["tagger"]["model"]["tok2vec"]["wrapped_listener"][
+            "@architectures"
+        ]
+        == listener_entrypoint
+    )
+    doc2 = nlp(text)
+    assert preds == [t.tag_ for t in doc2]
+    pred_tensor = tagger_tok2vec.predict([doc2])
+    xp_assert_array_equal(doc_tensor, pred_tensor)
+
+    optimizer = nlp.resume_training()
+    trf_output_frozen = tagger_tok2vec.layers[0].predict([doc2])
+    for i in range(5):
+        losses = {}
+        nlp.update(examples, sgd=optimizer, losses=losses)
+        assert losses["tagger"] > 0.0
+    trf_output_frozen_after_update = tagger_tok2vec.layers[0].predict([doc2])
+
+    for x, y in zip(
+        trf_output_frozen.all_outputs, trf_output_frozen_after_update.all_outputs
+    ):
+        for x1, y1 in zip(x, y):
+            xp_assert_array_equal(x1.dataXd, y1.dataXd)
+
+    tagger_tok2vec.frozen_transformer = False
+    trf_output = tagger_tok2vec.layers[0].predict([doc2])
+    # attempt training with the new pipeline
+    for i in range(5):
+        losses = {}
+        nlp.update(examples, sgd=optimizer, losses=losses)
+        assert losses["tagger"] > 0.0
+    trained_trf_output = tagger_tok2vec.layers[0].predict([doc2])
+
+    for x, y in zip(trf_output.all_outputs, trained_trf_output.all_outputs):
+        for x1, y1 in zip(x, y):
+            assert not numpy.array_equal(x1.dataXd, y1.dataXd)
+
+    # ensure IO goes OK
+    doc_tensor_trained = tagger_tok2vec.predict([doc])
+
+    with make_tempdir() as d:
+        file_path = d / "trained_nlp"
+        nlp.to_disk(file_path)
+        nlp2 = util.load_model_from_path(file_path)
+        doc3 = nlp2(text)
+        tagger2 = nlp2.get_pipe("tagger")
+        tagger_tok2vec2 = tagger2.model.get_ref("tok2vec")
+        pred_tensor = tagger_tok2vec2.predict([doc3])
+        xp_assert_array_equal(doc_tensor_trained, pred_tensor)
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/pipeline/toy-en-corpus.spacy`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_registry.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/test_torchscript_wrapper.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/test_torchscript_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_char_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/test_xlmr_adapter.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-merges.txt` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy-vocab.json` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.model` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy.model`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tests/tokenization/toy.wordpieces` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tests/tokenization/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/__init__.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/bbpe_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/bbpe_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/char_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/char_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/hf_loader.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/hf_loader.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_adapters.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/sentencepiece_adapters.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/sentencepiece_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/sentencepiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/types.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/types.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/tokenization/wordpiece_encoder.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/tokenization/wordpiece_encoder.py`

 * *Files identical despite different names*

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers/util.py` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from typing import Any, Callable, Any, Iterable, Dict, TYPE_CHECKING
+import itertools
 from functools import partial
+from typing import TYPE_CHECKING, Any, Callable, Dict, Iterable
+
 from spacy.language import Language
-import itertools
+
 import thinc
 
 from .errors import Errors
 
 if TYPE_CHECKING:
-    from .pipeline.transformer import Transformer
+    from .pipeline.transformer import CuratedTransformer
 
 thinc.registry.create("model_loaders", entry_points=True)
 registry = thinc.registry
 
 
 def all_equal(iterable: Iterable[Any]) -> bool:
     """Return True if all the elements are equal to each other
@@ -24,36 +26,36 @@
     nlp: Language,
     callback_args: Dict[str, Any],
     freeze_params: Dict[str, int],
 ):
     current_step = callback_args["step"]
 
     # Scoped import to avoid import cycles.
-    from .pipeline.transformer import Transformer
+    from .pipeline.transformer import CuratedTransformer
 
     for name, pipe in nlp.components:
         unfreeze_step = freeze_params.get(name)
         if unfreeze_step is None:
             continue
-        elif not isinstance(pipe, Transformer):
+        elif not isinstance(pipe, CuratedTransformer):
             raise TypeError(Errors.E025.format(pipe_name=name))
 
         pipe.frozen = current_step < unfreeze_step
 
 
 def gradual_transformer_unfreezing_all_pipes(
     nlp: Language, callback_args: Dict[str, Any], unfreeze_step: int
 ):
     current_step = callback_args["step"]
 
     # Scoped import to avoid import cycles.
-    from .pipeline.transformer import Transformer
+    from .pipeline.transformer import CuratedTransformer
 
     for _, pipe in nlp.components:
-        if not isinstance(pipe, Transformer):
+        if not isinstance(pipe, CuratedTransformer):
             continue
 
         pipe.frozen = current_step < unfreeze_step
 
 
 def create_gradual_transformer_unfreezing(
     target_pipes: Dict[str, int]
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/SOURCES.txt` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 spacy_curated_transformers.egg-info/dependency_links.txt
 spacy_curated_transformers.egg-info/entry_points.txt
 spacy_curated_transformers.egg-info/requires.txt
 spacy_curated_transformers.egg-info/top_level.txt
 spacy_curated_transformers.egg-info/zip-safe
 spacy_curated_transformers/cli/__init__.py
 spacy_curated_transformers/cli/debug_pieces.py
-spacy_curated_transformers/cli/quantize.py
 spacy_curated_transformers/models/__init__.py
 spacy_curated_transformers/models/architectures.py
 spacy_curated_transformers/models/hf_loader.py
 spacy_curated_transformers/models/listeners.py
 spacy_curated_transformers/models/output.py
 spacy_curated_transformers/models/pooling.py
 spacy_curated_transformers/models/remove_eos_bos.py
```

### Comparing `spacy-curated-transformers-0.1.1/spacy_curated_transformers.egg-info/entry_points.txt` & `spacy-curated-transformers-0.2.0/spacy_curated_transformers.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 spacy-curated-transformers.XlmrTransformer.v1 = spacy_curated_transformers.models:build_xlmr_transformer_model_v1
 
 [spacy_callbacks]
 spacy-curated-transformers.gradual_transformer_unfreezing.v1 = spacy_curated_transformers.util:create_gradual_transformer_unfreezing
 
 [spacy_cli]
 spacy-curated-transformers.debug_pieces = spacy_curated_transformers.cli.debug_pieces:debug_pieces_cli
-spacy-curated-transformers.quantize = spacy_curated_transformers.cli.quantize:quantize_cli
 
 [spacy_factories]
 curated_transformer = spacy_curated_transformers.pipeline.transformer:make_transformer
 
 [thinc_model_loaders]
 spacy-curated-transformers.ByteBpeLoader.v1 = spacy_curated_transformers.tokenization:build_byte_bpe_encoder_loader_v1
 spacy-curated-transformers.CharEncoderLoader.v1 = spacy_curated_transformers.tokenization:build_char_encoder_loader_v1
```

