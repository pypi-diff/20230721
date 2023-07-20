# Comparing `tmp/eleuther-elk-0.1.tar.gz` & `tmp/eleuther-elk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eleuther-elk-0.1.tar", last modified: Sat Mar  4 04:55:09 2023, max compression
+gzip compressed data, was "eleuther-elk-0.1.1.tar", last modified: Thu Jul 20 23:30:34 2023, max compression
```

## Comparing `eleuther-elk-0.1.tar` & `eleuther-elk-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,751 @@
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.568770 eleuther-elk-0.1/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1067 2023-03-04 04:19:51.000000 eleuther-elk-0.1/LICENSE.md
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     4012 2023-03-04 04:55:09.568770 eleuther-elk-0.1/PKG-INFO
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     3665 2023-03-04 04:22:04.000000 eleuther-elk-0.1/README.md
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.560770 eleuther-elk-0.1/eleuther_elk.egg-info/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     4012 2023-03-04 04:55:09.000000 eleuther-elk-0.1/eleuther_elk.egg-info/PKG-INFO
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)      723 2023-03-04 04:55:09.000000 eleuther-elk-0.1/eleuther_elk.egg-info/SOURCES.txt
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)        1 2023-03-04 04:55:09.000000 eleuther-elk-0.1/eleuther_elk.egg-info/dependency_links.txt
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)       41 2023-03-04 04:55:09.000000 eleuther-elk-0.1/eleuther_elk.egg-info/entry_points.txt
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)      242 2023-03-04 04:55:09.000000 eleuther-elk-0.1/eleuther_elk.egg-info/requires.txt
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)       24 2023-03-04 04:55:09.000000 eleuther-elk-0.1/eleuther_elk.egg-info/top_level.txt
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.560770 eleuther-elk-0.1/elk/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)       73 2023-02-21 05:12:44.000000 eleuther-elk-0.1/elk/__init__.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1846 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/__main__.py
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.560770 eleuther-elk-0.1/elk/extraction/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)      182 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/extraction/__init__.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)    10483 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/extraction/extraction.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1754 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/extraction/generator.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     9285 2023-03-04 04:19:51.000000 eleuther-elk-0.1/elk/extraction/prompt_dataset.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1075 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/files.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1548 2023-02-21 05:12:44.000000 eleuther-elk-0.1/elk/math.py
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.564770 eleuther-elk-0.1/elk/training/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)       89 2023-03-01 02:55:44.000000 eleuther-elk-0.1/elk/training/__init__.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1441 2023-02-19 07:33:33.000000 eleuther-elk-0.1/elk/training/losses.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1698 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/training/preprocessing.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)    13070 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/training/reporter.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     5531 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/training/train.py
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.568770 eleuther-elk-0.1/elk/utils/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)      299 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/utils/__init__.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     3650 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/utils/data_utils.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     4929 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/utils/gpu_utils.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)      968 2023-02-19 12:16:03.000000 eleuther-elk-0.1/elk/utils/tree_utils.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)      326 2023-03-02 22:11:45.000000 eleuther-elk-0.1/elk/utils/typing.py
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.568770 eleuther-elk-0.1/promptsource_module/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1807 2023-03-03 20:00:18.000000 eleuther-elk-0.1/promptsource_module/setup.py
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1936 2023-03-04 04:53:28.000000 eleuther-elk-0.1/pyproject.toml
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)       38 2023-03-04 04:55:09.568770 eleuther-elk-0.1/setup.cfg
-drwxrwxr-x   0 mchorse   (1000) mchorse   (1000)        0 2023-03-04 04:55:09.568770 eleuther-elk-0.1/tests/
--rw-rw-r--   0 mchorse   (1000) mchorse   (1000)     1106 2023-02-21 05:12:44.000000 eleuther-elk-0.1/tests/test_math.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.296879 eleuther-elk-0.1.1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1067 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/LICENSE.md
+-rw-rw-r--   0 nora      (1000) nora      (1000)       81 2023-07-20 22:54:21.000000 eleuther-elk-0.1.1/MANIFEST.in
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5276 2023-07-20 23:30:34.296879 eleuther-elk-0.1.1/PKG-INFO
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4905 2023-06-07 18:44:30.000000 eleuther-elk-0.1.1/README.md
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.176878 eleuther-elk-0.1.1/eleuther_elk.egg-info/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5276 2023-07-20 23:30:34.000000 eleuther-elk-0.1.1/eleuther_elk.egg-info/PKG-INFO
+-rw-rw-r--   0 nora      (1000) nora      (1000)    19269 2023-07-20 23:30:34.000000 eleuther-elk-0.1.1/eleuther_elk.egg-info/SOURCES.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)        1 2023-07-20 23:30:34.000000 eleuther-elk-0.1.1/eleuther_elk.egg-info/dependency_links.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)       41 2023-07-20 23:30:34.000000 eleuther-elk-0.1.1/eleuther_elk.egg-info/entry_points.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)      299 2023-07-20 23:30:34.000000 eleuther-elk-0.1.1/eleuther_elk.egg-info/requires.txt
+-rw-rw-r--   0 nora      (1000) nora      (1000)        4 2023-07-20 23:30:34.000000 eleuther-elk-0.1.1/eleuther_elk.egg-info/top_level.txt
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.176878 eleuther-elk-0.1.1/elk/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      264 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      652 2023-06-07 18:44:30.000000 eleuther-elk-0.1.1/elk/__main__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2051 2023-07-04 21:04:13.000000 eleuther-elk-0.1.1/elk/debug_logging.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.176878 eleuther-elk-0.1.1/elk/evaluation/
+-rw-rw-r--   0 nora      (1000) nora      (1000)       54 2023-04-26 11:29:35.000000 eleuther-elk-0.1.1/elk/evaluation/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2817 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/evaluation/evaluate.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.176878 eleuther-elk-0.1.1/elk/extraction/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      402 2023-07-04 21:04:13.000000 eleuther-elk-0.1.1/elk/extraction/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3669 2023-07-04 21:04:13.000000 eleuther-elk-0.1.1/elk/extraction/balanced_sampler.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      524 2023-05-02 23:51:16.000000 eleuther-elk-0.1.1/elk/extraction/dataset_name.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)    17119 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/extraction/extraction.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2627 2023-05-02 23:51:16.000000 eleuther-elk-0.1.1/elk/extraction/generator.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)        0 2023-04-21 02:25:54.000000 eleuther-elk-0.1.1/elk/extraction/prompt_dataset.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6576 2023-07-04 21:04:13.000000 eleuther-elk-0.1.1/elk/extraction/prompt_loading.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1420 2023-06-07 18:44:30.000000 eleuther-elk-0.1.1/elk/files.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/metrics/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      405 2023-04-21 02:26:05.000000 eleuther-elk-0.1.1/elk/metrics/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3326 2023-04-21 02:26:05.000000 eleuther-elk-0.1.1/elk/metrics/accuracy.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3264 2023-04-25 20:38:42.000000 eleuther-elk-0.1.1/elk/metrics/calibration.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3774 2023-07-03 23:43:00.000000 eleuther-elk-0.1.1/elk/metrics/eval.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5236 2023-04-21 02:26:05.000000 eleuther-elk-0.1.1/elk/metrics/roc_auc.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      978 2023-04-06 03:55:07.000000 eleuther-elk-0.1.1/elk/parsing.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/plotting/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1648 2023-06-07 18:44:30.000000 eleuther-elk-0.1.1/elk/plotting/command.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)    14664 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/plotting/visualize.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/
+-rw-rw-r--   0 nora      (1000) nora      (1000)       94 2023-04-06 03:55:07.000000 eleuther-elk-0.1.1/elk/promptsource/__init__.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.172878 eleuther-elk-0.1.1/elk/promptsource/templates/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.076878 eleuther-elk-0.1.1/elk/promptsource/templates/Zaid/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/Zaid/coqa_expanded/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4753 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/Zaid/coqa_expanded/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/Zaid/quac_expanded/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3319 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/Zaid/quac_expanded/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/acronym_identification/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    14592 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/acronym_identification/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.076878 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/Ade_corpus_v2_classification/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1689 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/Ade_corpus_v2_classification/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/Ade_corpus_v2_drug_ade_relation/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2776 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/Ade_corpus_v2_drug_ade_relation/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/Ade_corpus_v2_drug_dosage_relation/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2753 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ade_corpus_v2/Ade_corpus_v2_drug_dosage_relation/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.080878 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.180878 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/adversarialQA/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2912 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/adversarialQA/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/dbert/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2904 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/dbert/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/dbidaf/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2905 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/dbidaf/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/droberta/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2907 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/adversarial_qa/droberta/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/aeslc/
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     3724 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/aeslc/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/ag_news/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8394 2023-05-03 08:34:13.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ag_news/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.080878 eleuther-elk-0.1.1/elk/promptsource/templates/ai2_arc/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/ai2_arc/ARC-Challenge/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3644 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ai2_arc/ARC-Challenge/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/ai2_arc/ARC-Easy/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3639 2023-04-18 05:52:41.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ai2_arc/ARC-Easy/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_polarity/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5872 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_polarity/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.080878 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_reviews_multi/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_reviews_multi/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3939 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_reviews_multi/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.080878 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_us_reviews/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_us_reviews/Wireless_v1_00/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3106 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/amazon_us_reviews/Wireless_v1_00/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.080878 eleuther-elk-0.1.1/elk/promptsource/templates/ambig_qa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.184878 eleuther-elk-0.1.1/elk/promptsource/templates/ambig_qa/light/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7243 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ambig_qa/light/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/anli/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7890 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/anli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/app_reviews/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2522 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/app_reviews/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.084878 eleuther-elk-0.1.1/elk/promptsource/templates/aqua_rat/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/aqua_rat/raw/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3599 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/aqua_rat/raw/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/art/
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     3280 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/art/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/asnq/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5449 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/asnq/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.084878 eleuther-elk-0.1.1/elk/promptsource/templates/asset/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/asset/ratings/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3749 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/asset/ratings/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/asset/simplification/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4281 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/asset/simplification/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/banking77/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    16918 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/banking77/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/billsum/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3721 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/billsum/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.188878 eleuther-elk-0.1.1/elk/promptsource/templates/bing_coronavirus_query_set/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2843 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/bing_coronavirus_query_set/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/biosses/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6032 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/biosses/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.084878 eleuther-elk-0.1.1/elk/promptsource/templates/blbooksgenre/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/blbooksgenre/title_genre_classifiction/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1950 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/blbooksgenre/title_genre_classifiction/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/blended_skill_talk/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2402 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/blended_skill_talk/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/boolq_pt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5153 2023-04-14 05:24:43.000000 eleuther-elk-0.1.1/elk/promptsource/templates/boolq_pt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.088878 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/CN/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3982 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/CN/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/NE/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3982 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/NE/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/P/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3981 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/P/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/V/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3981 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/V/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/raw/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2703 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cbt/raw/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/cc_news/
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     6491 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cc_news/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.088878 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.192878 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/ag_news_pt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8505 2023-04-14 05:24:43.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/ag_news_pt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/boolq_pt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5173 2023-04-14 05:24:43.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/boolq_pt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_ar/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6392 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_ar/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_es/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6142 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_es/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_fr/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6060 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_fr/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_pt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6040 2023-04-14 05:24:43.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_pt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_zh/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5993 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/christykoh/imdb_zh/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/circa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4087 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/circa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/climate_fever/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5529 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/climate_fever/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.092878 eleuther-elk-0.1.1/elk/promptsource/templates/cnn_dailymail/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/cnn_dailymail/3.0.0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4138 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cnn_dailymail/3.0.0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.092878 eleuther-elk-0.1.1/elk/promptsource/templates/codah/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/codah/codah/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4964 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/codah/codah/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.196879 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5035 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5035 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5035 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_3/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5035 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_3/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_4/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5035 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/codah/fold_4/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/code_x_glue_tc_text_to_code/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1488 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/code_x_glue_tc_text_to_code/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/common_gen/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4851 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/common_gen/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/commonsense_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3014 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/commonsense_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/conv_ai/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6222 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/conv_ai/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/conv_ai_2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5395 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/conv_ai_2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/conv_ai_3/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4238 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/conv_ai_3/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.200878 eleuther-elk-0.1.1/elk/promptsource/templates/coqa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3149 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/coqa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.096878 eleuther-elk-0.1.1/elk/promptsource/templates/cord19/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/cord19/metadata/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2511 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cord19/metadata/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.096878 eleuther-elk-0.1.1/elk/promptsource/templates/cos_e/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/cos_e/v1.0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6198 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cos_e/v1.0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/cos_e/v1.11/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6234 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cos_e/v1.11/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/cosmos_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8286 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/cosmos_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/covid_qa_castorini/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1465 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/covid_qa_castorini/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.100878 eleuther-elk-0.1.1/elk/promptsource/templates/craffel/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/craffel/openai_lambada/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2469 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/craffel/openai_lambada/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/craigslist_bargains/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8282 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/craigslist_bargains/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/crows_pairs/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5032 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/crows_pairs/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/dbpedia_14/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8660 2023-05-03 08:34:13.000000 eleuther-elk-0.1.1/elk/promptsource/templates/dbpedia_14/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.100878 eleuther-elk-0.1.1/elk/promptsource/templates/discofuse/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/discofuse/discofuse-sport/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8097 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/discofuse/discofuse-sport/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.204878 eleuther-elk-0.1.1/elk/promptsource/templates/discofuse/discofuse-wikipedia/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8099 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/discofuse/discofuse-wikipedia/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.100878 eleuther-elk-0.1.1/elk/promptsource/templates/discovery/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/discovery/discovery/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    16008 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/discovery/discovery/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/docred/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    12292 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/docred/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/dream/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2647 2023-04-13 19:41:42.000000 eleuther-elk-0.1.1/elk/promptsource/templates/dream/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/drop/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2791 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/drop/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.100878 eleuther-elk-0.1.1/elk/promptsource/templates/duorc/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/duorc/ParaphraseRC/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5605 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/duorc/ParaphraseRC/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/duorc/SelfRC/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5599 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/duorc/SelfRC/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/e2e_nlg_cleaned/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8894 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/e2e_nlg_cleaned/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.104878 eleuther-elk-0.1.1/elk/promptsource/templates/ecthr_cases/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/ecthr_cases/alleged-violation-prediction/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5291 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ecthr_cases/alleged-violation-prediction/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/emo/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6851 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/emo/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/emotion/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3209 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/emotion/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.104878 eleuther-elk-0.1.1/elk/promptsource/templates/enriched_web_nlg/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.208879 eleuther-elk-0.1.1/elk/promptsource/templates/enriched_web_nlg/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2580 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/enriched_web_nlg/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/esnli/
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     6462 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/esnli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.104878 eleuther-elk-0.1.1/elk/promptsource/templates/evidence_infer_treatment/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/evidence_infer_treatment/1.1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7368 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/evidence_infer_treatment/1.1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/evidence_infer_treatment/2.0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7368 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/evidence_infer_treatment/2.0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.104878 eleuther-elk-0.1.1/elk/promptsource/templates/fever/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/fever/v1.0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3087 2023-04-30 16:14:46.000000 eleuther-elk-0.1.1/elk/promptsource/templates/fever/v1.0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/fever/v2.0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3087 2023-04-30 16:14:46.000000 eleuther-elk-0.1.1/elk/promptsource/templates/fever/v2.0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.104878 eleuther-elk-0.1.1/elk/promptsource/templates/financial_phrasebank/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/financial_phrasebank/sentences_allagree/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5377 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/financial_phrasebank/sentences_allagree/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/freebase_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3745 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/freebase_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/generated_reviews_enth/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2514 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/generated_reviews_enth/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/gigaword/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3695 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/gigaword/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.112878 eleuther-elk-0.1.1/elk/promptsource/templates/glue/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/ax/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3198 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/ax/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.212879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/cola/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2690 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/cola/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mnli/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7903 2023-04-30 16:14:46.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mnli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mnli_matched/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7911 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mnli_matched/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mnli_mismatched/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7914 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mnli_mismatched/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mrpc/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3483 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/mrpc/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/qnli/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2575 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/qnli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/qqp/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2942 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/qqp/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/rte/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2672 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/rte/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/sst2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2440 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/sst2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/stsb/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3110 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/stsb/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/glue/wnli/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2547 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/glue/wnli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.216879 eleuther-elk-0.1.1/elk/promptsource/templates/google_wellformed_query/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3468 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/google_wellformed_query/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/great_code/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    10177 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/great_code/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.112878 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_genre_1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7666 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_genre_1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_topic_1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7666 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_topic_1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_topic_4/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7666 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_topic_4/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_topic_7/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7666 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/guardian_authorship/cross_topic_7/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/gutenberg_time/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4170 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/gutenberg_time/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/hans/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4831 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hans/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/hate_speech18/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      591 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hate_speech18/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.112878 eleuther-elk-0.1.1/elk/promptsource/templates/head_qa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/head_qa/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4807 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/head_qa/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/health_fact/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3216 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/health_fact/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.220878 eleuther-elk-0.1.1/elk/promptsource/templates/hellaswag/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7273 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hellaswag/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/hlgd/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7152 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hlgd/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.116878 eleuther-elk-0.1.1/elk/promptsource/templates/hotpot_qa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/hotpot_qa/distractor/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5412 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hotpot_qa/distractor/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/hotpot_qa/fullwiki/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5936 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hotpot_qa/fullwiki/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.116878 eleuther-elk-0.1.1/elk/promptsource/templates/humicroedit/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/humicroedit/subtask-1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5155 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/humicroedit/subtask-1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/humicroedit/subtask-2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7933 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/humicroedit/subtask-2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.116878 eleuther-elk-0.1.1/elk/promptsource/templates/hyperpartisan_news_detection/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/hyperpartisan_news_detection/byarticle/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4094 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hyperpartisan_news_detection/byarticle/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/hyperpartisan_news_detection/bypublisher/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3489 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/hyperpartisan_news_detection/bypublisher/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/imdb/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6073 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/elk/promptsource/templates/imdb/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/jfleg/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3898 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/jfleg/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/jigsaw_unintended_bias/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5863 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/jigsaw_unintended_bias/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.224879 eleuther-elk-0.1.1/elk/promptsource/templates/kelm/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4432 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/kelm/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.116878 eleuther-elk-0.1.1/elk/promptsource/templates/kilt_tasks/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/kilt_tasks/hotpotqa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2493 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/kilt_tasks/hotpotqa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/kilt_tasks/nq/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4223 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/kilt_tasks/nq/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.120878 eleuther-elk-0.1.1/elk/promptsource/templates/lama/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/lama/trex/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2594 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/lama/trex/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/lambada/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2454 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/lambada/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.120878 eleuther-elk-0.1.1/elk/promptsource/templates/lauritowal/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/lauritowal/redefine_math/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      775 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/lauritowal/redefine_math/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/liar/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5723 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/liar/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/limit/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7713 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/limit/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.120878 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_1d/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5241 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_1d/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_1d_composed/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5482 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_1d_composed/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_2d/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5241 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_2d/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.228879 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_2d_composed/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5482 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/math_dataset/algebra__linear_2d_composed/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/math_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3258 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/math_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/mc_taco/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5936 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/mc_taco/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.124878 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/task1_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3790 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/task1_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/task2_recs/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1898 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/task2_recs/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/task3_qarecs/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6925 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/mdd/task3_qarecs/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/medal/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4044 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/medal/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/medical_questions_pairs/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4944 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/medical_questions_pairs/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.124878 eleuther-elk-0.1.1/elk/promptsource/templates/meta_woz/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/meta_woz/dialogues/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4967 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/meta_woz/dialogues/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/mocha/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5492 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/mocha/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.232879 eleuther-elk-0.1.1/elk/promptsource/templates/movie_rationales/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3191 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/movie_rationales/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/multi_news/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3963 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/multi_news/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/multi_nli/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7895 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/multi_nli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/multi_x_science_sum/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4472 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/multi_x_science_sum/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/mwsc/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2454 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/mwsc/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/narrativeqa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4194 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/narrativeqa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/ncbi_disease/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8977 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ncbi_disease/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.128878 eleuther-elk-0.1.1/elk/promptsource/templates/neural_code_search/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/neural_code_search/evaluation_dataset/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      987 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/neural_code_search/evaluation_dataset/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/newspop/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4246 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/newspop/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/nlu_evaluation_data/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    10436 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/nlu_evaluation_data/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/nq_open/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2880 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/nq_open/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/numer_sense/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3240 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/numer_sense/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.236878 eleuther-elk-0.1.1/elk/promptsource/templates/onestop_english/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3938 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/onestop_english/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/openai_humaneval/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1627 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/openai_humaneval/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.128878 eleuther-elk-0.1.1/elk/promptsource/templates/openbookqa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/openbookqa/additional/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3759 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/openbookqa/additional/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/openbookqa/main/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3909 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/openbookqa/main/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.128878 eleuther-elk-0.1.1/elk/promptsource/templates/paws/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/paws/labeled_final/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6212 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/paws/labeled_final/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/paws/labeled_swap/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6211 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/paws/labeled_swap/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/paws/unlabeled_final/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6214 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/paws/unlabeled_final/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.128878 eleuther-elk-0.1.1/elk/promptsource/templates/paws-x/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/paws-x/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6203 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/paws-x/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/piqa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6230 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/elk/promptsource/templates/piqa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/poem_sentiment/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4330 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/poem_sentiment/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.132878 eleuther-elk-0.1.1/elk/promptsource/templates/pubmed_qa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/pubmed_qa/pqa_labeled/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4907 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/pubmed_qa/pqa_labeled/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.240879 eleuther-elk-0.1.1/elk/promptsource/templates/qa_srl/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3679 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/qa_srl/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/qa_zre/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4928 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/qa_zre/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/qasc/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6337 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/qasc/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/qed/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3227 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/qed/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/quac/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4605 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/quac/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/quail/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7814 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/quail/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/quarel/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2901 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/quarel/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/quartz/
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     6286 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/quartz/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/quora/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3146 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/quora/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/quoref/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5255 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/quoref/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.136878 eleuther-elk-0.1.1/elk/promptsource/templates/race/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/race/all/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5121 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/race/all/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.244879 eleuther-elk-0.1.1/elk/promptsource/templates/race/high/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5122 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/race/high/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/race/middle/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5124 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/race/middle/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.136878 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_ar/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5387 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_ar/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_es/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5155 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_es/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_fr/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5162 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_fr/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_pt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5193 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_pt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_zh/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5086 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/boolq_zh/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6678 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_ar/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7160 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_ar/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_es/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6749 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_es/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_fr/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6708 2023-07-20 21:18:24.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_fr/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.248879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_pt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6740 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_pt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_zh/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6556 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/promptsource/templates/reaganjlee/truthful_qa_mc_zh/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/riddle_sense/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2973 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/riddle_sense/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/ropes/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6668 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/ropes/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/rotten_tomatoes/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4524 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/rotten_tomatoes/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/samsum/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2868 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/samsum/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.140878 eleuther-elk-0.1.1/elk/promptsource/templates/scan/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/addprim_jump/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8885 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/addprim_jump/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/addprim_turn_left/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8890 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/addprim_turn_left/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num0/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8884 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num0/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8884 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8884 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.252879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num3/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8884 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/filler_num3/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/length/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8879 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/length/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/simple/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8879 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/simple/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_around_right/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8894 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_around_right/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_jump_around_right/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8899 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_jump_around_right/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_opposite_right/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8896 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_opposite_right/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_right/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8887 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scan/template_right/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scicite/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3046 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scicite/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.144878 eleuther-elk-0.1.1/elk/promptsource/templates/scientific_papers/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scientific_papers/arxiv/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3848 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scientific_papers/arxiv/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scientific_papers/pubmed/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3760 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scientific_papers/pubmed/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/sciq/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4763 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sciq/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.144878 eleuther-elk-0.1.1/elk/promptsource/templates/scitail/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.256879 eleuther-elk-0.1.1/elk/promptsource/templates/scitail/snli_format/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      643 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scitail/snli_format/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/scitail/tsv_format/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2897 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scitail/tsv_format/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.144878 eleuther-elk-0.1.1/elk/promptsource/templates/scitldr/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/scitldr/Abstract/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3042 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/scitldr/Abstract/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.144878 eleuther-elk-0.1.1/elk/promptsource/templates/selqa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/selqa/answer_selection_analysis/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4087 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/selqa/answer_selection_analysis/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/sem_eval_2010_task_8/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5689 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sem_eval_2010_task_8/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/sem_eval_2014_task_1/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4232 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sem_eval_2014_task_1/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/sent_comp/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3203 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sent_comp/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/sick/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2918 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sick/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/sms_spam/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2261 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sms_spam/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/snips_built_in_intents/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5445 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/snips_built_in_intents/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/snli/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7890 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/snli/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.260879 eleuther-elk-0.1.1/elk/promptsource/templates/social_i_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3387 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/social_i_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/species_800/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    12476 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/species_800/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/squad/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2798 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/squad/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.148878 eleuther-elk-0.1.1/elk/promptsource/templates/squad_adversarial/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/squad_adversarial/AddSent/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2826 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/squad_adversarial/AddSent/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/squad_v2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8590 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/squad_v2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.148878 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/amazon/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4498 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/amazon/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/new_wiki/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4994 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/new_wiki/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/nyt/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4511 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/squadshifts/nyt/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.148878 eleuther-elk-0.1.1/elk/promptsource/templates/sst/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/sst/default/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2464 2023-04-07 06:51:23.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sst/default/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/sst2/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5642 2023-04-17 16:24:30.000000 eleuther-elk-0.1.1/elk/promptsource/templates/sst2/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.152878 eleuther-elk-0.1.1/elk/promptsource/templates/story_cloze/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/story_cloze/2016/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3913 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/story_cloze/2016/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.152878 eleuther-elk-0.1.1/elk/promptsource/templates/stsb_multi_mt/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.264879 eleuther-elk-0.1.1/elk/promptsource/templates/stsb_multi_mt/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2488 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/stsb_multi_mt/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.152878 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/books/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6483 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/books/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/electronics/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6489 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/electronics/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/grocery/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6485 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/grocery/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/movies/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6484 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/movies/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/restaurants/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6489 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/restaurants/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/tripadvisor/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6489 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/subjqa/tripadvisor/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.156878 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/axb/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4859 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/axb/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/axg/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4849 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/axg/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/boolq/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5101 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/boolq/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/cb/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8371 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/cb/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.268879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/copa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7935 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/copa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/multirc/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5411 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/multirc/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/record/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    13505 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/record/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/rte/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5658 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/rte/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/wic/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5957 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/wic/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/wsc.fixed/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5875 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/super_glue/wsc.fixed/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.156878 eleuther-elk-0.1.1/elk/promptsource/templates/swag/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/swag/regular/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4507 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/swag/regular/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.156878 eleuther-elk-0.1.1/elk/promptsource/templates/tab_fact/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/tab_fact/tab_fact/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3555 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tab_fact/tab_fact/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/tmu_gfm_dataset/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3934 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tmu_gfm_dataset/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/trec/
+-rw-rw-r--   0 nora      (1000) nora      (1000)    13419 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/trec/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.156878 eleuther-elk-0.1.1/elk/promptsource/templates/trivia_qa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/trivia_qa/unfiltered/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2558 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/trivia_qa/unfiltered/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.272879 eleuther-elk-0.1.1/elk/promptsource/templates/turk/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3954 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/turk/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.160878 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/emoji/
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     2361 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/emoji/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/emotion/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2757 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/emotion/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/hate/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2234 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/hate/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/irony/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2281 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/irony/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/offensive/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2346 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/offensive/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/sentiment/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2708 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/sentiment/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_abortion/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2981 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_abortion/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_atheism/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2969 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_atheism/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_climate/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3017 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_climate/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_feminist/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2981 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_feminist/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.276879 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_hillary/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2969 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tweet_eval/stance_hillary/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.160878 eleuther-elk-0.1.1/elk/promptsource/templates/tydiqa/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/tydiqa/primary_task/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5552 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tydiqa/primary_task/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/tydiqa/secondary_task/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6154 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/tydiqa/secondary_task/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/web_questions/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2052 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/web_questions/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_bio/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4146 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_bio/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.164878 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_hop/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_hop/masked/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4944 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_hop/masked/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_hop/original/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7636 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_hop/original/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6088 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_split/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4416 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wiki_split/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.164878 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type1_anti/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4942 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type1_anti/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type1_pro/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4941 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type1_pro/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.280879 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type2_anti/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4942 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type2_anti/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type2_pro/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4941 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wino_bias/type2_pro/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.164878 eleuther-elk-0.1.1/elk/promptsource/templates/winograd_wsc/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winograd_wsc/wsc273/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4790 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winograd_wsc/wsc273/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winograd_wsc/wsc285/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4790 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winograd_wsc/wsc285/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.168878 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_debiased/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3230 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_debiased/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_l/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3223 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_l/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_m/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3223 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_m/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_s/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3223 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_s/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_xl/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3224 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_xl/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_xs/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3224 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/winogrande/winogrande_xs/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/wiqa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5280 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/wiqa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.168878 eleuther-elk-0.1.1/elk/promptsource/templates/xnli/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.284879 eleuther-elk-0.1.1/elk/promptsource/templates/xnli/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7901 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/xnli/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.168878 eleuther-elk-0.1.1/elk/promptsource/templates/xquad/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/xquad/xquad.en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2815 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/xquad/xquad.en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.168878 eleuther-elk-0.1.1/elk/promptsource/templates/xquad_r/
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/xquad_r/en/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2811 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/xquad_r/en/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/xsum/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4502 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/xsum/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/yahoo_answers_qa/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3968 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/yahoo_answers_qa/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/yahoo_answers_topics/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5563 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/yahoo_answers_topics/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/yelp_polarity/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3888 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/yelp_polarity/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/yelp_review_full/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3290 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/yelp_review_full/templates.yaml
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/promptsource/templates/zest/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5042 2023-03-07 08:39:47.000000 eleuther-elk-0.1.1/elk/promptsource/templates/zest/templates.yaml
+-rw-rw-r--   0 nora      (1000) nora      (1000)    10383 2023-05-03 08:34:13.000000 eleuther-elk-0.1.1/elk/promptsource/templates.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.288879 eleuther-elk-0.1.1/elk/resources/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1646 2023-03-02 22:11:45.000000 eleuther-elk-0.1.1/elk/resources/adjectives.json
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2800 2023-03-02 22:11:45.000000 eleuther-elk-0.1.1/elk/resources/names.json
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6780 2023-07-20 23:09:47.000000 eleuther-elk-0.1.1/elk/run.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.292879 eleuther-elk-0.1.1/elk/training/
+-rw-rw-r--   0 nora      (1000) nora      (1000)      365 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)    10504 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/ccs_reporter.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8031 2023-06-15 00:33:44.000000 eleuther-elk-0.1.1/elk/training/classifier.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      857 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/common.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8656 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/eigen_reporter.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     5104 2023-04-06 03:55:07.000000 eleuther-elk-0.1.1/elk/training/losses.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1216 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/platt_scaling.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1058 2023-04-26 07:56:41.000000 eleuther-elk-0.1.1/elk/training/supervised.py
+-rwxrwxr-x   0 nora      (1000) nora      (1000)     7491 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/sweep.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     7092 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/elk/training/train.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     8644 2023-06-07 18:44:03.000000 eleuther-elk-0.1.1/elk/truncated_eigh.py
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.292879 eleuther-elk-0.1.1/elk/utils/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1093 2023-07-20 20:06:53.000000 eleuther-elk-0.1.1/elk/utils/__init__.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      230 2023-06-07 18:44:30.000000 eleuther-elk-0.1.1/elk/utils/constants.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1182 2023-07-20 21:04:37.000000 eleuther-elk-0.1.1/elk/utils/cv_utils.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     4314 2023-05-02 23:51:16.000000 eleuther-elk-0.1.1/elk/utils/data_utils.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     6832 2023-05-02 23:51:16.000000 eleuther-elk-0.1.1/elk/utils/gpu_utils.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3711 2023-05-03 08:34:13.000000 eleuther-elk-0.1.1/elk/utils/hf_utils.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2377 2023-07-20 20:06:53.000000 eleuther-elk-0.1.1/elk/utils/math_util.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      698 2023-05-02 23:51:16.000000 eleuther-elk-0.1.1/elk/utils/pretty.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      967 2023-04-06 03:55:07.000000 eleuther-elk-0.1.1/elk/utils/tree_utils.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      844 2023-05-03 08:34:13.000000 eleuther-elk-0.1.1/elk/utils/typing.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2506 2023-07-20 22:54:21.000000 eleuther-elk-0.1.1/pyproject.toml
+-rw-rw-r--   0 nora      (1000) nora      (1000)       38 2023-07-20 23:30:34.296879 eleuther-elk-0.1.1/setup.cfg
+drwxrwxr-x   0 nora      (1000) nora      (1000)        0 2023-07-20 23:30:34.296879 eleuther-elk-0.1.1/tests/
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1634 2023-04-06 03:55:07.000000 eleuther-elk-0.1.1/tests/test_classifier.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1685 2023-07-20 21:18:25.000000 eleuther-elk-0.1.1/tests/test_eigen_reporter.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      313 2023-03-20 07:54:17.000000 eleuther-elk-0.1.1/tests/test_gpu_example.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1587 2023-05-02 23:51:16.000000 eleuther-elk-0.1.1/tests/test_load_prompts.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1341 2023-07-20 20:06:53.000000 eleuther-elk-0.1.1/tests/test_math.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3551 2023-04-25 20:38:42.000000 eleuther-elk-0.1.1/tests/test_metrics.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     2020 2023-07-04 21:04:13.000000 eleuther-elk-0.1.1/tests/test_samplers.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1954 2023-07-20 23:09:47.000000 eleuther-elk-0.1.1/tests/test_smoke_elicit.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     3509 2023-07-20 23:09:47.000000 eleuther-elk-0.1.1/tests/test_smoke_eval.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)     1991 2023-04-10 21:18:00.000000 eleuther-elk-0.1.1/tests/test_truncated_eigh.py
+-rw-rw-r--   0 nora      (1000) nora      (1000)      926 2023-06-07 18:44:30.000000 eleuther-elk-0.1.1/tests/test_viz.py
```

### Comparing `eleuther-elk-0.1/LICENSE.md` & `eleuther-elk-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eleuther-elk-0.1/PKG-INFO` & `eleuther-elk-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,116 @@
-Metadata-Version: 2.1
-Name: eleuther-elk
-Version: 0.1
-Summary: Keeping language models honest by directly eliciting knowledge encoded in their activations
-License: MIT License
-Keywords: nlp,interpretability,language-models,explainable-ai
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 ## Introduction
 
 **WIP: This codebase is under active development**
 
-Because language models are trained to predict the next token in naturally occurring text, they often reproduce common human errors and misconceptions, even when they "know better" in some sense. More worryingly, when models are trained to generate text that's rated highly by humans, they may learn to output false statements that human evaluators can't detect. We aim to circumvent this issue by directly [**eliciting latent knowledge**](https://docs.google.com/document/d/1WwsnJQstPq91_Yh-Ch2XRL8H_EpsnjrC1dwZXR37PC8/edit) (ELK) inside the activations of a language model.
-
-Specifically, we're building on the **Contrast Consistent Search** (CCS) method described in the paper [Discovering Latent Knowledge in Language Models Without Supervision](https://arxiv.org/abs/2212.03827) by Burns et al. (2022). In CCS, we search for features in the hidden states of a language model which satisfy certain logical consistency requirements. It turns out that these features are often useful for question-answering and text classification tasks, even though the features are trained without labels.
+Because language models are trained to predict the next token in naturally occurring text, they often reproduce common
+human errors and misconceptions, even when they "know better" in some sense. More worryingly, when models are trained to
+generate text that's rated highly by humans, they may learn to output false statements that human evaluators can't
+detect. We aim to circumvent this issue by directly [**eliciting latent knowledge
+**](https://docs.google.com/document/d/1WwsnJQstPq91_Yh-Ch2XRL8H_EpsnjrC1dwZXR37PC8/edit) (ELK) inside the activations
+of a language model.
+
+Specifically, we're building on the **Contrastive Representation Clustering** (CRC) method described in the
+paper [Discovering Latent Knowledge in Language Models Without Supervision](https://arxiv.org/abs/2212.03827) by Burns
+et al. (2022). In CRC, we search for features in the hidden states of a language model which satisfy certain logical
+consistency requirements. It turns out that these features are often useful for question-answering and text
+classification tasks, even though the features are trained without labels.
 
 ### Quick **Start**
 
-Our code is based on [PyTorch](http://pytorch.org) and [Huggingface Transformers](https://huggingface.co/docs/transformers/index). We test the code on Python 3.9 and 3.10.
+Our code is based on [PyTorch](http://pytorch.org)
+and [Huggingface Transformers](https://huggingface.co/docs/transformers/index). We test the code on Python 3.10 and
+3.11.
 
-First install the package with `pip install -e .` in the root directory, or `pip install -e .[dev]` if you'd like to contribute to the project (see **Development** section below). This should install all the necessary dependencies.
+First install the package with `pip install -e .` in the root directory, or `pip install -e .[dev]` if you'd like to
+contribute to the project (see **Development** section below). This should install all the necessary dependencies.
 
 To fit reporters for the HuggingFace model `model` and dataset `dataset`, just run:
 
 ```bash
 elk elicit microsoft/deberta-v2-xxlarge-mnli imdb
 ```
 
-This will automatically download the model and dataset, run the model and extract the relevant representations if they aren't cached on disk, fit reporters on them, and save the reporter checkpoints to the `elk-reporters` folder in your home directory. It will also evaluate the reporter classification performance on a held out test set and save it to a CSV file in the same folder.
-
-## Caching
+This will automatically download the model and dataset, run the model and extract the relevant representations if they
+aren't cached on disk, fit reporters on them, and save the reporter checkpoints to the `elk-reporters` folder in your
+home directory. It will also evaluate the reporter classification performance on a held out test set and save it to a
+CSV file in the same folder.
 
-The hidden states resulting from `elk elicit` are cached as a HuggingFace dataset to avoid having to recompute them every time we want to train a probe. The cache is stored in the same place as all other HuggingFace datasets, which is usually `~/.cache/huggingface/datasets`.
+The following will generate a CCS (Contrast Consistent Search) reporter instead of the CRC-based reporter, which is the
+default.
 
-## Other commands
+```bash
+elk elicit microsoft/deberta-v2-xxlarge-mnli imdb --net ccs
+```
 
-To only extract the hidden states for the model `model` and the dataset `dataset` and save them to `my_output_dir`, without training any reporters, you can run:
+The following command will evaluate the probe from the run naughty-northcutt on the hidden states extracted from the
+model deberta-v2-xxlarge-mnli for the imdb dataset. It will result in an `eval.csv` and `cfg.yaml` file, which are
+stored under a subfolder in `elk-reporters/naughty-northcutt/transfer_eval`.
 
 ```bash
-elk extract microsoft/deberta-v2-xxlarge-mnli imdb -o my_output_dir
+elk eval naughty-northcutt microsoft/deberta-v2-xxlarge-mnli imdb
 ```
 
-## Development
-To clone the repo and its submodules
+The following runs `elicit` on the Cartesian product of the listed models and datasets, storing it in a special folder
+ELK_DIR/sweeps/<memorable_name>. Moreover, `--add_pooled` adds an additional dataset that pools all of the datasets
+together. You can also add a `--visualize` flag to visualize the results of the sweep.
+
 ```bash
-git clone --recurse-submodules https://github.com/EleutherAI/elk.git
+elk sweep --models gpt2-{medium,large,xl} --datasets imdb amazon_polarity --add_pooled
 ```
-If you already cloned the repo but are missing the promptsource_module submodule, run
+
+If you just do `elk plot`, it will plot the results from the most recent sweep.
+If you want to plot a specific sweep, you can do so with:
+
 ```bash
-git submodule update --init --recursive
+elk plot {sweep_name}
 ```
 
+## Caching
+
+The hidden states resulting from `elk elicit` are cached as a HuggingFace dataset to avoid having to recompute them
+every time we want to train a probe. The cache is stored in the same place as all other HuggingFace datasets, which is
+usually `~/.cache/huggingface/datasets`.
+
+## Development
 
 Use `pip install pre-commit && pre-commit install` in the root folder before your first commit.
 
+### Devcontainer
+
+[
+![Open in Remote - Containers](
+https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
+)
+](
+https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/EleutherAI/elk
+)
+
 ### Run tests
+
 ```bash
 pytest
 ```
+
 ### Run type checking
-We use [pyright](https://github.com/microsoft/pyright), which is built into the VSCode editor. If you'd like to run it as a standalone tool, it requires a [nodejs installation.](https://nodejs.org/en/download/)
+
+We use [pyright](https://github.com/microsoft/pyright), which is built into the VSCode editor. If you'd like to run it
+as a standalone tool, it requires a [nodejs installation.](https://nodejs.org/en/download/)
+
 ```bash
 pyright
 ```
 
-If you work on a new feature / fix or some other code task, make sure to create an issue and assign it to yourself (Maybe, even share it in the elk channel of Eleuther's Discord with a small note). In this way, others know you are working on the issue and people won't do the same thing twice 👍 Also others can contact you easily.
+### Run the linter
+
+We use [ruff](https://beta.ruff.rs/docs/). It is installed as a pre-commit hook, so you don't have to run it manually.
+If you want to run it manually, you can do so with:
+
+```bash
+ruff . --fix
+```
+
+### Contributing to this repository
+
+If you work on a new feature / fix or some other code task, make sure to create an issue and assign it to yourself (
+Maybe, even share it in the elk channel of Eleuther's Discord with a small note). In this way, others know you are
+working on the issue and people won't do the same thing twice 👍 Also others can contact you easily.
```

### Comparing `eleuther-elk-0.1/eleuther_elk.egg-info/PKG-INFO` & `eleuther-elk-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,128 @@
 Metadata-Version: 2.1
 Name: eleuther-elk
-Version: 0.1
+Version: 0.1.1
 Summary: Keeping language models honest by directly eliciting knowledge encoded in their activations
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: 8bit
 License-File: LICENSE.md
 
 ## Introduction
 
 **WIP: This codebase is under active development**
 
-Because language models are trained to predict the next token in naturally occurring text, they often reproduce common human errors and misconceptions, even when they "know better" in some sense. More worryingly, when models are trained to generate text that's rated highly by humans, they may learn to output false statements that human evaluators can't detect. We aim to circumvent this issue by directly [**eliciting latent knowledge**](https://docs.google.com/document/d/1WwsnJQstPq91_Yh-Ch2XRL8H_EpsnjrC1dwZXR37PC8/edit) (ELK) inside the activations of a language model.
-
-Specifically, we're building on the **Contrast Consistent Search** (CCS) method described in the paper [Discovering Latent Knowledge in Language Models Without Supervision](https://arxiv.org/abs/2212.03827) by Burns et al. (2022). In CCS, we search for features in the hidden states of a language model which satisfy certain logical consistency requirements. It turns out that these features are often useful for question-answering and text classification tasks, even though the features are trained without labels.
+Because language models are trained to predict the next token in naturally occurring text, they often reproduce common
+human errors and misconceptions, even when they "know better" in some sense. More worryingly, when models are trained to
+generate text that's rated highly by humans, they may learn to output false statements that human evaluators can't
+detect. We aim to circumvent this issue by directly [**eliciting latent knowledge
+**](https://docs.google.com/document/d/1WwsnJQstPq91_Yh-Ch2XRL8H_EpsnjrC1dwZXR37PC8/edit) (ELK) inside the activations
+of a language model.
+
+Specifically, we're building on the **Contrastive Representation Clustering** (CRC) method described in the
+paper [Discovering Latent Knowledge in Language Models Without Supervision](https://arxiv.org/abs/2212.03827) by Burns
+et al. (2022). In CRC, we search for features in the hidden states of a language model which satisfy certain logical
+consistency requirements. It turns out that these features are often useful for question-answering and text
+classification tasks, even though the features are trained without labels.
 
 ### Quick **Start**
 
-Our code is based on [PyTorch](http://pytorch.org) and [Huggingface Transformers](https://huggingface.co/docs/transformers/index). We test the code on Python 3.9 and 3.10.
+Our code is based on [PyTorch](http://pytorch.org)
+and [Huggingface Transformers](https://huggingface.co/docs/transformers/index). We test the code on Python 3.10 and
+3.11.
 
-First install the package with `pip install -e .` in the root directory, or `pip install -e .[dev]` if you'd like to contribute to the project (see **Development** section below). This should install all the necessary dependencies.
+First install the package with `pip install -e .` in the root directory, or `pip install -e .[dev]` if you'd like to
+contribute to the project (see **Development** section below). This should install all the necessary dependencies.
 
 To fit reporters for the HuggingFace model `model` and dataset `dataset`, just run:
 
 ```bash
 elk elicit microsoft/deberta-v2-xxlarge-mnli imdb
 ```
 
-This will automatically download the model and dataset, run the model and extract the relevant representations if they aren't cached on disk, fit reporters on them, and save the reporter checkpoints to the `elk-reporters` folder in your home directory. It will also evaluate the reporter classification performance on a held out test set and save it to a CSV file in the same folder.
-
-## Caching
+This will automatically download the model and dataset, run the model and extract the relevant representations if they
+aren't cached on disk, fit reporters on them, and save the reporter checkpoints to the `elk-reporters` folder in your
+home directory. It will also evaluate the reporter classification performance on a held out test set and save it to a
+CSV file in the same folder.
 
-The hidden states resulting from `elk elicit` are cached as a HuggingFace dataset to avoid having to recompute them every time we want to train a probe. The cache is stored in the same place as all other HuggingFace datasets, which is usually `~/.cache/huggingface/datasets`.
+The following will generate a CCS (Contrast Consistent Search) reporter instead of the CRC-based reporter, which is the
+default.
 
-## Other commands
+```bash
+elk elicit microsoft/deberta-v2-xxlarge-mnli imdb --net ccs
+```
 
-To only extract the hidden states for the model `model` and the dataset `dataset` and save them to `my_output_dir`, without training any reporters, you can run:
+The following command will evaluate the probe from the run naughty-northcutt on the hidden states extracted from the
+model deberta-v2-xxlarge-mnli for the imdb dataset. It will result in an `eval.csv` and `cfg.yaml` file, which are
+stored under a subfolder in `elk-reporters/naughty-northcutt/transfer_eval`.
 
 ```bash
-elk extract microsoft/deberta-v2-xxlarge-mnli imdb -o my_output_dir
+elk eval naughty-northcutt microsoft/deberta-v2-xxlarge-mnli imdb
 ```
 
-## Development
-To clone the repo and its submodules
+The following runs `elicit` on the Cartesian product of the listed models and datasets, storing it in a special folder
+ELK_DIR/sweeps/<memorable_name>. Moreover, `--add_pooled` adds an additional dataset that pools all of the datasets
+together. You can also add a `--visualize` flag to visualize the results of the sweep.
+
 ```bash
-git clone --recurse-submodules https://github.com/EleutherAI/elk.git
+elk sweep --models gpt2-{medium,large,xl} --datasets imdb amazon_polarity --add_pooled
 ```
-If you already cloned the repo but are missing the promptsource_module submodule, run
+
+If you just do `elk plot`, it will plot the results from the most recent sweep.
+If you want to plot a specific sweep, you can do so with:
+
 ```bash
-git submodule update --init --recursive
+elk plot {sweep_name}
 ```
 
+## Caching
+
+The hidden states resulting from `elk elicit` are cached as a HuggingFace dataset to avoid having to recompute them
+every time we want to train a probe. The cache is stored in the same place as all other HuggingFace datasets, which is
+usually `~/.cache/huggingface/datasets`.
+
+## Development
 
 Use `pip install pre-commit && pre-commit install` in the root folder before your first commit.
 
+### Devcontainer
+
+[
+![Open in Remote - Containers](
+https://img.shields.io/static/v1?label=Remote%20-%20Containers&message=Open&color=blue&logo=visualstudiocode
+)
+](
+https://vscode.dev/redirect?url=vscode://ms-vscode-remote.remote-containers/cloneInVolume?url=https://github.com/EleutherAI/elk
+)
+
 ### Run tests
+
 ```bash
 pytest
 ```
+
 ### Run type checking
-We use [pyright](https://github.com/microsoft/pyright), which is built into the VSCode editor. If you'd like to run it as a standalone tool, it requires a [nodejs installation.](https://nodejs.org/en/download/)
+
+We use [pyright](https://github.com/microsoft/pyright), which is built into the VSCode editor. If you'd like to run it
+as a standalone tool, it requires a [nodejs installation.](https://nodejs.org/en/download/)
+
 ```bash
 pyright
 ```
 
-If you work on a new feature / fix or some other code task, make sure to create an issue and assign it to yourself (Maybe, even share it in the elk channel of Eleuther's Discord with a small note). In this way, others know you are working on the issue and people won't do the same thing twice 👍 Also others can contact you easily.
+### Run the linter
+
+We use [ruff](https://beta.ruff.rs/docs/). It is installed as a pre-commit hook, so you don't have to run it manually.
+If you want to run it manually, you can do so with:
+
+```bash
+ruff . --fix
+```
+
+### Contributing to this repository
+
+If you work on a new feature / fix or some other code task, make sure to create an issue and assign it to yourself (
+Maybe, even share it in the elk channel of Eleuther's Discord with a small note). In this way, others know you are
+working on the issue and people won't do the same thing twice 👍 Also others can contact you easily.
```

### Comparing `eleuther-elk-0.1/elk/extraction/generator.py` & `eleuther-elk-0.1.1/elk/extraction/generator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,57 +1,87 @@
+from copy import deepcopy
 from dataclasses import dataclass, field
-from typing import Callable, Optional, Any, Dict
+from typing import Any, Callable
 
-import datasets
+from datasets import (
+    BuilderConfig,
+    DatasetInfo,
+    Features,
+    GeneratorBasedBuilder,
+    SplitInfo,
+)
 from datasets.splits import NamedSplit
 
 
 @dataclass
-class _GeneratorConfig(datasets.BuilderConfig):
-    generator: Optional[Callable] = None
+class _GeneratorConfig(BuilderConfig):
+    generator: Callable | None = None
     gen_kwargs: dict[str, Any] = field(default_factory=dict)
-    features: Optional[datasets.Features] = None
+    features: Features | None = None
+
+    def create_config_id(
+        self, config_kwargs: dict, custom_features: Features | None
+    ) -> str:
+        config_kwargs = deepcopy(config_kwargs)
+
+        # By default the values in gen_kwargs are lists of length world_size. We want
+        # to erase the world_size dimension so that the config id is the same no matter
+        # how many processes are used. We also remove the explicit device, rank, and
+        # world_size keys.
+        config_kwargs["gen_kwargs"] = {
+            k: v[0]
+            for k, v in config_kwargs.get("gen_kwargs", {}).items()
+            if k not in ("device", "rank", "world_size")
+        }
+        return super().create_config_id(config_kwargs, custom_features)
 
 
 @dataclass
 class _SplitGenerator:
     """
     datasets.SplitGenerator but use given `split_info` instead initializing a new one
     """
 
     name: str
-    split_info: datasets.SplitInfo
-    gen_kwargs: Dict = field(default_factory=dict)
+    split_info: SplitInfo
+    gen_kwargs: dict = field(default_factory=dict)
 
     def __post_init__(self):
         self.name = str(self.name)  # Make sure we convert NamedSplits in strings
         NamedSplit(self.name)  # check that it's a valid split name
 
 
-class _GeneratorBuilder(datasets.GeneratorBasedBuilder):
+class _GeneratorBuilder(GeneratorBasedBuilder):
     """Patched version of `datasets.Generator` allowing for splits besides `train`"""
 
     BUILDER_CONFIG_CLASS = _GeneratorConfig
     config: _GeneratorConfig
 
-    def __init__(self, split_name: str, split_info: datasets.SplitInfo, **kwargs):
+    def __init__(
+        self,
+        split_name: str,
+        split_info: SplitInfo,
+        **kwargs,
+    ):
         self.split_name = split_name
         self.split_info = split_info
 
         super().__init__(**kwargs)
 
     def _info(self):
-        return datasets.DatasetInfo(features=self.config.features)
+        # Use the same builder and config name as the original builder
+        return DatasetInfo(features=self.config.features)
 
     def _split_generators(self, dl_manager):
         return [
             _SplitGenerator(
                 name=self.split_name,
                 split_info=self.split_info,
                 gen_kwargs=self.config.gen_kwargs,
             )
         ]
 
     def _generate_examples(self, **gen_kwargs):
         assert self.config.generator is not None, "generator must be specified"
+
         for idx, ex in enumerate(self.config.generator(**gen_kwargs)):
             yield idx, ex
```

### Comparing `eleuther-elk-0.1/elk/math.py` & `eleuther-elk-0.1.1/elk/utils/math_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,47 @@
 import math
 import random
 
+import torch
+from torch import Tensor
+
+
+@torch.jit.script
+def batch_cov(x: Tensor) -> Tensor:
+    """Compute a batch of covariance matrices.
+
+    Args:
+        x: A tensor of shape [..., n, d].
+
+    Returns:
+        A tensor of shape [..., d, d].
+    """
+    x_ = x - x.mean(dim=-2, keepdim=True)
+    return x_.mT @ x_ / x_.shape[-2]
+
+
+@torch.jit.script
+def cov_mean_fused(x: Tensor) -> Tensor:
+    """Compute the mean of the covariance matrices of a batch of data matrices.
+
+    The computation is done in a memory-efficient way, without materializing all
+    the covariance matrices in VRAM.
+
+    Args:
+        x: A tensor of shape [batch, n, d].
+
+    Returns:
+        A tensor of shape [d, d].
+    """
+    b, n, d = x.shape
+
+    x_ = x - x.mean(dim=1, keepdim=True)
+    x_ = x_.reshape(-1, d)
+    return x_.mT @ x_ / (b * n)
+
 
 def stochastic_round_constrained(x: list[float], rng: random.Random) -> list[int]:
     """Stochastic rounding under integer constraints.
 
     Given a list of floats which sum to an integer, stochastically round each float to
     an integer while maintaining the same sum. The expectation of the rounded values
     should be (nearly?) equal to the original values.
```

### Comparing `eleuther-elk-0.1/elk/utils/gpu_utils.py` & `eleuther-elk-0.1.1/elk/utils/gpu_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,166 @@
 """Utilities that use PyNVML to get GPU usage info, and select GPUs accordingly."""
 
 import os
+import time
+import warnings
+from functools import cache
+
 import pynvml
 import torch
-import warnings
+
+from .typing import assert_type
 
 
-def select_usable_devices(max_gpus: int = -1, *, min_memory: int = 0) -> list[str]:
+# We cache the results primarily so that we don't display "Using N of M GPUs..."
+# multiple times during the same run. This does sort of assume that once we identify
+# a GPU as being available, it will remain available for the duration of the run.
+# This seems to be a reasonable assumption because PyTorch tends to hold onto VRAM
+# for later use once it's been allocated. Calling torch.cuda.empty_cache() might break
+# this assumption, but we never do that.
+@cache
+def select_usable_devices(
+    num_gpus: int = -1, *, min_memory: int | None = None
+) -> list[str]:
     """Select a set of devices that have at least `min_memory` bytes of free memory.
+    Blocks until at least `num_gpus` devices are available.
 
     When there are more than enough GPUs to satisfy the request, the GPUs with the
     most free memory will be selected. With default arguments, this function will
     simply return a list of all available GPU indices. A human-readable message will
     be printed to stdout indicating which GPUs were selected.
 
     This function uses the PyNVML library to get usage info. Unfortunately, PyNVML does
     not respect the `CUDA_VISIBLE_DEVICES` environment variable, while PyTorch does.
     Correctly converting PyNVML device indices to PyTorch indices is nontrivial and was
     only recently (commit `dc4f2af` on 9 Feb. 2023) implemented in PyTorch `master`. We
     can't depend on PyTorch nightly and we also don't want to copy-paste the code here.
 
-    For now, we simply return `list(range(max_gpus))` whenever `CUDA_VISIBLE_DEVICES`
+    For now, we simply return `list(range(num_gpus))` whenever `CUDA_VISIBLE_DEVICES`
     is set. Arguably this is expected behavior. If the user set `CUDA_VISIBLE_DEVICES`,
     they probably want to use all & only those GPUs.
 
     Args:
-        num_gpus: Maximum number of GPUs to select. If negative, all available GPUs
+        num_gpus: Number of GPUs to select. If negative, all available GPUs
             meeting the criteria will be selected.
         min_memory: Minimum amount of free memory (in bytes) required to select a GPU.
+            If None, `min_memory` is set to 90% of the per-GPU memory.
 
     Returns:
-        A list of suitable PyTorch device strings, in ascending numerical order.
+        A list of suitable PyTorch device strings, in ascending numerical order, with
+        exactly `num_gpus` elements.
 
     Raises:
-        ValueError: If `max_gpus` is greater than the number of visible GPUs.
+        ValueError: If `num_gpus` is greater than the number of visible GPUs.
     """
     # Trivial case: no GPUs requested or available
     num_visible = torch.cuda.device_count()
-    if max_gpus == 0 or num_visible == 0:
+    if num_gpus == 0 or num_visible == 0:
         return ["cpu"]
 
     # Sanity checks
-    if max_gpus > num_visible:
+    if num_gpus > num_visible:
         raise ValueError(
-            f"Requested {max_gpus} GPUs, but only {num_visible} are visible."
+            f"Requested {num_gpus} GPUs, but only {num_visible} are visible."
         )
-    elif max_gpus < 0:
-        max_gpus = num_visible
+    elif num_gpus < 0:
+        num_gpus = num_visible
 
     # No limits, so try to use all installed GPUs
-    if max_gpus == num_visible and min_memory <= 0:
+    if num_gpus == num_visible and min_memory == 0:
         print(f"Using all {num_visible} GPUs.")
-        return [f"cuda:{i}" for i in range(max_gpus)]
+        return [f"cuda:{i}" for i in range(num_gpus)]
 
     # The user set CUDA_VISIBLE_DEVICES and also requested a specific number of GPUs.
     # The environment variable takes precedence, so we'll just use all visible GPUs.
-    count_msg = "all" if max_gpus == num_visible else f"first {max_gpus}"
+    count_msg = "all" if num_gpus == num_visible else f"first {num_gpus}"
     if "CUDA_VISIBLE_DEVICES" in os.environ:
         warnings.warn(
             f"Smart GPU selection not supported when CUDA_VISIBLE_DEVICES is set. "
             f"Will use {count_msg} visible devices."
         )
-        return [f"cuda:{i}" for i in range(max_gpus)]
+        return [f"cuda:{i}" for i in range(num_gpus)]
 
-    # pynvml.nvmlInit() will raise if we're using non-NVIDIA GPUs
+    # Initialize PyNVML
     try:
         pynvml.nvmlInit()
     except pynvml.NVMLError:
         warnings.warn(
             f"Unable to initialize PyNVML; are you using non-NVIDIA GPUs? Will use "
             f"{count_msg} visible devices."
         )
-        return [f"cuda:{i}" for i in range(max_gpus)]
+        return [f"cuda:{i}" for i in range(num_gpus)]
 
     try:
         # PyNVML and PyTorch device indices should agree when CUDA_VISIBLE_DEVICES is
         # not set. We need them to agree so that the PyNVML indices match the PyTorch
         # indices, and we don't have to do any complex error-prone conversions.
         num_installed = pynvml.nvmlDeviceGetCount()
         assert num_installed == num_visible, "PyNVML and PyTorch disagree on GPU count"
 
-        # List of (-free memory, GPU index) tuples. Sorted descending by free memory,
-        # then ascending by GPU index.
-        memories_and_indices = sorted(
-            (
-                -int(pynvml.nvmlDeviceGetMemoryInfo(handle).free),
-                pynvml.nvmlDeviceGetIndex(handle),
+        # Set default value for `min_memory`
+        if min_memory is None:
+            min_device_ram = min(
+                (
+                    assert_type(
+                        int,
+                        pynvml.nvmlDeviceGetMemoryInfo(
+                            pynvml.nvmlDeviceGetHandleByIndex(idx)
+                        ).total,
+                    )
+                    for idx in range(num_installed)
+                )
             )
-            for handle in map(pynvml.nvmlDeviceGetHandleByIndex, range(num_installed))
-        )
-        usable_indices = [
-            index for neg_mem, index in memories_and_indices if -neg_mem >= min_memory
-        ]
+            min_memory = int(0.9 * min_device_ram)
+
+        # Get free memory for each GPU
+        num_tries = 0
+        while True:
+            # check if at least `num_gpus` GPUs have at least `min_memory`
+            # bytes of free memory
+
+            try:
+                # List of (-free memory, GPU index) tuples. Sorted descending by
+                # free memory, then ascending by GPU index.
+                memories_and_indices = sorted(
+                    (
+                        -int(pynvml.nvmlDeviceGetMemoryInfo(handle).free),
+                        pynvml.nvmlDeviceGetIndex(handle),
+                    )
+                    for handle in map(
+                        pynvml.nvmlDeviceGetHandleByIndex, range(num_installed)
+                    )
+                )
+                usable_indices = [
+                    index
+                    for neg_mem, index in memories_and_indices
+                    if -neg_mem >= min_memory
+                ]
+                if len(usable_indices) >= num_gpus:
+                    break
+                elif num_tries % 60 == 0:  # Print every 10 minutes
+                    print(
+                        f"Waiting for {num_gpus} GPUs with "
+                        f"at least {min_memory / 10 ** 9:.2f} GB "
+                        f"of free memory. {len(usable_indices)} GPUs "
+                        "currently available."
+                    )
+            except Exception as e:
+                warnings.warn(
+                    f"Unable to query GPU memory: {e}. Will try again in 10 seconds."
+                )
+
+            # Wait a bit before trying again
+            time.sleep(10)
+            num_tries += 1
     finally:
-        # Make sure we always shut down PyNVML
+        # make sure to shut down PyNVML
         pynvml.nvmlShutdown()
 
-    # Indices are sorted descending by free memory, so we want the first `max_gpus`
+    # Indices are sorted descending by free memory, so we want the first `num_gpus`
     # items. For printing purposes, though, we sort the indices numerically.
-    selection = sorted(usable_indices[:max_gpus])
+    selection = sorted(usable_indices[:num_gpus])
 
-    # Did we get the maximum number of GPUs requested?
-    if len(selection) == max_gpus:
-        print(f"Using {len(selection)} of {num_visible} GPUs: {selection}")
-    else:
-        print(f"Using {len(selection)} of {max_gpus} requested GPUs: {selection}")
-        print(
-            f"{num_visible - len(selection)} GPUs have insufficient free memory "
-            f"({min_memory / 10 ** 9:.2f} GB needed)."
-        )
+    assert len(selection) == num_gpus
+    print(f"Using {len(selection)} of {num_visible} GPUs: {selection}")
 
-    if len(selection) > 0:
-        return [f"cuda:{i}" for i in selection]
-    else:
-        return ["cpu"]
+    return [f"cuda:{i}" for i in selection]
```

### Comparing `eleuther-elk-0.1/elk/utils/tree_utils.py` & `eleuther-elk-0.1.1/elk/utils/tree_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 In JAX, "pytrees" are nested collections (lists, tuples, dicts) of tensors which can be
 mapped over. See <https://jax.readthedocs.io/en/latest/pytrees.html>.
 """
 
 from typing import Callable, Mapping, TypeVar
 
-
 TreeType = TypeVar("TreeType")
 
 
 def pytree_map(func: Callable, tree: TreeType) -> TreeType:
     """
     Recursively apply a function to all objects in a pytree, returning the results
     in a new pytree with the same structure.
```

### Comparing `eleuther-elk-0.1/tests/test_math.py` & `eleuther-elk-0.1.1/tests/test_math.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-from elk.math import stochastic_round_constrained
-from hypothesis import given, strategies as st
-from random import Random
 import math
+from random import Random
+
 import numpy as np
-import pytest
+import torch
+from hypothesis import given
+from hypothesis import strategies as st
+
+from elk.utils import batch_cov, cov_mean_fused, stochastic_round_constrained
+
+
+def test_cov_mean_fused():
+    X = torch.randn(10, 500, 100, dtype=torch.float64)
+    cov_gt = batch_cov(X).mean(dim=0)
+    cov_fused = cov_mean_fused(X)
+    assert torch.allclose(cov_gt, cov_fused)
 
 
 @given(
     # Let Hypothesis generate the number of floats...
     st.integers(min_value=1, max_value=100),
     # ...and the total sum of the floats
     st.integers(min_value=1, max_value=int(np.finfo(np.float32).max)),
 )
-@pytest.mark.cpu
 def test_stochastic_rounding(num_parts: int, total: int):
     # Randomly sample the breakdown of the total into floats
     rng = np.random.default_rng(42)
     x = rng.dirichlet(np.ones(num_parts), size=1) * total
 
     # Stochastically round the floats
     rounded = stochastic_round_constrained(x[0].tolist(), Random(42))
```

