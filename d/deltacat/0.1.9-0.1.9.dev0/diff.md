# Comparing `tmp/deltacat-0.1.9.tar.gz` & `tmp/deltacat-0.1.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltacat-0.1.9.tar", last modified: Thu Jan 19 23:27:55 2023, max compression
+gzip compressed data, was "dist/deltacat-0.1.9.dev0.tar", last modified: Wed Feb  8 23:07:26 2023, max compression
```

## Comparing `deltacat-0.1.9.tar` & `deltacat-0.1.9.dev0.tar`

### file list

```diff
@@ -1,145 +1,144 @@
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.786885 deltacat-0.1.9/
--rw-r--r--   0 rootliu    (504) staff       (20)    11357 2022-10-10 21:31:22.000000 deltacat-0.1.9/LICENSE
--rw-r--r--   0 rootliu    (504) staff       (20)       24 2023-01-04 22:20:29.000000 deltacat-0.1.9/MANIFEST.in
--rw-r--r--   0 rootliu    (504) staff       (20)     1101 2023-01-19 23:27:55.786714 deltacat-0.1.9/PKG-INFO
--rw-r--r--   0 rootliu    (504) staff       (20)      484 2022-12-15 05:32:50.000000 deltacat-0.1.9/README.md
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.756351 deltacat-0.1.9/deltacat/
--rw-r--r--   0 rootliu    (504) staff       (20)     1675 2023-01-19 23:27:44.000000 deltacat-0.1.9/deltacat/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.758495 deltacat-0.1.9/deltacat/aws/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/aws/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1936 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/aws/clients.py
--rw-r--r--   0 rootliu    (504) staff       (20)      204 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/aws/constants.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.758877 deltacat-0.1.9/deltacat/aws/redshift/
--rw-r--r--   0 rootliu    (504) staff       (20)      247 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/aws/redshift/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.759218 deltacat-0.1.9/deltacat/aws/redshift/model/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/aws/redshift/model/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     9575 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/aws/redshift/model/manifest.py
--rw-r--r--   0 rootliu    (504) staff       (20)    18817 2023-01-13 01:15:59.000000 deltacat-0.1.9/deltacat/aws/s3u.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.759864 deltacat-0.1.9/deltacat/catalog/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/catalog/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     9272 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/catalog/delegate.py
--rw-r--r--   0 rootliu    (504) staff       (20)     6783 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/catalog/interface.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.760598 deltacat-0.1.9/deltacat/catalog/model/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/catalog/model/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2270 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/catalog/model/catalog.py
--rw-r--r--   0 rootliu    (504) staff       (20)      697 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/catalog/model/table_definition.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.760775 deltacat-0.1.9/deltacat/compute/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.761093 deltacat-0.1.9/deltacat/compute/compactor/
--rw-r--r--   0 rootliu    (504) staff       (20)     1103 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)    26126 2023-01-19 23:26:30.000000 deltacat-0.1.9/deltacat/compute/compactor/compaction_session.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.762689 deltacat-0.1.9/deltacat/compute/compactor/model/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7599 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/model/delta_annotated.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1855 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/model/delta_file_envelope.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1736 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/delta_file_locator.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1267 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/materialize_result.py
--rw-r--r--   0 rootliu    (504) staff       (20)    10524 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/primary_key_index.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1343 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/pyarrow_write_result.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2755 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/round_completion_info.py
--rw-r--r--   0 rootliu    (504) staff       (20)     4062 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/model/sort_key.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.763765 deltacat-0.1.9/deltacat/compute/compactor/steps/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)    16277 2023-01-14 01:00:57.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/dedupe.py
--rw-r--r--   0 rootliu    (504) staff       (20)     6636 2023-01-14 01:00:09.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/hash_bucket.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7272 2023-01-14 01:28:07.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/materialize.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.764375 deltacat-0.1.9/deltacat/compute/compactor/steps/rehash/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/rehash/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1794 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/rehash/rehash_bucket.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1869 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/steps/rehash/rewrite_index.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.765460 deltacat-0.1.9/deltacat/compute/compactor/utils/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/compactor/utils/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     9678 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/utils/io.py
--rw-r--r--   0 rootliu    (504) staff       (20)    10864 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/utils/primary_key_index.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2116 2022-11-07 23:46:50.000000 deltacat-0.1.9/deltacat/compute/compactor/utils/round_completion_file.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7003 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/compactor/utils/system_columns.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.766005 deltacat-0.1.9/deltacat/compute/metastats/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.766190 deltacat-0.1.9/deltacat/compute/metastats/config/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/config/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)    20588 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/meta_stats.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.769209 deltacat-0.1.9/deltacat/compute/metastats/model/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/model/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1405 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/model/partition_stats_dict.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2766 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7375 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/stats.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.770570 deltacat-0.1.9/deltacat/compute/metastats/utils/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/utils/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)      869 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/utils/constants.py
--rw-r--r--   0 rootliu    (504) staff       (20)     8531 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/utils/io.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1135 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
--rw-r--r--   0 rootliu    (504) staff       (20)     4591 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/metastats/utils/ray_utils.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.771390 deltacat-0.1.9/deltacat/compute/stats/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     9415 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/basic.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.772789 deltacat-0.1.9/deltacat/compute/stats/models/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/models/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3296 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/stats/models/delta_column_stats.py
--rw-r--r--   0 rootliu    (504) staff       (20)     8711 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/stats/models/delta_stats.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1609 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/models/delta_stats_cache_result.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2363 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/stats/models/manifest_entry_stats.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3753 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/stats/models/stats_result.py
--rw-r--r--   0 rootliu    (504) staff       (20)      215 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/types.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.773591 deltacat-0.1.9/deltacat/compute/stats/utils/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/utils/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3049 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/utils/intervals.py
--rw-r--r--   0 rootliu    (504) staff       (20)     8587 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/compute/stats/utils/io.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3811 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/compute/stats/utils/manifest_stats_file.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1092 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/constants.py
--rw-r--r--   0 rootliu    (504) staff       (20)      146 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/exceptions.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.774568 deltacat-0.1.9/deltacat/io/
--rw-r--r--   0 rootliu    (504) staff       (20)      153 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/io/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.778970 deltacat-0.1.9/deltacat/io/aws/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/io/aws/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.779436 deltacat-0.1.9/deltacat/io/aws/redshift/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/io/aws/redshift/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)    22765 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/io/aws/redshift/redshift_datasource.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3821 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/io/dataset.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7109 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/io/read_api.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3879 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/logs.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.780101 deltacat-0.1.9/deltacat/storage/
--rw-r--r--   0 rootliu    (504) staff       (20)     1337 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/storage/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)    22080 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/storage/interface.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.782282 deltacat-0.1.9/deltacat/storage/model/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/storage/model/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)    13912 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/storage/model/delta.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2445 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/storage/model/list_result.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1296 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/storage/model/locator.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2108 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/storage/model/namespace.py
--rw-r--r--   0 rootliu    (504) staff       (20)    11165 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/storage/model/partition.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7818 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/storage/model/stream.py
--rw-r--r--   0 rootliu    (504) staff       (20)     4252 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/storage/model/table.py
--rw-r--r--   0 rootliu    (504) staff       (20)     7086 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/storage/model/table_version.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1579 2023-01-10 04:24:58.000000 deltacat-0.1.9/deltacat/storage/model/types.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.782579 deltacat-0.1.9/deltacat/tests/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/tests/__init__.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.782866 deltacat-0.1.9/deltacat/tests/stats/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/tests/stats/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2137 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/tests/stats/test_intervals.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.783388 deltacat-0.1.9/deltacat/types/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/types/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2186 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/types/media.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3814 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/types/tables.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.784986 deltacat-0.1.9/deltacat/utils/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/utils/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1449 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/utils/common.py
--rw-r--r--   0 rootliu    (504) staff       (20)     2094 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/utils/numpy.py
--rw-r--r--   0 rootliu    (504) staff       (20)    10067 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/utils/pandas.py
--rw-r--r--   0 rootliu    (504) staff       (20)      670 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/utils/performance.py
--rw-r--r--   0 rootliu    (504) staff       (20)     8868 2023-01-19 23:17:45.000000 deltacat-0.1.9/deltacat/utils/placement.py
--rw-r--r--   0 rootliu    (504) staff       (20)    10611 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/utils/pyarrow.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.786342 deltacat-0.1.9/deltacat/utils/ray_utils/
--rw-r--r--   0 rootliu    (504) staff       (20)        0 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/utils/ray_utils/__init__.py
--rw-r--r--   0 rootliu    (504) staff       (20)     1950 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/utils/ray_utils/collections.py
--rw-r--r--   0 rootliu    (504) staff       (20)     4906 2023-01-14 00:10:07.000000 deltacat-0.1.9/deltacat/utils/ray_utils/concurrency.py
--rw-r--r--   0 rootliu    (504) staff       (20)     3319 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/utils/ray_utils/dataset.py
--rw-r--r--   0 rootliu    (504) staff       (20)      515 2022-10-10 21:31:22.000000 deltacat-0.1.9/deltacat/utils/ray_utils/performance.py
--rw-r--r--   0 rootliu    (504) staff       (20)     4810 2023-01-04 22:20:29.000000 deltacat-0.1.9/deltacat/utils/ray_utils/runtime.py
-drwxr-xr-x   0 rootliu    (504) staff       (20)        0 2023-01-19 23:27:55.757485 deltacat-0.1.9/deltacat.egg-info/
--rw-r--r--   0 rootliu    (504) staff       (20)     1101 2023-01-19 23:27:55.000000 deltacat-0.1.9/deltacat.egg-info/PKG-INFO
--rw-r--r--   0 rootliu    (504) staff       (20)     4319 2023-01-19 23:27:55.000000 deltacat-0.1.9/deltacat.egg-info/SOURCES.txt
--rw-r--r--   0 rootliu    (504) staff       (20)        1 2023-01-19 23:27:55.000000 deltacat-0.1.9/deltacat.egg-info/dependency_links.txt
--rw-r--r--   0 rootliu    (504) staff       (20)      151 2023-01-19 23:27:55.000000 deltacat-0.1.9/deltacat.egg-info/requires.txt
--rw-r--r--   0 rootliu    (504) staff       (20)        9 2023-01-19 23:27:55.000000 deltacat-0.1.9/deltacat.egg-info/top_level.txt
--rw-r--r--   0 rootliu    (504) staff       (20)       38 2023-01-19 23:27:55.786935 deltacat-0.1.9/setup.cfg
--rw-r--r--   0 rootliu    (504) staff       (20)     1924 2023-01-18 00:52:37.000000 deltacat-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/redshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/aws/redshift/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/redshift/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9575 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/redshift/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/aws/s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9272 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/catalog/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/catalog/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/catalog/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/catalog/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/catalog/model/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/catalog/model/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/compaction_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/delta_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/delta_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/delta_file_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/materialize_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10524 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/pyarrow_write_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/round_completion_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/model/sort_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5953 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/materialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/rehash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/rehash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/rehash/rehash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/rehash/rewrite_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12491 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/round_completion_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/system_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20588 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/meta_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/model/partition_stats_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/ray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9415 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:43.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/delta_column_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/delta_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/delta_stats_cache_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/manifest_entry_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/models/stats_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/compute/stats/utils/manifest_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/io/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/io/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/io/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/io/aws/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22765 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/io/aws/redshift/redshift_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/io/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22080 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/storage/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/list_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/table_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/storage/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/tests/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/tests/stats/test_intervals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/placement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/deltacat/utils/ray_utils/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/deltacat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 23:07:26.000000 deltacat-0.1.9.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-02-08 23:06:44.000000 deltacat-0.1.9.dev0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `deltacat-0.1.9/PKG-INFO` & `deltacat-0.1.9.dev0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 0.1.9
+Version: 0.1.9.dev0
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
+License: UNKNOWN
+Description: # DeltaCAT
+        
+        DeltaCAT is a Pythonic Data Catalog powered by Ray.
+        
+        Its data storage model allows you to define and manage fast, scalable,
+        ACID-compliant data catalogs through git-like stage/commit APIs, and has been
+        used to successfully host exabyte-scale enterprise data lakes.
+        
+        DeltaCAT uses the Ray distributed compute framework together with Apache Arrow
+        for common table management tasks, including petabyte-scale
+        change-data-capture, data consistency checks, and table repair.
+        
+        ## Getting Started
+        ---
+        ### Install
+        ```
+        pip install deltacat
+        ```
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DeltaCAT
-
-DeltaCAT is a Pythonic Data Catalog powered by Ray.
-
-Its data storage model allows you to define and manage fast, scalable, 
-ACID-compliant data catalogs through git-like stage/commit APIs, and has been 
-used to successfully host exabyte-scale enterprise data lakes.
-
-DeltaCAT uses the Ray distributed compute framework together with Apache Arrow
-for common table management tasks, including petabyte-scale 
-change-data-capture, data consistency checks, and table repair.
```

### Comparing `deltacat-0.1.9/deltacat/__init__.py` & `deltacat-0.1.9.dev0/deltacat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     refresh_table, list_tables, get_table, truncate_table, rename_table, \
     table_exists, list_namespaces, alter_namespace, create_namespace, \
     drop_namespace, default_namespace, get_namespace, namespace_exists, \
     write_to_table, read_table
 
 logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-__version__ = "0.1.9"
+__version__ = "0.1.9.dev0"
 
 
 __all__ = [
     "__version__",
     "all_catalogs",
     "alter_table",
     "create_table",
```

### Comparing `deltacat-0.1.9/deltacat/aws/clients.py` & `deltacat-0.1.9.dev0/deltacat/aws/clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/aws/redshift/model/manifest.py` & `deltacat-0.1.9.dev0/deltacat/aws/redshift/model/manifest.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/aws/s3u.py` & `deltacat-0.1.9.dev0/deltacat/aws/s3u.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 from botocore.client import BaseClient
 from botocore.exceptions import ClientError
 from tenacity import Retrying
 from tenacity import wait_random_exponential
 from tenacity import stop_after_delay
 from tenacity import retry_if_exception_type, retry_if_not_exception_type
 
-from typing import Any, Callable, Dict, List, Optional, Generator, Union, Tuple
+from typing import Any, Callable, Dict, List, Optional, Generator, Union
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-
-@ray.remote
+# TODO(raghumdani): refactor redshift datasource to reuse the 
+# same module for writing output files.
 class CapturedBlockWritePaths:
     def __init__(self):
         self._write_paths: List[str] = []
         self._block_refs: List[ObjectRef[Block]] = []
 
     def extend(
             self,
@@ -66,22 +66,22 @@
         return self._block_refs
 
 
 class UuidBlockWritePathProvider(BlockWritePathProvider):
     """Block write path provider implementation that writes each
     dataset block out to a file of the form: {base_path}/{uuid}
     """
-    def __init__(self, capture_actor: CapturedBlockWritePaths):
+    def __init__(self, capture_object: CapturedBlockWritePaths):
         self.write_paths: List[str] = []
         self.block_refs: List[ObjectRef[Block]] = []
-        self.capture_actor = capture_actor
+        self.capture_object = capture_object
 
     def __del__(self):
         if self.write_paths or self.block_refs:
-            self.capture_actor.extend.remote(
+            self.capture_object.extend(
                 self.write_paths,
                 self.block_refs,
             )
 
     def _get_write_path_for_block(
             self,
             base_path: str,
@@ -353,28 +353,28 @@
     """
     Writes the given table to 1 or more S3 files and return Redshift
     manifest entries describing the uploaded files.
     """
     if s3_table_writer_kwargs is None:
         s3_table_writer_kwargs = {}
 
-    capture_actor = CapturedBlockWritePaths.remote()
-    block_write_path_provider = UuidBlockWritePathProvider(capture_actor)
+    capture_object = CapturedBlockWritePaths()
+    block_write_path_provider = UuidBlockWritePathProvider(capture_object)
     s3_table_writer_func(
         table,
         s3_base_url,
         s3_file_system,
         block_write_path_provider,
         content_type.value,
         **s3_table_writer_kwargs
     )
     # TODO: Add a proper fix for block_refs and write_paths not persisting in Ray actors
     del block_write_path_provider
-    block_refs = ray.get(capture_actor.block_refs.remote())
-    write_paths = ray.get(capture_actor.write_paths.remote())
+    block_refs = capture_object.block_refs()
+    write_paths = capture_object.write_paths()
     metadata = _get_metadata(table, write_paths, block_refs)
     manifest_entries = ManifestEntryList()
     for block_idx, s3_url in enumerate(write_paths):
         try:
             manifest_entry = ManifestEntry.from_s3_obj_url(
                 s3_url,
                 metadata[block_idx].num_rows,
@@ -440,46 +440,30 @@
     return table
 
 
 def _download_manifest_entries(
         manifest: Manifest,
         token_holder: Optional[Dict[str, Any]] = None,
         table_type: TableType = TableType.PYARROW,
-        ignore_missing_manifest: bool = False,
         column_names: Optional[List[str]] = None,
         include_columns: Optional[List[str]] = None,
         file_reader_kwargs_provider: Optional[ReadKwargsProvider] = None) \
-        -> Tuple[LocalDataset,Optional[List[int]]]:
+        -> LocalDataset:
 
-    if ignore_missing_manifest:
-        result = []
-        missing = []
-        for ide, e in enumerate(manifest.entries):
-            try: 
-                tmp = download_manifest_entry(e, token_holder, table_type, column_names,
-                                        include_columns, file_reader_kwargs_provider)
-                result.append(tmp)
-            except Exception as e:
-                missing.append(ide)
-                logger.info(f"missing {len(missing)} manifest_entry")
-                pass
+    return [
+        download_manifest_entry(e, token_holder, table_type, column_names,
+                                include_columns, file_reader_kwargs_provider)
+        for e in manifest.entries
+    ]
 
-        return result, missing
-    else:
-        return [
-            download_manifest_entry(e, token_holder, table_type, column_names,
-                                    include_columns, file_reader_kwargs_provider)
-            for e in manifest.entries
-        ]
 
 def _download_manifest_entries_parallel(
         manifest: Manifest,
         token_holder: Optional[Dict[str, Any]] = None,
         table_type: TableType = TableType.PYARROW,
-        ignore_missing_manifest: bool = False,
         max_parallelism: Optional[int] = None,
         column_names: Optional[List[str]] = None,
         include_columns: Optional[List[str]] = None,
         file_reader_kwargs_provider: Optional[ReadKwargsProvider] = None) \
         -> LocalDataset:
 
     tables = []
@@ -497,37 +481,34 @@
     return tables
 
 
 def download_manifest_entries(
         manifest: Manifest,
         token_holder: Optional[Dict[str, Any]] = None,
         table_type: TableType = TableType.PYARROW,
-        ignore_missing_manifest: bool = False,
         max_parallelism: Optional[int] = 1,
         column_names: Optional[List[str]] = None,
         include_columns: Optional[List[str]] = None,
         file_reader_kwargs_provider: Optional[ReadKwargsProvider] = None) \
-        -> Tuple[LocalDataset,Optional[List[int]]]:
+        -> LocalDataset:
 
     if max_parallelism and max_parallelism <= 1:
         return _download_manifest_entries(
             manifest,
             token_holder,
             table_type,
-            ignore_missing_manifest,
             column_names,
             include_columns,
             file_reader_kwargs_provider,
         )
     else:
         return _download_manifest_entries_parallel(
             manifest,
             token_holder,
             table_type,
-            ignore_missing_manifest,
             max_parallelism,
             column_names,
             include_columns,
             file_reader_kwargs_provider,
         )
```

### Comparing `deltacat-0.1.9/deltacat/catalog/delegate.py` & `deltacat-0.1.9.dev0/deltacat/catalog/delegate.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/catalog/interface.py` & `deltacat-0.1.9.dev0/deltacat/catalog/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/catalog/model/catalog.py` & `deltacat-0.1.9.dev0/deltacat/catalog/model/catalog.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/catalog/model/table_definition.py` & `deltacat-0.1.9.dev0/deltacat/catalog/model/table_definition.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/__init__.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/delta_annotated.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/delta_annotated.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/delta_file_envelope.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/delta_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/delta_file_locator.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/delta_file_locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/materialize_result.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/materialize_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/primary_key_index.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/pyarrow_write_result.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/pyarrow_write_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/round_completion_info.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/round_completion_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/model/sort_key.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/model/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/steps/hash_bucket.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/hash_bucket.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,26 +24,26 @@
 
 _PK_BYTES_DELIMITER = b'L6kl7u5f'
 
 HashBucketGroupToObjectId = np.ndarray
 HashBucketResult = Tuple[HashBucketGroupToObjectId, List[ObjectRef[DeltaFileEnvelopeGroups]]]
 
 
-def group_by_pk_hash_bucket(
+def _group_by_pk_hash_bucket(
         table: pa.Table,
         num_buckets: int,
         primary_keys: List[str]) -> np.ndarray:
 
     # generate the primary key digest column
     all_pk_column_fields = []
     for pk_name in primary_keys:
         # casting a primary key column to numpy also ensures no nulls exist
         column_fields = table[pk_name].to_numpy()
         all_pk_column_fields.append(column_fields)
-    hash_column_generator = hash_pk_bytes_generator(all_pk_column_fields)
+    hash_column_generator = _hash_pk_bytes_generator(all_pk_column_fields)
     table = sc.append_pk_hash_column(table, hash_column_generator)
 
     # drop primary key columns to free up memory
     table = table.drop(primary_keys)
 
     # group hash bucket record indices
     hash_bucket_to_indices = group_record_indices_by_hash_bucket(
@@ -58,48 +58,46 @@
             hash_bucket_to_table[hb] = sc.append_record_idx_col(
                 table.take(indices),
                 indices,
             )
     return hash_bucket_to_table
 
 
-def hash_pk_bytes_generator(all_column_fields) -> Generator[bytes, None, None]:
+def _hash_pk_bytes_generator(all_column_fields) -> Generator[bytes, None, None]:
     for field_index in range(len(all_column_fields[0])):
         bytes_to_join = []
         for column_fields in all_column_fields:
             bytes_to_join.append(
                 bytes(str(column_fields[field_index]), "utf-8")
             )
         yield sha1_digest(_PK_BYTES_DELIMITER.join(bytes_to_join))
 
 
-def group_file_records_by_pk_hash_bucket(
+def _group_file_records_by_pk_hash_bucket(
         annotated_delta: DeltaAnnotated,
         num_hash_buckets: int,
         primary_keys: List[str],
         sort_key_names: List[str],
-        ignore_missing_manifest: bool = False,
         deltacat_storage=unimplemented_deltacat_storage) \
         -> Optional[DeltaFileEnvelopeGroups]:
 
     # read input parquet s3 objects into a list of delta file envelopes
-    delta_file_envelopes = read_delta_file_envelopes(
+    delta_file_envelopes = _read_delta_file_envelopes(
         annotated_delta,
         primary_keys,
         sort_key_names,
-        ignore_missing_manifest,
         deltacat_storage,
     )
     if delta_file_envelopes is None:
         return None
 
     # group the data by primary key hash value
     hb_to_delta_file_envelopes = np.empty([num_hash_buckets], dtype="object")
     for dfe in delta_file_envelopes:
-        hash_bucket_to_table = group_by_pk_hash_bucket(
+        hash_bucket_to_table = _group_by_pk_hash_bucket(
             dfe.table,
             num_hash_buckets,
             primary_keys,
         )
         for hb, table in enumerate(hash_bucket_to_table):
             if table:
                 if hb_to_delta_file_envelopes[hb] is None:
@@ -108,42 +106,29 @@
                     DeltaFileEnvelope.of(
                         dfe.stream_position,
                         dfe.file_index,
                         dfe.delta_type,
                         table))
     return hb_to_delta_file_envelopes
 
-
-def read_delta_file_envelopes(
+def _read_delta_file_envelopes(
         annotated_delta: DeltaAnnotated,
         primary_keys: List[str],
         sort_key_names: List[str],
-        ignore_missing_manifest: bool = False,
         deltacat_storage=unimplemented_deltacat_storage) \
         -> Optional[List[DeltaFileEnvelope]]:
 
     columns_to_read = list(chain(primary_keys, sort_key_names))
-    missing_ids=[]
-    tables_and_missing_ids = deltacat_storage.download_delta(
+    tables = deltacat_storage.download_delta(
         annotated_delta,
-        max_parallelism=1, # if >1, will use python multiprocessing
+        max_parallelism=1,
         columns=columns_to_read,
         storage_type=StorageType.LOCAL,
-        ignore_missing_manifest=ignore_missing_manifest,
     )
-    if ignore_missing_manifest:
-        missing_ids = tables_and_missing_ids[1]
-        tables=tables_and_missing_ids[0]
-    else:
-        tables = tables_and_missing_ids
     annotations = annotated_delta.annotations
-    if len(missing_ids)>0:
-        print(f"missing files:{len(missing_ids)}")
-        for id_missing in sorted(missing_ids, reverse=True):
-            del annotations[id_missing]
     assert(len(tables) == len(annotations),
            f"Unexpected Error: Length of downloaded delta manifest tables "
            f"({len(tables)}) doesn't match the length of delta manifest "
            f"annotations ({len(annotations)}).")
     if not tables:
         return None
 
@@ -162,25 +147,23 @@
 @ray.remote(num_returns=2)
 def hash_bucket(
         annotated_delta: DeltaAnnotated,
         primary_keys: List[str],
         sort_keys: List[SortKey],
         num_buckets: int,
         num_groups: int,
-        ignore_missing_manifest: bool = False,
         deltacat_storage=unimplemented_deltacat_storage) -> HashBucketResult:
 
     logger.info(f"Starting hash bucket task...")
     sort_key_names = [key.key_name for key in sort_keys]
-    delta_file_envelope_groups = group_file_records_by_pk_hash_bucket(
+    delta_file_envelope_groups = _group_file_records_by_pk_hash_bucket(
         annotated_delta,
         num_buckets,
         primary_keys,
         sort_key_names,
-        ignore_missing_manifest,
         deltacat_storage,
     )
     hash_bucket_group_to_obj_id, object_refs = group_hash_bucket_indices(
         delta_file_envelope_groups,
         num_buckets,
         num_groups,
     )
```

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/steps/materialize.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/materialize.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,39 @@
-import logging,time
+import logging
 import ray
 import pyarrow as pa
 
 from collections import defaultdict
-
-from deltacat.compute.compactor.steps.dedupe import DedupeTaskIndexWithObjectId, \
-    DeltaFileLocatorToRecords
 from itertools import chain, repeat
+from typing import List, Optional, Tuple
 
+import pyarrow as pa
+import ray
 from pyarrow import compute as pc
-
 from ray import cloudpickle
 
 from deltacat import logs
-from deltacat.storage import Delta, DeltaLocator, Partition, PartitionLocator, \
-    interface as unimplemented_deltacat_storage
-from deltacat.compute.compactor import MaterializeResult, PyArrowWriteResult, \
-    RoundCompletionInfo
+from deltacat.compute.compactor import (
+    MaterializeResult,
+    PyArrowWriteResult,
+    RoundCompletionInfo,
+)
+from deltacat.compute.compactor.steps.dedupe import (
+    DedupeTaskIndexWithObjectId,
+    DeltaFileLocatorToRecords,
+)
 from deltacat.compute.compactor.utils import system_columns as sc
-from deltacat.types.media import ContentType, DELIMITED_TEXT_CONTENT_TYPES
-from typing import List, Tuple, Optional
-
-from deltacat.utils.pyarrow import ReadKwargsProviderPyArrowSchemaOverride
-
+from deltacat.storage import Delta, DeltaLocator, Partition, PartitionLocator
+from deltacat.storage import interface as unimplemented_deltacat_storage
+from deltacat.types.media import DELIMITED_TEXT_CONTENT_TYPES, ContentType
 from deltacat.types.tables import TABLE_CLASS_TO_SIZE_FUNC
-from deltacat.utils.pyarrow import ReadKwargsProviderPyArrowCsvPureUtf8
+from deltacat.utils.pyarrow import (
+    ReadKwargsProviderPyArrowCsvPureUtf8,
+    ReadKwargsProviderPyArrowSchemaOverride,
+)
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
 @ray.remote
 def materialize(
         source_partition_locator: PartitionLocator,
@@ -37,20 +42,66 @@
         mat_bucket_index: int,
         dedupe_task_idx_and_obj_id_tuples: List[DedupeTaskIndexWithObjectId],
         max_records_per_output_file: int,
         compacted_file_content_type: ContentType,
         schema: Optional[pa.Schema] = None,
         deltacat_storage=unimplemented_deltacat_storage) -> MaterializeResult:
 
+    def _materialize(
+            compacted_tables: List[pa.Table],
+            compacted_tables_record_count: int) -> MaterializeResult:
+        compacted_tables_size = sum([TABLE_CLASS_TO_SIZE_FUNC[type(tbl)](tbl)
+                                     for tbl in compacted_tables])
+        logger.debug(f"Uploading {len(compacted_tables)} compacted tables "
+                     f"with size: {compacted_tables_size} bytes "
+                     f"and record count: {compacted_tables_record_count}")
+        compacted_table = pa.concat_tables(compacted_tables)
+        if compacted_file_content_type in DELIMITED_TEXT_CONTENT_TYPES:
+            # TODO (ricmiyam): Investigate if we still need to convert this table to pandas DataFrame
+            # TODO (pdames): compare performance to pandas-native materialize path
+            df = compacted_table.to_pandas(
+                split_blocks=True,
+                self_destruct=True,
+                zero_copy_only=True
+            )
+            compacted_table = df
+        delta = deltacat_storage.stage_delta(
+            compacted_table,
+            partition,
+            max_records_per_entry=max_records_per_output_file,
+            content_type=compacted_file_content_type,
+        )
+        manifest = delta.manifest
+        manifest_records = manifest.meta.record_count
+        assert(manifest_records == len(compacted_table),
+               f"Unexpected Error: Materialized delta manifest record count "
+               f"({manifest_records}) does not equal compacted table record count "
+               f"({len(compacted_table)})")
+
+        materialize_result = MaterializeResult.of(
+            delta,
+            mat_bucket_index,
+            # TODO (pdames): Generalize WriteResult to contain in-memory-table-type
+            #  and in-memory-table-bytes instead of tight coupling to paBytes
+            PyArrowWriteResult.of(
+                len(manifest.entries),
+                TABLE_CLASS_TO_SIZE_FUNC[type(compacted_table)](compacted_table),
+                manifest.meta.content_length,
+                len(compacted_table),
+            ),
+        )
+        logger.info(f"Materialize result: {materialize_result}")
+        return materialize_result
+
     logger.info(f"Starting materialize task...")
     dedupe_task_idx_and_obj_ref_tuples = [
         (
-            t[0],
-            cloudpickle.loads(t[1])
-        ) for t in dedupe_task_idx_and_obj_id_tuples
+            t1,
+            cloudpickle.loads(t2),
+        ) for t1, t2 in dedupe_task_idx_and_obj_id_tuples
     ]
     logger.info(f"Resolved materialize task obj refs...")
     dedupe_task_indices, obj_refs = zip(
         *dedupe_task_idx_and_obj_ref_tuples
     )
     # this depends on `ray.get` result order matching input order, as per the
     # contract established in: https://github.com/ray-project/ray/pull/16763
@@ -60,14 +111,16 @@
         dedupe_task_idx = dedupe_task_indices[i]
         for src_dfl, record_numbers in src_file_records.items():
             all_src_file_records[src_dfl].append(
                 (record_numbers, repeat(dedupe_task_idx, len(record_numbers)))
             )
     manifest_cache = {}
     compacted_tables = []
+    materialized_results: List[MaterializeResult] = []
+    total_record_count = 0
     for src_dfl in sorted(all_src_file_records.keys()):
         record_numbers_dd_task_idx_tpl_list: List[Tuple[DeltaFileLocatorToRecords, repeat]] = \
             all_src_file_records[src_dfl]
         record_numbers_tpl, dedupe_task_idx_iter_tpl = zip(
             *record_numbers_dd_task_idx_tpl_list
         )
         is_src_partition_file_np = src_dfl.is_source_delta
@@ -95,75 +148,65 @@
         # enforce a consistent schema if provided, when reading files into PyArrow tables
         elif schema is not None:
             read_kwargs_provider = ReadKwargsProviderPyArrowSchemaOverride(
                 schema=schema)
         pa_table = deltacat_storage.download_delta_manifest_entry(
             Delta.of(delta_locator, None, None, None, manifest),
             src_file_idx_np.item(),
-            file_reader_kwargs=read_kwargs_provider,
+            file_reader_kwargs_provider=read_kwargs_provider,
         )
-        mask_pylist = list(repeat(False, len(pa_table)))
+        record_count = len(pa_table)
+        mask_pylist = list(repeat(False, record_count))
         record_numbers = chain.from_iterable(record_numbers_tpl)
+        # TODO(raghumdani): reference the same file URIs while writing the files
+        # instead of copying the data over and creating new files. 
         for record_number in record_numbers:
             mask_pylist[record_number] = True
         mask = pa.array(mask_pylist)
-        compacted_table = pa_table.filter(mask)
+        pa_table = pa_table.filter(mask)
 
         # appending, sorting, taking, and dropping has 2-3X latency of a
         # single filter on average, and thus provides better average
         # performance than repeatedly filtering the table in dedupe task index
         # order
         dedupe_task_indices = chain.from_iterable(dedupe_task_idx_iter_tpl)
-        compacted_table = sc.append_dedupe_task_idx_col(
-            compacted_table,
+        pa_table = sc.append_dedupe_task_idx_col(
+            pa_table,
             dedupe_task_indices,
         )
         pa_sort_keys = [(sc._DEDUPE_TASK_IDX_COLUMN_NAME, "ascending")]
-        compacted_table = compacted_table.take(
-            pc.sort_indices(compacted_table, sort_keys=pa_sort_keys),
+        pa_table = pa_table.take(
+            pc.sort_indices(pa_table, sort_keys=pa_sort_keys),
         )
-        compacted_table = compacted_table.drop(
+        pa_table = pa_table.drop(
             [sc._DEDUPE_TASK_IDX_COLUMN_NAME]
         )
-        compacted_tables.append(compacted_table)
 
-    # TODO (pdames): save memory by writing output files eagerly whenever
-    #  len(compacted_table) >= max_records_per_output_file (but don't write
-    #  partial slices from the compacted_table remainder every time!)
-    compacted_table = pa.concat_tables(compacted_tables)
-    if compacted_file_content_type in DELIMITED_TEXT_CONTENT_TYPES:
-        # convert to pandas since pyarrow doesn't support custom delimiters
-        # and doesn't support utf-8 conversion of all types (e.g. Decimal128)
-        # TODO (pdames): compare performance to pandas-native materialize path
-        df = compacted_table.to_pandas(
-            split_blocks=True,
-            self_destruct=True,
-        )
-        del compacted_table
-        compacted_table = df
-    delta = deltacat_storage.stage_delta(
-        compacted_table,
-        partition,
-        max_records_per_entry=max_records_per_output_file,
-        content_type=compacted_file_content_type,
-    )
-    manifest = delta.manifest
-    manifest_records = manifest.meta.record_count
-    assert(manifest_records == len(compacted_table),
-           f"Unexpected Error: Materialized delta manifest record count "
-           f"({manifest_records}) does not equal compacted table record count "
-           f"({len(compacted_table)})")
-    materialize_result = MaterializeResult.of(
-        delta,
-        mat_bucket_index,
-        # TODO (pdames): Generalize WriteResult to contain in-memory-table-type
-        #  and in-memory-table-bytes instead of tight coupling to paBytes
-        PyArrowWriteResult.of(
-            len(manifest.entries),
-            TABLE_CLASS_TO_SIZE_FUNC[type(compacted_table)](compacted_table),
-            manifest.meta.content_length,
-            len(compacted_table),
-        ),
-    )
-    logger.info(f"Materialize result: {materialize_result}")
+        # Write manifests up to max_records_per_output_file
+        # TODO(raghumdani): Write exactly the same number of records into each file to
+        # produce a read-optimized view of the tables.
+        if compacted_tables and \
+                total_record_count + record_count > max_records_per_output_file:
+            materialized_results.append(_materialize(compacted_tables, total_record_count))
+            # Free up written tables in memory
+            compacted_tables.clear()
+            total_record_count = 0
+
+        total_record_count += record_count
+        compacted_tables.append(pa_table)
+
+    materialized_results.append(_materialize(compacted_tables, total_record_count))
+    # Free up written tables in memory
+    compacted_tables.clear()
+
+    merged_delta = Delta.merge_deltas([mr.delta for mr in materialized_results])
+    assert materialized_results and len(materialized_results) > 0, \
+        f"Expected at least one materialized result in materialize step."
+
+    # Merge all new deltas into one for this materialize bucket index
+    merged_materialize_result = MaterializeResult.of(merged_delta,
+                                                     materialized_results[0].task_index,
+                                                     PyArrowWriteResult.union([mr.pyarrow_write_result
+                                                                               for mr in materialized_results]))
+
     logger.info(f"Finished materialize task...")
-    return materialize_result
+    return merged_materialize_result
```

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/steps/rehash/rehash_bucket.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/rehash/rehash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/steps/rehash/rewrite_index.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/steps/rehash/rewrite_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import ray
 import logging
-import pyarrow as pa
 from collections import defaultdict
-from ray import cloudpickle
-from deltacat import logs
+from typing import Any, List, Tuple
 
+import pyarrow as pa
+import ray
+from ray import cloudpickle
 from ray.types import ObjectRef
 
-from deltacat.compute.compactor import PrimaryKeyIndexVersionLocator, \
-    PyArrowWriteResult
+from deltacat import logs
+from deltacat.compute.compactor import PrimaryKeyIndexVersionLocator, PyArrowWriteResult
 from deltacat.compute.compactor.utils import primary_key_index as pki
 
-from typing import Any, List, Tuple
-
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
 @ray.remote(num_cpus=1, num_returns=2)
 def rewrite_index(
         object_ids: List[Any],
         s3_bucket: str,
```

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/utils/io.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/utils/primary_key_index.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/primary_key_index.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,46 @@
-import logging
 import json
-import ray
-import pyarrow as pa
-import numpy as np
-import s3fs
+import logging
 from collections import defaultdict
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
-from deltacat.utils.common import ReadKwargsProvider
+import numpy as np
+import pyarrow as pa
+import ray
+import s3fs
 from ray import cloudpickle
+from deltacat.constants import PRIMARY_KEY_INDEX_WRITE_BOTO3_CONFIG
+from ray.types import ObjectRef
 
 from deltacat.storage import Manifest, PartitionLocator
-from deltacat.utils.ray_utils.concurrency import invoke_parallel, \
-    round_robin_options_provider
+from deltacat.utils.ray_utils.concurrency import invoke_parallel
 from deltacat.compute.compactor import PyArrowWriteResult, \
     RoundCompletionInfo, PrimaryKeyIndexMeta, PrimaryKeyIndexLocator, \
     PrimaryKeyIndexVersionMeta, PrimaryKeyIndexVersionLocator
+from deltacat import logs
+from deltacat.aws import s3u
+from deltacat.compute.compactor import (
+    PrimaryKeyIndexLocator,
+    PrimaryKeyIndexMeta,
+    PrimaryKeyIndexVersionLocator,
+    PrimaryKeyIndexVersionMeta,
+    PyArrowWriteResult,
+    RoundCompletionInfo,
+)
+from deltacat.compute.compactor.steps.rehash import rehash_bucket as rb
+from deltacat.compute.compactor.steps.rehash import rewrite_index as ri
 from deltacat.compute.compactor.utils import round_completion_file as rcf
 from deltacat.compute.compactor.utils import system_columns as sc
-from deltacat.compute.compactor.steps.rehash import rehash_bucket as rb, \
-    rewrite_index as ri
-from deltacat.types.tables import get_table_writer, get_table_slicer
-from deltacat.types.media import ContentType, ContentEncoding
-from deltacat.aws import s3u
-from deltacat import logs
-
-from typing import Any, Callable, Dict, List, Optional, Tuple
-
-from ray.types import ObjectRef
+from deltacat.storage import Manifest, PartitionLocator
+from deltacat.types.media import ContentEncoding, ContentType
+from deltacat.types.tables import get_table_slicer, get_table_writer
+from deltacat.utils.common import ReadKwargsProvider
+from deltacat.utils.ray_utils.concurrency import (
+    invoke_parallel
+)
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
 def rehash(
         options_provider: Callable[[int, Any], Dict[str, Any]],
         s3_bucket: str,
@@ -185,14 +195,17 @@
     return hash_bucket_to_indices
 
 
 def group_hash_bucket_indices(
         hash_bucket_object_groups: np.ndarray,
         num_buckets: int,
         num_groups: int) -> Tuple[np.ndarray, List[ObjectRef]]:
+    """
+    Groups all the ObjectRef that belongs to a particular hash bucket group and hash bucket index. 
+    """
 
     object_refs = []
     hash_bucket_group_to_obj_id = np.empty([num_groups], dtype="object")
 
     if hash_bucket_object_groups is None:
         return hash_bucket_group_to_obj_id, object_refs
 
@@ -202,25 +215,39 @@
             hb_group = hb_index % num_groups
             if hb_group_to_object[hb_group] is None:
                 hb_group_to_object[hb_group] = np.empty(
                     [num_buckets], dtype="object")
             hb_group_to_object[hb_group][hb_index] = obj
 
     for hb_group, obj in enumerate(hb_group_to_object):
-        if obj is not None:
-            obj_ref = ray.put(obj)
-            object_refs.append(obj_ref)
-            hash_bucket_group_to_obj_id[hb_group] = cloudpickle.dumps(obj_ref)
-
+        if obj is None:
+            continue
+        obj_ref = ray.put(obj)
+        pickled_obj_ref = cloudpickle.dumps(obj_ref)
+        object_refs.append(pickled_obj_ref)
+        hash_bucket_group_to_obj_id[hb_group] = pickled_obj_ref
+        # NOTE: The cloudpickle.dumps API call creates an out of band object reference to the object_ref variable. 
+        # After pickling, Ray cannot track the serialized copy of the object or determine when the ObjectRef has been deserialized 
+        # (e.g., if the ObjectRef is deserialized by a non-Ray process). 
+        # Thus the object_ref cannot be tracked by Ray's distributed reference counter, even if it goes out of scope. 
+        # The object now has a permanent reference and the data can't be freed from Ray’s object store. 
+        # Manually deleting the untrackable object references offsets these permanent references and 
+        # helps to allow these objects to be garbage collected normally. 
+        del obj_ref
+        del pickled_obj_ref
     return hash_bucket_group_to_obj_id, object_refs
 
 
 def pk_digest_to_hash_bucket_index(
         digest,
         num_buckets: int) -> int:
+    """
+    Deterministically get the hash bucket a particular digest belongs to
+    based on number of total hash buckets.
+    """
 
     return int.from_bytes(digest, "big") % num_buckets
 
 
 def write_primary_key_index_files(
         table: pa.Table,
         primary_key_index_version_locator: PrimaryKeyIndexVersionLocator,
@@ -228,24 +255,27 @@
         hb_index: int,
         records_per_index_file: int) -> PyArrowWriteResult:
     """
     Writes primary key index files for the given hash bucket index out to the
     specified S3 bucket at the path identified by the given primary key index
     version locator. Output is written as 1 or more Parquet files with the
     given maximum number of records per file.
+
+    TODO(raghumdani): Support writing primary key index to any data catalog
     """
     logger.info(f"Writing primary key index files for hash bucket {hb_index}. "
                 f"Primary key index version locator: "
                 f"{primary_key_index_version_locator}.")
     s3_file_system = s3fs.S3FileSystem(
         anon=False,
         s3_additional_kwargs={
             "ContentType": ContentType.PARQUET.value,
             "ContentEncoding": ContentEncoding.IDENTITY.value,
-        }
+        },
+        config_kwargs=PRIMARY_KEY_INDEX_WRITE_BOTO3_CONFIG
     )
     pkiv_hb_index_s3_url_base = primary_key_index_version_locator\
         .get_pkiv_hb_index_s3_url_base(s3_bucket, hb_index)
     manifest_entries = s3u.upload_sliced_table(
         table,
         pkiv_hb_index_s3_url_base,
         s3_file_system,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/utils/round_completion_file.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/round_completion_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/compactor/utils/system_columns.py` & `deltacat-0.1.9.dev0/deltacat/compute/compactor/utils/system_columns.py`

 * *Files 4% similar despite different names*

```diff
@@ -266,9 +266,12 @@
     return table
 
 
 def get_minimal_hb_schema() -> pa.schema:
     return pa.schema([
         _PK_HASH_COLUMN_FIELD,
         _ORDERED_RECORD_IDX_COLUMN_FIELD,
-        _ORDERED_FILE_IDX_COLUMN_FIELD
+        _ORDERED_FILE_IDX_COLUMN_FIELD,
+        _PARTITION_STREAM_POSITION_COLUMN_FIELD,
+        _DELTA_TYPE_COLUMN_FIELD,
+        _IS_SOURCE_COLUMN_FIELD
     ])
```

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/meta_stats.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/meta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/model/partition_stats_dict.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/model/partition_stats_dict.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/model/stats_cluster_size_estimator.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/model/stats_cluster_size_estimator.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/stats.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/utils/constants.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/utils/io.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/metastats/utils/ray_utils.py` & `deltacat-0.1.9.dev0/deltacat/compute/metastats/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/basic.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/basic.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/models/delta_column_stats.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/models/delta_column_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/models/delta_stats.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/models/delta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/models/delta_stats_cache_result.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/models/delta_stats_cache_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/models/manifest_entry_stats.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/models/manifest_entry_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/models/stats_result.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/models/stats_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/utils/intervals.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/utils/io.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/compute/stats/utils/manifest_stats_file.py` & `deltacat-0.1.9.dev0/deltacat/compute/stats/utils/manifest_stats_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/constants.py` & `deltacat-0.1.9.dev0/deltacat/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,11 +21,18 @@
 # This should be kept larger than actual average inflation multipliers.
 # Note that this is a very rough guess since actual observed pyarrow
 # inflation multiplier for snappy-compressed parquet is about 5.45X for
 # all rows, but here we're trying to guess the inflation multipler for just
 # a primary key SHA1 digest and sort key columns (which could be all columns
 # of the table in the worst case, but here we're assuming that they
 # represent no more than ~1/4th of the total table bytes)
-PYARROW_INFLATION_MULTIPLIER = 1.5
+PYARROW_INFLATION_MULTIPLIER = 2.5
 
 # Inflation multiplier from snappy-compressed parquet to pyarrow for all columns.
-PYARROW_INFLATION_MULTIPLIER_ALL_COLUMNS = 6
+PYARROW_INFLATION_MULTIPLIER_ALL_COLUMNS = 6
+
+PRIMARY_KEY_INDEX_WRITE_BOTO3_CONFIG = {
+   "retries": {
+      'max_attempts': 25,
+      'mode': 'standard'
+   }
+}
```

### Comparing `deltacat-0.1.9/deltacat/io/aws/redshift/redshift_datasource.py` & `deltacat-0.1.9.dev0/deltacat/io/aws/redshift/redshift_datasource.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/io/dataset.py` & `deltacat-0.1.9.dev0/deltacat/io/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/io/read_api.py` & `deltacat-0.1.9.dev0/deltacat/io/read_api.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/logs.py` & `deltacat-0.1.9.dev0/deltacat/logs.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/__init__.py` & `deltacat-0.1.9.dev0/deltacat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/interface.py` & `deltacat-0.1.9.dev0/deltacat/storage/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/delta.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/list_result.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/list_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/locator.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/namespace.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/namespace.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/partition.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/partition.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/stream.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/stream.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/table.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/table.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/table_version.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/table_version.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/storage/model/types.py` & `deltacat-0.1.9.dev0/deltacat/storage/model/types.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/tests/stats/test_intervals.py` & `deltacat-0.1.9.dev0/deltacat/tests/stats/test_intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/types/media.py` & `deltacat-0.1.9.dev0/deltacat/types/media.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/types/tables.py` & `deltacat-0.1.9.dev0/deltacat/types/tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/common.py` & `deltacat-0.1.9.dev0/deltacat/utils/common.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/numpy.py` & `deltacat-0.1.9.dev0/deltacat/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/pandas.py` & `deltacat-0.1.9.dev0/deltacat/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/performance.py` & `deltacat-0.1.9.dev0/deltacat/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/placement.py` & `deltacat-0.1.9.dev0/deltacat/utils/placement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ray
 import re
 import time
 import yaml
 import logging
+from dataclasses import dataclass
 from typing import Optional, Union, List, Dict, Any, Callable, Tuple
 from ray.util.placement_group import (
 	placement_group,
 	placement_group_table,
 	get_current_placement_group
 )
 
@@ -18,14 +19,20 @@
 from deltacat.utils.ray_utils.runtime import live_node_resource_keys
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 #Limitation of current node group or placement group manager
 #Must run on driver or head node bc state.api needs to query dashboard api server at 127.0.0.1.
 #Issue: https://github.com/ray-project/ray/issues/29959
 
+@dataclass
+class PlacementGroupConfig():
+	def __init__(self, opts, resource):
+		self.opts = opts
+		self.resource = resource
+
 class NodeGroupManager():
 
 	def __init__(self,path: str, gname: str):
 		"""Node Group Manager
 		Args:
 			path: cluster yaml file
 			gname: node group prefix, e.g., 'partition'
@@ -156,15 +163,14 @@
 		try:
 			group_res['group_res']=ray.available_resources()[gname]
 		except Exception as e:
 			logger.info(f"There is no available resources for {gname}")
 			return None
 		return group_res
 
-
 class PlacementGroupManager():
 	"""Placement Group Manager
 	Create a list of placement group with the desired number of cpus
 	e.g., create a pg with 32 cpus, then this class will look for a node that has 32 cpus, and collect all 
 	resources, including cpu, memory, and object store;
 	How to use:
 		```
@@ -174,69 +180,78 @@
 			opts = pg_configs[0][0]
 			fun.options(**opts).remote()
 		```
 	Args:
 		num_pgs: number of placement groups to be created
 		instance_cpus: number of cpus per instance
 	"""
-	#TODO: add para for taking the head res key
-	def __init__(self, num_pgs: int, instance_cpus: int, instance_type: int = 8, time_out: Optional[float] = None):
+	def __init__(self, num_pgs: int, 
+				total_cpus_per_pg: int, 
+				cpu_per_bundle: int, 
+				strategy="SPREAD",
+				capture_child_tasks=True):
 		head_res_key = self.get_current_node_resource_key()
-		all_node_res_key = live_node_resource_keys()
-		all_node_res_key.remove(head_res_key)
-		num_bundles = (int)(instance_cpus/instance_type)
-		self._pg_configs = ray.get([_config.options(resources={head_res_key:0.01}).remote(instance_cpus, instance_type, all_node_res_key[i*num_bundles:(i+1)*num_bundles]) for i in range(num_pgs)])
+		#run the task on head and consume a fractional cpu, so that pg can be created on non-head node
+		#if cpu_per_bundle is less than the cpus per node, the pg can still be created on head
+		#curent assumption is that the cpu_per_bundle = cpus per node
+		#TODO: figure out how to create pg on non-head explicitly
+		self._pg_configs = ray.get([_config.options(resources={head_res_key:0.01}).remote(total_cpus_per_pg, \
+			cpu_per_bundle, strategy, capture_child_tasks) for i in range(num_pgs)])
+		#TODO: handle the cases where cpu_per_bundle is larger than max cpus per node, support it on ec2/flex/manta
+		
 	@property
 	def pgs(self):
 		return self._pg_configs
 
 	def get_current_node_resource_key(self) -> str: 
-	    current_node_id = ray.get_runtime_context().node_id.hex() 
-	    for node in ray.nodes(): 
-	        if node["NodeID"] == current_node_id: 
-	            # Found the node. 
-	            for key in node["Resources"].keys(): 
-	                if key.startswith("node:"): 
-	                    return key
+		#on ec2: address="172.31.34.51:6379"
+		#on manta: address = "2600:1f10:4674:6815:aadb:2dc8:de61:bc8e:6379"
+		current_node_name = ray.experimental.internal_kv.global_gcs_client.address[:-5]
+		for node in ray.nodes(): 
+			if node["NodeName"] == current_node_name: 
+				# Found the node. 
+				for key in node["Resources"].keys(): 
+					if key.startswith("node:"): 
+						return key
+
 @ray.remote(num_cpus=0.01)
-def _config(instance_cpus: int, instance_type: int, node_res_keys: List[str], time_out: Optional[float] = None) -> Tuple[Dict[str,Any], Dict[str,Any]]:
+def _config(total_cpus_per_pg: int, 
+			cpu_per_node: int, 
+			strategy="SPREAD",
+			capture_child_tasks=True,
+			time_out: Optional[float] = None) -> Tuple[Dict[str,Any], Dict[str,Any]]:
 	pg_config = None
-	try:
-		opts ={}
-		cluster_resources={}
-		num_bundles = (int)(instance_cpus/instance_type)
-		bundles = [{'CPU':instance_type,node_res_keys[i]:1} for i in range(num_bundles)]
-		pg = placement_group(bundles, strategy="SPREAD")
-		ray.get(pg.ready(), timeout=time_out)
-		if not pg:
-			return None
-		opts = {"scheduling_strategy":PlacementGroupSchedulingStrategy(
-			placement_group=pg, placement_group_capture_child_tasks=True)
-		}
-		pg_id = placement_group_table(pg)['placement_group_id']
-		pg_details = get_placement_group(pg_id)
-		bundles = pg_details['bundles']
-		node_ids =[]
-		for bd in bundles:
-			node_ids.append(bd['node_id'])
-		#query available resources given list of node id
-		all_nodes_available_res = ray._private.state.state._available_resources_per_node()
-		pg_res = {'CPU':0,'memory':0,'object_store_memory':0,'node_id':[]}
-		for node_id in node_ids:
-			if node_id in all_nodes_available_res:
-				v = all_nodes_available_res[node_id]
-				node_detail = get_node(node_id)
-				pg_res['CPU']+=node_detail['resources_total']['CPU']
-				pg_res['memory']+=v['memory']
-				pg_res['object_store_memory']+=v['object_store_memory']
-		cluster_resources['CPU'] = int(pg_res['CPU'])
-		cluster_resources['memory'] = float(pg_res['memory'])
-		cluster_resources['object_store_memory'] = float(pg_res['object_store_memory'])
-		cluster_resources['node_id'] = node_res_keys
-		pg_config=[opts,cluster_resources]
-		logger.info(f"pg has resources:{cluster_resources}")
-
-	except Exception as e:
-		logger.error(f"placement group error:{e}")
-		pass
+	opts ={}
+	cluster_resources={}
+	num_bundles = (int)(total_cpus_per_pg/cpu_per_node)
+	bundles = [{'CPU':cpu_per_node} for i in range(num_bundles)]
+	pg = placement_group(bundles, strategy=strategy)
+	ray.get(pg.ready(), timeout=time_out)
+	if not pg:
+		return None
+	opts = {"scheduling_strategy":PlacementGroupSchedulingStrategy(
+		placement_group=pg, placement_group_capture_child_tasks=capture_child_tasks)
+	}
+	pg_id = placement_group_table(pg)['placement_group_id']
+	pg_details = get_placement_group(pg_id)
+	bundles = pg_details['bundles']
+	node_ids = []
+	for bd in bundles:
+		node_ids.append(bd['node_id'])
+	#query available resources given list of node id
+	all_nodes_available_res = ray._private.state.state._available_resources_per_node()
+	pg_res = {'CPU':0,'memory':0,'object_store_memory':0}
+	for node_id in node_ids:
+		if node_id in all_nodes_available_res:
+			v = all_nodes_available_res[node_id]
+			node_detail = get_node(node_id)
+			pg_res['CPU']+=node_detail['resources_total']['CPU']
+			pg_res['memory']+=v['memory']
+			pg_res['object_store_memory']+=v['object_store_memory']
+	cluster_resources['CPU'] = int(pg_res['CPU'])
+	cluster_resources['memory'] = float(pg_res['memory'])
+	cluster_resources['object_store_memory'] = float(pg_res['object_store_memory'])
+	pg_config=PlacementGroupConfig(opts,cluster_resources) 
+	logger.info(f"pg has resources:{cluster_resources}")
+
 	return pg_config
```

### Comparing `deltacat-0.1.9/deltacat/utils/pyarrow.py` & `deltacat-0.1.9.dev0/deltacat/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/ray_utils/collections.py` & `deltacat-0.1.9.dev0/deltacat/utils/ray_utils/collections.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/ray_utils/concurrency.py` & `deltacat-0.1.9.dev0/deltacat/utils/ray_utils/concurrency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import ray
 
 from ray._private.ray_constants import MIN_RESOURCE_GRANULARITY
 from ray.types import ObjectRef
 
 from deltacat.utils.ray_utils.runtime import current_node_resource_key
+import copy
 
 from typing import Any, Iterable, Callable, Dict, List, Tuple, Union, Optional
 import itertools
 
 def invoke_parallel(
         items: Iterable,
         ray_task: Callable,
         *args,
         max_parallelism: Optional[int] = 1000,
-        num_cpus: int = 1,
         options_provider: Callable[[int, Any], Dict[str, Any]] = None,
         kwargs_provider: Callable[[int, Any], Dict[str, Any]] = None,
         **kwargs) -> List[Union[ObjectRef, Tuple[ObjectRef, ...]]]:
     """
     Creates a limited number of parallel remote invocations of the given ray
     task. By default each task is provided an ordered item from the input
     collection as its first argument followed by additional ordered arguments
@@ -58,17 +58,17 @@
                     list(itertools.chain(*pending_ids)),
                     num_returns=int(
                         len(pending_ids[0])*(len(pending_ids) - max_parallelism)
                     )
                 )
             else:
                 ray.wait(pending_ids, num_returns=len(pending_ids)-max_parallelism)
-        opt = {"num_cpus":num_cpus}
+        opt = {}
         if options_provider:
-            opt.update(options_provider(i, item))
+            opt = options_provider(i, item)
         if not kwargs_provider:
             pending_id = ray_task.options(**opt).remote(item, *args, **kwargs)
         else:
             kwargs_dict = kwargs_provider(i, item)
             kwargs.update(kwargs_dict)
             pending_id = ray_task.options(**opt).remote(*args, **kwargs)
         pending_ids.append(pending_id)
@@ -101,11 +101,18 @@
     ```
     resource_keys = live_node_resource_keys()
     for i in range(100):
         opt = round_robin_options_provider(i, resource_keys=resource_keys)
         foo.options(**opt).remote()
     ```
     """
-    assert resource_keys, f"No resource keys given to round robin!"
-    resource_key_index = i % len(resource_keys)
-    key = resource_keys[resource_key_index]
-    return {"resources": {key: resource_amount_provider(resource_key_index)}}
+    opts = kwargs.get("pg_config")
+    if opts:
+        new_opts = copy.deepcopy(opts)
+        bundle_key_index = i % len(new_opts['scheduling_strategy'].placement_group.bundle_specs)
+        new_opts['scheduling_strategy'].placement_group_bundle_index = bundle_key_index
+        return new_opts
+    else:
+        assert resource_keys, f"No resource keys given to round robin!"
+        resource_key_index = i % len(resource_keys)
+        key = resource_keys[resource_key_index]
+        return {"resources": {key: resource_amount_provider(resource_key_index)}}
```

### Comparing `deltacat-0.1.9/deltacat/utils/ray_utils/dataset.py` & `deltacat-0.1.9.dev0/deltacat/utils/ray_utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/ray_utils/performance.py` & `deltacat-0.1.9.dev0/deltacat/utils/ray_utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat/utils/ray_utils/runtime.py` & `deltacat-0.1.9.dev0/deltacat/utils/ray_utils/runtime.py`

 * *Files identical despite different names*

### Comparing `deltacat-0.1.9/deltacat.egg-info/PKG-INFO` & `deltacat-0.1.9.dev0/deltacat.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 0.1.9
+Version: 0.1.9.dev0
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
+License: UNKNOWN
+Description: # DeltaCAT
+        
+        DeltaCAT is a Pythonic Data Catalog powered by Ray.
+        
+        Its data storage model allows you to define and manage fast, scalable,
+        ACID-compliant data catalogs through git-like stage/commit APIs, and has been
+        used to successfully host exabyte-scale enterprise data lakes.
+        
+        DeltaCAT uses the Ray distributed compute framework together with Apache Arrow
+        for common table management tasks, including petabyte-scale
+        change-data-capture, data consistency checks, and table repair.
+        
+        ## Getting Started
+        ---
+        ### Install
+        ```
+        pip install deltacat
+        ```
+        
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# DeltaCAT
-
-DeltaCAT is a Pythonic Data Catalog powered by Ray.
-
-Its data storage model allows you to define and manage fast, scalable, 
-ACID-compliant data catalogs through git-like stage/commit APIs, and has been 
-used to successfully host exabyte-scale enterprise data lakes.
-
-DeltaCAT uses the Ray distributed compute framework together with Apache Arrow
-for common table management tasks, including petabyte-scale 
-change-data-capture, data consistency checks, and table repair.
```

### Comparing `deltacat-0.1.9/deltacat.egg-info/SOURCES.txt` & `deltacat-0.1.9.dev0/deltacat.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-LICENSE
 MANIFEST.in
 README.md
 setup.py
-/Volumes/workplace/SunGate/build/SunGate/SunGate-1.0/AL2_x86_64/DEV.STD.PTHREAD/build/superjar/SunGate-1.0-super.jar
 deltacat/__init__.py
 deltacat/constants.py
 deltacat/exceptions.py
 deltacat/logs.py
 deltacat.egg-info/PKG-INFO
 deltacat.egg-info/SOURCES.txt
 deltacat.egg-info/dependency_links.txt
```

### Comparing `deltacat-0.1.9/setup.py` & `deltacat-0.1.9.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 ROOT_DIR = os.path.dirname(__file__)
 
 
 def find_version(*paths):
     version_file_path = os.path.join(ROOT_DIR, *paths)
     with open(version_file_path) as file_stream:
         version_match = re.search(
-            r"^__version__ = ['\"]([^'\"]*)['\"]",
-            file_stream.read(),
-            re.M)
+            r"^__version__ = ['\"]([^'\"]*)['\"]", file_stream.read(), re.M
+        )
         if version_match:
             return version_match.group(1)
         raise RuntimeError(f"Failed to find version at: {version_file_path}")
 
 
 with open(os.path.join(ROOT_DIR, "README.md"), "r", encoding="utf-8") as fh:
     long_description = fh.read()
@@ -32,32 +31,32 @@
     description="A scalable, fast, ACID-compliant Data Catalog powered by Ray.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ray-project/deltacat",
     packages=setuptools.find_packages(where=".", include="deltacat*"),
     install_requires=[
         # any changes here should also be reflected in requirements.txt
-        "s3fs == 2022.1.0",
-        "tenacity == 8.0.1",
-        "ray[default] == 2.0.0",
-        "pandas >= 1.3.1",
-        "pyarrow == 8.0.0",
-        "pydantic == 1.10.2",
-        "numpy >= 1.21.1",
         "boto3 == 1.20.24",
-        "typing-extensions == 4.4.0"
+        "numpy == 1.21.5",
+        "pandas == 1.3.5",
+        "pyarrow == 10.0.1",
+        "pydantic == 1.10.4",
+        "ray[default] == 2.0.0",
+        "s3fs == 2022.2.0",
+        "tenacity == 8.1.0",
+        "typing-extensions == 4.4.0",
     ],
     setup_requires=["wheel"],
     package_data={
         "compute/metastats": ["*.yaml"],
-        },
+    },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
-)
+)
```

