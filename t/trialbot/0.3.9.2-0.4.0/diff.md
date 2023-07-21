# Comparing `tmp/trialbot-0.3.9.2.tar.gz` & `tmp/trialbot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trialbot-0.3.9.2.tar", last modified: Fri Nov  4 13:11:01 2022, max compression
+gzip compressed data, was "trialbot-0.4.0.tar", last modified: Fri Jul 21 13:58:02 2023, max compression
```

## Comparing `trialbot-0.3.9.2.tar` & `trialbot-0.4.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.502401 trialbot-0.3.9.2/
--rw-r--r--   0 zxarukas   (501) staff       (20)      526 2022-11-04 13:11:01.501751 trialbot-0.3.9.2/PKG-INFO
--rw-r--r--   0 zxarukas   (501) staff       (20)       69 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/README.md
--rw-r--r--   0 zxarukas   (501) staff       (20)       38 2022-11-04 13:11:01.502592 trialbot-0.3.9.2/setup.cfg
--rw-r--r--   0 zxarukas   (501) staff       (20)      652 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/setup.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.486135 trialbot-0.3.9.2/trialbot/
--rw-r--r--   0 zxarukas   (501) staff       (20)       48 2022-11-04 13:10:37.000000 trialbot-0.3.9.2/trialbot/__init__.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.489961 trialbot-0.3.9.2/trialbot/data/
--rw-r--r--   0 zxarukas   (501) staff       (20)     1229 2021-08-05 08:16:04.000000 trialbot-0.3.9.2/trialbot/data/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      564 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/_translation_base.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     4030 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/dataset.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.493733 trialbot-0.3.9.2/trialbot/data/datasets/
--rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      539 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/consecutive_lines_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1015 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/file_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      357 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/index_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      223 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/json_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      205 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/jsonl_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2244 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/pickle_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1821 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/redis_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      436 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/seq2dict_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      246 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/tabular_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      908 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/datasets/tsv_dataset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      880 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/field.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.494389 trialbot-0.3.9.2/trialbot/data/fields/
--rw-r--r--   0 zxarukas   (501) staff       (20)       31 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/fields/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2889 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/fields/seq_field.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3246 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterator.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.495618 trialbot-0.3.9.2/trialbot/data/iterators/
--rw-r--r--   0 zxarukas   (501) staff       (20)      134 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterators/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3367 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterators/bucket_iterator.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1354 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/iterators/cluster_iterator.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3580 2021-06-25 08:26:10.000000 trialbot-0.3.9.2/trialbot/data/iterators/random_iterator.py
--rw-r--r--   0 zxarukas   (501) staff       (20)    28102 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/data/ns_vocabulary.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2328 2021-08-05 07:16:06.000000 trialbot-0.3.9.2/trialbot/data/translator.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.496203 trialbot-0.3.9.2/trialbot/data/translators/
--rw-r--r--   0 zxarukas   (501) staff       (20)       56 2021-08-05 08:16:04.000000 trialbot-0.3.9.2/trialbot/data/translators/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2029 2021-08-05 08:20:44.000000 trialbot-0.3.9.2/trialbot/data/translators/known_field_translator.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.498258 trialbot-0.3.9.2/trialbot/training/
--rw-r--r--   0 zxarukas   (501) staff       (20)      265 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     8700 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/event_engine.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     2478 2022-11-04 13:10:37.000000 trialbot-0.3.9.2/trialbot/training/extensions.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1199 2021-11-10 05:47:23.000000 trialbot-0.3.9.2/trialbot/training/hparamset.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1195 2021-11-08 13:15:31.000000 trialbot-0.3.9.2/trialbot/training/opt_parser.py
--rw-r--r--   0 zxarukas   (501) staff       (20)    13697 2022-11-04 09:30:54.000000 trialbot-0.3.9.2/trialbot/training/trial_bot.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1724 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/trial_registry.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1815 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/updater.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.498973 trialbot-0.3.9.2/trialbot/training/updaters/
--rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/training/updaters/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1689 2021-11-08 13:15:31.000000 trialbot-0.3.9.2/trialbot/training/updaters/testing_updater.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     3154 2021-11-10 05:47:23.000000 trialbot-0.3.9.2/trialbot/training/updaters/training_updater.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.500786 trialbot-0.3.9.2/trialbot/utils/
--rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/__init__.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1075 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/file_reader.py
--rw-r--r--   0 zxarukas   (501) staff       (20)      256 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/fix_seed.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1737 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/grid_search_helper.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1180 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/move_to_device.py
--rw-r--r--   0 zxarukas   (501) staff       (20)     1119 2021-06-24 13:24:41.000000 trialbot-0.3.9.2/trialbot/utils/root_finder.py
-drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2022-11-04 13:11:01.487753 trialbot-0.3.9.2/trialbot.egg-info/
--rw-r--r--   0 zxarukas   (501) staff       (20)      526 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/PKG-INFO
--rw-r--r--   0 zxarukas   (501) staff       (20)     1704 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/SOURCES.txt
--rw-r--r--   0 zxarukas   (501) staff       (20)        1 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/dependency_links.txt
--rw-r--r--   0 zxarukas   (501) staff       (20)        9 2022-11-04 13:11:01.000000 trialbot-0.3.9.2/trialbot.egg-info/top_level.txt
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.749002 trialbot-0.4.0/
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1065 2021-06-24 13:24:41.000000 trialbot-0.4.0/LICENSE
+-rw-r--r--   0 zxarukas   (501) staff       (20)      482 2023-07-21 13:58:02.748747 trialbot-0.4.0/PKG-INFO
+-rw-r--r--   0 zxarukas   (501) staff       (20)       69 2021-06-24 13:24:41.000000 trialbot-0.4.0/README.md
+-rw-r--r--   0 zxarukas   (501) staff       (20)       38 2023-07-21 13:58:02.749076 trialbot-0.4.0/setup.cfg
+-rw-r--r--   0 zxarukas   (501) staff       (20)      652 2021-06-24 13:24:41.000000 trialbot-0.4.0/setup.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.721716 trialbot-0.4.0/trialbot/
+-rw-r--r--   0 zxarukas   (501) staff       (20)       46 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/__init__.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.727529 trialbot-0.4.0/trialbot/data/
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1229 2021-08-05 08:16:04.000000 trialbot-0.4.0/trialbot/data/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      911 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/data/_translation_base.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     4030 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/dataset.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.732289 trialbot-0.4.0/trialbot/data/datasets/
+-rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      539 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/consecutive_lines_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1015 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/file_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      334 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/data/datasets/index_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      223 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/json_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      205 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/jsonl_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2238 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/data/datasets/pickle_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1821 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/redis_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      414 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/data/datasets/seq2dict_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      246 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/tabular_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      908 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/datasets/tsv_dataset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      987 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/data/field.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.733031 trialbot-0.4.0/trialbot/data/fields/
+-rw-r--r--   0 zxarukas   (501) staff       (20)       31 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/fields/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2781 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/data/fields/seq_field.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3256 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/data/iterator.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.737923 trialbot-0.4.0/trialbot/data/iterators/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      134 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/iterators/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3367 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/iterators/bucket_iterator.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1354 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/data/iterators/cluster_iterator.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3580 2021-06-25 08:26:10.000000 trialbot-0.4.0/trialbot/data/iterators/random_iterator.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)    28103 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/data/ns_vocabulary.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2499 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/data/translator.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.739081 trialbot-0.4.0/trialbot/data/translators/
+-rw-r--r--   0 zxarukas   (501) staff       (20)       56 2021-08-05 08:16:04.000000 trialbot-0.4.0/trialbot/data/translators/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1972 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/data/translators/known_field_translator.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.744342 trialbot-0.4.0/trialbot/training/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      265 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/training/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     8700 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/training/event_engine.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2717 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/training/extensions.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1013 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/training/hparamset.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1195 2021-11-08 13:15:31.000000 trialbot-0.4.0/trialbot/training/opt_parser.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      992 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/training/select_optims.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)    14304 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/training/trial_bot.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1727 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/training/trial_registry.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     2290 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/training/updater.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.745636 trialbot-0.4.0/trialbot/training/updaters/
+-rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/training/updaters/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1209 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/training/updaters/testing_updater.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     3254 2023-07-21 13:57:44.000000 trialbot-0.4.0/trialbot/training/updaters/training_updater.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.748185 trialbot-0.4.0/trialbot/utils/
+-rw-r--r--   0 zxarukas   (501) staff       (20)        0 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/utils/__init__.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1075 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/utils/file_reader.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      258 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/utils/fix_seed.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1719 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/utils/grid_search_helper.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1180 2021-06-24 13:24:41.000000 trialbot-0.4.0/trialbot/utils/move_to_device.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)      805 2023-07-11 08:54:10.000000 trialbot-0.4.0/trialbot/utils/prepend_pythonpath.py
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1112 2023-07-21 13:57:43.000000 trialbot-0.4.0/trialbot/utils/root_finder.py
+drwxr-xr-x   0 zxarukas   (501) staff       (20)        0 2023-07-21 13:58:02.723276 trialbot-0.4.0/trialbot.egg-info/
+-rw-r--r--   0 zxarukas   (501) staff       (20)      482 2023-07-21 13:58:02.000000 trialbot-0.4.0/trialbot.egg-info/PKG-INFO
+-rw-r--r--   0 zxarukas   (501) staff       (20)     1784 2023-07-21 13:58:02.000000 trialbot-0.4.0/trialbot.egg-info/SOURCES.txt
+-rw-r--r--   0 zxarukas   (501) staff       (20)        1 2023-07-21 13:58:02.000000 trialbot-0.4.0/trialbot.egg-info/dependency_links.txt
+-rw-r--r--   0 zxarukas   (501) staff       (20)        9 2023-07-21 13:58:02.000000 trialbot-0.4.0/trialbot.egg-info/top_level.txt
```

### Comparing `trialbot-0.3.9.2/setup.py` & `trialbot-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/__init__.py` & `trialbot-0.4.0/trialbot/data/__init__.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/dataset.py` & `trialbot-0.4.0/trialbot/data/dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/datasets/consecutive_lines_dataset.py` & `trialbot-0.4.0/trialbot/data/datasets/consecutive_lines_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/datasets/file_dataset.py` & `trialbot-0.4.0/trialbot/data/datasets/file_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/datasets/pickle_dataset.py` & `trialbot-0.4.0/trialbot/data/datasets/pickle_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Optional, Tuple
+from typing import Optional
 import pickle
 import logging
 from datetime import datetime as dt
 import redis
 
 from trialbot.data.dataset import Dataset
 
+
 class PickleDataset(Dataset):
     def __init__(self,
                  filename: str,
-                 conn: Optional[Tuple[str, int, int]] = None,
+                 conn: Optional[tuple[str, int, int]] = None,
                  prefix: str = None,
                  ignore_missing_data: bool = True,
                  ):
         super().__init__()
         self.filename = filename
 
         self.r = None
```

### Comparing `trialbot-0.3.9.2/trialbot/data/datasets/redis_dataset.py` & `trialbot-0.4.0/trialbot/data/datasets/redis_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/datasets/tsv_dataset.py` & `trialbot-0.4.0/trialbot/data/datasets/tsv_dataset.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/field.py` & `trialbot-0.4.0/trialbot/data/field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from typing import List, Mapping, Optional
+from abc import ABC
+
 import torch
-from ._translation_base import _TranslationBase, NullableTensor
+from ._translation_base import _TranslationBase, T
+
 
-class Field(_TranslationBase):
+class Field(_TranslationBase, ABC):
     """
     A field is not actually a translator, this is experimental
     and will later be refactored to inherit from another interface.
     """
-    def batch_tensor_by_key(self,
-                            tensors_by_keys: Mapping[str, List[NullableTensor]]
-                            ) -> Mapping[str, torch.Tensor]:
+    def build_batch_by_key(self, input_dict: dict[str, list[T]]) -> dict[str, torch.Tensor | list[T]]:
         """
         A normal translator accept a batch of tensors,
         which is an iterable collection containing the instances from Translator.to_tensor interface.
         A field will handle the tensor list by some predefined key,
         but will accept all the possible tensors batch dict by the keys.
-        :param tensors_by_keys:
-        :return:
+        :param input_dict:
+        :return: a dict mapping string keys to values that can be either
+                - a tensor representing a feature of the batch,
+                - a list of something that ignored by the translator but usable to the model.
         """
         raise NotImplementedError
-
```

### Comparing `trialbot-0.3.9.2/trialbot/data/fields/seq_field.py` & `trialbot-0.4.0/trialbot/data/fields/seq_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from typing import List, Mapping, Generator, Tuple, Optional, Any, Literal
-from ..field import Field, NullableTensor
+from typing import Any
+from ..field import Field, T
+from collections.abc import Iterator
 import torch
-from trialbot.data import START_SYMBOL, END_SYMBOL, PADDING_TOKEN, NSVocabulary
+from trialbot.data import START_SYMBOL, END_SYMBOL
 from itertools import product
 from torch.nn.utils.rnn import pad_sequence
 
+
 class SeqField(Field):
     def get_sent(self, example):
         return example.get(self.source_key)
 
-    def generate_namespace_tokens(self, example) -> Generator[Tuple[str, str], None, None]:
+    def generate_namespace_tokens(self, example: Any) -> Iterator[tuple[str, str]]:
         if self.add_start_end_toks:
             yield from product([self.ns], [START_SYMBOL, END_SYMBOL])
 
         seq_raw = self.get_sent(example)
         if seq_raw is not None:
-            yield from product([self.ns], (x.lower() if self.lower_case else x for x in self.split(seq_raw)))
+            yield from product([self.ns], (x.lower() if self.lower_case else x
+                                           for x in self.split(seq_raw)))
 
-    def to_tensor(self, example) -> Mapping[str, NullableTensor]:
+    def to_input(self, example) -> dict[str, T | None]:
         seq_raw = self.get_sent(example)
         if seq_raw is None:
             return {self.renamed_key: torch.tensor([self.padding])}
 
         seq_toks = self.split(seq_raw)
         if len(seq_toks) == 0:
             return {self.renamed_key: torch.tensor([self.padding])}
@@ -35,18 +38,16 @@
         if self.add_start_end_toks:
             seq_toks = [START_SYMBOL] + seq_toks + [END_SYMBOL]
 
         seq_toks = [self.vocab.get_token_index(tok, self.ns) for tok in seq_toks]
         seq_tensor = torch.tensor(seq_toks)
         return {self.renamed_key: seq_tensor}
 
-    def batch_tensor_by_key(self,
-                            tensors_by_keys: Mapping[str, List[NullableTensor]]
-                            ) -> Mapping[str, torch.Tensor]:
-        tensor_list = tensors_by_keys.get(self.renamed_key)
+    def build_batch_by_key(self, input_dict: dict[str, list[T]]) -> dict[str, torch.Tensor | list[T]]:
+        tensor_list = input_dict.get(self.renamed_key)
         if tensor_list is None or len(tensor_list) == 0:
             raise KeyError(f'Empty field key {self.renamed_key} confronted. Failed to build the instance tensors')
 
         batch_tensor = pad_sequence(tensor_list, batch_first=True, padding_value=self.padding)
         return {self.renamed_key: batch_tensor}
 
     def __init__(self, source_key: str,
```

### Comparing `trialbot-0.3.9.2/trialbot/data/iterator.py` & `trialbot-0.4.0/trialbot/data/iterator.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 #
-from typing import Sequence
+from collections.abc import Sequence
+
 
 class Iterator(object):
     """Base class of all dataset iterators.
 
     Iterator iterates over the dataset, yielding a sequence of indices at each iteration.
     The indices sequence usually indicates a list of examples of a minibatch.
     Each implementation should implement an iterator protocol (e.g., the :meth:`__next__` method).
```

### Comparing `trialbot-0.3.9.2/trialbot/data/iterators/bucket_iterator.py` & `trialbot-0.4.0/trialbot/data/iterators/bucket_iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/iterators/cluster_iterator.py` & `trialbot-0.4.0/trialbot/data/iterators/cluster_iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/iterators/random_iterator.py` & `trialbot-0.4.0/trialbot/data/iterators/random_iterator.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/data/ns_vocabulary.py` & `trialbot-0.4.0/trialbot/data/ns_vocabulary.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 DEFAULT_NON_PADDED_NAMESPACES = ("*tags", "*labels")
 DEFAULT_OOV_TOKEN = "@@UNKNOWN@@"
 NAMESPACE_PADDING_FILE = 'non_padded_namespaces.txt'
 PADDING_TOKEN = "@@PADDING@@"
 START_SYMBOL = '@start@'
 END_SYMBOL = '@end@'
 
+
 class _NamespaceDependentDefaultDict(defaultdict):
     """
     This is a `defaultdict
     <https://docs.python.org/2/library/collections.html#collections.defaultdict>`_ where the
     default value is dependent on the key that is passed.
 
     We use "namespaces" in the :class:`Vocabulary` object to keep track of several different
```

### Comparing `trialbot-0.3.9.2/trialbot/data/translators/known_field_translator.py` & `trialbot-0.4.0/trialbot/data/translators/known_field_translator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Mapping, Set, Optional, List, Any
-from ..translator import FieldAwareTranslator, NullableTensor
+from ..translator import FieldAwareTranslator, T
+import torch
 
 
 class _DictKeyRefWrapper(dict):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ref_set = set()
 
@@ -21,34 +21,34 @@
     """
     A Translator aware of fields,
     not only translates known keys of an instance into the tensors as the specified fields,
     but collects other unknown field of an instance and arrange them into an array.
     """
     def __init__(self, accessed_field_set=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._accessed_field_set: Optional[Set] = accessed_field_set
+        self._accessed_field_set: set | None = accessed_field_set
 
-    def to_tensor(self, example) -> Mapping[str, NullableTensor]:
+    def to_input(self, example) -> dict[str, T | None]:
         output = {}
         if self._accessed_field_set is None:
             example = _DictKeyRefWrapper(example)
-            output.update(super().to_tensor(example))
+            output.update(super().to_input(example))
             self._accessed_field_set = set(example.ref_set)
         else:
-            output.update(super().to_tensor(example))
+            output.update(super().to_input(example))
 
         for field in filter(lambda k: k not in self._accessed_field_set, example.keys()):
             output[field] = example[field]
 
         return output
 
-    def batch_tensor(self, tensors: List[Mapping[str, NullableTensor]]) -> Mapping[str, Any]:
+    def build_batch(self, input_list: list[dict[str, T | None]]) -> dict[str, torch.Tensor | list[T]]:
         processed_fields = self._accessed_field_set or set()
-        tensors = list(filter(lambda x: all(v is not None for v in x.values()), tensors))
+        tensors = list(filter(lambda x: all(v is not None for v in x.values()), input_list))
         batch_dict = self.list_of_dict_to_dict_of_list(tensors)
         output = {}
         for field in self.fields:
-            output.update(field.batch_tensor_by_key(batch_dict))
+            output.update(field.build_batch_by_key(batch_dict))
         for k, v in batch_dict.items():
             if k not in processed_fields and k not in output.keys():
                 output[k] = v
         return output
```

### Comparing `trialbot-0.3.9.2/trialbot/training/event_engine.py` & `trialbot-0.4.0/trialbot/training/event_engine.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/training/extensions.py` & `trialbot-0.4.0/trialbot/training/extensions.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,41 +46,47 @@
 
 
 def print_hyperparameters(bot):
     bot.logger.info(f"Cmd Arguments Used:\n{bot.args}")
     bot.logger.info(f"Hyperparamset Used: {bot.args.hparamset}\n{str(bot.hparams)}")
 
 
-def print_snaptshot_path(bot):
-    bot.logger.info("Snapshot Dir: " + bot.savepath)
+def print_snaptshot_path(bot, use_absolute_path: bool = True):
+    path = bot.savepath
+    if use_absolute_path:
+        path = os.path.abspath(path)
+    bot.logger.info("Snapshot Dir: " + path)
 
 
 def print_models(bot):
     bot.logger.info("Model Specs:\n" + str(bot.models))
 
 
 def collect_garbage(bot):
     import gc
-    for optim in bot.updater._optims:
-        optim.zero_grad()
+    from .updaters.training_updater import TrainingUpdater
+    if isinstance(bot.updater, TrainingUpdater):
+        bot.updater.optim.zero_grad()
 
     if hasattr(bot.state, "output") and bot.state.output is not None:
         bot.state.output = None
     gc.collect()
     if bot.args.device >= 0:
         import torch.cuda
         torch.cuda.empty_cache()
 
 
 def end_with_nan_loss(bot):
     import numpy as np
     output = getattr(bot.state, 'output', None)
     if output is None:
         return
-    loss = output["loss"]
+    loss = output.get('loss', None)
+    if loss is None:
+        return
 
     def _isnan(x):
         if isinstance(x, torch.Tensor):
             return bool(torch.isnan(x).any())
         elif isinstance(x, np.ndarray):
             return bool(np.isnan(x).any())
         else:
```

### Comparing `trialbot-0.3.9.2/trialbot/training/opt_parser.py` & `trialbot-0.4.0/trialbot/training/opt_parser.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/training/trial_bot.py` & `trialbot-0.4.0/trialbot/training/trial_bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from typing import Callable, Optional, Dict, Any
+import argparse
+from typing import Callable, Optional, Any
 import torch.nn
 import os.path
-import json
 from datetime import datetime
 
 from trialbot.data.dataset import Dataset
 from trialbot.data.ns_vocabulary import NSVocabulary
 from tqdm import tqdm
 from enum import Enum
 
@@ -14,30 +14,33 @@
 from .opt_parser import get_trial_bot_common_opt_parser
 from .trial_registry import Registry
 from .event_engine import Engine
 from . import extensions as exts
 import logging
 logging.basicConfig()
 
+
 class Events(Enum):
     """Predefined events for TrialBot training."""
     EPOCH_STARTED = "epoch_started"
     EPOCH_COMPLETED = "epoch_completed"
     STARTED = "started"
     COMPLETED = "completed"
     ITERATION_STARTED = "iteration_started"
     ITERATION_COMPLETED = "iteration_completed"
     EXCEPTION_RAISED = "exception_raised"
 
+
 class State(object):
     """An object that is used to pass internal and user-defined state between event handlers."""
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
+
 class TrialBot:
     """
     A TrialBot is the direct manager for an experiment, which is responsible for only two requirements,
     Run and Serve, corresponding to run the experiment or to get loaded by some server.
 
     A TrialBot maintains several Components, and schedules the experiment procedure.
     Components are as follows so far,
@@ -66,16 +69,16 @@
        to the engine for some specific events and get run by the event engine when the very event is
        fired.
        By default, the loop contains some epochs and some iterations of each epoch.
        The loop relies on the updater, and start a new epoch only after the updater raise an StopIteration exception.
 
     """
     def __init__(self,
-                 args = None,
-                 trial_name="default_savedir",
+                 args: argparse.Namespace | None = None,
+                 trial_name: str = "default_savedir",
                  get_model_func: Optional[Callable[[Any, NSVocabulary], torch.nn.Module]] = None,
                  clean_engine: bool = False,
                  ):
         if args is None:
             parser = TrialBot.get_default_parser()
             args = parser.parse_args()
 
@@ -126,17 +129,15 @@
     def model(self):
         return self.models[0]
 
     @staticmethod
     def get_default_parser():
         parser = get_trial_bot_common_opt_parser()
         parser.add_argument('models', nargs='*', help='pretrained models for the same setting')
-        parser.add_argument('--dry-run', action="store_true")
-        parser.add_argument('--skip', type=int, help='skip NUM examples for the first iteration, intended for debug use.')
-        parser.add_argument('--vocab-dump', help="the file path to save and load the vocab obj")
+        parser.add_argument('--vocab-path', help="the file path to save and load the vocab obj")
 
         parser.add_argument('--batch-size', type=int, default=0,
                             help='overwrite the hparamset.batch_sz if specified at CLI')
         parser.add_argument('--epoch', type=int, default=0,
                             help='overwrite the hparamset.TRAINING_LIMIT if specified at CLI')
         return parser
 
@@ -155,37 +156,48 @@
             self.logger.setLevel(logging.INFO)
 
         hparams = Registry.get_hparamset(args.hparamset)
         if args.batch_size > 0:
             hparams.batch_sz = args.batch_size
         if args.epoch > 0:
             hparams.TRAINING_LIMIT = args.epoch
+        if args.translator:
+            hparams.TRANSLATOR = args.translator
 
         self.hparams = hparams
-        savepath = args.snapshot_dir if args.snapshot_dir else (os.path.join(
-            hparams.SNAPSHOT_PATH,
-            args.dataset,
-            self.name,
-            datetime.now().strftime('%Y%m%d-%H%M%S') + ('-' + args.memo if args.memo else '')
-        ))
-        self.savepath = savepath
+        self.savepath = args.snapshot_dir if args.snapshot_dir else self._default_savepath()
 
         self._init_dataset()
         self._init_translator()
 
         self.vocab = self._init_vocab(self.train_set, self.translator)
 
         self.translator.index_with_vocab(self.vocab)
         self.models = self._init_models(hparams, self.vocab)
 
     def _init_dataset(self):
         args = self.args
         self.datasets = Registry.get_dataset(args.dataset)
         return self.datasets
 
+    def _default_savepath(self):
+        args = self.args
+
+        if args.test and len(args.models) > 0:
+            # use the first model path as the savepath,
+            # if this is not expected, please specify manually the
+            return os.path.abspath(os.path.expanduser(os.path.dirname(args.models[0])))
+
+        return os.path.join(
+            self.hparams.SNAPSHOT_PATH,
+            args.dataset,
+            self.name,
+            datetime.now().strftime('%Y%m%d-%H%M%S') + ('-' + args.memo if args.memo else '')
+        )
+
     @property
     def train_set(self):
         return self._get_classical_dataset_split(0)
 
     @property
     def dev_set(self):
         return self._get_classical_dataset_split(1)
@@ -195,63 +207,78 @@
         return self._get_classical_dataset_split(2)
 
     def _get_classical_dataset_split(self, i):
         assert len(self.datasets) >= 3 and all(isinstance(x, Dataset) for x in self.datasets[:3])
         return self.datasets[i]
 
     def _init_translator(self):
-        args, p = self.args, self.hparams
+        p = self.hparams
         translator_kwargs = getattr(p, 'TRANSLATOR_KWARGS', dict())
-        translator = Registry.get_translator(args.translator, **translator_kwargs)
+        translator = Registry.get_translator(p.TRANSLATOR, **translator_kwargs)
         self.translator = translator
         return translator
 
     def _init_vocab(self,
                     dataset: Dataset,
                     translator: Translator):
         args, logger = self.args, self.logger
         hparams = self.hparams
 
-        if args.vocab_dump and os.path.exists(args.vocab_dump):
-            logger.info(f"read vocab from file {args.vocab_dump}")
-            vocab = NSVocabulary.from_files(args.vocab_dump)
+        if args.vocab_path:
+            vocab_path = args.vocab_path
+        else:
+            vocab_path = os.path.join(self.savepath, 'vocab')
+            logger.info(f'assuming the vocab is located at {vocab_path}')
+
+        if os.path.exists(vocab_path):
+            logger.info(f"read vocab from file {vocab_path}")
+            vocab = NSVocabulary.from_files(vocab_path)
 
         else:
             logger.info("initialize vocab from training data")
             # count for a counter
-            logger.debug("start initializing vocab")
-            counter: Dict[str, Dict[str, int]] = dict()
+            counter: dict[str, dict[str, int]] = dict()
             for example in tqdm(iter(dataset)):
                 for namespace, w in translator.generate_namespace_tokens(example):
                     if namespace not in counter:
                         counter[namespace] = dict()
 
                     if w not in counter[namespace]:
                         counter[namespace][w] = 0
 
                     counter[namespace][w] += 1
 
             vocab = NSVocabulary(counter, **hparams.NS_VOCAB_KWARGS)
 
-        if args.vocab_dump:
-            os.makedirs(args.vocab_dump, exist_ok=True)
-            vocab.save_to_files(args.vocab_dump)
+            if args.test:
+                logger.warning(f'the vocab is not saved by default in eval mode '
+                               f'although it is just built from scratch.')
+            else:
+                vocab.save_to_files(vocab_path)
+
         logger.info(str(vocab))
 
         return vocab
 
     def _init_models(self, hparams, vocab):
         args = self.args
         models = self.get_model(hparams, vocab)
         if not isinstance(models, list) and not isinstance(models, tuple):
             models = [models]
 
         if args.models:
+            def int_to_device(device):
+                if isinstance(device, torch.device):
+                    return device
+                if device < 0:
+                    return torch.device("cpu")
+                return torch.device(device)
+
             for model, model_path in zip(models, args.models):
-                model.load_state_dict(torch.load(model_path))
+                model.load_state_dict(torch.load(model_path, map_location=int_to_device(args.device)))
 
         if args.device >= 0:
             models = [model.cuda(args.device) for model in models]
         return models
 
     def run(self, training_epoch: int = 0):
         if training_epoch == 0:
@@ -263,22 +290,18 @@
             if self.updater is None:
                 from .updaters.testing_updater import TestingUpdater
                 self.updater = TestingUpdater.from_bot(self)
             self._testing_engine_loop(self.updater)
 
         else:
             # training procedure
-            # 1. save vocab; 2. init updater; 3. start main engine
+            # 1. ensure snapshot-dir (savepath); 2. init updater; 3. start main engine
             savepath = self.savepath
             if not os.path.exists(savepath):
                 os.makedirs(savepath, mode=0o755)
-            vocab_path = os.path.join(savepath, 'vocab')
-            if not os.path.exists(vocab_path):
-                os.makedirs(vocab_path, mode=0o755)
-                self.vocab.save_to_files(vocab_path)
 
             if self.updater is None:
                 from .updaters.training_updater import TrainingUpdater
                 self.updater = TrainingUpdater.from_bot(self)
             self._training_engine_loop(self.updater, training_epoch)
 
     def _training_engine_loop(self, updater, max_epoch):
@@ -289,20 +312,19 @@
             engine.fire_event(Events.EPOCH_STARTED, bot=self)
             updater.start_epoch()
             while True:
                 self.state.iteration += 1
                 engine.fire_event(Events.ITERATION_STARTED, bot=self)
                 try:
                     self.state.output = next(updater)
+                    engine.fire_event(Events.ITERATION_COMPLETED, bot=self)
                 except StopIteration:
                     self.state.iteration -= 1
                     self.state.output = None
                     break
-                finally:
-                    engine.fire_event(Events.ITERATION_COMPLETED, bot=self)
 
             engine.fire_event(Events.EPOCH_COMPLETED, bot=self)
         engine.fire_event(Events.COMPLETED, bot=self)
 
     def _testing_engine_loop(self, updater):
         engine = self._engine
         with torch.no_grad():
@@ -310,29 +332,28 @@
             engine.fire_event(Events.EPOCH_STARTED, bot=self)
             updater.start_epoch()
             while True:
                 self.state.iteration += 1
                 engine.fire_event(Events.ITERATION_STARTED, bot=self)
                 try:
                     self.state.output = next(updater)
+                    engine.fire_event(Events.ITERATION_COMPLETED, bot=self)
                 except StopIteration:
                     self.state.iteration -= 1
                     self.state.output = None
                     break
-                finally:
-                    engine.fire_event(Events.ITERATION_COMPLETED, bot=self)
 
             engine.fire_event(Events.EPOCH_COMPLETED, bot=self)
             engine.fire_event(Events.COMPLETED, bot=self)
 
     def attach_extension(self,
                          event_name: str = Events.ITERATION_COMPLETED,
                          priority: int = 100,):
         """Used as a decorator only. To add extension directly, use add_event_handler instead."""
         def decorator(handler):
             self._engine.add_event_handler(event_name, handler, priority)
             return handler
         return decorator
 
-    def add_event_handler(self, *args, **kwargs):
-        self._engine.add_event_handler(*args, **kwargs)
+    def add_event_handler(self, event_name, handler, priority=100, *args, **kwargs):
+        self._engine.add_event_handler(event_name, handler, priority, *args, **kwargs)
```

### Comparing `trialbot-0.3.9.2/trialbot/training/trial_registry.py` & `trialbot-0.4.0/trialbot/training/trial_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-from typing import Callable, Tuple
+from collections.abc import Callable
 
 from trialbot.data.dataset import Dataset
 from trialbot.data.translator import Translator
 from .hparamset import HyperParamSet
 
+
 class Registry:
     """
     A static class contains references to all registered
     datasets, translators, and hparamsets by the user script.
     """
     _datasets = {}
     _translators = {}
     _hparamsets = {}
 
     @staticmethod
     def dataset(name=None):
-        def decorator(dataset_fn: Callable[[], Tuple[Dataset, Dataset, Dataset]]):
+        def decorator(dataset_fn: Callable[[], tuple[Dataset, Dataset, Dataset]]):
             nonlocal name
             if name is None:
                 name = dataset_fn.__name__
             Registry._datasets[name] = dataset_fn
             return dataset_fn
         return decorator
 
     @staticmethod
-    def get_dataset(name) -> Tuple[Dataset, Dataset, Dataset]:
+    def get_dataset(name) -> tuple[Dataset, Dataset, Dataset]:
         return Registry._datasets[name]()
 
     @staticmethod
     def translator(name=None):
         def decorator(translator_fn: Callable[[], Translator]):
             nonlocal name
             if name is None:
```

### Comparing `trialbot-0.3.9.2/trialbot/training/updaters/testing_updater.py` & `trialbot-0.4.0/trialbot/training/updaters/testing_updater.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,37 @@
-from trialbot.utils.move_to_device import move_to_device
-import logging
 from ..trial_bot import TrialBot
 from trialbot.data.iterators import RandomIterator
 from ..updater import Updater
 from trialbot.data.translator import Translator
+from .training_updater import BatchMixin
 
-class TestingUpdater(Updater):
-    def __init__(self, dataset, translator: Translator, models, iterators, optims, device=-1):
-        super().__init__(models, iterators, optims, device)
+
+class TestingUpdater(Updater, BatchMixin):
+    def __init__(self, dataset, translator, model, iterator, device: int = -1):
+        super().__init__()
         self.dataset = dataset
+        self.model = model
+        self.iterator = iterator
+        self.device = device
         self.translator: Translator = translator
 
     def update_epoch(self):
-        model, iterator, device = self._models[0], self._iterators[0], self._device
+        model = self.model
         model.eval()
 
-        indices = next(iterator)
-        tensor_list = [self.translator.to_tensor(self.dataset[index]) for index in indices]
-        try:
-            batch = self.translator.batch_tensor(tensor_list)
-        except Exception as e:
-            logging.getLogger(self.__class__.__name__).warning(
-                f'skipping the preprocessing of the batch which raises an exception ... {str(e)}'
-            )
+        batch = self.next_batch()
+        if batch is None:
             return None
 
-        if iterator.is_end_of_epoch:
-            self.stop_epoch()
-        if device >= 0:
-            batch = move_to_device(batch, device)
         output = model(**batch)
+
+        if self.iterator.is_end_of_epoch:
+            self.stop_epoch()
         return output
 
     @classmethod
     def from_bot(cls, bot: TrialBot) -> 'TestingUpdater':
         args, model, hparams = bot.args, bot.model, bot.hparams
-        device = args.device
         dataset = bot.dev_set if args.dev else bot.test_set
         iterator = RandomIterator(len(dataset), hparams.batch_sz, shuffle=False, repeat=False)
-        updater = cls(dataset, bot.translator, model, iterator, None, device)
+        updater = cls(dataset, bot.translator, model, iterator, args.device)
         return updater
-
```

### Comparing `trialbot-0.3.9.2/trialbot/utils/file_reader.py` & `trialbot-0.4.0/trialbot/utils/file_reader.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/utils/grid_search_helper.py` & `trialbot-0.4.0/trialbot/utils/grid_search_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-from typing import List, Mapping, Callable
+from typing import Callable
 from trialbot.training import Registry
 from itertools import product
 
 
-def expand_hparams(grid_conf: Mapping[str, list]):
+def expand_hparams(grid_conf: dict[str, list]):
     keys, value_lists = zip(*grid_conf.items())
     for v in product(*value_lists):
         params = dict(zip(keys, v))
         yield params
 
+
 def update_registry_params(name_prefix, i, params, base_params_fn: Callable):
     name = f"{name_prefix}{i}"
 
     def hparams_wrapper_fn():
         p = base_params_fn()
         for k, v in params.items():
             setattr(p, k, v)
         return p
 
     Registry._hparamsets[name] = hparams_wrapper_fn
     return name
 
-def import_grid_search_parameters(grid_conf: Mapping[str, list], base_param_fn: Callable, name_prefix: str = None):
+
+def import_grid_search_parameters(grid_conf: dict[str, list], base_param_fn: Callable, name_prefix: str = None):
     param_sets = list(expand_hparams(grid_conf))
     import re
     if name_prefix is None:
         name_prefix = re.sub('[^a-zA-Z_0-9]', '', base_param_fn.__name__) + '_'
     names = [update_registry_params(name_prefix, i, params, base_param_fn) for i, params in enumerate(param_sets)]
     return names
 
+
 if __name__ == '__main__':
     grid_conf = {"batch_size": [64, 128, 256], "hidden_size": [300, 600]}
     grid_conf = {
                     "num_inner_loops": [1, 2, 3, 5, 10],
                     "batch_sz": [20, 40, 80],
                     "support_batch_sz": [100, 200, 400]
                 }
```

### Comparing `trialbot-0.3.9.2/trialbot/utils/move_to_device.py` & `trialbot-0.4.0/trialbot/utils/move_to_device.py`

 * *Files identical despite different names*

### Comparing `trialbot-0.3.9.2/trialbot/utils/root_finder.py` & `trialbot-0.4.0/trialbot/utils/root_finder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import Union, Optional
+from typing import Optional
 import os.path
 
+
 def find_root(root_indicator_file: str = ".ROOT",
               startpoint: Optional[str] = None):
     if startpoint is None:
         startpoint = os.getcwd()
     else:
         startpoint = os.path.normpath(os.path.abspath(startpoint))
 
     rootpath = check_dir_(root_indicator_file, startpoint)
     if rootpath is None:
         raise ValueError('ROOT directory not found until the root of the drive.')
 
     # return relative path in case of directory privacy
     return os.path.relpath(rootpath, os.curdir)
 
+
 def check_dir_(root_filename: str, dirpath: str):
     if root_filename in os.listdir(dirpath):
         return dirpath
 
     # go upper level
     parent = get_upper_level_dir_(dirpath)
     if parent == dirpath:   # root of fs encountered
         return None
 
     return check_dir_(root_filename, parent)
 
+
 def get_upper_level_dir_(dirpath: str) -> str:
     canonical_dirpath = os.path.normpath(os.path.abspath(dirpath))
     parent = os.path.join(canonical_dirpath, os.path.pardir)
     canonical_parent = os.path.normpath(parent)
 
     return canonical_parent
 
-
-
-
```

### Comparing `trialbot-0.3.9.2/trialbot.egg-info/SOURCES.txt` & `trialbot-0.4.0/trialbot.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 trialbot/__init__.py
 trialbot.egg-info/PKG-INFO
 trialbot.egg-info/SOURCES.txt
 trialbot.egg-info/dependency_links.txt
 trialbot.egg-info/top_level.txt
@@ -32,19 +33,21 @@
 trialbot/data/translators/__init__.py
 trialbot/data/translators/known_field_translator.py
 trialbot/training/__init__.py
 trialbot/training/event_engine.py
 trialbot/training/extensions.py
 trialbot/training/hparamset.py
 trialbot/training/opt_parser.py
+trialbot/training/select_optims.py
 trialbot/training/trial_bot.py
 trialbot/training/trial_registry.py
 trialbot/training/updater.py
 trialbot/training/updaters/__init__.py
 trialbot/training/updaters/testing_updater.py
 trialbot/training/updaters/training_updater.py
 trialbot/utils/__init__.py
 trialbot/utils/file_reader.py
 trialbot/utils/fix_seed.py
 trialbot/utils/grid_search_helper.py
 trialbot/utils/move_to_device.py
+trialbot/utils/prepend_pythonpath.py
 trialbot/utils/root_finder.py
```

