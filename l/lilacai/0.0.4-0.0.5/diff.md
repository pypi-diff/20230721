# Comparing `tmp/lilacai-0.0.4.tar.gz` & `tmp/lilacai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilacai-0.0.4.tar", max compression
+gzip compressed data, was "lilacai-0.0.5.tar", max compression
```

## Comparing `lilacai-0.0.4.tar` & `lilacai-0.0.5.tar`

### file list

```diff
@@ -1,222 +1,108 @@
--rw-r--r--   0        0        0    11343 2023-05-25 16:32:17.546928 lilacai-0.0.4/LICENSE
--rw-r--r--   0        0        0     5378 2023-07-20 19:37:02.878837 lilacai-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554199 lilacai-0.0.4/lilacai/__init__.py
--rw-r--r--   0        0        0     1800 2023-07-20 19:37:02.879223 lilacai-0.0.4/lilacai/auth.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554252 lilacai-0.0.4/lilacai/concepts/__init__.py
--rw-r--r--   0        0        0      142 2023-05-25 16:33:06.625432 lilacai-0.0.4/lilacai/concepts/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    14978 2023-07-14 16:20:33.334816 lilacai-0.0.4/lilacai/concepts/__pycache__/concept.cpython-39.pyc
--rw-r--r--   0        0        0     3741 2023-05-25 17:56:09.596012 lilacai-0.0.4/lilacai/concepts/__pycache__/concept_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3741 2023-06-29 20:36:35.530262 lilacai-0.0.4/lilacai/concepts/__pycache__/concept_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    14857 2023-07-13 13:55:47.960867 lilacai-0.0.4/lilacai/concepts/__pycache__/db_concept.cpython-39.pyc
--rw-r--r--   0        0        0    26850 2023-06-29 18:31:03.929394 lilacai-0.0.4/lilacai/concepts/__pycache__/db_concept_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    27675 2023-07-05 20:35:04.899345 lilacai-0.0.4/lilacai/concepts/__pycache__/db_concept_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    16253 2023-07-14 16:20:32.053478 lilacai-0.0.4/lilacai/concepts/concept.py
--rw-r--r--   0        0        0     2933 2023-05-25 17:54:51.059050 lilacai-0.0.4/lilacai/concepts/concept_test.py
--rw-r--r--   0        0        0    16062 2023-07-13 13:55:37.904006 lilacai-0.0.4/lilacai/concepts/db_concept.py
--rw-r--r--   0        0        0    22218 2023-07-05 20:35:03.080739 lilacai-0.0.4/lilacai/concepts/db_concept_test.py
--rw-r--r--   0        0        0      570 2023-07-13 13:55:37.904856 lilacai-0.0.4/lilacai/config.py
--rw-r--r--   0        0        0     1026 2023-06-20 15:48:50.744732 lilacai-0.0.4/lilacai/conftest.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554669 lilacai-0.0.4/lilacai/data/__init__.py
--rw-r--r--   0        0        0      138 2023-05-25 16:33:22.229970 lilacai-0.0.4/lilacai/data/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1286 2023-05-25 17:38:50.204350 lilacai-0.0.4/lilacai/data/__pycache__/conftest.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    16829 2023-07-20 12:27:57.956385 lilacai-0.0.4/lilacai/data/__pycache__/dataset.cpython-39.pyc
--rw-r--r--   0        0        0     9781 2023-06-09 14:17:45.871161 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_chain_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     9819 2023-07-19 23:03:24.128430 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_chain_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    20740 2023-06-22 15:45:21.847855 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    20448 2023-07-19 23:03:24.145583 lilacai-0.0.4/lilacai/data/__pycache__/dataset_compute_signal_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    49358 2023-07-20 12:27:58.774666 lilacai-0.0.4/lilacai/data/__pycache__/dataset_duckdb.cpython-39.pyc
--rw-r--r--   0        0        0     8732 2023-06-22 15:45:21.858435 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_groups_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     9482 2023-07-20 12:24:55.916581 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_groups_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     4070 2023-05-30 23:23:49.738222 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_filter_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     6802 2023-06-30 16:45:10.244985 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_filter_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    17328 2023-06-20 15:48:54.176929 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_schema_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    17328 2023-07-15 00:14:43.016746 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_schema_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    11793 2023-06-25 13:04:36.821457 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_search_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    11783 2023-07-05 20:35:04.929716 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_search_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    20762 2023-06-20 12:39:17.922849 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_sort_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    20955 2023-07-19 23:03:24.180529 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_sort_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    16029 2023-06-09 14:18:19.042372 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_udf_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    15916 2023-07-19 23:03:24.282234 lilacai-0.0.4/lilacai/data/__pycache__/dataset_select_rows_udf_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2173 2023-07-18 17:21:20.479288 lilacai-0.0.4/lilacai/data/__pycache__/dataset_settings_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     5621 2023-06-22 15:45:21.880636 lilacai-0.0.4/lilacai/data/__pycache__/dataset_stats_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     7082 2023-07-20 12:24:55.947147 lilacai-0.0.4/lilacai/data/__pycache__/dataset_stats_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    21844 2023-06-20 15:48:54.211586 lilacai-0.0.4/lilacai/data/__pycache__/dataset_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    21673 2023-07-19 23:03:24.308993 lilacai-0.0.4/lilacai/data/__pycache__/dataset_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     4366 2023-07-20 12:27:59.227750 lilacai-0.0.4/lilacai/data/__pycache__/dataset_test_utils.cpython-39.pyc
--rw-r--r--   0        0        0    12560 2023-07-19 23:03:42.331879 lilacai-0.0.4/lilacai/data/__pycache__/dataset_utils.cpython-39.pyc
--rw-r--r--   0        0        0     4223 2023-05-30 23:23:49.825084 lilacai-0.0.4/lilacai/data/__pycache__/dataset_utils_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     7484 2023-07-20 19:55:49.769644 lilacai-0.0.4/lilacai/data/__pycache__/dataset_utils_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0      960 2023-07-05 20:36:01.119393 lilacai-0.0.4/lilacai/data/__pycache__/duckdb_utils.cpython-39.pyc
--rw-r--r--   0        0        0    13670 2023-07-20 12:24:54.802549 lilacai-0.0.4/lilacai/data/dataset.py
--rw-r--r--   0        0        0     7535 2023-07-19 23:03:22.225623 lilacai-0.0.4/lilacai/data/dataset_compute_signal_chain_test.py
--rw-r--r--   0        0        0    17152 2023-07-19 23:03:22.226067 lilacai-0.0.4/lilacai/data/dataset_compute_signal_test.py
--rw-r--r--   0        0        0    70045 2023-07-20 12:24:54.803173 lilacai-0.0.4/lilacai/data/dataset_duckdb.py
--rw-r--r--   0        0        0     7974 2023-07-20 12:24:54.803351 lilacai-0.0.4/lilacai/data/dataset_select_groups_test.py
--rw-r--r--   0        0        0     4992 2023-06-30 16:45:07.674307 lilacai-0.0.4/lilacai/data/dataset_select_rows_filter_test.py
--rw-r--r--   0        0        0    16368 2023-07-15 00:14:39.378163 lilacai-0.0.4/lilacai/data/dataset_select_rows_schema_test.py
--rw-r--r--   0        0        0    12029 2023-07-05 20:35:03.081709 lilacai-0.0.4/lilacai/data/dataset_select_rows_search_test.py
--rw-r--r--   0        0        0    25198 2023-07-19 23:03:22.227067 lilacai-0.0.4/lilacai/data/dataset_select_rows_sort_test.py
--rw-r--r--   0        0        0    11657 2023-07-19 23:03:22.227295 lilacai-0.0.4/lilacai/data/dataset_select_rows_udf_test.py
--rw-r--r--   0        0        0      933 2023-07-18 17:09:32.351044 lilacai-0.0.4/lilacai/data/dataset_settings_test.py
--rw-r--r--   0        0        0     3993 2023-07-20 12:24:54.803501 lilacai-0.0.4/lilacai/data/dataset_stats_test.py
--rw-r--r--   0        0        0    19473 2023-07-19 23:03:22.227509 lilacai-0.0.4/lilacai/data/dataset_test.py
--rw-r--r--   0        0        0     3999 2023-07-20 12:24:54.803655 lilacai-0.0.4/lilacai/data/dataset_test_utils.py
--rw-r--r--   0        0        0    13836 2023-07-19 23:03:22.227770 lilacai-0.0.4/lilacai/data/dataset_utils.py
--rw-r--r--   0        0        0     3790 2023-07-20 19:55:47.509593 lilacai-0.0.4/lilacai/data/dataset_utils_test.py
--rw-r--r--   0        0        0      686 2023-07-05 20:35:03.081959 lilacai-0.0.4/lilacai/data/duckdb_utils.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.556132 lilacai-0.0.4/lilacai/data/sources/__init__.py
--rw-r--r--   0        0        0      146 2023-05-25 16:33:22.230251 lilacai-0.0.4/lilacai/data/sources/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2948 2023-07-14 14:31:43.463140 lilacai-0.0.4/lilacai/data/sources/__pycache__/csv_source.cpython-39.pyc
--rw-r--r--   0        0        0     2147 2023-06-20 12:39:17.946669 lilacai-0.0.4/lilacai/data/sources/__pycache__/csv_source_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2147 2023-06-29 20:36:35.832119 lilacai-0.0.4/lilacai/data/sources/__pycache__/csv_source_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0      825 2023-06-06 15:27:08.044491 lilacai-0.0.4/lilacai/data/sources/__pycache__/default_sources.cpython-39.pyc
--rw-r--r--   0        0        0     6891 2023-07-20 18:27:24.388906 lilacai-0.0.4/lilacai/data/sources/__pycache__/gmail_source.cpython-39.pyc
--rw-r--r--   0        0        0     5156 2023-06-27 20:41:56.561276 lilacai-0.0.4/lilacai/data/sources/__pycache__/huggingface_source.cpython-39.pyc
--rw-r--r--   0        0        0     4478 2023-06-20 12:39:17.951391 lilacai-0.0.4/lilacai/data/sources/__pycache__/huggingface_source_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4478 2023-06-29 20:36:35.836672 lilacai-0.0.4/lilacai/data/sources/__pycache__/huggingface_source_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2382 2023-06-30 16:45:08.555862 lilacai-0.0.4/lilacai/data/sources/__pycache__/json_source.cpython-39.pyc
--rw-r--r--   0        0        0     3354 2023-06-20 12:39:17.955342 lilacai-0.0.4/lilacai/data/sources/__pycache__/json_source_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3354 2023-06-29 20:36:35.839834 lilacai-0.0.4/lilacai/data/sources/__pycache__/json_source_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1991 2023-06-20 12:39:15.981892 lilacai-0.0.4/lilacai/data/sources/__pycache__/pandas_source.cpython-39.pyc
--rw-r--r--   0        0        0     2786 2023-06-20 12:39:17.958635 lilacai-0.0.4/lilacai/data/sources/__pycache__/pandas_source_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2786 2023-06-29 20:36:35.842951 lilacai-0.0.4/lilacai/data/sources/__pycache__/pandas_source_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1981 2023-06-20 12:39:15.983117 lilacai-0.0.4/lilacai/data/sources/__pycache__/reddit_hf_source.cpython-39.pyc
--rw-r--r--   0        0        0     4008 2023-06-30 16:45:08.343946 lilacai-0.0.4/lilacai/data/sources/__pycache__/source.cpython-39.pyc
--rw-r--r--   0        0        0     1653 2023-05-25 16:33:43.625612 lilacai-0.0.4/lilacai/data/sources/__pycache__/source_registry.cpython-39.pyc
--rw-r--r--   0        0        0     3233 2023-06-20 12:39:17.961608 lilacai-0.0.4/lilacai/data/sources/__pycache__/source_registry_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3233 2023-06-29 20:36:35.845613 lilacai-0.0.4/lilacai/data/sources/__pycache__/source_registry_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     6975 2023-05-26 15:29:09.387029 lilacai-0.0.4/lilacai/data/sources/__pycache__/tfds_source.cpython-39.pyc
--rw-r--r--   0        0        0     2585 2023-07-14 14:31:41.393638 lilacai-0.0.4/lilacai/data/sources/csv_source.py
--rw-r--r--   0        0        0      977 2023-06-20 12:39:14.682662 lilacai-0.0.4/lilacai/data/sources/csv_source_test.py
--rw-r--r--   0        0        0      606 2023-06-06 15:27:06.003752 lilacai-0.0.4/lilacai/data/sources/default_sources.py
--rw-r--r--   0        0        0     8190 2023-07-20 18:27:22.410168 lilacai-0.0.4/lilacai/data/sources/gmail_source.py
--rw-r--r--   0        0        0     5834 2023-06-27 20:41:54.787722 lilacai-0.0.4/lilacai/data/sources/huggingface_source.py
--rw-r--r--   0        0        0     4052 2023-06-20 12:39:14.683879 lilacai-0.0.4/lilacai/data/sources/huggingface_source_test.py
--rw-r--r--   0        0        0     1874 2023-06-30 16:45:07.675244 lilacai-0.0.4/lilacai/data/sources/json_source.py
--rw-r--r--   0        0        0     1687 2023-06-20 12:39:14.684467 lilacai-0.0.4/lilacai/data/sources/json_source_test.py
--rw-r--r--   0        0        0     1119 2023-06-20 12:39:14.685119 lilacai-0.0.4/lilacai/data/sources/pandas_source.py
--rw-r--r--   0        0        0     1717 2023-06-20 12:39:14.685632 lilacai-0.0.4/lilacai/data/sources/pandas_source_test.py
--rw-r--r--   0        0        0     1463 2023-06-20 12:39:14.685957 lilacai-0.0.4/lilacai/data/sources/reddit_hf_source.py
--rw-r--r--   0        0        0     3237 2023-06-30 16:45:07.675479 lilacai-0.0.4/lilacai/data/sources/source.py
--rw-r--r--   0        0        0     1363 2023-05-25 16:32:17.556830 lilacai-0.0.4/lilacai/data/sources/source_registry.py
--rw-r--r--   0        0        0     1228 2023-06-20 12:39:14.686782 lilacai-0.0.4/lilacai/data/sources/source_registry_test.py
--rw-r--r--   0        0        0     4522 2023-07-20 19:27:47.282556 lilacai-0.0.4/lilacai/data_loader.py
--rw-r--r--   0        0        0     2063 2023-06-20 12:39:14.687292 lilacai-0.0.4/lilacai/data_loader_test.py
--rw-r--r--   0        0        0     1430 2023-07-01 13:53:22.647752 lilacai-0.0.4/lilacai/db_manager.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.557162 lilacai-0.0.4/lilacai/embeddings/__init__.py
--rw-r--r--   0        0        0      144 2023-05-25 16:33:20.655912 lilacai-0.0.4/lilacai/embeddings/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2441 2023-07-20 18:27:24.660578 lilacai-0.0.4/lilacai/embeddings/__pycache__/cohere.cpython-39.pyc
--rw-r--r--   0        0        0     3973 2023-07-14 16:20:33.697005 lilacai-0.0.4/lilacai/embeddings/__pycache__/embedding.cpython-39.pyc
--rw-r--r--   0        0        0     4297 2023-06-19 15:55:32.925051 lilacai-0.0.4/lilacai/embeddings/__pycache__/embedding_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     5238 2023-07-14 16:20:35.348301 lilacai-0.0.4/lilacai/embeddings/__pycache__/embedding_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2955 2023-07-20 18:27:24.661645 lilacai-0.0.4/lilacai/embeddings/__pycache__/openai.cpython-39.pyc
--rw-r--r--   0        0        0     2730 2023-07-20 18:27:24.667100 lilacai-0.0.4/lilacai/embeddings/__pycache__/palm.cpython-39.pyc
--rw-r--r--   0        0        0     2560 2023-07-20 18:27:24.668638 lilacai-0.0.4/lilacai/embeddings/__pycache__/sbert.cpython-39.pyc
--rw-r--r--   0        0        0     2097 2023-06-09 20:36:16.224765 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store.cpython-39.pyc
--rw-r--r--   0        0        0     2983 2023-07-14 18:14:01.396374 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store_numpy.cpython-39.pyc
--rw-r--r--   0        0        0     5894 2023-06-09 20:45:02.896412 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     5894 2023-06-29 20:36:35.855642 lilacai-0.0.4/lilacai/embeddings/__pycache__/vector_store_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1885 2023-07-20 18:27:22.410682 lilacai-0.0.4/lilacai/embeddings/cohere.py
--rw-r--r--   0        0        0     4274 2023-07-14 16:20:32.054385 lilacai-0.0.4/lilacai/embeddings/embedding.py
--rw-r--r--   0        0        0     3051 2023-07-14 16:20:32.054666 lilacai-0.0.4/lilacai/embeddings/embedding_test.py
--rw-r--r--   0        0        0     2354 2023-07-20 18:27:22.410904 lilacai-0.0.4/lilacai/embeddings/openai.py
--rw-r--r--   0        0        0     2269 2023-07-20 18:27:22.411212 lilacai-0.0.4/lilacai/embeddings/palm.py
--rw-r--r--   0        0        0     2580 2023-07-20 18:27:22.411503 lilacai-0.0.4/lilacai/embeddings/sbert.py
--rw-r--r--   0        0        0     1483 2023-06-09 20:36:08.693683 lilacai-0.0.4/lilacai/embeddings/vector_store.py
--rw-r--r--   0        0        0     2886 2023-07-14 18:13:59.183687 lilacai-0.0.4/lilacai/embeddings/vector_store_numpy.py
--rw-r--r--   0        0        0     2690 2023-06-09 20:36:08.699912 lilacai-0.0.4/lilacai/embeddings/vector_store_test.py
--rw-r--r--   0        0        0      768 2023-07-20 19:28:06.306494 lilacai-0.0.4/lilacai/make_openapi.py
--rw-r--r--   0        0        0     2453 2023-05-26 18:51:52.618951 lilacai-0.0.4/lilacai/parquet_writer.py
--rw-r--r--   0        0        0     7819 2023-07-20 18:27:22.411690 lilacai-0.0.4/lilacai/router_concept.py
--rw-r--r--   0        0        0     2464 2023-07-20 19:28:16.506968 lilacai-0.0.4/lilacai/router_data_loader.py
--rw-r--r--   0        0        0    10847 2023-07-19 23:03:22.228507 lilacai-0.0.4/lilacai/router_dataset.py
--rw-r--r--   0        0        0     2142 2023-07-20 19:37:02.879424 lilacai-0.0.4/lilacai/router_google_login.py
--rw-r--r--   0        0        0     1366 2023-07-06 19:35:06.524109 lilacai-0.0.4/lilacai/router_signal.py
--rw-r--r--   0        0        0      355 2023-05-25 16:32:17.558021 lilacai-0.0.4/lilacai/router_tasks.py
--rw-r--r--   0        0        0      892 2023-05-25 16:32:17.558089 lilacai-0.0.4/lilacai/router_utils.py
--rw-r--r--   0        0        0    19299 2023-07-18 17:09:32.352505 lilacai-0.0.4/lilacai/schema.py
--rw-r--r--   0        0        0     7534 2023-05-31 19:20:41.732336 lilacai-0.0.4/lilacai/schema_test.py
--rw-r--r--   0        0        0     5640 2023-07-20 19:37:02.879793 lilacai-0.0.4/lilacai/server.py
--rw-r--r--   0        0        0    15119 2023-07-19 23:03:22.228906 lilacai-0.0.4/lilacai/server_concept_test.py
--rw-r--r--   0        0        0     9376 2023-07-19 23:03:22.229057 lilacai-0.0.4/lilacai/server_dataset_test.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.558575 lilacai-0.0.4/lilacai/signals/__init__.py
--rw-r--r--   0        0        0      141 2023-05-25 16:33:21.312087 lilacai-0.0.4/lilacai/signals/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2538 2023-07-10 19:43:01.845713 lilacai-0.0.4/lilacai/signals/__pycache__/concept_labels.cpython-39.pyc
--rw-r--r--   0        0        0     5338 2023-06-20 12:39:17.971321 lilacai-0.0.4/lilacai/signals/__pycache__/concept_labels_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     5338 2023-06-29 20:36:35.861540 lilacai-0.0.4/lilacai/signals/__pycache__/concept_labels_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     3457 2023-07-15 00:15:39.697437 lilacai-0.0.4/lilacai/signals/__pycache__/concept_scorer.cpython-39.pyc
--rw-r--r--   0        0        0    12587 2023-06-20 12:39:17.981373 lilacai-0.0.4/lilacai/signals/__pycache__/concept_scorer_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    13294 2023-07-13 13:55:52.375098 lilacai-0.0.4/lilacai/signals/__pycache__/concept_scorer_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1135 2023-07-19 12:31:05.301162 lilacai-0.0.4/lilacai/signals/__pycache__/default_signals.cpython-39.pyc
--rw-r--r--   0        0        0     2268 2023-07-20 18:27:22.466894 lilacai-0.0.4/lilacai/signals/__pycache__/lang_detection.cpython-39.pyc
--rw-r--r--   0        0        0     1661 2023-07-20 18:27:22.465620 lilacai-0.0.4/lilacai/signals/__pycache__/lang_detection_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     7666 2023-07-18 17:21:19.902763 lilacai-0.0.4/lilacai/signals/__pycache__/minhash_dup.cpython-39.pyc
--rw-r--r--   0        0        0     1865 2023-07-18 17:21:19.901110 lilacai-0.0.4/lilacai/signals/__pycache__/near_dup.cpython-39.pyc
--rw-r--r--   0        0        0     2161 2023-07-18 17:21:20.505848 lilacai-0.0.4/lilacai/signals/__pycache__/near_dup_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2515 2023-07-20 18:27:22.470411 lilacai-0.0.4/lilacai/signals/__pycache__/ner.cpython-39.pyc
--rw-r--r--   0        0        0     2080 2023-07-06 19:35:08.489259 lilacai-0.0.4/lilacai/signals/__pycache__/ner_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2515 2023-07-20 18:27:22.472352 lilacai-0.0.4/lilacai/signals/__pycache__/pii.cpython-39.pyc
--rw-r--r--   0        0        0     3576 2023-07-20 15:05:48.248628 lilacai-0.0.4/lilacai/signals/__pycache__/pii_ip_address.cpython-39.pyc
--rw-r--r--   0        0        0     3670 2023-07-20 15:06:14.959294 lilacai-0.0.4/lilacai/signals/__pycache__/pii_secrets.cpython-39.pyc
--rw-r--r--   0        0        0     2360 2023-05-31 19:20:42.595460 lilacai-0.0.4/lilacai/signals/__pycache__/pii_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3286 2023-07-17 16:27:30.928786 lilacai-0.0.4/lilacai/signals/__pycache__/pii_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2845 2023-05-25 17:54:37.709786 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_search.cpython-39.pyc
--rw-r--r--   0        0        0     4418 2023-05-25 17:54:41.434136 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_search_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3472 2023-06-09 15:06:25.513033 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_similarity.cpython-39.pyc
--rw-r--r--   0        0        0     4598 2023-06-09 14:18:55.738564 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_similarity_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     4598 2023-06-29 20:36:35.879375 lilacai-0.0.4/lilacai/signals/__pycache__/semantic_similarity_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0    11402 2023-07-15 00:15:45.703610 lilacai-0.0.4/lilacai/signals/__pycache__/signal.cpython-39.pyc
--rw-r--r--   0        0        0     8825 2023-06-01 14:18:45.547562 lilacai-0.0.4/lilacai/signals/__pycache__/signal_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     8825 2023-06-29 20:36:35.885373 lilacai-0.0.4/lilacai/signals/__pycache__/signal_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1876 2023-06-01 14:18:38.849669 lilacai-0.0.4/lilacai/signals/__pycache__/substring_search.cpython-39.pyc
--rw-r--r--   0        0        0     2129 2023-05-31 19:20:42.618860 lilacai-0.0.4/lilacai/signals/__pycache__/substring_search_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2129 2023-06-29 20:36:35.889481 lilacai-0.0.4/lilacai/signals/__pycache__/substring_search_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2781 2023-07-20 18:27:22.481788 lilacai-0.0.4/lilacai/signals/__pycache__/text_statistics.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2023-06-20 12:39:17.996390 lilacai-0.0.4/lilacai/signals/__pycache__/text_statistics_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2693 2023-06-29 20:36:35.891867 lilacai-0.0.4/lilacai/signals/__pycache__/text_statistics_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2541 2023-07-10 19:42:59.609736 lilacai-0.0.4/lilacai/signals/concept_labels.py
--rw-r--r--   0        0        0     4759 2023-06-20 12:39:14.689841 lilacai-0.0.4/lilacai/signals/concept_labels_test.py
--rw-r--r--   0        0        0     3277 2023-07-15 00:15:37.808580 lilacai-0.0.4/lilacai/signals/concept_scorer.py
--rw-r--r--   0        0        0    12036 2023-07-13 13:55:37.919378 lilacai-0.0.4/lilacai/signals/concept_scorer_test.py
--rw-r--r--   0        0        0     1000 2023-07-19 12:31:03.318388 lilacai-0.0.4/lilacai/signals/default_signals.py
--rw-r--r--   0        0        0     1995 2023-07-20 18:27:22.412174 lilacai-0.0.4/lilacai/signals/lang_detection.py
--rw-r--r--   0        0        0      819 2023-07-20 18:27:22.412677 lilacai-0.0.4/lilacai/signals/lang_detection_test.py
--rw-r--r--   0        0        0     6477 2023-07-18 17:09:32.353151 lilacai-0.0.4/lilacai/signals/minhash_dup.py
--rw-r--r--   0        0        0     1306 2023-07-18 17:09:32.353516 lilacai-0.0.4/lilacai/signals/near_dup.py
--rw-r--r--   0        0        0      629 2023-07-18 17:09:32.353708 lilacai-0.0.4/lilacai/signals/near_dup_test.py
--rw-r--r--   0        0        0     1813 2023-07-20 18:27:22.412849 lilacai-0.0.4/lilacai/signals/ner.py
--rw-r--r--   0        0        0      957 2023-07-06 19:35:06.525211 lilacai-0.0.4/lilacai/signals/ner_test.py
--rw-r--r--   0        0        0     2176 2023-07-20 18:27:22.413114 lilacai-0.0.4/lilacai/signals/pii.py
--rw-r--r--   0        0        0     3771 2023-07-20 15:05:47.735774 lilacai-0.0.4/lilacai/signals/pii_ip_address.py
--rw-r--r--   0        0        0     3835 2023-07-20 15:06:12.956980 lilacai-0.0.4/lilacai/signals/pii_secrets.py
--rw-r--r--   0        0        0     1774 2023-07-17 16:27:29.936555 lilacai-0.0.4/lilacai/signals/pii_test.py
--rw-r--r--   0        0        0     2962 2023-06-09 15:06:22.815280 lilacai-0.0.4/lilacai/signals/semantic_similarity.py
--rw-r--r--   0        0        0     2732 2023-06-09 14:18:52.477786 lilacai-0.0.4/lilacai/signals/semantic_similarity_test.py
--rw-r--r--   0        0        0    10745 2023-07-15 00:15:44.780425 lilacai-0.0.4/lilacai/signals/signal.py
--rw-r--r--   0        0        0     4013 2023-06-01 14:18:35.037543 lilacai-0.0.4/lilacai/signals/signal_test.py
--rw-r--r--   0        0        0        0 2023-05-25 16:32:17.559184 lilacai-0.0.4/lilacai/signals/splitters/__init__.py
--rw-r--r--   0        0        0      151 2023-05-25 16:33:51.092841 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5467 2023-06-19 15:55:31.667495 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/chunk_splitter.cpython-39.pyc
--rw-r--r--   0        0        0     3044 2023-05-29 23:27:31.978383 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/chunk_splitter_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3044 2023-06-29 20:36:35.895019 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/chunk_splitter_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     2476 2023-07-20 18:27:22.487078 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_spacy.cpython-39.pyc
--rw-r--r--   0        0        0     2490 2023-05-25 17:38:57.381087 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_spacy_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2522 2023-07-20 18:27:22.486467 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_spacy_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     1490 2023-07-06 19:35:08.490242 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_test_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1319 2023-05-25 17:38:57.382952 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_test_utils_test.cpython-39-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1319 2023-06-29 20:36:35.899964 lilacai-0.0.4/lilacai/signals/splitters/__pycache__/text_splitter_test_utils_test.cpython-39-pytest-7.4.0.pyc
--rw-r--r--   0        0        0     7236 2023-06-19 15:55:30.003798 lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter.py
--rw-r--r--   0        0        0     1548 2023-05-29 23:27:25.899676 lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter_test.py
--rw-r--r--   0        0        0     1596 2023-07-20 18:27:22.413494 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy.py
--rw-r--r--   0        0        0     1108 2023-07-20 18:27:22.413696 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy_test.py
--rw-r--r--   0        0        0     1260 2023-07-06 19:35:06.527582 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_test_utils.py
--rw-r--r--   0        0        0      479 2023-05-25 16:32:17.559463 lilacai-0.0.4/lilacai/signals/splitters/text_splitter_test_utils_test.py
--rw-r--r--   0        0        0     1011 2023-06-01 14:18:34.599490 lilacai-0.0.4/lilacai/signals/substring_search.py
--rw-r--r--   0        0        0      754 2023-05-31 19:20:41.736419 lilacai-0.0.4/lilacai/signals/substring_search_test.py
--rw-r--r--   0        0        0     2481 2023-07-20 18:27:22.414079 lilacai-0.0.4/lilacai/signals/text_statistics.py
--rw-r--r--   0        0        0     1233 2023-06-20 12:39:14.692018 lilacai-0.0.4/lilacai/signals/text_statistics_test.py
--rw-r--r--   0        0        0    10564 2023-07-17 14:57:58.411331 lilacai-0.0.4/lilacai/tasks.py
--rw-r--r--   0        0        0      685 2023-05-30 23:23:46.459074 lilacai-0.0.4/lilacai/test_utils.py
--rw-r--r--   0        0        0     9711 2023-07-10 17:51:12.979596 lilacai-0.0.4/lilacai/utils.py
--rw-r--r--   0        0        0     5670 2023-07-20 20:06:39.642165 lilacai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8457 1970-01-01 00:00:00.000000 lilacai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-25 16:32:17.546928 lilacai-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5624 2023-07-20 20:29:16.004495 lilacai-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554199 lilacai-0.0.5/lilacai/__init__.py
+-rw-r--r--   0        0        0     1800 2023-07-20 19:37:02.879223 lilacai-0.0.5/lilacai/auth.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554252 lilacai-0.0.5/lilacai/concepts/__init__.py
+-rw-r--r--   0        0        0    16253 2023-07-14 16:20:32.053478 lilacai-0.0.5/lilacai/concepts/concept.py
+-rw-r--r--   0        0        0     2933 2023-05-25 17:54:51.059050 lilacai-0.0.5/lilacai/concepts/concept_test.py
+-rw-r--r--   0        0        0    16062 2023-07-13 13:55:37.904006 lilacai-0.0.5/lilacai/concepts/db_concept.py
+-rw-r--r--   0        0        0    22218 2023-07-05 20:35:03.080739 lilacai-0.0.5/lilacai/concepts/db_concept_test.py
+-rw-r--r--   0        0        0      570 2023-07-13 13:55:37.904856 lilacai-0.0.5/lilacai/config.py
+-rw-r--r--   0        0        0     1026 2023-06-20 15:48:50.744732 lilacai-0.0.5/lilacai/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.554669 lilacai-0.0.5/lilacai/data/__init__.py
+-rw-r--r--   0        0        0    13670 2023-07-20 12:24:54.802549 lilacai-0.0.5/lilacai/data/dataset.py
+-rw-r--r--   0        0        0     7535 2023-07-19 23:03:22.225623 lilacai-0.0.5/lilacai/data/dataset_compute_signal_chain_test.py
+-rw-r--r--   0        0        0    17152 2023-07-19 23:03:22.226067 lilacai-0.0.5/lilacai/data/dataset_compute_signal_test.py
+-rw-r--r--   0        0        0    70045 2023-07-20 12:24:54.803173 lilacai-0.0.5/lilacai/data/dataset_duckdb.py
+-rw-r--r--   0        0        0     7974 2023-07-20 12:24:54.803351 lilacai-0.0.5/lilacai/data/dataset_select_groups_test.py
+-rw-r--r--   0        0        0     4992 2023-06-30 16:45:07.674307 lilacai-0.0.5/lilacai/data/dataset_select_rows_filter_test.py
+-rw-r--r--   0        0        0    16368 2023-07-15 00:14:39.378163 lilacai-0.0.5/lilacai/data/dataset_select_rows_schema_test.py
+-rw-r--r--   0        0        0    12029 2023-07-05 20:35:03.081709 lilacai-0.0.5/lilacai/data/dataset_select_rows_search_test.py
+-rw-r--r--   0        0        0    25198 2023-07-19 23:03:22.227067 lilacai-0.0.5/lilacai/data/dataset_select_rows_sort_test.py
+-rw-r--r--   0        0        0    11657 2023-07-19 23:03:22.227295 lilacai-0.0.5/lilacai/data/dataset_select_rows_udf_test.py
+-rw-r--r--   0        0        0      933 2023-07-18 17:09:32.351044 lilacai-0.0.5/lilacai/data/dataset_settings_test.py
+-rw-r--r--   0        0        0     3993 2023-07-20 12:24:54.803501 lilacai-0.0.5/lilacai/data/dataset_stats_test.py
+-rw-r--r--   0        0        0    19473 2023-07-19 23:03:22.227509 lilacai-0.0.5/lilacai/data/dataset_test.py
+-rw-r--r--   0        0        0     3999 2023-07-20 12:24:54.803655 lilacai-0.0.5/lilacai/data/dataset_test_utils.py
+-rw-r--r--   0        0        0    13836 2023-07-19 23:03:22.227770 lilacai-0.0.5/lilacai/data/dataset_utils.py
+-rw-r--r--   0        0        0     3790 2023-07-20 19:55:47.509593 lilacai-0.0.5/lilacai/data/dataset_utils_test.py
+-rw-r--r--   0        0        0      686 2023-07-05 20:35:03.081959 lilacai-0.0.5/lilacai/data/duckdb_utils.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.556132 lilacai-0.0.5/lilacai/data/sources/__init__.py
+-rw-r--r--   0        0        0     2585 2023-07-14 14:31:41.393638 lilacai-0.0.5/lilacai/data/sources/csv_source.py
+-rw-r--r--   0        0        0      977 2023-06-20 12:39:14.682662 lilacai-0.0.5/lilacai/data/sources/csv_source_test.py
+-rw-r--r--   0        0        0      606 2023-06-06 15:27:06.003752 lilacai-0.0.5/lilacai/data/sources/default_sources.py
+-rw-r--r--   0        0        0     8190 2023-07-20 18:27:22.410168 lilacai-0.0.5/lilacai/data/sources/gmail_source.py
+-rw-r--r--   0        0        0     5834 2023-06-27 20:41:54.787722 lilacai-0.0.5/lilacai/data/sources/huggingface_source.py
+-rw-r--r--   0        0        0     4052 2023-06-20 12:39:14.683879 lilacai-0.0.5/lilacai/data/sources/huggingface_source_test.py
+-rw-r--r--   0        0        0     1874 2023-06-30 16:45:07.675244 lilacai-0.0.5/lilacai/data/sources/json_source.py
+-rw-r--r--   0        0        0     1687 2023-06-20 12:39:14.684467 lilacai-0.0.5/lilacai/data/sources/json_source_test.py
+-rw-r--r--   0        0        0     1119 2023-06-20 12:39:14.685119 lilacai-0.0.5/lilacai/data/sources/pandas_source.py
+-rw-r--r--   0        0        0     1717 2023-06-20 12:39:14.685632 lilacai-0.0.5/lilacai/data/sources/pandas_source_test.py
+-rw-r--r--   0        0        0     1463 2023-06-20 12:39:14.685957 lilacai-0.0.5/lilacai/data/sources/reddit_hf_source.py
+-rw-r--r--   0        0        0     3237 2023-06-30 16:45:07.675479 lilacai-0.0.5/lilacai/data/sources/source.py
+-rw-r--r--   0        0        0     1363 2023-05-25 16:32:17.556830 lilacai-0.0.5/lilacai/data/sources/source_registry.py
+-rw-r--r--   0        0        0     1228 2023-06-20 12:39:14.686782 lilacai-0.0.5/lilacai/data/sources/source_registry_test.py
+-rw-r--r--   0        0        0     4522 2023-07-20 19:27:47.282556 lilacai-0.0.5/lilacai/data_loader.py
+-rw-r--r--   0        0        0     2063 2023-06-20 12:39:14.687292 lilacai-0.0.5/lilacai/data_loader_test.py
+-rw-r--r--   0        0        0     1430 2023-07-01 13:53:22.647752 lilacai-0.0.5/lilacai/db_manager.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.557162 lilacai-0.0.5/lilacai/embeddings/__init__.py
+-rw-r--r--   0        0        0     1885 2023-07-20 18:27:22.410682 lilacai-0.0.5/lilacai/embeddings/cohere.py
+-rw-r--r--   0        0        0     4274 2023-07-14 16:20:32.054385 lilacai-0.0.5/lilacai/embeddings/embedding.py
+-rw-r--r--   0        0        0     3051 2023-07-14 16:20:32.054666 lilacai-0.0.5/lilacai/embeddings/embedding_test.py
+-rw-r--r--   0        0        0     2354 2023-07-20 18:27:22.410904 lilacai-0.0.5/lilacai/embeddings/openai.py
+-rw-r--r--   0        0        0     2269 2023-07-20 18:27:22.411212 lilacai-0.0.5/lilacai/embeddings/palm.py
+-rw-r--r--   0        0        0     2580 2023-07-20 18:27:22.411503 lilacai-0.0.5/lilacai/embeddings/sbert.py
+-rw-r--r--   0        0        0     1483 2023-06-09 20:36:08.693683 lilacai-0.0.5/lilacai/embeddings/vector_store.py
+-rw-r--r--   0        0        0     2886 2023-07-14 18:13:59.183687 lilacai-0.0.5/lilacai/embeddings/vector_store_numpy.py
+-rw-r--r--   0        0        0     2690 2023-06-09 20:36:08.699912 lilacai-0.0.5/lilacai/embeddings/vector_store_test.py
+-rw-r--r--   0        0        0      768 2023-07-20 19:28:06.306494 lilacai-0.0.5/lilacai/make_openapi.py
+-rw-r--r--   0        0        0     2453 2023-05-26 18:51:52.618951 lilacai-0.0.5/lilacai/parquet_writer.py
+-rw-r--r--   0        0        0     7819 2023-07-20 18:27:22.411690 lilacai-0.0.5/lilacai/router_concept.py
+-rw-r--r--   0        0        0     2464 2023-07-20 19:28:16.506968 lilacai-0.0.5/lilacai/router_data_loader.py
+-rw-r--r--   0        0        0    10847 2023-07-19 23:03:22.228507 lilacai-0.0.5/lilacai/router_dataset.py
+-rw-r--r--   0        0        0     2142 2023-07-20 19:37:02.879424 lilacai-0.0.5/lilacai/router_google_login.py
+-rw-r--r--   0        0        0     1366 2023-07-06 19:35:06.524109 lilacai-0.0.5/lilacai/router_signal.py
+-rw-r--r--   0        0        0      355 2023-05-25 16:32:17.558021 lilacai-0.0.5/lilacai/router_tasks.py
+-rw-r--r--   0        0        0      892 2023-05-25 16:32:17.558089 lilacai-0.0.5/lilacai/router_utils.py
+-rw-r--r--   0        0        0    19299 2023-07-18 17:09:32.352505 lilacai-0.0.5/lilacai/schema.py
+-rw-r--r--   0        0        0     7534 2023-05-31 19:20:41.732336 lilacai-0.0.5/lilacai/schema_test.py
+-rw-r--r--   0        0        0     5640 2023-07-20 19:37:02.879793 lilacai-0.0.5/lilacai/server.py
+-rw-r--r--   0        0        0    15119 2023-07-19 23:03:22.228906 lilacai-0.0.5/lilacai/server_concept_test.py
+-rw-r--r--   0        0        0     9376 2023-07-19 23:03:22.229057 lilacai-0.0.5/lilacai/server_dataset_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.558575 lilacai-0.0.5/lilacai/signals/__init__.py
+-rw-r--r--   0        0        0     2541 2023-07-10 19:42:59.609736 lilacai-0.0.5/lilacai/signals/concept_labels.py
+-rw-r--r--   0        0        0     4759 2023-06-20 12:39:14.689841 lilacai-0.0.5/lilacai/signals/concept_labels_test.py
+-rw-r--r--   0        0        0     3277 2023-07-15 00:15:37.808580 lilacai-0.0.5/lilacai/signals/concept_scorer.py
+-rw-r--r--   0        0        0    12036 2023-07-13 13:55:37.919378 lilacai-0.0.5/lilacai/signals/concept_scorer_test.py
+-rw-r--r--   0        0        0     1000 2023-07-19 12:31:03.318388 lilacai-0.0.5/lilacai/signals/default_signals.py
+-rw-r--r--   0        0        0     1995 2023-07-20 18:27:22.412174 lilacai-0.0.5/lilacai/signals/lang_detection.py
+-rw-r--r--   0        0        0      819 2023-07-20 18:27:22.412677 lilacai-0.0.5/lilacai/signals/lang_detection_test.py
+-rw-r--r--   0        0        0     6477 2023-07-18 17:09:32.353151 lilacai-0.0.5/lilacai/signals/minhash_dup.py
+-rw-r--r--   0        0        0     1306 2023-07-18 17:09:32.353516 lilacai-0.0.5/lilacai/signals/near_dup.py
+-rw-r--r--   0        0        0      629 2023-07-18 17:09:32.353708 lilacai-0.0.5/lilacai/signals/near_dup_test.py
+-rw-r--r--   0        0        0     1813 2023-07-20 18:27:22.412849 lilacai-0.0.5/lilacai/signals/ner.py
+-rw-r--r--   0        0        0      957 2023-07-06 19:35:06.525211 lilacai-0.0.5/lilacai/signals/ner_test.py
+-rw-r--r--   0        0        0     2176 2023-07-20 18:27:22.413114 lilacai-0.0.5/lilacai/signals/pii.py
+-rw-r--r--   0        0        0     3771 2023-07-20 15:05:47.735774 lilacai-0.0.5/lilacai/signals/pii_ip_address.py
+-rw-r--r--   0        0        0     3835 2023-07-20 15:06:12.956980 lilacai-0.0.5/lilacai/signals/pii_secrets.py
+-rw-r--r--   0        0        0     1774 2023-07-17 16:27:29.936555 lilacai-0.0.5/lilacai/signals/pii_test.py
+-rw-r--r--   0        0        0     2962 2023-06-09 15:06:22.815280 lilacai-0.0.5/lilacai/signals/semantic_similarity.py
+-rw-r--r--   0        0        0     2732 2023-06-09 14:18:52.477786 lilacai-0.0.5/lilacai/signals/semantic_similarity_test.py
+-rw-r--r--   0        0        0    10745 2023-07-15 00:15:44.780425 lilacai-0.0.5/lilacai/signals/signal.py
+-rw-r--r--   0        0        0     4013 2023-06-01 14:18:35.037543 lilacai-0.0.5/lilacai/signals/signal_test.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:32:17.559184 lilacai-0.0.5/lilacai/signals/splitters/__init__.py
+-rw-r--r--   0        0        0     7236 2023-06-19 15:55:30.003798 lilacai-0.0.5/lilacai/signals/splitters/chunk_splitter.py
+-rw-r--r--   0        0        0     1548 2023-05-29 23:27:25.899676 lilacai-0.0.5/lilacai/signals/splitters/chunk_splitter_test.py
+-rw-r--r--   0        0        0     1596 2023-07-20 18:27:22.413494 lilacai-0.0.5/lilacai/signals/splitters/text_splitter_spacy.py
+-rw-r--r--   0        0        0     1108 2023-07-20 18:27:22.413696 lilacai-0.0.5/lilacai/signals/splitters/text_splitter_spacy_test.py
+-rw-r--r--   0        0        0     1260 2023-07-06 19:35:06.527582 lilacai-0.0.5/lilacai/signals/splitters/text_splitter_test_utils.py
+-rw-r--r--   0        0        0      479 2023-05-25 16:32:17.559463 lilacai-0.0.5/lilacai/signals/splitters/text_splitter_test_utils_test.py
+-rw-r--r--   0        0        0     1011 2023-06-01 14:18:34.599490 lilacai-0.0.5/lilacai/signals/substring_search.py
+-rw-r--r--   0        0        0      754 2023-05-31 19:20:41.736419 lilacai-0.0.5/lilacai/signals/substring_search_test.py
+-rw-r--r--   0        0        0     2481 2023-07-20 18:27:22.414079 lilacai-0.0.5/lilacai/signals/text_statistics.py
+-rw-r--r--   0        0        0     1233 2023-06-20 12:39:14.692018 lilacai-0.0.5/lilacai/signals/text_statistics_test.py
+-rw-r--r--   0        0        0    10564 2023-07-17 14:57:58.411331 lilacai-0.0.5/lilacai/tasks.py
+-rw-r--r--   0        0        0      685 2023-05-30 23:23:46.459074 lilacai-0.0.5/lilacai/test_utils.py
+-rw-r--r--   0        0        0     9711 2023-07-10 17:51:12.979596 lilacai-0.0.5/lilacai/utils.py
+-rw-r--r--   0        0        0     5670 2023-07-20 20:30:33.711920 lilacai-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8703 1970-01-01 00:00:00.000000 lilacai-0.0.5/PKG-INFO
```

### Comparing `lilacai-0.0.4/LICENSE` & `lilacai-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/README.md` & `lilacai-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -96,14 +96,23 @@
 ```py
 import string
 import random
 key = ''.join(random.choices(string.ascii_uppercase + string.digits, k=64))
 print(f"LILAC_OAUTH_SECRET_KEY='{key}'")
 ```
 
+### Publishing on pip
+
+To authenticate, add the `PYPI_TOKEN` to your `.env.local` file. You can get the token from
+[pypi.org](https://pypi.org/manage/project/lilacai/settings/). Then run the following script:
+
+```sh
+./scripts/publish_pip.sh
+```
+
 ### Configuration
 
 To use various API's, API keys need to be provided. Create a file named `.env.local` in the root, and add variables that are listed in `.env` with your own values.
 
 #### Testing
 
 Run all the checks before mailing:
```

### Comparing `lilacai-0.0.4/lilacai/auth.py` & `lilacai-0.0.5/lilacai/auth.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/concepts/concept.py` & `lilacai-0.0.5/lilacai/concepts/concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/concepts/concept_test.py` & `lilacai-0.0.5/lilacai/concepts/concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/concepts/db_concept.py` & `lilacai-0.0.5/lilacai/concepts/db_concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/concepts/db_concept_test.py` & `lilacai-0.0.5/lilacai/concepts/db_concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/config.py` & `lilacai-0.0.5/lilacai/config.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/conftest.py` & `lilacai-0.0.5/lilacai/conftest.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset.py` & `lilacai-0.0.5/lilacai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_compute_signal_chain_test.py` & `lilacai-0.0.5/lilacai/data/dataset_compute_signal_chain_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_compute_signal_test.py` & `lilacai-0.0.5/lilacai/data/dataset_compute_signal_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_duckdb.py` & `lilacai-0.0.5/lilacai/data/dataset_duckdb.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_select_groups_test.py` & `lilacai-0.0.5/lilacai/data/dataset_select_groups_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_select_rows_filter_test.py` & `lilacai-0.0.5/lilacai/data/dataset_select_rows_filter_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_select_rows_schema_test.py` & `lilacai-0.0.5/lilacai/data/dataset_select_rows_schema_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_select_rows_search_test.py` & `lilacai-0.0.5/lilacai/data/dataset_select_rows_search_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_select_rows_sort_test.py` & `lilacai-0.0.5/lilacai/data/dataset_select_rows_sort_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_select_rows_udf_test.py` & `lilacai-0.0.5/lilacai/data/dataset_select_rows_udf_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_settings_test.py` & `lilacai-0.0.5/lilacai/data/dataset_settings_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_stats_test.py` & `lilacai-0.0.5/lilacai/data/dataset_stats_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_test.py` & `lilacai-0.0.5/lilacai/data/dataset_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_test_utils.py` & `lilacai-0.0.5/lilacai/data/dataset_test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_utils.py` & `lilacai-0.0.5/lilacai/data/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/dataset_utils_test.py` & `lilacai-0.0.5/lilacai/data/dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/duckdb_utils.py` & `lilacai-0.0.5/lilacai/data/duckdb_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/csv_source.py` & `lilacai-0.0.5/lilacai/data/sources/csv_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/csv_source_test.py` & `lilacai-0.0.5/lilacai/data/sources/csv_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/default_sources.py` & `lilacai-0.0.5/lilacai/data/sources/default_sources.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/gmail_source.py` & `lilacai-0.0.5/lilacai/data/sources/gmail_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/huggingface_source.py` & `lilacai-0.0.5/lilacai/data/sources/huggingface_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/huggingface_source_test.py` & `lilacai-0.0.5/lilacai/data/sources/huggingface_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/json_source.py` & `lilacai-0.0.5/lilacai/data/sources/json_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/json_source_test.py` & `lilacai-0.0.5/lilacai/data/sources/json_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/pandas_source.py` & `lilacai-0.0.5/lilacai/data/sources/pandas_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/pandas_source_test.py` & `lilacai-0.0.5/lilacai/data/sources/pandas_source_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/reddit_hf_source.py` & `lilacai-0.0.5/lilacai/data/sources/reddit_hf_source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/source.py` & `lilacai-0.0.5/lilacai/data/sources/source.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/source_registry.py` & `lilacai-0.0.5/lilacai/data/sources/source_registry.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data/sources/source_registry_test.py` & `lilacai-0.0.5/lilacai/data/sources/source_registry_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data_loader.py` & `lilacai-0.0.5/lilacai/data_loader.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/data_loader_test.py` & `lilacai-0.0.5/lilacai/data_loader_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/db_manager.py` & `lilacai-0.0.5/lilacai/db_manager.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/cohere.py` & `lilacai-0.0.5/lilacai/embeddings/cohere.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/embedding.py` & `lilacai-0.0.5/lilacai/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/embedding_test.py` & `lilacai-0.0.5/lilacai/embeddings/embedding_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/openai.py` & `lilacai-0.0.5/lilacai/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/palm.py` & `lilacai-0.0.5/lilacai/embeddings/palm.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/sbert.py` & `lilacai-0.0.5/lilacai/embeddings/sbert.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/vector_store.py` & `lilacai-0.0.5/lilacai/embeddings/vector_store.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/vector_store_numpy.py` & `lilacai-0.0.5/lilacai/embeddings/vector_store_numpy.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/embeddings/vector_store_test.py` & `lilacai-0.0.5/lilacai/embeddings/vector_store_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/make_openapi.py` & `lilacai-0.0.5/lilacai/make_openapi.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/parquet_writer.py` & `lilacai-0.0.5/lilacai/parquet_writer.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/router_concept.py` & `lilacai-0.0.5/lilacai/router_concept.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/router_data_loader.py` & `lilacai-0.0.5/lilacai/router_data_loader.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/router_dataset.py` & `lilacai-0.0.5/lilacai/router_dataset.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/router_google_login.py` & `lilacai-0.0.5/lilacai/router_google_login.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/router_signal.py` & `lilacai-0.0.5/lilacai/router_signal.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/router_utils.py` & `lilacai-0.0.5/lilacai/router_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/schema.py` & `lilacai-0.0.5/lilacai/schema.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/schema_test.py` & `lilacai-0.0.5/lilacai/schema_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/server.py` & `lilacai-0.0.5/lilacai/server.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/server_concept_test.py` & `lilacai-0.0.5/lilacai/server_concept_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/server_dataset_test.py` & `lilacai-0.0.5/lilacai/server_dataset_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/concept_labels.py` & `lilacai-0.0.5/lilacai/signals/concept_labels.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/concept_labels_test.py` & `lilacai-0.0.5/lilacai/signals/concept_labels_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/concept_scorer.py` & `lilacai-0.0.5/lilacai/signals/concept_scorer.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/concept_scorer_test.py` & `lilacai-0.0.5/lilacai/signals/concept_scorer_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/default_signals.py` & `lilacai-0.0.5/lilacai/signals/default_signals.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/lang_detection.py` & `lilacai-0.0.5/lilacai/signals/lang_detection.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/lang_detection_test.py` & `lilacai-0.0.5/lilacai/signals/lang_detection_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/minhash_dup.py` & `lilacai-0.0.5/lilacai/signals/minhash_dup.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/near_dup.py` & `lilacai-0.0.5/lilacai/signals/near_dup.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/near_dup_test.py` & `lilacai-0.0.5/lilacai/signals/near_dup_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/ner.py` & `lilacai-0.0.5/lilacai/signals/ner.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/ner_test.py` & `lilacai-0.0.5/lilacai/signals/ner_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/pii.py` & `lilacai-0.0.5/lilacai/signals/pii.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/pii_ip_address.py` & `lilacai-0.0.5/lilacai/signals/pii_ip_address.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/pii_secrets.py` & `lilacai-0.0.5/lilacai/signals/pii_secrets.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/pii_test.py` & `lilacai-0.0.5/lilacai/signals/pii_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/semantic_similarity.py` & `lilacai-0.0.5/lilacai/signals/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/semantic_similarity_test.py` & `lilacai-0.0.5/lilacai/signals/semantic_similarity_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/signal.py` & `lilacai-0.0.5/lilacai/signals/signal.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/signal_test.py` & `lilacai-0.0.5/lilacai/signals/signal_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter.py` & `lilacai-0.0.5/lilacai/signals/splitters/chunk_splitter.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/splitters/chunk_splitter_test.py` & `lilacai-0.0.5/lilacai/signals/splitters/chunk_splitter_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy.py` & `lilacai-0.0.5/lilacai/signals/splitters/text_splitter_spacy.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/splitters/text_splitter_spacy_test.py` & `lilacai-0.0.5/lilacai/signals/splitters/text_splitter_spacy_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/splitters/text_splitter_test_utils.py` & `lilacai-0.0.5/lilacai/signals/splitters/text_splitter_test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/substring_search.py` & `lilacai-0.0.5/lilacai/signals/substring_search.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/substring_search_test.py` & `lilacai-0.0.5/lilacai/signals/substring_search_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/text_statistics.py` & `lilacai-0.0.5/lilacai/signals/text_statistics.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/signals/text_statistics_test.py` & `lilacai-0.0.5/lilacai/signals/text_statistics_test.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/tasks.py` & `lilacai-0.0.5/lilacai/tasks.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/test_utils.py` & `lilacai-0.0.5/lilacai/test_utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/lilacai/utils.py` & `lilacai-0.0.5/lilacai/utils.py`

 * *Files identical despite different names*

### Comparing `lilacai-0.0.4/pyproject.toml` & `lilacai-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Lilac AI Inc. <info@lilacml.com>"]
 description = "Organize unstructured data"
 license = "Apache-2.0"
 name = "lilacai"
 packages = [{include = "lilacai"}]
 readme = "README.md"
-version = "0.0.4"
+version = "0.0.5"
 
 [tool.poetry.dependencies]
 
 ### Required dependencies. ###
 authlib = "^1.2.1"
 dask = "^2023.3.2"
 datasets = "^2.12.0"
```

### Comparing `lilacai-0.0.4/PKG-INFO` & `lilacai-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilacai
-Version: 0.0.4
+Version: 0.0.5
 Summary: Organize unstructured data
 License: Apache-2.0
 Author: Lilac AI Inc.
 Author-email: info@lilacml.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -159,14 +159,23 @@
 ```py
 import string
 import random
 key = ''.join(random.choices(string.ascii_uppercase + string.digits, k=64))
 print(f"LILAC_OAUTH_SECRET_KEY='{key}'")
 ```
 
+### Publishing on pip
+
+To authenticate, add the `PYPI_TOKEN` to your `.env.local` file. You can get the token from
+[pypi.org](https://pypi.org/manage/project/lilacai/settings/). Then run the following script:
+
+```sh
+./scripts/publish_pip.sh
+```
+
 ### Configuration
 
 To use various API's, API keys need to be provided. Create a file named `.env.local` in the root, and add variables that are listed in `.env` with your own values.
 
 #### Testing
 
 Run all the checks before mailing:
```

