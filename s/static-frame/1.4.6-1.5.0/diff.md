# Comparing `tmp/static-frame-1.4.6.tar.gz` & `tmp/static-frame-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-1.4.6.tar", last modified: Sun Jun 25 04:40:42 2023, max compression
+gzip compressed data, was "static-frame-1.5.0.tar", last modified: Fri Jul 21 20:34:24 2023, max compression
```

## Comparing `static-frame-1.4.6.tar` & `static-frame-1.5.0.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.430760 static-frame-1.4.6/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2023-03-23 21:26:53.000000 static-frame-1.4.6/LICENSE.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-01-11 20:49:28.000000 static-frame-1.4.6/MANIFEST.in
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23469 2023-06-25 04:40:42.430760 static-frame-1.4.6/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24106 2023-06-25 02:02:42.000000 static-frame-1.4.6/README.rst
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2023-03-23 21:26:53.000000 static-frame-1.4.6/requirements-extras.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      363 2023-06-25 02:02:42.000000 static-frame-1.4.6/requirements-test.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-06-25 02:02:42.000000 static-frame-1.4.6/requirements.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-06-25 04:40:42.430760 static-frame-1.4.6/setup.cfg
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3777 2023-03-23 21:26:53.000000 static-frame-1.4.6/setup.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.410759 static-frame-1.4.6/static_frame/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-06-25 02:02:56.000000 static-frame-1.4.6/static_frame/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/__main__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.422759 static-frame-1.4.6/static_frame/core/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/core/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    44502 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      223 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/assign.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5475 2023-05-16 23:32:31.000000 static-frame-1.4.6/static_frame/core/axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    59324 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    50681 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24157 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    70680 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35163 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9232 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17470 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1599 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/core/display_html_datatables.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15864 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/display_visidata.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    28891 2023-04-19 18:21:25.000000 static-frame-1.4.6/static_frame/core/doc_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3447 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/exception.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3098 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   378509 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1141 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    56897 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6466 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17792 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5455 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21196 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/core/index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   107732 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16869 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47042 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      514 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/interface_meta.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15041 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23859 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/core/loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9635 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35827 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/core/node_dt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    24236 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/core/node_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5312 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_hashlib.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    32016 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/node_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14190 2023-04-19 18:21:25.000000 static-frame-1.4.6/static_frame/core/node_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    12353 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_selector.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    34445 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_str.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15388 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/node_transpose.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10018 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/node_values.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31469 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1623 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11771 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17337 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/protocol_dfi_abc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    53391 2023-04-19 18:21:25.000000 static-frame-1.4.6/static_frame/core/quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4631 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   127343 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/core/series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9996 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6249 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_client_mixin.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15150 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/store_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14880 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/core/store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5888 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7057 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    26087 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    21484 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5117 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   177922 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   129931 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/core/util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     9952 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    27762 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/core/yarn.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/py.typed
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.422759 static-frame-1.4.6/static_frame/test/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/test/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/test_case.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.430760 static-frame-1.4.6/static_frame/test/unit/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-01-11 20:49:28.000000 static-frame-1.4.6/static_frame/test/unit/__init__.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    25950 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_archive_npy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7340 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_axis_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   138362 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_batch.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    81209 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_bus.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      599 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_container.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    35989 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_container_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    36712 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_display.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_display_color.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      358 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_display_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5247 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_doc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      937 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_fill_value_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   642225 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_frame.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2254 2022-03-15 15:56:11.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    60358 2023-04-24 22:32:18.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_iter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    31756 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_join.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     6644 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_via_fill_value.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5022 2022-03-15 15:56:11.000000 static-frame-1.4.6/static_frame/test/unit/test_frame_via_re.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2317 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_hloc.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    64304 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_index.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4044 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_index_auto.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1323 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_index_base.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1416 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_index_correspondence.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    41844 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_index_datetime.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   164692 2023-05-16 23:32:31.000000 static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     3526 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     5856 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/test/unit/test_interface.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    19608 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_loc_map.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    16279 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_memory_measure.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    22632 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4455 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_pivot.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      373 2022-03-15 15:56:11.000000 static-frame-1.4.6/static_frame/test/unit/test_platform.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15253 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_protocol_dfi.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    74931 2023-05-16 23:32:31.000000 static-frame-1.4.6/static_frame/test/unit/test_quilt.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    11263 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_rank.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   244185 2023-05-25 15:11:48.000000 static-frame-1.4.6/static_frame/test/unit/test_series.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     2384 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_series_he.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    13468 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    14506 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/test/unit/test_store_filter.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     7409 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_hdf5.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     8114 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_sqlite.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    15968 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_xlsx.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    17381 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_store_zip.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      884 2023-03-23 21:26:53.000000 static-frame-1.4.6/static_frame/test/unit/test_style_config.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   161330 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_type_blocks.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)   114907 2023-06-25 02:02:16.000000 static-frame-1.4.6/static_frame/test/unit/test_util.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    10401 2023-05-12 15:14:12.000000 static-frame-1.4.6/static_frame/test/unit/test_www.py
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    47732 2023-05-04 17:09:05.000000 static-frame-1.4.6/static_frame/test/unit/test_yarn.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-25 04:40:42.414759 static-frame-1.4.6/static_frame.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)    23469 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/requires.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-06-25 04:40:42.000000 static-frame-1.4.6/static_frame.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-07-21 20:34:24.959982 static-frame-1.5.0/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1777 2022-09-18 23:42:20.000000 static-frame-1.5.0/LICENSE.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      105 2022-08-07 22:56:47.000000 static-frame-1.5.0/MANIFEST.in
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23418 2023-07-21 20:34:24.959982 static-frame-1.5.0/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24106 2023-07-21 20:00:06.000000 static-frame-1.5.0/README.rst
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      144 2022-09-18 23:42:20.000000 static-frame-1.5.0/requirements-extras.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      364 2023-07-21 20:00:06.000000 static-frame-1.5.0/requirements-test.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       46 2023-07-21 20:00:06.000000 static-frame-1.5.0/requirements.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       77 2023-07-21 20:34:24.963981 static-frame-1.5.0/setup.cfg
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3723 2023-07-18 20:04:43.000000 static-frame-1.5.0/setup.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-07-21 20:34:24.903992 static-frame-1.5.0/static_frame/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7638 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1573 2022-09-18 23:42:20.000000 static-frame-1.5.0/static_frame/__main__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-07-21 20:34:24.931987 static-frame-1.5.0/static_frame/core/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.5.0/static_frame/core/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    44538 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      259 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/assign.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5511 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    59402 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    50703 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24179 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    70715 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35199 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9267 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17506 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1633 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/display_html_datatables.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15899 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/display_visidata.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    28925 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/doc_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3483 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/exception.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3133 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   378484 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1177 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    56904 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6501 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17814 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5491 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21232 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   107744 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16905 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47161 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      536 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/interface_meta.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15077 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23895 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9671 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    35862 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_dt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    24272 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5348 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_hashlib.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    32051 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14226 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    12816 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_selector.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    34481 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_str.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15423 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_transpose.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10054 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/node_values.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31505 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1659 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11807 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17373 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/protocol_dfi_abc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    53341 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4667 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   127430 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10031 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6284 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_client_mixin.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15185 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14916 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5924 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7093 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    26152 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    21520 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5153 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   178319 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   129800 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     9988 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    27784 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/core/yarn.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.5.0/static_frame/py.typed
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-07-21 20:34:24.935987 static-frame-1.5.0/static_frame/test/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.5.0/static_frame/test/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11984 2023-01-30 03:11:00.000000 static-frame-1.5.0/static_frame/test/test_case.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-07-21 20:34:24.959982 static-frame-1.5.0/static_frame/test/unit/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        0 2022-08-07 22:56:47.000000 static-frame-1.5.0/static_frame/test/unit/__init__.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    25986 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_archive_npy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7376 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_axis_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   138432 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_batch.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    81245 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_bus.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      635 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_container.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36025 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_container_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    36748 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_display.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1052 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_display_color.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      394 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_display_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5283 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_doc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      973 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_fill_value_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   642427 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_frame.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2290 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_frame_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    60708 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_frame_iter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    31762 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_frame_join.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     6680 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5058 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_frame_via_re.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2353 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_hloc.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    64340 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4080 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index_auto.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1359 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index_base.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1452 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index_correspondence.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    41734 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index_datetime.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   164743 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index_hierarchy.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     3562 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     5892 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_interface.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    19644 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_loc_map.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16315 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_memory_measure.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    22668 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4491 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_pivot.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      409 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_platform.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    15289 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_protocol_dfi.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    74968 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_quilt.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    11299 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_rank.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   244432 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_series.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2420 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_series_he.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    13504 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_store.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    14542 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_store_filter.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     7445 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_store_hdf5.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     8150 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_store_sqlite.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    16004 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_store_xlsx.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    17417 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_store_zip.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      920 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_style_config.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   161337 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_type_blocks.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)   114943 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_util.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    10437 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_www.py
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    47768 2023-07-21 20:00:06.000000 static-frame-1.5.0/static_frame/test/unit/test_yarn.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-07-21 20:34:24.907992 static-frame-1.5.0/static_frame.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)    23418 2023-07-21 20:34:24.000000 static-frame-1.5.0/static_frame.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     4328 2023-07-21 20:34:24.000000 static-frame-1.5.0/static_frame.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-07-21 20:34:24.000000 static-frame-1.5.0/static_frame.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      200 2023-07-21 20:34:24.000000 static-frame-1.5.0/static_frame.egg-info/requires.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       13 2023-07-21 20:34:24.000000 static-frame-1.5.0/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-1.4.6/LICENSE.txt` & `static-frame-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.6/PKG-INFO` & `static-frame-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.6
+Version: 1.5.0
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -54,22 +54,22 @@
         
         
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
-        - Python>=3.7
-        - NumPy>=1.18.5
+        - Python>=3.8
+        - numpy>=1.19.5
         - arraymap==0.1.9
         - arraykit==0.4.9
         
         For extended input and output, the following packages are required:
         
-        - pandas>=0.24.2
+        - pandas>=0.25.3
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
         - tables>=3.6.1
         - pyarrow>=0.17.0
         - visidata>=2.4
         
@@ -362,14 +362,13 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >3.7.0
+Requires-Python: >=3.8
 Provides-Extra: extras
```

### Comparing `static-frame-1.4.6/README.rst` & `static-frame-1.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -96,22 +96,22 @@
 
 
 Dependencies
 --------------
 
 Core StaticFrame requires the following:
 
-- Python>=3.7
-- NumPy>=1.18.5
+- Python>=3.8
+- numpy>=1.19.5
 - arraymap==0.1.9
 - arraykit==0.4.9
 
 For extended input and output, the following packages are required:
 
-- pandas>=0.24.2
+- pandas>=0.25.3
 - xlsxwriter>=1.1.2
 - openpyxl>=3.0.9
 - xarray>=0.13.0
 - tables>=3.6.1
 - pyarrow>=0.17.0
 - visidata>=2.4
```

### Comparing `static-frame-1.4.6/setup.py` & `static-frame-1.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     return {'extras': list(_get_requirements('requirements-extras.txt'))}
 
 setup(
     name='static-frame',
     version=get_version(),
     description='Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.',
     long_description=get_long_description(),
-    python_requires='>3.7.0',
+    python_requires='>=3.8',
     install_requires=list(get_install_requires()),
     extras_require=get_extras_require(),
     url='https://github.com/static-frame/static-frame',
     author='Christopher Ariza',
     license='MIT',
     package_data={'static_frame': ['py.typed']},
 
@@ -84,15 +84,14 @@
             'Topic :: Software Development',
             'Topic :: Scientific/Engineering',
             'Topic :: Scientific/Engineering :: Information Analysis',
             'License :: OSI Approved :: MIT License',
             'Operating System :: MacOS :: MacOS X',
             'Operating System :: Microsoft :: Windows',
             'Operating System :: POSIX',
-            'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
             'Programming Language :: Python :: 3.11',
             ],
 
     keywords='staticframe pandas numpy immutable array',
```

### Comparing `static-frame-1.4.6/static_frame/__init__.py` & `static-frame-1.5.0/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 from static_frame.core.util import IndexSpecifier as IndexSpecifier
 from static_frame.core.util import KeyOrKeys as KeyOrKeys
 from static_frame.core.util import PathSpecifierOrFileLike as PathSpecifierOrFileLike
 from static_frame.core.util import SeriesInitializer as SeriesInitializer
 from static_frame.core.www import WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '1.4.6'
+__version__ = '1.5.0'
```

### Comparing `static-frame-1.4.6/static_frame/__main__.py` & `static-frame-1.5.0/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.6/static_frame/core/archive_npy.py` & `static-frame-1.5.0/static_frame/core/archive_npy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import mmap
 import os
 import shutil
 import struct
 import typing as tp
 from ast import literal_eval
```

### Comparing `static-frame-1.4.6/static_frame/core/axis_map.py` & `static-frame-1.5.0/static_frame/core/axis_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from copy import deepcopy
 from functools import partial
 
 from arraykit import array_deepcopy
 
 from static_frame.core.bus import Bus
```

### Comparing `static-frame-1.4.6/static_frame/core/batch.py` & `static-frame-1.5.0/static_frame/core/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.bus import Bus
 from static_frame.core.container import ContainerOperand
 from static_frame.core.display import Display
@@ -13,15 +15,15 @@
 from static_frame.core.frame import Frame
 from static_frame.core.index_auto import IndexAutoFactoryType
 from static_frame.core.index_auto import RelabelInput
 from static_frame.core.node_dt import InterfaceBatchDatetime
 from static_frame.core.node_fill_value import InterfaceBatchFillValue
 from static_frame.core.node_re import InterfaceBatchRe
 from static_frame.core.node_selector import InterfaceBatchAsType
-from static_frame.core.node_selector import InterfaceGetItem
+from static_frame.core.node_selector import InterfaceGetItemCompound
 from static_frame.core.node_selector import InterfaceSelectTrio
 from static_frame.core.node_str import InterfaceBatchString
 from static_frame.core.node_transpose import InterfaceBatchTranspose
 from static_frame.core.node_values import InterfaceBatchValues
 from static_frame.core.series import Series
 from static_frame.core.store import Store
 from static_frame.core.store_client_mixin import StoreClientMixin
@@ -440,15 +442,15 @@
             for label, v in self._items:
                 yield label, normalize_container(v)
         return self._derive(gen)
 
     #---------------------------------------------------------------------------
     # name interface
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def name(self) -> NameType:
         '''{}'''
         return self._name
 
     #---------------------------------------------------------------------------
     @property
@@ -714,24 +716,24 @@
                 key=key
                 )
 
     #---------------------------------------------------------------------------
     # interfaces
 
     @property
-    def loc(self) -> InterfaceGetItem['Batch']:
-        return InterfaceGetItem(self._extract_loc)
+    def loc(self) -> InterfaceGetItemCompound['Batch']:
+        return InterfaceGetItemCompound(self._extract_loc)
 
     @property
-    def iloc(self) -> InterfaceGetItem['Batch']:
-        return InterfaceGetItem(self._extract_iloc)
+    def iloc(self) -> InterfaceGetItemCompound['Batch']:
+        return InterfaceGetItemCompound(self._extract_iloc)
 
     @property
-    def bloc(self) -> InterfaceGetItem['Batch']:
-        return InterfaceGetItem(self._extract_bloc)
+    def bloc(self) -> InterfaceGetItemCompound['Batch']:
+        return InterfaceGetItemCompound(self._extract_bloc)
 
     @property
     def drop(self) -> InterfaceSelectTrio['Batch']:
         return InterfaceSelectTrio( #type: ignore
             func_iloc=self._drop_iloc,
             func_loc=self._drop_loc,
             func_getitem=self._drop_getitem)
```

### Comparing `static-frame-1.4.6/static_frame/core/bus.py` & `static-frame-1.5.0/static_frame/core/bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from itertools import chain
 from itertools import zip_longest
 
 import numpy as np
 
 from static_frame.core.container import ContainerBase
@@ -541,15 +543,15 @@
     #             config=self._config,
     #             max_persiste=self._max_persist,
     #             )
 
     #---------------------------------------------------------------------------
     # name interface
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def name(self) -> NameType:
         '''{}'''
         return self._name
 
     def rename(self, name: NameType) -> 'Bus':
         '''
```

### Comparing `static-frame-1.4.6/static_frame/core/container.py` & `static-frame-1.5.0/static_frame/core/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from collections import deque
 from functools import partial
 
 import numpy as np
 
 from static_frame.core.display import Display
@@ -44,15 +46,15 @@
     # class attrs
 
     STATIC: bool = True
 
     #---------------------------------------------------------------------------
     # common display functions
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def interface(self) -> 'Frame':
         '''{}'''
         from static_frame.core.interface import InterfaceSummary
         return InterfaceSummary.to_frame(self.__class__)
 
     # def __sizeof__(self) -> int:
```

### Comparing `static-frame-1.4.6/static_frame/core/container_util.py` & `static-frame-1.5.0/static_frame/core/container_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''
 This module us for utilty functions that take as input and / or return Container subclasses such as Index, Series, or Frame, and that need to be shared by multiple such Container classes.
 '''
+from __future__ import annotations
 
 import datetime
 import typing as tp
 from collections import defaultdict
 from fractions import Fraction
 from functools import partial
 from itertools import zip_longest
```

### Comparing `static-frame-1.4.6/static_frame/core/display.py` & `static-frame-1.5.0/static_frame/core/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import html
 import inspect
 import os
 import platform
 import re
 import sys
 import typing as tp
```

### Comparing `static-frame-1.4.6/static_frame/core/display_color.py` & `static-frame-1.5.0/static_frame/core/display_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 
 #-------------------------------------------------------------------------------
 # https://www.w3.org/TR/css-color-3/#svg-color
 
 _COLOR_NAME_X11 = {
```

### Comparing `static-frame-1.4.6/static_frame/core/display_config.py` & `static-frame-1.5.0/static_frame/core/display_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import json
 import re
 import typing as tp
 from enum import Enum
 
 import numpy as np
```

### Comparing `static-frame-1.4.6/static_frame/core/display_html_datatables.py` & `static-frame-1.5.0/static_frame/core/display_html_datatables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+from __future__ import annotations
 
 from functools import partial
 
 VERSION_BOOTSTRAP = '4.3.1'
 VERSION_DATATABLES = '1.10.19'
 VERSION_JQUERY = '3.3.1'
 VERSION_JQUERY_UI = '1.12.0'
```

### Comparing `static-frame-1.4.6/static_frame/core/display_visidata.py` & `static-frame-1.5.0/static_frame/core/display_visidata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # This module follows the conventions of the VisiData project for naming and style.
 # This module is excluded from mypy and lint checking
+from __future__ import annotations
 
 import re
 from datetime import date
 
 import numpy as np
 from visidata import Column
 from visidata import ColumnAttr
```

### Comparing `static-frame-1.4.6/static_frame/core/doc_str.py` & `static-frame-1.5.0/static_frame/core/doc_str.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Storage for common doc strings and templates shared in non-related classes and methods.
 '''
-
+from __future__ import annotations
 
 import typing as tp
 
 from static_frame.core.util import AnyCallable
 
 #-------------------------------------------------------------------------------
 # common strings
```

### Comparing `static-frame-1.4.6/static_frame/core/exception.py` & `static-frame-1.5.0/static_frame/core/exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 import warnings
 
 
 class ErrorInit(RuntimeError):
     '''Error in Container initialization.
     '''
```

### Comparing `static-frame-1.4.6/static_frame/core/fill_value_auto.py` & `static-frame-1.5.0/static_frame/core/fill_value_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.util import NAT
 from static_frame.core.util import NAT_TD64
```

### Comparing `static-frame-1.4.6/static_frame/core/frame.py` & `static-frame-1.5.0/static_frame/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+from __future__ import annotations
+
 import csv
 import json
 import pickle
 import sqlite3
 import typing as tp
 from collections import deque
 from collections.abc import Set
 from copy import deepcopy
+from dataclasses import is_dataclass
 from functools import partial
 from io import BytesIO
 from io import StringIO
 from itertools import chain
 from itertools import product
 from itertools import zip_longest
 from operator import itemgetter
@@ -92,15 +95,15 @@
 from static_frame.core.node_iter import IterNodeGroupOther
 from static_frame.core.node_iter import IterNodeType
 from static_frame.core.node_iter import IterNodeWindow
 from static_frame.core.node_re import InterfaceRe
 from static_frame.core.node_selector import InterfaceAssignQuartet
 from static_frame.core.node_selector import InterfaceAsType
 from static_frame.core.node_selector import InterfaceConsolidate
-from static_frame.core.node_selector import InterfaceGetItem
+from static_frame.core.node_selector import InterfaceGetItemCompound
 from static_frame.core.node_selector import InterfaceSelectTrio
 from static_frame.core.node_str import InterfaceString
 from static_frame.core.node_transpose import InterfaceTranspose
 from static_frame.core.node_values import InterfaceValues
 from static_frame.core.pivot import pivot_derive_constructors
 from static_frame.core.pivot import pivot_index_map
 from static_frame.core.protocol_dfi import DFIDataFrame
@@ -173,15 +176,14 @@
 from static_frame.core.util import dtype_kind_to_na
 from static_frame.core.util import dtype_to_fill_value
 from static_frame.core.util import file_like_manager
 from static_frame.core.util import full_for_fill
 from static_frame.core.util import get_tuple_constructor
 from static_frame.core.util import iloc_to_insertion_iloc
 from static_frame.core.util import is_callable_or_mapping
-from static_frame.core.util import is_dataclass
 from static_frame.core.util import is_dtype_specifier
 from static_frame.core.util import isfalsy_array
 from static_frame.core.util import isna_array
 from static_frame.core.util import iterable_to_array_1d
 from static_frame.core.util import iterable_to_array_nd
 from static_frame.core.util import key_normalize
 from static_frame.core.util import path_filter
@@ -862,49 +864,49 @@
                         name=name,
                         dtypes=dtypes,
                         )
             raise ErrorInitFrame('no rows available in records, and no columns defined.')
 
         if hasattr(rows, '__getitem__'):
             rows_to_iter = False
-            row_reference = rows[0] # type: ignore
+            row_reference = rows[0]
         else: # dict view, or other sized iterable that does not support getitem
             rows_to_iter = True
             row_reference = next(iter(rows))
 
         if isinstance(row_reference, Series):
             raise ErrorInitFrame('Frame.from_records() does not support Series records. Use Frame.from_concat() instead.')
         if isinstance(row_reference, dict):
             raise ErrorInitFrame('Frame.from_records() does not support dictionary records. Use Frame.from_dict_records() instead.')
 
-        is_dataclass = hasattr(row_reference, '__dataclass_fields__')
-        if is_dataclass:
+        is_dc_inst = hasattr(row_reference, '__dataclass_fields__')
+        if is_dc_inst:
             fields_dc = tuple(row_reference.__dataclass_fields__.keys())
 
 
         column_name_getter = None
         # NOTE: even if getter is defined, columns list is needed to be available to get_col_dtype after it is populated
         if columns is None and hasattr(row_reference, '_fields'): # NamedTuple
             column_name_getter = row_reference._fields.__getitem__
             columns = []
-        elif columns is None and is_dataclass:
+        elif columns is None and is_dc_inst:
             column_name_getter = fields_dc.__getitem__
             columns = []
 
         get_col_dtype = None if dtypes is None else get_col_dtype_factory(dtypes, columns) # type: ignore
 
         # NOTE: row data by definition does not have Index data, so col count is length of row
         if hasattr(row_reference, '__len__'):
             col_count = len(row_reference)
-        elif is_dataclass:
+        elif is_dc_inst:
             col_count = len(fields_dc) # defined in branch above
         else:
             raise NotImplementedError(f'cannot get col_count from {row_reference}')
 
-        if not is_dataclass:
+        if not is_dc_inst:
             def get_value_iter(col_key: tp.Hashable, col_idx: int) -> tp.Iterator[tp.Any]:
                 rows_iter = rows if not rows_to_iter else iter(rows)
                 return (row[col_key] for row in rows_iter)
         else:
             def get_value_iter(col_key: tp.Hashable, col_idx: int) -> tp.Iterator[tp.Any]:
                 rows_iter = rows if not rows_to_iter else iter(rows)
                 return (getattr(row, fields_dc[col_key]) for row in rows_iter) #type: ignore
@@ -1774,15 +1776,15 @@
             cursor.execute(query, parameters)
 
             if columns_select:
                 columns_select = set(columns_select)
                 # selector function defined below
                 def filter_row(row: tp.Sequence[tp.Any]) -> tp.Sequence[tp.Any]:
                     post = selector(row)
-                    return post if not selector_reduces else (post,)
+                    return post if not selector_reduces else (post,) # type: ignore
 
             if columns_depth > 0 or columns_select:
                 # always need to derive labels if using columns_select
                 labels = (col for (col, *_) in cursor.description[index_depth:])
 
             if columns_depth <= 1 and columns_select:
                 iloc_sel, labels = zip(*(
@@ -1835,15 +1837,15 @@
                 # parital to include everything but values
                 index_constructor = constructor_from_optional_constructors(
                         depth=index_depth,
                         default_constructor=default_constructor,
                         explicit_constructors=index_constructors,
                         )
                 def row_gen() -> tp.Iterator[tp.Sequence[tp.Any]]:
-                    for row in cursor: # type: ignore
+                    for row in cursor:
                         index.append(row[0])
                         yield row[1:]
             else: # > 1
                 index = [list() for _ in range(index_depth)]
 
                 def default_constructor(
                         iterables: tp.Iterable[tp.Hashable],
@@ -1863,15 +1865,15 @@
                 index_constructor = constructor_from_optional_constructors(
                         depth=index_depth,
                         default_constructor=default_constructor,
                         explicit_constructors=index_constructors,
                         )
 
                 def row_gen() -> tp.Iterator[tp.Sequence[tp.Any]]:
-                    for row in cursor: # type: ignore
+                    for row in cursor:
                         for i, label in enumerate(row[:index_depth]):
                             index[i].append(label)
                         yield row[index_depth:]
 
             if columns_select:
                 row_gen_final = (filter_row(row) for row in row_gen()) # type: ignore
             else:
@@ -2168,15 +2170,15 @@
                 if isinstance(fp, str):
                     with open(fp, 'r', encoding=encoding) as f:
                         for i, row in enumerate(f):
                             if i >= skip_footer:
                                 yield row_buffer.popleft()
                             row_buffer.append(row)
                 else:
-                    for i, row in enumerate(fp): # type: ignore
+                    for i, row in enumerate(fp):
                         if i >= skip_footer:
                             yield row_buffer.popleft()
                         row_buffer.append(row)
 
         row_iter = file_like()
         if skip_header:
             for _ in range(skip_header):
@@ -3242,15 +3244,15 @@
         # we can determine if columns or index are empty only if they are not iterators; those cases will have to use a deferred evaluation
         columns_empty = index_constructor_empty(columns)
         index_empty = index_constructor_empty(index)
 
         #-----------------------------------------------------------------------
         # blocks assignment
 
-        blocks_constructor = None
+        blocks_constructor: tp.Optional[tp.Callable[[tp.Tuple[int, ...]], None]] = None
 
         if data.__class__ is TypeBlocks: # PERF: no sublcasses supported
             if own_data:
                 self._blocks = data # type: ignore
             else:
                 # assume we need to create a new TB instance; this will not copy underlying arrays as all blocks are immutable
                 self._blocks = TypeBlocks.from_blocks(data._blocks) # type: ignore
@@ -3439,24 +3441,24 @@
                 own_data=True,
                 own_index=True)
 
     #---------------------------------------------------------------------------
     # interfaces
 
     @property
-    def loc(self) -> InterfaceGetItem['Frame']:
-        return InterfaceGetItem(self._extract_loc)
+    def loc(self) -> InterfaceGetItemCompound['Frame']:
+        return InterfaceGetItemCompound(self._extract_loc)
 
     @property
-    def iloc(self) -> InterfaceGetItem['Frame']:
-        return InterfaceGetItem(self._extract_iloc)
+    def iloc(self) -> InterfaceGetItemCompound['Frame']:
+        return InterfaceGetItemCompound(self._extract_iloc)
 
     @property
-    def bloc(self) -> InterfaceGetItem['Frame']:
-        return InterfaceGetItem(self._extract_bloc)
+    def bloc(self) -> InterfaceGetItemCompound['Frame']:
+        return InterfaceGetItemCompound(self._extract_bloc)
 
     @property
     def drop(self) -> InterfaceSelectTrio['Frame']:
         return InterfaceSelectTrio( # type: ignore # NOTE: does not reuturn Frame, but a delegate
             func_iloc=self._drop_iloc,
             func_loc=self._drop_loc,
             func_getitem=self._drop_getitem)
@@ -3482,15 +3484,15 @@
             func_iloc=self._extract_iloc_assign,
             func_loc=self._extract_loc_assign,
             func_getitem=self._extract_getitem_assign,
             func_bloc=self._extract_bloc_assign,
             delegate=FrameAssign,
             )
 
-    @property # type: ignore
+    @property
     @doc_inject(select='astype')
     def astype(self) -> InterfaceAsType['Frame']:
         '''
         Retype one or more columns. When used as a function, can be used to retype the entire ``Frame``. Alternatively, when used as a ``__getitem__`` interface, loc-style column selection can be used to type one or more coloumns.
 
         Args:
             {dtype}
@@ -3861,15 +3863,15 @@
                 function_items=partial(self._axis_group_other_items,
                         as_array=True),
                 yield_type=IterNodeType.ITEMS,
                 apply_type=IterNodeApplyType.SERIES_ITEMS_GROUP_VALUES,
                 )
 
     #---------------------------------------------------------------------------
-    @property # type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window(self) -> IterNodeWindow['Frame']:
         '''
         Iterator of windowed values, where values are given as a :obj:`Frame`.
 
         {args}
         '''
@@ -3879,15 +3881,15 @@
                 container=self,
                 function_values=function_values,
                 function_items=function_items,
                 yield_type=IterNodeType.VALUES,
                 apply_type=IterNodeApplyType.SERIES_ITEMS,
                 )
 
-    @property # type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window_items(self) -> IterNodeWindow['Frame']:
         '''
         Iterator of pairs of label, windowed values, where values are given as a :obj:`Frame`.
 
         {args}
         '''
@@ -3897,15 +3899,15 @@
                 container=self,
                 function_values=function_values,
                 function_items=function_items,
                 yield_type=IterNodeType.ITEMS,
                 apply_type=IterNodeApplyType.SERIES_ITEMS,
                 )
 
-    @property # type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window_array(self) -> IterNodeWindow['Frame']:
         '''
         Iterator of windowed values, where values are given as a :obj:`np.array`.
 
         {args}
         '''
@@ -3915,15 +3917,15 @@
                 container=self,
                 function_values=function_values,
                 function_items=function_items,
                 yield_type=IterNodeType.VALUES,
                 apply_type=IterNodeApplyType.SERIES_ITEMS,
                 )
 
-    @property # type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window_array_items(self) -> IterNodeWindow['Frame']:
         '''
         Iterator of pairs of label, windowed values, where values are given as a :obj:`np.array`.
 
         {args}
         '''
@@ -4432,15 +4434,15 @@
         return self.__class__(
                 blocks, # does not copy arrays
                 index=index,
                 columns=columns,
                 name=self._name,
                 own_data=True,
                 own_index=index is not IndexAutoFactory,
-                own_columns=columns is not IndexAutoFactory, # type: ignore
+                own_columns=columns is not IndexAutoFactory,
                 )
 
 
 
     def rehierarch(self,
             index: tp.Optional[tp.Iterable[int]] = None,
             columns: tp.Optional[tp.Iterable[int]] = None,
@@ -5493,15 +5495,15 @@
                 raise AxisInvalid(f'no support for axis {axis}')
             # uses _make method to call with iterable
             ctor = get_tuple_constructor(labels)
         elif isinstance(constructor, type):
             if (issubclass(constructor, tuple) and
                     hasattr(constructor, '_make')):
                 # discover named tuples, use _make method for single-value calling
-                ctor = constructor._make # type: ignore
+                ctor = constructor._make
             elif is_dataclass(constructor):
                 # this will fail if kw_only is true in python 3.10
                 ctor = lambda args: constructor(*args)
             else: # assume it can take a single arguments
                 ctor = constructor
         else:
             ctor = constructor #type: ignore
```

### Comparing `static-frame-1.4.6/static_frame/core/hloc.py` & `static-frame-1.5.0/static_frame/core/hloc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 from static_frame.core.util import EMPTY_TUPLE
 from static_frame.core.util import GetItemKeyType
 from static_frame.core.util import key_to_str
```

### Comparing `static-frame-1.4.6/static_frame/core/index.py` & `static-frame-1.5.0/static_frame/core/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from collections import Counter
 from copy import deepcopy
 from itertools import chain
 from itertools import zip_longest
 
 import numpy as np
@@ -458,15 +460,15 @@
                 apply_type=IterNodeApplyType.INDEX_LABELS
                 )
 
 
     #---------------------------------------------------------------------------
     # common attributes from the numpy array
 
-    @property # type: ignore
+    @property
     @doc_inject()
     def mloc(self) -> int:
         '''{doc_int}
         '''
         if self._recache:
             self._update_array_cache()
         return mloc(self._labels)
@@ -701,15 +703,15 @@
                 header_depth=header_depth,
                 style_config=style_config,
                 )
 
     #---------------------------------------------------------------------------
     # core internal representation
 
-    @property #type: ignore
+    @property
     @doc_inject(selector='values_1d', class_name='Index')
     def values(self) -> np.ndarray:
         '''
         {}
         '''
         if self._recache:
             self._update_array_cache()
```

### Comparing `static-frame-1.4.6/static_frame/core/index_auto.py` & `static-frame-1.5.0/static_frame/core/index_auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.exception import InvalidDatetime64Initializer
 from static_frame.core.index import Index
```

### Comparing `static-frame-1.4.6/static_frame/core/index_base.py` & `static-frame-1.5.0/static_frame/core/index_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from functools import partial
 from itertools import chain
 
 import numpy as np
 from arraykit import resolve_dtype
 
@@ -319,15 +321,15 @@
             key: GetItemKeyType
             ) -> tp.Union[I, tp.Hashable]:
         raise NotImplementedError() #pragma: no cover
 
     #---------------------------------------------------------------------------
     # name interface
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def name(self) -> NameType:
         '''{}'''
         return self._name
 
     def _name_is_names(self) -> bool:
         return isinstance(self._name, tuple) and len(self._name) == self.depth
```

### Comparing `static-frame-1.4.6/static_frame/core/index_correspondence.py` & `static-frame-1.5.0/static_frame/core/index_correspondence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 from static_frame.core.util import DTYPE_BOOL
 from static_frame.core.util import GetItemKeyType
 from static_frame.core.util import PositionsAllocator
 from static_frame.core.util import array2d_to_tuples
 from static_frame.core.util import intersect1d
```

### Comparing `static-frame-1.4.6/static_frame/core/index_datetime.py` & `static-frame-1.5.0/static_frame/core/index_datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import typing as tp
 from functools import partial
 
 import numpy as np
 from arraymap import AutoMap  # pylint: disable = E0611
```

### Comparing `static-frame-1.4.6/static_frame/core/index_hierarchy.py` & `static-frame-1.5.0/static_frame/core/index_hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import itertools
 import operator
 import typing as tp
 from ast import literal_eval
 from copy import deepcopy
 from functools import partial
 from itertools import chain
@@ -99,15 +101,15 @@
     from static_frame.core.series import Series  # pylint: disable=W0611,C0412 # pragma: no cover
 
 IH = tp.TypeVar('IH', bound='IndexHierarchy')
 IHGO = tp.TypeVar('IHGO', bound='IndexHierarchyGO')
 IHAsType = tp.TypeVar('IHAsType', bound='IndexHierarchyAsType')
 
 SingleLabelType = tp.Tuple[tp.Hashable, ...]
-TreeNodeT = tp.Dict[tp.Hashable, tp.Union[tp.Sequence[tp.Hashable], 'TreeNodeT']]
+TreeNodeT = tp.Dict[tp.Hashable, tp.Union[Index, 'TreeNodeT']]
 
 _NBYTES_GETTER = operator.attrgetter('nbytes')
 
 CompoundLabelType = tp.Tuple[tp.Union[slice, tp.Hashable, tp.List[tp.Hashable]], ...]
 LocKeyType = tp.Union[
     'IndexHierarchy',
     HLoc,
@@ -157,15 +159,15 @@
     all_index_reps = np.cumprod(padded_lengths[::-1])[-3::-1]
 
     # Impl borrowed from pandas/core/reshape/util.py:cartesian_product
     result = np.array(
         [
             np.tile(
                     np.repeat(PositionsAllocator.get(list_length), repeats=all_index_reps[i]),
-                    reps=np.product(all_group_reps[i])
+                    reps=np.prod(all_group_reps[i])
                     )
             for i, list_length
             in enumerate(list_lengths)
         ],
         dtype=DTYPE_INT_DEFAULT,
     )
     result.flags.writeable = False
@@ -2451,15 +2453,15 @@
         if all(isinstance(other, IndexHierarchy) for other in others):
             return index_hierarchy_difference(self, *others) # type: ignore
 
         return IndexBase.difference(self, *others)
 
     #---------------------------------------------------------------------------
 
-    def _drop_missing(self,
+    def _drop_missing(self: IH,
             func: tp.Callable[[np.ndarray], np.ndarray],
             condition: tp.Callable[[np.ndarray], bool],
             ) -> IH:
         '''
         Return a new obj:`IndexHierarchy` after removing rows (axis 0) or columns (axis 1) where any or all values are NA (NaN or None). The condition is determined by  a NumPy ufunc that process the Boolean array returned by ``isna()``; the default is ``np.all``.
 
         Args:
@@ -2469,31 +2471,31 @@
         # returns Boolean areas that define axis to keep
         row_key, _ = self._blocks.drop_missing_to_keep_locations(
                 axis=0, # always labels (rows) for IH
                 condition=condition,
                 func=func,
                 )
         if self.STATIC and row_key.all(): #type: ignore
-            return self #type: ignore
+            return self
 
         return self._drop_iloc(~row_key) #type: ignore
 
-    def dropna(self, *,
+    def dropna(self: IH, *,
             condition: tp.Callable[[np.ndarray], bool] = np.all,
             ) -> IH:
         '''
         Return a new obj:`IndexHierarchy` after removing labels where any or all values are NA (NaN or None). The condition is determined by a NumPy ufunc that process the Boolean array returned by ``isna()``; the default is ``np.all``.
 
         Args:
             *,
             condition:
         '''
         return self._drop_missing(isna_array, condition)
 
-    def dropfalsy(self, *,
+    def dropfalsy(self: IH, *,
             condition: tp.Callable[[np.ndarray], bool] = np.all,
             ) -> IH:
         '''
         Return a new obj:`IndexHierarchy` after removing labels where any or all values are falsy. The condition is determined by a NumPy ufunc that process the Boolean array returned by ``isna()``; the default is ``np.all``.
 
         Args:
             *,
```

### Comparing `static-frame-1.4.6/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-1.5.0/static_frame/core/index_hierarchy_set_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from functools import partial
 
 import numpy as np
 
 from static_frame.core.container_util import index_many_to_one
 from static_frame.core.exception import ErrorInitIndex
```

### Comparing `static-frame-1.4.6/static_frame/core/interface.py` & `static-frame-1.5.0/static_frame/core/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 '''
 Tools for documenting the SF interface.
 '''
+from __future__ import annotations
+
 import inspect
 import typing as tp
 from collections import namedtuple
 from itertools import chain
 
 import numpy as np
 
@@ -61,14 +63,15 @@
 from static_frame.core.node_selector import Interface
 from static_frame.core.node_selector import InterfaceAssignQuartet
 from static_frame.core.node_selector import InterfaceAssignTrio
 from static_frame.core.node_selector import InterfaceAsType
 from static_frame.core.node_selector import InterfaceBatchAsType
 from static_frame.core.node_selector import InterfaceConsolidate
 from static_frame.core.node_selector import InterfaceGetItem
+from static_frame.core.node_selector import InterfaceGetItemCompound
 from static_frame.core.node_selector import InterfaceSelectDuo
 from static_frame.core.node_selector import InterfaceSelectTrio
 from static_frame.core.node_selector import TContainer
 from static_frame.core.node_str import InterfaceBatchString
 from static_frame.core.node_str import InterfaceString
 from static_frame.core.node_transpose import InterfaceBatchTranspose
 from static_frame.core.node_transpose import InterfaceTranspose
@@ -720,15 +723,15 @@
                 reference,
                 use_signature=True,
                 is_attr=True, # doc as attr so sphinx does not add parens to sig
                 signature_no_args=signature_no_args,
                 )
         # TypeBlocks as iter_* methods that are just functions
         if hasattr(obj, 'CLS_DELEGATE'):
-            cls_interface = obj.CLS_DELEGATE #type: ignore
+            cls_interface = obj.CLS_DELEGATE
             # IterNodeDelegate or IterNodeDelegateMapable
 
             for field in cls_interface.INTERFACE: # apply, map, etc
                 delegate_obj = getattr(cls_interface, field)
                 delegate_reference = f'{cls_interface.__name__}.{field}'
                 doc = Features.scrub_doc(
                         delegate_obj.__doc__,
@@ -1186,15 +1189,15 @@
                 yield from InterfaceRecord.gen_from_consolidate(**kwargs)
             elif callable(obj) and name.startswith('from_') or name == '__init__':
                 yield from InterfaceRecord.gen_from_constructor(**kwargs)
             elif callable(obj) and name.startswith('to_'):
                 yield from InterfaceRecord.gen_from_exporter(**kwargs)
             elif name.startswith('iter_'):
                 yield from InterfaceRecord.gen_from_iterator(**kwargs)
-            elif isinstance(obj, InterfaceGetItem) or name == cls.GETITEM:
+            elif isinstance(obj, (InterfaceGetItem, InterfaceGetItemCompound)) or name == cls.GETITEM:
                 yield from InterfaceRecord.gen_from_getitem(**kwargs)
 
             elif obj.__class__ in INTERFACE_ATTRIBUTE_CLS:
                 yield from InterfaceRecord.gen_from_accessor(
                         cls_interface=obj.__class__,
                         **kwargs,
                         )
```

### Comparing `static-frame-1.4.6/static_frame/core/interface_meta.py` & `static-frame-1.5.0/static_frame/core/interface_meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+from __future__ import annotations
+
 import typing as tp
 
 from static_frame.core.doc_str import doc_inject
 
 if tp.TYPE_CHECKING:
     from static_frame.core.frame import Frame  # pylint: disable=W0611 #pragma: no cover
 
 class InterfaceMeta(type):
     '''Lowest level metaclass for providing interface property on class.
     '''
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def interface(cls) -> 'Frame':
         '''{}'''
         from static_frame.core.interface import InterfaceSummary
         return InterfaceSummary.to_frame(cls) #type: ignore
```

### Comparing `static-frame-1.4.6/static_frame/core/join.py` & `static-frame-1.5.0/static_frame/core/join.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from itertools import chain
 from itertools import product
 
 import numpy as np
 from arraykit import resolve_dtype
```

### Comparing `static-frame-1.4.6/static_frame/core/loc_map.py` & `static-frame-1.5.0/static_frame/core/loc_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import itertools
 import sys
 import typing as tp
 from copy import deepcopy
 from functools import reduce
 
 import numpy as np
```

### Comparing `static-frame-1.4.6/static_frame/core/memory_measure.py` & `static-frame-1.5.0/static_frame/core/memory_measure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from collections import abc
 from itertools import chain
 from sys import getsizeof
 from typing import NamedTuple
 
 import numpy as np
```

### Comparing `static-frame-1.4.6/static_frame/core/node_dt.py` & `static-frame-1.5.0/static_frame/core/node_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 from datetime import date
 from datetime import datetime
 
 import numpy as np
 from arraykit import isna_element
```

### Comparing `static-frame-1.4.6/static_frame/core/node_fill_value.py` & `static-frame-1.5.0/static_frame/core/node_fill_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.node_selector import Interface
 from static_frame.core.node_selector import InterfaceBatch
 from static_frame.core.node_selector import InterfaceGetItem
```

### Comparing `static-frame-1.4.6/static_frame/core/node_hashlib.py` & `static-frame-1.5.0/static_frame/core/node_hashlib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hashlib
 import typing as tp
 
 if tp.TYPE_CHECKING:
     from hashlib import _Hash  # pylint: disable = W0611 #pragma: no cover
     from hashlib import _VarLenHash  # pylint: disable = W0611 #pragma: no cover
```

### Comparing `static-frame-1.4.6/static_frame/core/node_iter.py` & `static-frame-1.5.0/static_frame/core/node_iter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''
 Tools for iterators in Series and Frame. These components are imported by both series.py and frame.py; these components also need to be able to return Series and Frame, and thus use deferred, function-based imports.
 '''
+from __future__ import annotations
 
 import typing as tp
 from enum import Enum
 from functools import partial
 
 import numpy as np
 from arraykit import name_filter
```

### Comparing `static-frame-1.4.6/static_frame/core/node_re.py` & `static-frame-1.5.0/static_frame/core/node_re.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.node_selector import Interface
 from static_frame.core.node_selector import InterfaceBatch
```

### Comparing `static-frame-1.4.6/static_frame/core/node_selector.py` & `static-frame-1.5.0/static_frame/core/node_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.assign import Assign
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.util import NULL_SLICE
 from static_frame.core.util import AnyCallable
 from static_frame.core.util import DtypesSpecifier
 from static_frame.core.util import GetItemKeyType
+from static_frame.core.util import GetItemKeyTypeCompound
 
 # from static_frame.core.util import AnyCallable
 
 if tp.TYPE_CHECKING:
     from static_frame.core.batch import Batch  # pylint: disable = W0611 #pragma: no cover
     from static_frame.core.bus import Bus  # pylint: disable = W0611 #pragma: no cover
     from static_frame.core.frame import Frame  # pylint: disable = W0611 #pragma: no cover
@@ -55,18 +58,31 @@
 
     __slots__ = ('_func',)
     INTERFACE = ('__getitem__',)
 
     _func: tp.Callable[[GetItemKeyType], TContainer]
 
     def __init__(self, func: tp.Callable[[GetItemKeyType], TContainer]) -> None:
-        self._func = func #type: ignore
+        self._func = func
 
     def __getitem__(self, key: GetItemKeyType) -> TContainer:
-        return self._func(key) #type: ignore
+        return self._func(key)
+
+class InterfaceGetItemCompound(Interface[TContainer]):
+
+    __slots__ = ('_func',)
+    INTERFACE = ('__getitem__',)
+
+    _func: tp.Callable[[GetItemKeyTypeCompound], TContainer]
+
+    def __init__(self, func: tp.Callable[[GetItemKeyTypeCompound], TContainer]) -> None:
+        self._func = func
+
+    def __getitem__(self, key: GetItemKeyTypeCompound) -> TContainer:
+        return self._func(key)
 
 #-------------------------------------------------------------------------------
 
 class InterfaceSelectDuo(Interface[TContainer]):
     '''An instance to serve as an interface to all of iloc and loc
     '''
```

### Comparing `static-frame-1.4.6/static_frame/core/node_str.py` & `static-frame-1.5.0/static_frame/core/node_str.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from functools import reduce
 
 import numpy as np
 from numpy import char as npc
 
 from static_frame.core.container_util import get_col_format_factory
```

### Comparing `static-frame-1.4.6/static_frame/core/node_transpose.py` & `static-frame-1.5.0/static_frame/core/node_transpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.node_selector import Interface
 from static_frame.core.node_selector import InterfaceBatch
```

### Comparing `static-frame-1.4.6/static_frame/core/node_values.py` & `static-frame-1.5.0/static_frame/core/node_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 from arraykit import column_2d_filter
 
 from static_frame.core.node_selector import Interface
 from static_frame.core.node_selector import InterfaceBatch
```

### Comparing `static-frame-1.4.6/static_frame/core/pivot.py` & `static-frame-1.5.0/static_frame/core/pivot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from collections import defaultdict
 from functools import partial
 from itertools import chain
 from itertools import product
 from itertools import repeat
```

### Comparing `static-frame-1.4.6/static_frame/core/platform.py` & `static-frame-1.5.0/static_frame/core/platform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import importlib
 import platform as platform_mod
 import sys
 import typing as tp
 
 import static_frame
 from static_frame.core.display import Display
```

### Comparing `static-frame-1.4.6/static_frame/core/protocol_dfi.py` & `static-frame-1.5.0/static_frame/core/protocol_dfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.protocol_dfi_abc import Buffer
 from static_frame.core.protocol_dfi_abc import CategoricalDescription
 from static_frame.core.protocol_dfi_abc import Column
```

### Comparing `static-frame-1.4.6/static_frame/core/protocol_dfi_abc.py` & `static-frame-1.5.0/static_frame/core/protocol_dfi_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import enum
 from abc import ABC
 from abc import abstractmethod
 from typing import Any
 from typing import Dict
 from typing import Iterable
 from typing import Optional
```

### Comparing `static-frame-1.4.6/static_frame/core/quilt.py` & `static-frame-1.5.0/static_frame/core/quilt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from functools import partial
 from itertools import chain
 from itertools import repeat
 from itertools import zip_longest
 
 import numpy as np
@@ -27,15 +29,15 @@
 from static_frame.core.index_base import IndexBase
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.node_iter import IterNodeApplyType
 from static_frame.core.node_iter import IterNodeAxis
 from static_frame.core.node_iter import IterNodeConstructorAxis
 from static_frame.core.node_iter import IterNodeType
 from static_frame.core.node_iter import IterNodeWindow
-from static_frame.core.node_selector import InterfaceGetItem
+from static_frame.core.node_selector import InterfaceGetItemCompound
 from static_frame.core.series import Series
 from static_frame.core.store import Store
 from static_frame.core.store_client_mixin import StoreClientMixin
 from static_frame.core.store_config import StoreConfigMapInitializer
 from static_frame.core.store_hdf5 import StoreHDF5
 from static_frame.core.store_sqlite import StoreSQLite
 from static_frame.core.store_xlsx import StoreXLSX
@@ -109,32 +111,32 @@
         starts = range(0, vector_len, chunksize)
         if len(starts) == 1:
             ends: tp.Iterable[int] = (vector_len,)
         else:
             ends = range(starts[1], vector_len, chunksize)
 
         if label_extractor is None:
-            label_extractor = lambda x: x.iloc[0] #type: ignore
+            label_extractor = lambda x: x.iloc[0]
 
         axis_map_components: tp.Dict[tp.Hashable, IndexBase] = {}
         opposite = None
 
         def values() -> tp.Iterator[Frame]:
             nonlocal opposite
 
             for start, end in zip_longest(starts, ends, fillvalue=vector_len):
                 if axis == 0: # along rows
                     f = frame.iloc[start:end]
-                    label = label_extractor(f.index) #type: ignore
+                    label = label_extractor(f.index)
                     axis_map_components[label] = f.index
                     if opposite is None:
                         opposite = f.columns
                 elif axis == 1: # along columns
                     f = frame.iloc[NULL_SLICE, start:end]
-                    label = label_extractor(f.columns) #type: ignore
+                    label = label_extractor(f.columns)
                     axis_map_components[label] = f.columns
                     if opposite is None:
                         opposite = f.index
                 else:
                     raise AxisInvalid(f'invalid axis {axis}')
                 yield f.rename(label)
 
@@ -511,15 +513,15 @@
         '''For the :obj:`Bus` or :obj:`Yarn` contained in this object, replace all loaded :obj:`Frame` with :obj:`FrameDeferred`.
         '''
         self._bus.unpersist()
 
     #---------------------------------------------------------------------------
     # name interface
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def name(self) -> NameType:
         '''{}'''
         return self._bus.name #type: ignore
 
     def rename(self, name: NameType) -> 'Quilt':
         '''
@@ -597,15 +599,15 @@
             if d._rows[-1][-1] == Display.CELL_ELLIPSIS:
                 d._rows[-1].pop()
         return d
 
     #---------------------------------------------------------------------------
     # accessors
 
-    @property #type: ignore
+    @property
     @doc_inject(selector='values_2d', class_name='Quilt')
     def values(self) -> np.ndarray:
         '''
         {}
         '''
         if self._assign_axis:
             self._update_axis_labels()
@@ -1144,20 +1146,20 @@
             self._update_axis_labels()
         return self._extract(*self._compound_loc_to_getitem_iloc(key))
 
     #---------------------------------------------------------------------------
     # interfaces
 
     @property
-    def loc(self) -> InterfaceGetItem['Frame']:
-        return InterfaceGetItem(self._extract_loc) #type: ignore
+    def loc(self) -> InterfaceGetItemCompound['Frame']:
+        return InterfaceGetItemCompound(self._extract_loc) #type: ignore
 
     @property
-    def iloc(self) -> InterfaceGetItem['Frame']:
-        return InterfaceGetItem(self._extract_iloc) #type: ignore
+    def iloc(self) -> InterfaceGetItemCompound['Frame']:
+        return InterfaceGetItemCompound(self._extract_iloc) #type: ignore
 
     #---------------------------------------------------------------------------
     # iterators
 
     @property
     def iter_array(self) -> IterNodeAxis['Quilt']:
         '''
@@ -1247,15 +1249,15 @@
                 yield_type=IterNodeType.ITEMS,
                 apply_type=IterNodeApplyType.SERIES_VALUES,
                 )
 
 
     #---------------------------------------------------------------------------
 
-    @property #type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window(self) -> IterNodeWindow['Quilt']:
         '''
         Iterator of windowed values, where values are given as a :obj:`Frame`.
 
         {args}
         '''
@@ -1267,15 +1269,15 @@
                 container=self,
                 function_values=function_values,
                 function_items=function_items,
                 yield_type=IterNodeType.VALUES,
                 apply_type=IterNodeApplyType.SERIES_ITEMS,
                 )
 
-    @property #type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window_items(self) -> IterNodeWindow['Quilt']:
         '''
         Iterator of pairs of label, windowed values, where values are given as a :obj:`Frame`.
 
         {args}
         '''
@@ -1287,15 +1289,15 @@
                 container=self,
                 function_values=function_values,
                 function_items=function_items,
                 yield_type=IterNodeType.ITEMS,
                 apply_type=IterNodeApplyType.SERIES_ITEMS,
                 )
 
-    @property #type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window_array(self) -> IterNodeWindow['Quilt']:
         '''
         Iterator of windowed values, where values are given as a :obj:`np.array`.
 
         {args}
         '''
@@ -1307,15 +1309,15 @@
                 container=self,
                 function_values=function_values,
                 function_items=function_items,
                 yield_type=IterNodeType.VALUES,
                 apply_type=IterNodeApplyType.SERIES_ITEMS,
                 )
 
-    @property #type: ignore
+    @property
     @doc_inject(selector='window')
     def iter_window_array_items(self) -> IterNodeWindow['Quilt']:
         '''
         Iterator of pairs of label, windowed values, where values are given as a :obj:`np.array`.
 
         {args}
         '''
```

### Comparing `static-frame-1.4.6/static_frame/core/rank.py` & `static-frame-1.5.0/static_frame/core/rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from enum import Enum
 
 import numpy as np
 
 from static_frame.core.util import DEFAULT_STABLE_SORT_KIND
 from static_frame.core.util import DTYPE_BOOL
```

### Comparing `static-frame-1.4.6/static_frame/core/series.py` & `static-frame-1.5.0/static_frame/core/series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import csv
 import typing as tp
 from collections.abc import Set
 from copy import deepcopy
 from functools import partial
 from itertools import chain
 from itertools import product
@@ -548,15 +550,15 @@
                     # set up for direct assignment below; index is always immutable
                     index = values.index
                     own_index = True
                 if name is NAME_DEFAULT:
                     name = values.name # propagate Series.name
             elif hasattr(values, '__iter__') and not isinstance(values, str):
                 # returned array is already immutable
-                self.values, _ = iterable_to_array_1d(values, dtype=dtype) #type: ignore
+                self.values, _ = iterable_to_array_1d(values, dtype=dtype)
             else: # it must be an element, or a string
                 raise ErrorInitSeries('Use Series.from_element to create a Series from an element.')
 
         else: # is numpy array
             if dtype is not None and dtype != values.dtype: #type: ignore
                 raise ErrorInitSeries(f'when supplying values via array, the dtype argument is not required; if provided ({dtype}), it must agree with the dtype of the array ({values.dtype})') #type: ignore
 
@@ -656,15 +658,15 @@
             :obj:`Index`
         '''
         return reversed(self._index)
 
     #---------------------------------------------------------------------------
     # name interface
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def name(self) -> NameType:
         '''{}'''
         return self._name
 
     def rename(self,
             name: NameType = NAME_DEFAULT,
@@ -1808,15 +1810,15 @@
                 display_cls=display_cls,
                 style_config=style_config,
                 )
 
     #---------------------------------------------------------------------------
     # common attributes from the numpy array
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def mloc(self) -> int:
         '''{doc_int}
         '''
         return mloc(self.values)
 
     @property
@@ -1890,15 +1892,18 @@
 
     def _extract_loc(self, key: GetItemKeyType) -> 'Series':
         '''
         Compatibility:
             Pandas supports taking in iterables of keys, where some keys are not found in the index; a Series is returned as if a reindex operation was performed. This is undesirable. Better instead is to use reindex()
         '''
         iloc_key = self._index._loc_to_iloc(key)
-        values = self.values[iloc_key]
+        try:
+            values = self.values[iloc_key]
+        except IndexError as e:
+            raise KeyError(iloc_key) from e
 
         if isinstance(iloc_key, INT_TYPES): # if we have a single element
             # NOTE: cannot check if we have an array as an array might be an element
             return values #type: ignore
 
         return self.__class__(values,
                 index=self._index.iloc[iloc_key],
```

### Comparing `static-frame-1.4.6/static_frame/core/store.py` & `static-frame-1.5.0/static_frame/core/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import os
 import typing as tp
 from functools import partial
 from functools import wraps
 from itertools import chain
 from weakref import WeakValueDictionary
```

### Comparing `static-frame-1.4.6/static_frame/core/store_client_mixin.py` & `static-frame-1.5.0/static_frame/core/store_client_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 import zipfile
 
 from static_frame.core.doc_str import doc_inject
 from static_frame.core.store_config import StoreConfigMap
 from static_frame.core.store_config import StoreConfigMapInitializer
```

### Comparing `static-frame-1.4.6/static_frame/core/store_config.py` & `static-frame-1.5.0/static_frame/core/store_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import typing as tp
 
 from static_frame.core.exception import ErrorInitStoreConfig
 from static_frame.core.frame import Frame
 from static_frame.core.interface_meta import InterfaceMeta
 from static_frame.core.util import DepthLevelSpecifier
```

### Comparing `static-frame-1.4.6/static_frame/core/store_filter.py` & `static-frame-1.5.0/static_frame/core/store_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.interface_meta import InterfaceMeta
 from static_frame.core.util import COMPLEX_TYPES
 from static_frame.core.util import DT64_MONTH
```

### Comparing `static-frame-1.4.6/static_frame/core/store_hdf5.py` & `static-frame-1.5.0/static_frame/core/store_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 # from static_frame.core.doc_str import doc_inject
 from static_frame.core.frame import Frame
 from static_frame.core.store import Store
```

### Comparing `static-frame-1.4.6/static_frame/core/store_sqlite.py` & `static-frame-1.5.0/static_frame/core/store_sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import sqlite3
 import typing as tp
 from contextlib import suppress
 from fractions import Fraction
 
 import numpy as np
```

### Comparing `static-frame-1.4.6/static_frame/core/store_xlsx.py` & `static-frame-1.5.0/static_frame/core/store_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 
 import datetime
 import typing as tp
 from functools import partial
 
 import numpy as np
 
@@ -262,25 +263,25 @@
                             )
 
         # post process to merge cells; need to get width of at depth
         if include_columns and merge_hierarchical_labels and columns_depth > 1:
             for depth in range(columns_depth - 1): # never most deep
                 row = depth
                 col = index_depth_effective # start after index
-                for label, width in frame._columns.label_widths_at_depth(depth):
+                for label, width in frame._columns.label_widths_at_depth(depth): # type: ignore
                     # TODO: use store_filter
                     if width > 1:
                         ws.merge_range(row, col, row, col + width - 1, label, format_columns)
                     col += width
 
         if include_index and merge_hierarchical_labels and index_depth > 1:
             for depth in range(index_depth - 1): # never most deep
                 row = columns_depth_effective
                 col = depth
-                for label, width in frame._index.label_widths_at_depth(depth):
+                for label, width in frame._index.label_widths_at_depth(depth): # type: ignore
                     # TODO: use store_filter
                     if width > 1:
                         ws.merge_range(row, col, row + width - 1, col, label, format_index)
                     row += width
 
     @store_coherent_write
     def write(self,
```

### Comparing `static-frame-1.4.6/static_frame/core/store_zip.py` & `static-frame-1.5.0/static_frame/core/store_zip.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import pickle
 import typing as tp
 import zipfile
 from io import BytesIO
 from io import StringIO
```

### Comparing `static-frame-1.4.6/static_frame/core/style_config.py` & `static-frame-1.5.0/static_frame/core/style_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 from static_frame.core.display_color import HexColor
 
 if tp.TYPE_CHECKING:
     from static_frame.core.container import ContainerOperand  # pylint: disable=W0611 #pragma: no cover
```

### Comparing `static-frame-1.4.6/static_frame/core/type_blocks.py` & `static-frame-1.5.0/static_frame/core/type_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from functools import partial
 from itertools import chain
 from itertools import repeat
 from itertools import zip_longest
 
 import numpy as np
@@ -630,15 +632,15 @@
         Return an immutable array that, for each block, reports the shape as a tuple.
         '''
         a = np.empty(len(self._blocks), dtype=DTYPE_OBJECT)
         a[:] = [b.shape for b in self._blocks]
         a.flags.writeable = False
         return a
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def mloc(self) -> np.ndarray:
         '''{doc_array}
         '''
         a = np.fromiter(
                 (mloc(b) for b in self._blocks),
                 count=len(self._blocks),
@@ -1468,17 +1470,24 @@
         Returns:
             A generator iterable of pairs, where values are pairs of either a block index and slice or, a block index and column index.
         '''
         if key is None or (key.__class__ is slice and key == NULL_SLICE):
             yield from self._index.iter_block()
         elif isinstance(key, INT_TYPES):
             # the index has the pair block, column integer
-            yield self._index[key]
+            try:
+                yield self._index[key]
+            except IndexError as e:
+                raise KeyError(key) from e
         else: # all cases where we try to get contiguous slices
-            yield from self._index.iter_contiguous(key, ascending=not retain_key_order)
+            try:
+                yield from self._index.iter_contiguous(key, ascending=not retain_key_order)
+            except TypeError as e:
+                # BlockIndex will raise TypeErrors in a number of cases of bad inputs; some of these are not easy to change
+                raise KeyError(key) from e
 
     #---------------------------------------------------------------------------
     def _mask_blocks(self,
             row_key: tp.Optional[GetItemKeyTypeCompound] = None,
             column_key: tp.Optional[GetItemKeyTypeCompound] = None) -> tp.Iterator[np.ndarray]:
         '''Return Boolean blocks of the same size and shape, where key selection sets values to True.
         '''
@@ -2661,15 +2670,15 @@
                         # If `row_key`` selects a non-array, we have selected an element; if b is an object dtype, we might have selected a list or other iterable that, if naively given to an array constructor, gets "flattened" into arrays. Thus, we create an empty and assign
                         b_fill = np.empty(1, dtype=b.dtype)
                         b_fill[0] = b_row
                         b_fill.flags.writeable = False
                         yield b_fill
         else:
             # convert column_key into a series of block slices; we have to do this as we stride blocks; do not have to convert row_key as can use directly per block slice
-            for block_idx, slc in self._key_to_block_slices(column_key): # PERF: most time from line profiler
+            for block_idx, slc in self._key_to_block_slices(column_key):
                 b = self._blocks[block_idx]
                 if b.ndim == 1: # given 1D array, our row key is all we need
                     if row_key_null:
                         b_sliced = b
                     else:
                         b_sliced = b[row_key] # PERF: slow from line profiler
                 else: # given 2D, use row key and column slice
@@ -2762,15 +2771,19 @@
         return array
 
     def _extract_array_column(self,
             key: int,
             ) -> np.ndarray:
         '''Alternative extractor that returns full-column arrays from single integer selection.
         '''
-        block_idx, column = self._index[key]
+        try:
+            block_idx, column = self._index[key]
+        except IndexError as e:
+            raise KeyError(key) from e
+
         b = self._blocks[block_idx]
         if b.ndim == 1:
             return b
         return b[NULL_SLICE, column]
 
     def iter_row_elements(self,
             key: int,
```

### Comparing `static-frame-1.4.6/static_frame/core/util.py` & `static-frame-1.5.0/static_frame/core/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,19 +335,14 @@
     '''
     if value is None:
         return False
     if value.__class__ is bool or value.__class__ is np.bool_:
         return False
     return isinstance(value, INT_TYPES)
 
-def is_dataclass(value: tp.Any) -> bool:
-    # avoid module-level import
-    from dataclasses import is_dataclass
-    return is_dataclass(value)
-
 def validate_depth_selection(
         key: GetItemKeyType,
         ) -> None:
     '''Determine if a key is strictly an ILoc-style key. This is used in `IndexHierarchy`, where at times we select "columns" (or depths) by integer (not name or per-depth names, as such attributes are not required), and we cannot assume the caller gives us integers, as some types of inputs (Python lists of Booleans) might work due to low-level duckyness.
 
     This does not permit selection by tuple elements at this time, as that is not possible for IndexHierarchy depth selection.
     '''
@@ -637,15 +632,15 @@
         self._gen: tp.Iterator[FGItemT]
         if hasattr(gen, '__next__'):
             self._gen = gen #type: ignore
         else:
             self._gen = iter(gen)
         self._src: tp.List[FGItemT] = []
 
-    def __getitem__(self, key: int) -> FGItemT:
+    def __getitem__(self, key: int) -> FGItemT: # type: ignore
         start = len(self._src)
         if key >= start:
             for k in range(start, key + 1):
                 try:
                     self._src.append(next(self._gen))
                 except StopIteration:
                     raise IndexError(k) from None
```

### Comparing `static-frame-1.4.6/static_frame/core/www.py` & `static-frame-1.5.0/static_frame/core/www.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import gzip
 import os
 import tempfile
 import typing as tp
 from io import BytesIO
 from io import StringIO
 from pathlib import Path
```

### Comparing `static-frame-1.4.6/static_frame/core/yarn.py` & `static-frame-1.5.0/static_frame/core/yarn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from collections.abc import Set
 from itertools import chain
 
 import numpy as np
 
 from static_frame.core.axis_map import buses_to_hierarchy
@@ -212,15 +214,15 @@
             :obj:`Index`
         '''
         return reversed(self._index)
 
     #---------------------------------------------------------------------------
     # name interface
 
-    @property #type: ignore
+    @property
     @doc_inject()
     def name(self) -> NameType:
         '''{}'''
         return self._series._name
 
     def rename(self, name: NameType) -> 'Yarn':
         '''
```

### Comparing `static-frame-1.4.6/static_frame/test/test_case.py` & `static-frame-1.5.0/static_frame/test/test_case.py`

 * *Files identical despite different names*

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_archive_npy.py` & `static-frame-1.5.0/static_frame/test/unit/test_archive_npy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import contextlib
 import os
 import zipfile
 from io import StringIO
 from io import UnsupportedOperation
 from tempfile import TemporaryDirectory
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_axis_map.py` & `static-frame-1.5.0/static_frame/test/unit/test_axis_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame.core.axis_map import bus_to_hierarchy
 from static_frame.core.axis_map import buses_to_hierarchy
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_batch.py` & `static-frame-1.5.0/static_frame/test/unit/test_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import time
 import typing as tp
 
 import frame_fixtures as ff
 import numpy as np
 
@@ -825,15 +827,15 @@
                 index=('z', 'y', 'x'),
                 name='f1')
         f2 = Frame.from_dict(
                 dict(b=(1, 20.234, 1.043), a=(1.043, 50.828, 1.043)),
                 index=('y', 'z', 'x'),
                 name='f2')
 
-        f3 = round(Batch.from_frames((f1, f2)), 1).to_frame() #type: ignore
+        f3 = round(Batch.from_frames((f1, f2)), 1).to_frame()
         self.assertEqual(f3.to_pairs(0),
                 (('b', ((('f1', 'z'), 20.0), (('f1', 'y'), 20.2), (('f1', 'x'), 0.0), (('f2', 'y'), 1.0), (('f2', 'z'), 20.2), (('f2', 'x'), 1.0))), ('a', ((('f1', 'z'), 20.2), (('f1', 'y'), 20.2), (('f1', 'x'), 50.8), (('f2', 'y'), 1.0), (('f2', 'z'), 50.8), (('f2', 'x'), 1.0))))
                 )
 
     #---------------------------------------------------------------------------
 
     def test_batch_roll_a(self) -> None:
@@ -1115,70 +1117,70 @@
         i = [1,4,7,2,5,8,3,6,9]
         f0 = Frame.from_items(
             (
                 ('i',i),
                 ('b',(b%2==0 for b in i))
             )
         )
-        f123 = (f0.iloc[0:3],f0.iloc[3:6],f0.iloc[6:9])
+        f123 = (f0.iloc[0:3], f0.iloc[3:6], f0.iloc[6:9])
         b123 = Batch.from_frames(f123).rank_dense()
         for i,(_, f) in enumerate(b123.items()): # type: ignore
-            self.assertEqual(f.values.tolist(), f123[i].rank_dense().values.tolist())
+            self.assertEqual(f.values.tolist(), f123[i].rank_dense().values.tolist()) # type: ignore
 
     def test_batch_rank_max(self) -> None:
         i = [1,4,7,2,5,8,3,6,9]
         f0 = Frame.from_items(
             (
                 ('i',i),
                 ('b',(b%2==0 for b in i))
             )
         )
         f123 = (f0.iloc[0:3],f0.iloc[3:6],f0.iloc[6:9])
         b123 = Batch.from_frames(f123).rank_max()
         for i,(_, f) in enumerate(b123.items()): # type: ignore
-            self.assertEqual(f.values.tolist(), f123[i].rank_max().values.tolist())
+            self.assertEqual(f.values.tolist(), f123[i].rank_max().values.tolist()) # type: ignore
 
     def test_batch_rank_mean(self) -> None:
         i = [1,4,7,2,5,8,3,6,9]
         f0 = Frame.from_items(
             (
                 ('i',i),
                 ('b',(b%2==0 for b in i))
             )
         )
         f123 = (f0.iloc[0:3],f0.iloc[3:6],f0.iloc[6:9])
         b123 = Batch.from_frames(f123).rank_mean()
         for i,(_, f) in enumerate(b123.items()): # type: ignore
-            self.assertEqual(f.values.tolist(), f123[i].rank_mean().values.tolist())
+            self.assertEqual(f.values.tolist(), f123[i].rank_mean().values.tolist()) # type: ignore
 
     def test_batch_rank_min(self) -> None:
         i = [1,4,7,2,5,8,3,6,9]
         f0 = Frame.from_items(
             (
                 ('i',i),
                 ('b',(b%2==0 for b in i))
             )
         )
         f123 = (f0.iloc[0:3],f0.iloc[3:6],f0.iloc[6:9])
         b123 = Batch.from_frames(f123).rank_min()
         for i,(_, f) in enumerate(b123.items()): # type: ignore
-            self.assertEqual(f.values.tolist(), f123[i].rank_min().values.tolist())
+            self.assertEqual(f.values.tolist(), f123[i].rank_min().values.tolist()) # type: ignore
 
     def test_batch_rank_ordinal(self) -> None:
         i = [1,4,7,2,5,8,3,6,9]
         f0 = Frame.from_items(
             (
                 ('i',i),
                 ('b',(b%2==0 for b in i))
             )
         )
         f123 = (f0.iloc[0:3],f0.iloc[3:6],f0.iloc[6:9])
         b123 = Batch.from_frames(f123).rank_ordinal()
         for i,(_, f) in enumerate(b123.items()): # type: ignore
-            self.assertEqual(f.values.tolist(), f123[i].rank_ordinal().values.tolist())
+            self.assertEqual(f.values.tolist(), f123[i].rank_ordinal().values.tolist()) # type: ignore
 
     #---------------------------------------------------------------------------
     def test_batch_shift_a(self) -> None:
         f1 = Frame.from_dict(
                 dict(b=(20,20,0), a=(20,20,50)),
                 index=('z', 'y', 'x'),
                 name='f1')
@@ -1325,15 +1327,15 @@
                 name='f1')
         f2 = Frame.from_dict(
                 dict(b=(1,10,100), a=(1,2,3)),
                 index=('y', 'z', 'x'),
                 name='f2')
 
         f3 = Batch.from_frames((f1, f2)).corr().to_frame()
-        self.assertEqual(round(f3, 6).to_pairs(), # type: ignore
+        self.assertEqual(round(f3, 6).to_pairs(),
                 (('b', ((('f1', 'b'), 1.0), (('f1', 'a'), 1.0), (('f2', 'b'), 1.0), (('f2', 'a'), 0.904194))), ('a', ((('f1', 'b'), 1.0), (('f1', 'a'), 1.0), (('f2', 'b'), 0.904194), (('f2', 'a'), 1.0))))
                 )
 
     #---------------------------------------------------------------------------
 
     def test_batch_count_a(self) -> None:
         f1 = Frame.from_dict(
@@ -1672,15 +1674,15 @@
 
 
     #---------------------------------------------------------------------------
     def test_batch_via_values_a(self) -> None:
         f1 = ff.parse('s(2,3)|v(int)|c(I,str)').rename('a')
         f2 = ff.parse('s(2,3)|v(int)|c(I,str)').rename('b')
         post = Batch.from_frames((f1, f2)).via_values.apply(np.cos).to_frame()
-        self.assertEqual(round(post, 2).to_pairs(), #type: ignore
+        self.assertEqual(round(post, 2).to_pairs(),
                 (('zZbu', ((('a', 0), -0.54), (('a', 1), 0.05), (('b', 0), -0.54), (('b', 1), 0.05))), ('ztsv', ((('a', 0), -0.96), (('a', 1), -0.54), (('b', 0), -0.96), (('b', 1), -0.54))), ('zUvW', ((('a', 0), -0.82), (('a', 1), 1.0), (('b', 0), -0.82), (('b', 1), 1.0))))
                 )
 
     def test_batch_via_values_b(self) -> None:
         f1 = ff.parse('s(2,3)|v(int)|c(I,str)').rename('a')
         f2 = ff.parse('s(2,3)|v(int)|c(I,str)').rename('b')
         post = np.sin(Batch.from_frames((f1, f2)).via_values).to_frame()
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_bus.py` & `static-frame-1.5.0/static_frame/test/unit/test_bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import os
 import pickle
 import typing as tp
 from datetime import date
 from datetime import datetime
 from hashlib import sha256
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_container.py` & `static-frame-1.5.0/static_frame/test/unit/test_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from static_frame.core.container import ContainerOperand
 from static_frame.core.interface import UFUNC_AXIS_SKIPNA
 from static_frame.core.interface import UFUNC_SHAPE_SKIPNA
 from static_frame.test.test_case import TestCase
 
 
 class TestUnit(TestCase):
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_container_util.py` & `static-frame-1.5.0/static_frame/test/unit/test_container_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import typing as tp
 
 import numpy as np
 
 from static_frame import Frame
 from static_frame import Index
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_display.py` & `static-frame-1.5.0/static_frame/test/unit/test_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import hashlib
 import json
 import string
 import typing as tp
 import unittest
 from itertools import combinations
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_display_color.py` & `static-frame-1.5.0/static_frame/test/unit/test_display_color.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,12 @@
+from __future__ import annotations
+
 from static_frame.core.display_color import HexColor
 from static_frame.test.test_case import TestCase
 
-# assuming located in the same directory
-# from static_frame import Index
-# from static_frame import IndexGO
-# from static_frame import Series
-# from static_frame import Frame
-# from static_frame import FrameGO
-# from static_frame import TypeBlocks
-# from static_frame import Display
-# from static_frame import mloc
-# from static_frame import DisplayConfig
-# from static_frame import DisplayConfigs
-
 
 class TestUnit(TestCase):
 
     def test_hex_str_to_int_a(self) -> None:
         post = HexColor._hex_str_to_int('aqua')
         self.assertEqual(post, 65535)
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_doc.py` & `static-frame-1.5.0/static_frame/test/unit/test_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import doctest
 import os
 import typing as tp
 
 from static_frame.test.test_case import TestCase
 from static_frame.test.test_case import skip_win
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-1.5.0/static_frame/test/unit/test_fill_value_auto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from static_frame.core.fill_value_auto import FillValueAuto
 from static_frame.core.util import NAT
 from static_frame.core.util import NAT_TD64
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_frame.py` & `static-frame-1.5.0/static_frame/test/unit/test_frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import dataclasses
 import datetime
 import io
 import itertools as it
 import os
 import pickle
@@ -1693,14 +1695,19 @@
         self.assertEqual(f1[('A', 2)].to_pairs(),
                 (('x', 2), ('y', 50))
                 )
         self.assertEqual(f1[[('A', 2), ('B', 1)]].to_pairs(0),
                 ((('A', 2), (('x', 2), ('y', 50))), (('B', 1), (('x', 'a'), ('y', 'b'))))
                 )
 
+    def test_frame_getitem_e(self) -> None:
+        f = sf.Frame()
+        with self.assertRaises(KeyError):
+            _ = f['a']
+
     #---------------------------------------------------------------------------
 
     def test_frame_length_a(self) -> None:
 
         records = (
                 (1, 2, 'a', False, True),
                 (30, 50, 'b', True, False))
@@ -2869,15 +2876,15 @@
         f2 = f1.assign.loc[:, f1.columns % 2 == 0](0)
 
         self.assertEqual(f2.to_pairs(),
                 ((0, ((0, 0), (1, 0))), (1, ((0, 162197), (1, -41157))), (2, ((0, 0), (1, 0))), (3, ((0, 129017), (1, 35021))), (4, ((0, 0), (1, 0))), (5, ((0, 84967), (1, 13448))), (6, ((0, 0), (1, 0))), (7, ((0, 137759), (1, -62964))), (8, ((0, 0), (1, 0))), (9, ((0, 126025), (1, 59728)))))
 
         self.assertEqual(f1.loc[:, f1.columns % 2 == 0].columns.values.tolist(),
                 [0, 2, 4, 6, 8]
-)
+                )
 
     #---------------------------------------------------------------------------
 
     def test_frame_assign_iloc_a(self) -> None:
 
         records = (
                 (1, 2, 'a', False, True),
@@ -9845,15 +9852,15 @@
         self.assertEqual(
                 f1.to_pairs(0),
                 ((0, ((0, 'x'), (1, 1))), (1, ((0, 't'), (1, 2))))
                 )
 
     def test_frame_from_records_p(self) -> None:
 
-        records = [('x', 't')] * 10 + [(1, 2)] #type: ignore
+        records = [('x', 't')] * 10 + [(1, 2)]
         f1 = sf.Frame.from_records(records)
         self.assertEqual(f1.to_pairs(0),
                 ((0, ((0, 'x'), (1, 'x'), (2, 'x'), (3, 'x'), (4, 'x'), (5, 'x'), (6, 'x'), (7, 'x'), (8, 'x'), (9, 'x'), (10, 1))), (1, ((0, 't'), (1, 't'), (2, 't'), (3, 't'), (4, 't'), (5, 't'), (6, 't'), (7, 't'), (8, 't'), (9, 't'), (10, 2))))
                 )
 
     def test_frame_from_records_q(self) -> None:
 
@@ -10698,15 +10705,15 @@
                     return self.frame #type: ignore
 
             c = C()
             f1 = c.mmap_frame
             self.assertEqual(f1.shape, (3, 3))
 
             s1 = c.mmap_frame.iloc[0]
-            self.assertEqual(round(s1, 1).to_pairs(), #type: ignore
+            self.assertEqual(round(s1, 1).to_pairs(),
                 ((0, 1930.4), (1, -610.8), (2, 694.3))
                 )
             c.__del__()
 
     def test_frame_from_npy_memory_map_e(self) -> None:
         f1 = ff.parse('s(3,3)|v(str,bool)').astype[2](object)
         with TemporaryDirectory() as fp:
@@ -10837,14 +10844,19 @@
 
         f2 = f1.astype[['c', 'd']](float)
         self.assertEqual(f2._blocks.shapes.tolist(),
                 [(2,), (2,), (2,), (2,)]
                 )
 
 
+    def test_frame_astype_k(self) -> None:
+        f1 = Frame(np.arange(12).reshape(3, 4))
+        with self.assertRaises(KeyError):
+            _ = f1.astype[20](float)
+
 
     #---------------------------------------------------------------------------
 
     def test_frame_pickle_a(self) -> None:
 
         records = (
                 (1, 2, 'a', False, True),
@@ -11574,15 +11586,15 @@
         self.assertEqual(f2.to_pairs(0),
                 (('a', (('x', 20), ('y', 20), ('z', 30))), ('b', (('x', 40), ('y', 20), ('z', 30))), ('c', (('x', 20), ('y', 20), ('z', 20))), ('d', (('x', 20), ('y', 20), ('z', 20)))))
 
     def test_frame_clip_l(self) -> None:
         f1 = ff.parse('s(2,6)|v(int,int,int,float,float,float)')
         f2 = ff.parse('s(2,6)|v(int,float)') * 0
         f3 = f1.clip(lower=f2)
-        self.assertEqual(round(f3).to_pairs(), #type: ignore
+        self.assertEqual(round(f3).to_pairs(),
                 ((0, ((0, 0.0), (1, 92867.0))), (1, ((0, 162197.0), (1, 0.0))), (2, ((0, 0.0), (1, 91301.0))), (3, ((0, 1080.0), (1, 2580.0))), (4, ((0, 3512.0), (1, 1175.0))), (5, ((0, 1857.0), (1, 1699.0))))
                 )
 
     #---------------------------------------------------------------------------
 
     def test_frame_from_dict_a(self) -> None:
 
@@ -13244,21 +13256,21 @@
     def test_frame_round_a(self) -> None:
         a1 = np.full(4, .33333, )
         a2 = np.full((4, 2), .88888, )
         a3 = np.full(4, .55555)
         tb1 = TypeBlocks.from_blocks((a1, a2, a3))
 
         f1 = Frame(tb1)
-        f2 = round(f1) #type: ignore
+        f2 = round(f1)
 
         self.assertEqual(f2.to_pairs(0),
                 ((0, ((0, 0.0), (1, 0.0), (2, 0.0), (3, 0.0))), (1, ((0, 1.0), (1, 1.0), (2, 1.0), (3, 1.0))), (2, ((0, 1.0), (1, 1.0), (2, 1.0), (3, 1.0))), (3, ((0, 1.0), (1, 1.0), (2, 1.0), (3, 1.0))))
                 )
 
-        f3 = round(f1, 2) #type: ignore
+        f3 = round(f1, 2)
         self.assertEqual(f3.to_pairs(0),
                 ((0, ((0, 0.33), (1, 0.33), (2, 0.33), (3, 0.33))), (1, ((0, 0.89), (1, 0.89), (2, 0.89), (3, 0.89))), (2, ((0, 0.89), (1, 0.89), (2, 0.89), (3, 0.89))), (3, ((0, 0.56), (1, 0.56), (2, 0.56), (3, 0.56))))
                 )
 
     #---------------------------------------------------------------------------
 
     def test_frame_str_capitalize_a(self) -> None:
@@ -13664,42 +13676,42 @@
     def test_frame_via_values_a(self) -> None:
 
         f = ff.parse('s(3,4)|v(int,float)|c(I,str)')
         # post1 = abs(f).via_values.apply(np.log)
 
         post1 = np.log(abs(f).via_values)
 
-        self.assertEqual(round(post1.fillna(0)).astype(int).to_pairs(), #type: ignore
+        self.assertEqual(round(post1.fillna(0)).astype(int).to_pairs(),
                 (('zZbu', ((0, 11), (1, 11), (2, 11))), ('ztsv', ((0, 6), (1, 8), (2, 7))), ('zUvW', ((0, 8), (1, 11), (2, 10))), ('zkuW', ((0, 7), (1, 8), (2, 7))))
                 )
 
         post2 = np.log(abs(f).via_values(unify_blocks=True))
-        self.assertEqual(round(post2.fillna(0)).astype(int).to_pairs(), #type: ignore
+        self.assertEqual(round(post2.fillna(0)).astype(int).to_pairs(),
                 (('zZbu', ((0, 11), (1, 11), (2, 11))), ('ztsv', ((0, 6), (1, 8), (2, 7))), ('zUvW', ((0, 8), (1, 11), (2, 10))), ('zkuW', ((0, 7), (1, 8), (2, 7))))
                 )
 
         post3 = np.log(abs(f).via_values(consolidate_blocks=True))
-        self.assertEqual(round(post3.fillna(0)).astype(int).to_pairs(), #type: ignore
+        self.assertEqual(round(post3.fillna(0)).astype(int).to_pairs(),
                 (('zZbu', ((0, 11), (1, 11), (2, 11))), ('ztsv', ((0, 6), (1, 8), (2, 7))), ('zUvW', ((0, 8), (1, 11), (2, 10))), ('zkuW', ((0, 7), (1, 8), (2, 7))))
                 )
 
         post4 = np.log(abs(f).via_values(consolidate_blocks=True, dtype=float))
-        self.assertEqual(round(post4.fillna(0)).astype(int).to_pairs(), #type: ignore
+        self.assertEqual(round(post4.fillna(0)).astype(int).to_pairs(),
                 (('zZbu', ((0, 11), (1, 11), (2, 11))), ('ztsv', ((0, 6), (1, 8), (2, 7))), ('zUvW', ((0, 8), (1, 11), (2, 10))), ('zkuW', ((0, 7), (1, 8), (2, 7))))
                 )
 
         post1 = np.log(abs(f).via_values(dtype=float))
-        self.assertEqual(round(post1.fillna(0)).astype(int).to_pairs(), #type: ignore
+        self.assertEqual(round(post1.fillna(0)).astype(int).to_pairs(),
                 (('zZbu', ((0, 11), (1, 11), (2, 11))), ('ztsv', ((0, 6), (1, 8), (2, 7))), ('zUvW', ((0, 8), (1, 11), (2, 10))), ('zkuW', ((0, 7), (1, 8), (2, 7))))
                 )
 
     def test_frame_via_values_b(self) -> None:
         f = ff.parse('s(3,4)|v(bool)|c(I,str)')
         post1 = np.sin(f.via_values)
-        self.assertEqual(round(post1).to_pairs(), #type: ignore
+        self.assertEqual(round(post1).to_pairs(),
                 (('zZbu', ((0, 0.0), (1, 0.0), (2, 0.0))), ('ztsv', ((0, 0.0), (1, 0.0), (2, 0.0))), ('zUvW', ((0, 1.0), (1, 0.0), (2, 0.0))), ('zkuW', ((0, 0.0), (1, 0.0), (2, 1.0))))
                 )
 
     def test_frame_via_values_c(self) -> None:
         f = ff.parse('s(3,4)|v(float)|c(I,str)')
         post1 = np.cos(f.via_values)
         self.assertEqual(post1.values.round(2).tolist(),
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_frame_he.py` & `static-frame-1.5.0/static_frame/test/unit/test_frame_he.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import frame_fixtures as ff
 
 from static_frame import FrameHE
 from static_frame.test.test_case import TestCase
 
 
 class TestUnit(TestCase):
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_frame_iter.py` & `static-frame-1.5.0/static_frame/test/unit/test_frame_iter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import frame_fixtures as ff
 import numpy as np
 
 import static_frame as sf
 from static_frame import Frame
@@ -570,14 +572,25 @@
                 index_constructor=IndexDate)
 
         self.assertEqual(post.index.__class__, IndexDate)
         self.assertEqual(post.to_pairs(),
             ((np.datetime64('1998-10-12'), 1),
             (np.datetime64('1998-10-13'), 2)))
 
+    def test_frame_iter_group_h(self) -> None:
+        f1 = sf.Frame(np.arange(25).reshape(5, 5), index=tuple("ABCDE"))
+
+        with self.assertRaises(KeyError):
+            f1.iter_group(-99).apply(lambda x: x)
+
+        with self.assertRaises(KeyError):
+            s2 = f1.iter_group('z').apply(lambda x: x)
+
+
+
     #---------------------------------------------------------------------------
     def test_frame_iter_group_array_a(self) -> None:
         f1 = ff.parse('s(7,3)|v(int)').assign[1].apply(
                 lambda s: s % 3)
 
         post = tuple(f1.iter_group_array(1))
         self.assertEqual([p.shape for p in post],
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_frame_join.py` & `static-frame-1.5.0/static_frame/test/unit/test_frame_join.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-# import frame_fixtures as ff
+from __future__ import annotations
+
 import numpy as np
 
 import static_frame as sf
 from static_frame import Frame
 from static_frame import IndexDate
 from static_frame import IndexHierarchy
 from static_frame.core.exception import InvalidFillValue
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-1.5.0/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame import Frame
 from static_frame import FrameGO
 from static_frame import Series
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_frame_via_re.py` & `static-frame-1.5.0/static_frame/test/unit/test_frame_via_re.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import re
 
 import frame_fixtures as ff
 
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_hloc.py` & `static-frame-1.5.0/static_frame/test/unit/test_hloc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 
 from static_frame import HLoc
 from static_frame.test.test_case import TestCase
 
 
 class TestUnit(TestCase):
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index.py` & `static-frame-1.5.0/static_frame/test/unit/test_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import datetime
 import pickle
 import typing as tp
 import unittest
 from hashlib import sha256
 from io import StringIO
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index_auto.py` & `static-frame-1.5.0/static_frame/test/unit/test_index_auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame.core.index import Index
 from static_frame.core.index import IndexGO
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index_base.py` & `static-frame-1.5.0/static_frame/test/unit/test_index_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from static_frame.core.index_base import IndexBase
 from static_frame.test.test_case import TestCase
 
 
 class TestUnit(TestCase):
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index_correspondence.py` & `static-frame-1.5.0/static_frame/test/unit/test_index_correspondence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from static_frame.core.index import Index
 from static_frame.core.index_correspondence import IndexCorrespondence
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index_datetime.py` & `static-frame-1.5.0/static_frame/test/unit/test_index_datetime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 from itertools import product
 
 import numpy as np
 
 from static_frame import Frame
 from static_frame import FrameGO
@@ -81,20 +83,20 @@
         self.assertEqual((index == '2017').sum(), 9)
         self.assertEqual((index == '2018-02').sum(), 14)
         self.assertEqual((index == '2018').sum(), 37)
 
     def test_index_date_d(self) -> None:
         index = IndexDate.from_date_range('2017-12-15', '2018-03-15', 2)
         # selct by year and year month
-        self.assertAlmostEqualValues(index.loc['2017'].values, #type: ignore
+        self.assertAlmostEqualValues(index.loc['2017'].values,
                 np.array(['2017-12-15', '2017-12-17', '2017-12-19', '2017-12-21',
                '2017-12-23', '2017-12-25', '2017-12-27', '2017-12-29',
                '2017-12-31'], dtype='datetime64[D]'))
 
-        self.assertAlmostEqualValues(index.loc['2018-02'].values, #type: ignore
+        self.assertAlmostEqualValues(index.loc['2018-02'].values,
                 np.array(['2018-02-01', '2018-02-03', '2018-02-05', '2018-02-07',
                '2018-02-09', '2018-02-11', '2018-02-13', '2018-02-15',
                '2018-02-17', '2018-02-19', '2018-02-21', '2018-02-23',
                '2018-02-25', '2018-02-27'], dtype='datetime64[D]'))
 
         self.assertEqual(index.loc['2018-02-19'],
                 np.datetime64('2018-02-19'))
@@ -425,38 +427,38 @@
             index.loc[np.datetime64('2004-01')]
 
 
     def test_index_year_loc_b(self) -> None:
 
         idx1 = IndexYear.from_year_range(1998, 2008)
         idx2 = idx1.loc[2002:2004]
-        self.assertEqual(tuple(idx2.values), # type: ignore
+        self.assertEqual(tuple(idx2.values),
             (np.datetime64('2002'), np.datetime64('2003'), np.datetime64('2004')))
 
         idx3 = idx1.loc['2002':'2004']
-        self.assertEqual(tuple(idx3.values), # type: ignore
+        self.assertEqual(tuple(idx3.values),
             (np.datetime64('2002'), np.datetime64('2003'), np.datetime64('2004')))
 
     def test_index_year_loc_c(self) -> None:
 
         idx1 = IndexYear.from_year_range(1998, 2008)
         idx2 = idx1.loc[[2001, 2004, 2005]]
-        self.assertEqual(tuple(idx2.values), # type: ignore
+        self.assertEqual(tuple(idx2.values),
             (np.datetime64('2001'), np.datetime64('2004'), np.datetime64('2005')))
 
         idx3 = idx1.loc[[2001, 2004, 2005]]
-        self.assertEqual(tuple(idx3.values), # type: ignore
+        self.assertEqual(tuple(idx3.values),
             (np.datetime64('2001'), np.datetime64('2004'), np.datetime64('2005')))
 
         idx4 = idx1.loc[(v for v in [2001, 2004, 2005])]
-        self.assertEqual(tuple(idx4.values), # type: ignore
+        self.assertEqual(tuple(idx4.values),
             (np.datetime64('2001'), np.datetime64('2004'), np.datetime64('2005')))
 
         idx5 = idx1.loc[np.array([2001, 2004, 2005])]
-        self.assertEqual(tuple(idx5.values), # type: ignore
+        self.assertEqual(tuple(idx5.values),
             (np.datetime64('2001'), np.datetime64('2004'), np.datetime64('2005')))
 
     def test_index_year_loc_d(self) -> None:
 
         idx1 = IndexYear.from_year_range(1998, 2008)
         with self.assertRaises(LocInvalid):
             idx2 = idx1.loc['2000-01-01': '2003-01-01']
@@ -514,21 +516,21 @@
                 np.datetime64('2016-04-30T20:21:07.848'))
 
         self.assertAlmostEqualValues(
                 idx.loc['2016-05-01T09:26:43.185':].values,  # type: ignore  # https://github.com/python/typeshed/pull/3024
                 np.array(['2016-05-01T09:26:43.185', '2016-05-01T13:45:22.576',
        '2016-05-01T15:25:46.150'], dtype='datetime64[ms]'))
 
-        self.assertAlmostEqualValues(idx.loc['2016-05'].values, #type: ignore
+        self.assertAlmostEqualValues(idx.loc['2016-05'].values,
                 np.array(['2016-05-01T00:00:33.483', '2016-05-01T03:02:03.584',
                '2016-05-01T09:26:43.185', '2016-05-01T13:45:22.576',
                '2016-05-01T15:25:46.150'], dtype='datetime64[ms]')
                 )
 
-        self.assertEqual(idx.loc['2016-05-01T00'].values, #type: ignore
+        self.assertEqual(idx.loc['2016-05-01T00'].values,
                 np.array(['2016-05-01T00:00:33.483'], dtype='datetime64[ms]'))
 
     def test_index_millisecond_b(self) -> None:
         # integer arguments are interpreted as milliseconds from the epoch
         idx = IndexMillisecond(range(10))
         self.assertAlmostEqualValues(idx.loc['1970-01-01T00:00:00.007':].values,  # type: ignore  # https://github.com/python/typeshed/pull/3024
                 np.array(['1970-01-01T00:00:00.007', '1970-01-01T00:00:00.008',
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-1.5.0/static_frame/test/unit/test_index_hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import datetime
 import pickle
 import typing as tp
 import unittest
 from collections import OrderedDict
 from functools import wraps
@@ -1617,15 +1619,15 @@
         with self.assertRaises(RuntimeError):
             (True, False, True, False) in ih #pylint: disable=W0104
 
     def test_hierarchy_contains_d(self) -> None:
         labels = ((True, 'A'), ('I', 'B'))
         ih = IndexHierarchy.from_labels(labels)
 
-        key = HLoc[:, 'A']
+        key = HLoc[:, 'A'] # type: ignore
 
         ih2 = ih.loc[key]
         self.assertEqual(tuple(ih2), ((True, 'A'),))
 
         self.assertIn(key, ih)
 
     def test_hierarchy_extract_a(self) -> None:
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-1.5.0/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 from string import ascii_letters
 
 from static_frame.core.index_base import IndexBase
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.index_hierarchy_set_utils import index_hierarchy_difference
 from static_frame.core.index_hierarchy_set_utils import index_hierarchy_intersection
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_interface.py` & `static-frame-1.5.0/static_frame/test/unit/test_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from static_frame import FillValueAuto
 from static_frame.core.frame import Frame
 from static_frame.core.frame import FrameGO
 from static_frame.core.interface import DOCUMENTED_COMPONENTS
 from static_frame.core.interface import InterfaceGroup
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_loc_map.py` & `static-frame-1.5.0/static_frame/test/unit/test_loc_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from copy import deepcopy
 
 import numpy as np
 
 from static_frame import IndexHierarchy
 from static_frame.core.exception import ErrorInitIndexNonUnique
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_memory_measure.py` & `static-frame-1.5.0/static_frame/test/unit/test_memory_measure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import unittest
 from sys import getsizeof
 
 import frame_fixtures as ff
 import numpy as np
 from arraymap import FrozenAutoMap  # pylint: disable=E0611
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-1.5.0/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 import unittest
 from sys import getsizeof
 
 import frame_fixtures as ff
 import numpy as np
 from arraymap import FrozenAutoMap  # pylint: disable=E0611
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_pivot.py` & `static-frame-1.5.0/static_frame/test/unit/test_pivot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame.core.frame import Frame
 from static_frame.core.index import Index
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.pivot import pivot_items_to_block
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-1.5.0/static_frame/test/unit/test_protocol_dfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame.core.index import Index
 from static_frame.core.protocol_dfi import ArrowCType
 from static_frame.core.protocol_dfi import DFIBuffer
 from static_frame.core.protocol_dfi import DFIColumn
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_quilt.py` & `static-frame-1.5.0/static_frame/test/unit/test_quilt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from hashlib import sha256
 
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame.core.axis_map import bus_to_hierarchy
@@ -31,14 +33,15 @@
 
         f1 = Frame.from_dict(
                 dict(a=(1,2), b=(3,4)),
                 index=('x', 'y'),
                 name='f1')
         f2 = Frame.from_dict(
                 dict(a=(1,2,3), b=(4,5,6)),
+
                 index=('x', 'y', 'z'),
                 name='f2')
         f3 = Frame.from_dict(
                 dict(a=(10,20), b=(50,60)),
                 index=('p', 'q'),
                 name='f3')
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_rank.py` & `static-frame-1.5.0/static_frame/test/unit/test_rank.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import numpy as np
 
 from static_frame.core.rank import RankMethod
 from static_frame.core.rank import rank_1d
 from static_frame.core.rank import rank_2d
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_series.py` & `static-frame-1.5.0/static_frame/test/unit/test_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import datetime
 import pickle
 import re
 import string
 import typing as tp
 from collections import OrderedDict
@@ -2387,14 +2389,21 @@
         s1 = Series(range(4), index=('a', 'b', 'c', 'd'))
         self.assertEqual(s1.get('q'), None)
         self.assertEqual(s1.get('a'), 0)
         self.assertEqual(s1.get('f', -1), -1)
 
     #---------------------------------------------------------------------------
 
+    def test_series_get_item_a(self) -> None:
+        s1 = Series(range(4))
+        with self.assertRaises(KeyError):
+            _ = s1[-99]
+
+    #---------------------------------------------------------------------------
+
     def test_series_all_a(self) -> None:
         s1 = Series(range(4), index=('a', 'b', 'c', 'd'))
 
         self.assertEqual(s1.all(), False)
         self.assertEqual(s1.any(), True)
 
     def test_series_all_b(self) -> None:
@@ -3987,15 +3996,15 @@
         with self.assertRaises(ValueError):
             bool(s1)
 
     #---------------------------------------------------------------------------
 
     def test_series_round_a(self) -> None:
         s1 = Series(np.arange(8) + .001)
-        s2 = round(s1) #type: ignore
+        s2 = round(s1)
 
         self.assertEqual(s2.to_pairs(),
                 ((0, 0.0), (1, 1.0), (2, 2.0), (3, 3.0), (4, 4.0), (5, 5.0), (6, 6.0), (7, 7.0)))
 
     #---------------------------------------------------------------------------
 
     def test_series_str_capitalize_a1(self) -> None:
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_series_he.py` & `static-frame-1.5.0/static_frame/test/unit/test_series_he.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import frame_fixtures as ff
 
 from static_frame import ILoc
 from static_frame import Series
 from static_frame import SeriesHE
 from static_frame.test.test_case import TestCase
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_store.py` & `static-frame-1.5.0/static_frame/test/unit/test_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import pickle
 from itertools import product
 
 import numpy as np
 
 from static_frame.core.exception import ErrorInitStoreConfig
 from static_frame.core.exception import StoreParameterConflict
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_store_filter.py` & `static-frame-1.5.0/static_frame/test/unit/test_store_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 from io import StringIO
 
 import numpy as np
 
 from static_frame.core.frame import Frame
 from static_frame.core.store_filter import STORE_FILTER_DEFAULT
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_store_hdf5.py` & `static-frame-1.5.0/static_frame/test/unit/test_store_hdf5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 from static_frame.core.frame import Frame
 from static_frame.core.index_hierarchy import IndexHierarchy
 from static_frame.core.store_config import StoreConfig
 from static_frame.core.store_config import StoreConfigMap
 from static_frame.core.store_hdf5 import StoreHDF5
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_store_sqlite.py` & `static-frame-1.5.0/static_frame/test/unit/test_store_sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 from fractions import Fraction
 
 import numpy as np
 
 from static_frame.core.frame import Frame
 from static_frame.core.index_hierarchy import IndexHierarchy
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_store_xlsx.py` & `static-frame-1.5.0/static_frame/test/unit/test_store_xlsx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import numpy as np
 
 from static_frame.core.frame import Frame
 from static_frame.core.hloc import HLoc
 from static_frame.core.index_hierarchy import IndexHierarchy
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_store_zip.py` & `static-frame-1.5.0/static_frame/test/unit/test_store_zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import typing as tp
 
 import frame_fixtures as ff
 
 from static_frame.core.exception import ErrorInitStore
 from static_frame.core.frame import Frame
 from static_frame.core.frame import FrameGO
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_style_config.py` & `static-frame-1.5.0/static_frame/test/unit/test_style_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from static_frame.core.frame import Frame
 from static_frame.core.style_config import StyleConfig
 from static_frame.core.style_config import style_config_css_factory
 from static_frame.test.test_case import TestCase
 
 
 class TestUnit(TestCase):
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_type_blocks.py` & `static-frame-1.5.0/static_frame/test/unit/test_type_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import copy
 import pickle
 from itertools import zip_longest
 
 import frame_fixtures as ff
 import numpy as np
 from arraykit import ErrorInitTypeBlocks
@@ -3577,20 +3579,20 @@
     def test_type_blocks_round_a(self) -> None:
 
         a1 = np.full(4, .33333, )
         a2 = np.full((4, 2), .88888, )
         a3 = np.full(4, .55555)
         tb1 = TypeBlocks.from_blocks((a1, a2, a3))
 
-        tb2 = round(tb1, 3) #type: ignore
+        tb2 = round(tb1, 3)
         self.assertEqual(
                 tb2.values.tolist(),
                 [[0.333, 0.889, 0.889, 0.556], [0.333, 0.889, 0.889, 0.556], [0.333, 0.889, 0.889, 0.556], [0.333, 0.889, 0.889, 0.556]]
                 )
-        tb3 = round(tb1, 1) #type: ignore
+        tb3 = round(tb1, 1)
         self.assertEqual(
                 tb3.values.tolist(),
                 [[0.3, 0.9, 0.9, 0.6], [0.3, 0.9, 0.9, 0.6], [0.3, 0.9, 0.9, 0.6], [0.3, 0.9, 0.9, 0.6]]
                 )
 
     #---------------------------------------------------------------------------
 
@@ -4117,15 +4119,15 @@
         a1 = np.array([False, True, False])
         tb1 = TypeBlocks.from_blocks((a1, ))
         self.assertTrue(tb1.unified_dtypes)
 
     #---------------------------------------------------------------------------
     def test_type_blocks_key_to_block_slices_exception(self) -> None:
         # as this is an loc-is-iloc index, the key gets passed directly to type blocks
-        with self.assertRaises(TypeError):
+        with self.assertRaises(KeyError):
             ff.parse('v(bool,str,bool,float)|s(4,8)')["foo"]
 
 
     def test_type_blocks_consolidate_select_a1(self) -> None:
 
         a1 = np.array([1, 2, 3])
         a2 = np.array([4, 5, 6])
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_util.py` & `static-frame-1.5.0/static_frame/test/unit/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 import json
 import typing as tp
 import unittest
 import warnings
 from enum import Enum
 from functools import partial
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_www.py` & `static-frame-1.5.0/static_frame/test/unit/test_www.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import gzip
 import io
 # import json
 import os
 import typing as tp
 import unittest
 from pathlib import Path
```

### Comparing `static-frame-1.4.6/static_frame/test/unit/test_yarn.py` & `static-frame-1.5.0/static_frame/test/unit/test_yarn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import datetime
 from hashlib import sha256
 
 import frame_fixtures as ff
 import numpy as np
 
 from static_frame import HLoc
```

### Comparing `static-frame-1.4.6/static_frame.egg-info/PKG-INFO` & `static-frame-1.5.0/static_frame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 1.4.6
+Version: 1.5.0
 Summary: Immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Description: A library of immutable and grow-only Pandas-like DataFrames with a more explicit and consistent interface. StaticFrame is suitable for applications in data science, data engineering, finance, scientific computing, and related fields where reducing opportunities for error by prohibiting in-place mutation is critical.
         
         While many interfaces are similar to Pandas, StaticFrame deviates from Pandas in many ways: all data is immutable, and all indices are unique; the full range of NumPy data types is preserved, and date-time indices use discrete NumPy units; hierarchical indices are seamlessly integrated; and uniform approaches to element, row, and column iteration and function application are provided. Core StaticFrame depends only on NumPy and two C-extension packages (maintained by the StaticFrame team): Pandas is not a dependency.
@@ -54,22 +54,22 @@
         
         
         Dependencies
         --------------
         
         Core StaticFrame requires the following:
         
-        - Python>=3.7
-        - NumPy>=1.18.5
+        - Python>=3.8
+        - numpy>=1.19.5
         - arraymap==0.1.9
         - arraykit==0.4.9
         
         For extended input and output, the following packages are required:
         
-        - pandas>=0.24.2
+        - pandas>=0.25.3
         - xlsxwriter>=1.1.2
         - openpyxl>=3.0.9
         - xarray>=0.13.0
         - tables>=3.6.1
         - pyarrow>=0.17.0
         - visidata>=2.4
         
@@ -362,14 +362,13 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >3.7.0
+Requires-Python: >=3.8
 Provides-Extra: extras
```

### Comparing `static-frame-1.4.6/static_frame.egg-info/SOURCES.txt` & `static-frame-1.5.0/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

