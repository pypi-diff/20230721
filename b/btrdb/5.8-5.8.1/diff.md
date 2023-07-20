# Comparing `tmp/btrdb-5.8.tar.gz` & `tmp/btrdb-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/btrdb-5.8.tar", last modified: Wed May 13 21:30:48 2020, max compression
+gzip compressed data, was "dist/btrdb-5.8.1.tar", last modified: Mon Jun 29 21:11:37 2020, max compression
```

## Comparing `btrdb-5.8.tar` & `btrdb-5.8.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.910657 btrdb-5.8/
--rw-r--r--   0 allen      (501) staff       (20)     1151 2020-05-13 21:11:01.000000 btrdb-5.8/.travis.yml
--rw-r--r--   0 allen      (501) staff       (20)      472 2019-03-06 21:01:18.000000 btrdb-5.8/DESCRIPTION.md
--rw-r--r--   0 allen      (501) staff       (20)     1678 2019-03-06 20:58:55.000000 btrdb-5.8/LICENSE.txt
--rw-r--r--   0 allen      (501) staff       (20)      346 2019-04-29 19:25:09.000000 btrdb-5.8/MANIFEST.in
--rw-r--r--   0 allen      (501) staff       (20)     1671 2019-11-18 16:49:45.000000 btrdb-5.8/Makefile
--rw-r--r--   0 allen      (501) staff       (20)     1905 2020-05-13 21:30:48.910936 btrdb-5.8/PKG-INFO
--rw-r--r--   0 allen      (501) staff       (20)     6561 2019-03-06 21:01:18.000000 btrdb-5.8/README.md
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.835634 btrdb-5.8/btrdb/
--rw-r--r--   0 allen      (501) staff       (20)     2674 2019-06-18 14:54:46.000000 btrdb-5.8/btrdb/__init__.py
--rw-r--r--   0 allen      (501) staff       (20)    10995 2019-06-20 20:48:30.000000 btrdb-5.8/btrdb/conn.py
--rw-r--r--   0 allen      (501) staff       (20)    10467 2019-11-27 20:09:10.000000 btrdb-5.8/btrdb/endpoint.py
--rw-r--r--   0 allen      (501) staff       (20)     1953 2019-06-20 13:27:12.000000 btrdb-5.8/btrdb/exceptions.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.844326 btrdb-5.8/btrdb/grpcinterface/
--rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8/btrdb/grpcinterface/__init__.py
--rw-r--r--   0 allen      (501) staff       (20)     7133 2019-03-06 21:01:19.000000 btrdb-5.8/btrdb/grpcinterface/btrdb.proto
--rw-r--r--   0 allen      (501) staff       (20)   124824 2019-05-08 20:25:29.000000 btrdb-5.8/btrdb/grpcinterface/btrdb_pb2.py
--rw-r--r--   0 allen      (501) staff       (20)    15751 2019-04-30 22:42:34.000000 btrdb-5.8/btrdb/grpcinterface/btrdb_pb2_grpc.py
--rw-r--r--   0 allen      (501) staff       (20)     6377 2019-11-27 20:09:10.000000 btrdb-5.8/btrdb/point.py
--rw-r--r--   0 allen      (501) staff       (20)    46883 2020-05-13 21:11:01.000000 btrdb-5.8/btrdb/stream.py
--rw-r--r--   0 allen      (501) staff       (20)    11275 2020-05-13 21:11:01.000000 btrdb-5.8/btrdb/transformers.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.850788 btrdb-5.8/btrdb/utils/
--rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8/btrdb/utils/__init__.py
--rw-r--r--   0 allen      (501) staff       (20)     2010 2019-03-06 21:01:18.000000 btrdb-5.8/btrdb/utils/buffer.py
--rw-r--r--   0 allen      (501) staff       (20)     3095 2019-08-01 19:53:35.000000 btrdb-5.8/btrdb/utils/conversion.py
--rw-r--r--   0 allen      (501) staff       (20)     4007 2020-05-13 21:11:01.000000 btrdb-5.8/btrdb/utils/credentials.py
--rw-r--r--   0 allen      (501) staff       (20)     4855 2019-06-17 18:48:35.000000 btrdb-5.8/btrdb/utils/general.py
--rw-r--r--   0 allen      (501) staff       (20)     7233 2019-09-30 22:27:35.000000 btrdb-5.8/btrdb/utils/timez.py
--rw-r--r--   0 allen      (501) staff       (20)     1259 2020-05-13 21:11:01.000000 btrdb-5.8/btrdb/version.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.839901 btrdb-5.8/btrdb.egg-info/
--rw-r--r--   0 allen      (501) staff       (20)     1905 2020-05-13 21:30:48.000000 btrdb-5.8/btrdb.egg-info/PKG-INFO
--rw-r--r--   0 allen      (501) staff       (20)     2040 2020-05-13 21:30:48.000000 btrdb-5.8/btrdb.egg-info/SOURCES.txt
--rw-r--r--   0 allen      (501) staff       (20)        1 2020-05-13 21:30:48.000000 btrdb-5.8/btrdb.egg-info/dependency_links.txt
--rw-r--r--   0 allen      (501) staff       (20)       20 2020-05-13 21:30:48.000000 btrdb-5.8/btrdb.egg-info/entry_points.txt
--rw-r--r--   0 allen      (501) staff       (20)        1 2020-02-01 19:59:27.000000 btrdb-5.8/btrdb.egg-info/not-zip-safe
--rw-r--r--   0 allen      (501) staff       (20)       48 2020-05-13 21:30:48.000000 btrdb-5.8/btrdb.egg-info/requires.txt
--rw-r--r--   0 allen      (501) staff       (20)       19 2020-05-13 21:30:48.000000 btrdb-5.8/btrdb.egg-info/top_level.txt
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.851858 btrdb-5.8/btrdb4/
--rw-r--r--   0 allen      (501) staff       (20)      889 2019-03-06 21:01:53.000000 btrdb-5.8/btrdb4/__init__.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.853606 btrdb-5.8/docs/
--rw-r--r--   0 allen      (501) staff       (20)     7668 2019-03-06 21:01:18.000000 btrdb-5.8/docs/Makefile
--rw-r--r--   0 allen      (501) staff       (20)       29 2019-03-06 21:01:18.000000 btrdb-5.8/docs/requirements.txt
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.859278 btrdb-5.8/docs/source/
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.860433 btrdb-5.8/docs/source/_static/
--rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/_static/.gitkeep
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.863557 btrdb-5.8/docs/source/_static/figures/
--rw-r--r--   0 allen      (501) staff       (20)    44155 2019-08-01 19:53:35.000000 btrdb-5.8/docs/source/_static/figures/multiprocessing_architecture.png
--rw-r--r--   0 allen      (501) staff       (20)  5852139 2019-08-01 19:53:35.000000 btrdb-5.8/docs/source/_static/figures/ui_zoom.gif
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.892102 btrdb-5.8/docs/source/api/
--rw-r--r--   0 allen      (501) staff       (20)       89 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/conn.rst
--rw-r--r--   0 allen      (501) staff       (20)      137 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/exceptions.rst
--rw-r--r--   0 allen      (501) staff       (20)       70 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/package.rst
--rw-r--r--   0 allen      (501) staff       (20)       69 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/points.rst
--rw-r--r--   0 allen      (501) staff       (20)      139 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/streams.rst
--rw-r--r--   0 allen      (501) staff       (20)      498 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/transformers.rst
--rw-r--r--   0 allen      (501) staff       (20)       89 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/api/utils-timez.rst
--rw-r--r--   0 allen      (501) staff       (20)     6154 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/concepts.rst
--rw-r--r--   0 allen      (501) staff       (20)     6286 2019-08-01 19:53:35.000000 btrdb-5.8/docs/source/conf.py
--rw-r--r--   0 allen      (501) staff       (20)     8822 2019-08-01 19:53:35.000000 btrdb-5.8/docs/source/explained.rst
--rw-r--r--   0 allen      (501) staff       (20)     3264 2019-08-01 19:53:35.000000 btrdb-5.8/docs/source/index.rst
--rw-r--r--   0 allen      (501) staff       (20)     1104 2019-05-08 20:25:29.000000 btrdb-5.8/docs/source/installing.rst
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.892830 btrdb-5.8/docs/source/maintainers/
--rw-r--r--   0 allen      (501) staff       (20)    35492 2020-05-13 21:11:01.000000 btrdb-5.8/docs/source/maintainers/anaconda.rst
--rw-r--r--   0 allen      (501) staff       (20)     4923 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/quick-start.rst
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.899838 btrdb-5.8/docs/source/working/
--rw-r--r--   0 allen      (501) staff       (20)     8519 2019-08-01 19:53:35.000000 btrdb-5.8/docs/source/working/multiprocessing.rst
--rw-r--r--   0 allen      (501) staff       (20)     3666 2019-06-11 20:26:43.000000 btrdb-5.8/docs/source/working/server.rst
--rw-r--r--   0 allen      (501) staff       (20)     1323 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/working/stream-manage-data.rst
--rw-r--r--   0 allen      (501) staff       (20)     4109 2019-11-27 20:09:10.000000 btrdb-5.8/docs/source/working/stream-manage-metadata.rst
--rw-r--r--   0 allen      (501) staff       (20)     3648 2019-06-20 20:48:30.000000 btrdb-5.8/docs/source/working/stream-query-manage.rst
--rw-r--r--   0 allen      (501) staff       (20)     8373 2020-05-13 21:11:01.000000 btrdb-5.8/docs/source/working/stream-view-data.rst
--rw-r--r--   0 allen      (501) staff       (20)    10511 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/working/streamsets.rst
--rw-r--r--   0 allen      (501) staff       (20)      372 2019-03-06 21:01:18.000000 btrdb-5.8/docs/source/working.rst
--rw-r--r--   0 allen      (501) staff       (20)      114 2019-06-06 15:38:15.000000 btrdb-5.8/requirements.txt
--rw-r--r--   0 allen      (501) staff       (20)      314 2020-05-13 21:30:48.912097 btrdb-5.8/setup.cfg
--rw-r--r--   0 allen      (501) staff       (20)     5168 2019-06-20 20:48:30.000000 btrdb-5.8/setup.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.900764 btrdb-5.8/tests/
--rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8/tests/__init__.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.905305 btrdb-5.8/tests/btrdb/
--rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8/tests/btrdb/__init__.py
--rw-r--r--   0 allen      (501) staff       (20)     3898 2020-05-13 21:11:01.000000 btrdb-5.8/tests/btrdb/test_base.py
--rw-r--r--   0 allen      (501) staff       (20)     8265 2019-09-25 14:27:08.000000 btrdb-5.8/tests/btrdb/test_conn.py
--rw-r--r--   0 allen      (501) staff       (20)     7390 2019-03-06 21:01:18.000000 btrdb-5.8/tests/btrdb/test_point.py
--rw-r--r--   0 allen      (501) staff       (20)    63199 2020-05-13 21:11:01.000000 btrdb-5.8/tests/btrdb/test_stream.py
--rw-r--r--   0 allen      (501) staff       (20)    25454 2020-05-13 21:11:01.000000 btrdb-5.8/tests/btrdb/test_transformers.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.909078 btrdb-5.8/tests/btrdb/utils/
--rw-r--r--   0 allen      (501) staff       (20)        0 2019-06-17 18:48:35.000000 btrdb-5.8/tests/btrdb/utils/__init__.py
--rw-r--r--   0 allen      (501) staff       (20)     4332 2019-03-06 21:01:18.000000 btrdb-5.8/tests/btrdb/utils/test_buffer.py
--rw-r--r--   0 allen      (501) staff       (20)     3767 2019-08-01 19:53:35.000000 btrdb-5.8/tests/btrdb/utils/test_conversions.py
--rw-r--r--   0 allen      (501) staff       (20)     4117 2019-06-20 20:48:30.000000 btrdb-5.8/tests/btrdb/utils/test_credentials.py
--rw-r--r--   0 allen      (501) staff       (20)     3621 2019-06-17 18:48:35.000000 btrdb-5.8/tests/btrdb/utils/test_general.py
--rw-r--r--   0 allen      (501) staff       (20)     6112 2019-09-30 22:27:35.000000 btrdb-5.8/tests/btrdb/utils/test_timez.py
-drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-05-13 21:30:48.909940 btrdb-5.8/tests/btrdb4/
--rw-r--r--   0 allen      (501) staff       (20)      837 2019-03-06 21:01:18.000000 btrdb-5.8/tests/btrdb4/test_import.py
--rw-r--r--   0 allen      (501) staff       (20)      138 2020-05-13 21:11:01.000000 btrdb-5.8/tests/requirements.txt
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/
+-rw-r--r--   0 allen      (501) staff       (20)     1911 2020-06-29 21:11:37.000000 btrdb-5.8.1/PKG-INFO
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb4/
+-rw-r--r--   0 allen      (501) staff       (20)      889 2019-03-06 21:01:53.000000 btrdb-5.8.1/btrdb4/__init__.py
+-rw-r--r--   0 allen      (501) staff       (20)      114 2020-06-29 21:04:28.000000 btrdb-5.8.1/requirements.txt
+-rw-r--r--   0 allen      (501) staff       (20)     1671 2019-11-18 16:49:45.000000 btrdb-5.8.1/Makefile
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/tests/
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/tests/btrdb4/
+-rw-r--r--   0 allen      (501) staff       (20)      837 2019-03-06 21:01:18.000000 btrdb-5.8.1/tests/btrdb4/test_import.py
+-rw-r--r--   0 allen      (501) staff       (20)      138 2020-05-13 21:11:01.000000 btrdb-5.8.1/tests/requirements.txt
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/tests/btrdb/
+-rw-r--r--   0 allen      (501) staff       (20)     7390 2019-03-06 21:01:18.000000 btrdb-5.8.1/tests/btrdb/test_point.py
+-rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8.1/tests/btrdb/__init__.py
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/tests/btrdb/utils/
+-rw-r--r--   0 allen      (501) staff       (20)     3767 2019-08-01 19:53:35.000000 btrdb-5.8.1/tests/btrdb/utils/test_conversions.py
+-rw-r--r--   0 allen      (501) staff       (20)     4332 2019-03-06 21:01:18.000000 btrdb-5.8.1/tests/btrdb/utils/test_buffer.py
+-rw-r--r--   0 allen      (501) staff       (20)     6112 2019-09-30 22:27:35.000000 btrdb-5.8.1/tests/btrdb/utils/test_timez.py
+-rw-r--r--   0 allen      (501) staff       (20)        0 2019-06-17 18:48:35.000000 btrdb-5.8.1/tests/btrdb/utils/__init__.py
+-rw-r--r--   0 allen      (501) staff       (20)     4117 2019-06-20 20:48:30.000000 btrdb-5.8.1/tests/btrdb/utils/test_credentials.py
+-rw-r--r--   0 allen      (501) staff       (20)     3620 2020-06-29 21:04:28.000000 btrdb-5.8.1/tests/btrdb/utils/test_general.py
+-rw-r--r--   0 allen      (501) staff       (20)     3900 2020-06-29 21:04:28.000000 btrdb-5.8.1/tests/btrdb/test_base.py
+-rw-r--r--   0 allen      (501) staff       (20)    25454 2020-05-13 21:11:01.000000 btrdb-5.8.1/tests/btrdb/test_transformers.py
+-rw-r--r--   0 allen      (501) staff       (20)     8265 2020-06-29 20:57:59.000000 btrdb-5.8.1/tests/btrdb/test_conn.py
+-rw-r--r--   0 allen      (501) staff       (20)    63199 2020-06-29 20:57:59.000000 btrdb-5.8.1/tests/btrdb/test_stream.py
+-rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8.1/tests/__init__.py
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb/
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb/grpcinterface/
+-rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8.1/btrdb/grpcinterface/__init__.py
+-rw-r--r--   0 allen      (501) staff       (20)    15751 2019-04-30 22:42:34.000000 btrdb-5.8.1/btrdb/grpcinterface/btrdb_pb2_grpc.py
+-rw-r--r--   0 allen      (501) staff       (20)   124824 2019-05-08 20:25:29.000000 btrdb-5.8.1/btrdb/grpcinterface/btrdb_pb2.py
+-rw-r--r--   0 allen      (501) staff       (20)     7133 2019-03-06 21:01:19.000000 btrdb-5.8.1/btrdb/grpcinterface/btrdb.proto
+-rw-r--r--   0 allen      (501) staff       (20)     1259 2020-06-29 21:04:28.000000 btrdb-5.8.1/btrdb/version.py
+-rw-r--r--   0 allen      (501) staff       (20)    11275 2020-05-13 21:11:01.000000 btrdb-5.8.1/btrdb/transformers.py
+-rw-r--r--   0 allen      (501) staff       (20)     2674 2020-06-29 20:57:59.000000 btrdb-5.8.1/btrdb/__init__.py
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb/utils/
+-rw-r--r--   0 allen      (501) staff       (20)     4007 2020-06-29 20:57:59.000000 btrdb-5.8.1/btrdb/utils/credentials.py
+-rw-r--r--   0 allen      (501) staff       (20)     3095 2019-08-01 19:53:35.000000 btrdb-5.8.1/btrdb/utils/conversion.py
+-rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8.1/btrdb/utils/__init__.py
+-rw-r--r--   0 allen      (501) staff       (20)     2010 2019-03-06 21:01:18.000000 btrdb-5.8.1/btrdb/utils/buffer.py
+-rw-r--r--   0 allen      (501) staff       (20)     7233 2019-09-30 22:27:35.000000 btrdb-5.8.1/btrdb/utils/timez.py
+-rw-r--r--   0 allen      (501) staff       (20)     4860 2020-06-29 21:04:28.000000 btrdb-5.8.1/btrdb/utils/general.py
+-rw-r--r--   0 allen      (501) staff       (20)    46883 2020-06-29 20:57:59.000000 btrdb-5.8.1/btrdb/stream.py
+-rw-r--r--   0 allen      (501) staff       (20)     6377 2019-11-27 20:09:10.000000 btrdb-5.8.1/btrdb/point.py
+-rw-r--r--   0 allen      (501) staff       (20)    10467 2019-11-27 20:09:10.000000 btrdb-5.8.1/btrdb/endpoint.py
+-rw-r--r--   0 allen      (501) staff       (20)     1953 2019-06-20 13:27:12.000000 btrdb-5.8.1/btrdb/exceptions.py
+-rw-r--r--   0 allen      (501) staff       (20)    10995 2020-06-29 20:57:59.000000 btrdb-5.8.1/btrdb/conn.py
+-rw-r--r--   0 allen      (501) staff       (20)      346 2019-04-29 19:25:09.000000 btrdb-5.8.1/MANIFEST.in
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/
+-rw-r--r--   0 allen      (501) staff       (20)       29 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/requirements.txt
+-rw-r--r--   0 allen      (501) staff       (20)     7668 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/Makefile
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/source/
+-rw-r--r--   0 allen      (501) staff       (20)     1104 2019-05-08 20:25:29.000000 btrdb-5.8.1/docs/source/installing.rst
+-rw-r--r--   0 allen      (501) staff       (20)     3264 2019-08-01 19:53:35.000000 btrdb-5.8.1/docs/source/index.rst
+-rw-r--r--   0 allen      (501) staff       (20)      372 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/working.rst
+-rw-r--r--   0 allen      (501) staff       (20)     6154 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/concepts.rst
+-rw-r--r--   0 allen      (501) staff       (20)     6286 2019-08-01 19:53:35.000000 btrdb-5.8.1/docs/source/conf.py
+-rw-r--r--   0 allen      (501) staff       (20)     4923 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/quick-start.rst
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/source/_static/
+-rw-r--r--   0 allen      (501) staff       (20)        0 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/_static/.gitkeep
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/source/_static/figures/
+-rw-r--r--   0 allen      (501) staff       (20)  5852139 2019-08-01 19:53:35.000000 btrdb-5.8.1/docs/source/_static/figures/ui_zoom.gif
+-rw-r--r--   0 allen      (501) staff       (20)    44155 2019-08-01 19:53:35.000000 btrdb-5.8.1/docs/source/_static/figures/multiprocessing_architecture.png
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/source/working/
+-rw-r--r--   0 allen      (501) staff       (20)     3666 2019-06-11 20:26:43.000000 btrdb-5.8.1/docs/source/working/server.rst
+-rw-r--r--   0 allen      (501) staff       (20)     3648 2020-06-29 20:57:59.000000 btrdb-5.8.1/docs/source/working/stream-query-manage.rst
+-rw-r--r--   0 allen      (501) staff       (20)    10511 2020-06-29 20:57:59.000000 btrdb-5.8.1/docs/source/working/streamsets.rst
+-rw-r--r--   0 allen      (501) staff       (20)     4109 2019-11-27 20:09:10.000000 btrdb-5.8.1/docs/source/working/stream-manage-metadata.rst
+-rw-r--r--   0 allen      (501) staff       (20)     1323 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/working/stream-manage-data.rst
+-rw-r--r--   0 allen      (501) staff       (20)     8373 2020-05-13 21:11:01.000000 btrdb-5.8.1/docs/source/working/stream-view-data.rst
+-rw-r--r--   0 allen      (501) staff       (20)     8519 2019-08-01 19:53:35.000000 btrdb-5.8.1/docs/source/working/multiprocessing.rst
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/source/maintainers/
+-rw-r--r--   0 allen      (501) staff       (20)    35492 2020-05-13 21:11:01.000000 btrdb-5.8.1/docs/source/maintainers/anaconda.rst
+-rw-r--r--   0 allen      (501) staff       (20)     8822 2019-08-01 19:53:35.000000 btrdb-5.8.1/docs/source/explained.rst
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/docs/source/api/
+-rw-r--r--   0 allen      (501) staff       (20)       70 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/package.rst
+-rw-r--r--   0 allen      (501) staff       (20)      139 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/streams.rst
+-rw-r--r--   0 allen      (501) staff       (20)       69 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/points.rst
+-rw-r--r--   0 allen      (501) staff       (20)      498 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/transformers.rst
+-rw-r--r--   0 allen      (501) staff       (20)       89 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/conn.rst
+-rw-r--r--   0 allen      (501) staff       (20)       89 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/utils-timez.rst
+-rw-r--r--   0 allen      (501) staff       (20)      137 2019-03-06 21:01:18.000000 btrdb-5.8.1/docs/source/api/exceptions.rst
+drwxr-xr-x   0 allen      (501) staff       (20)        0 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/
+-rw-r--r--   0 allen      (501) staff       (20)     1911 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/PKG-INFO
+-rw-r--r--   0 allen      (501) staff       (20)        1 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/not-zip-safe
+-rw-r--r--   0 allen      (501) staff       (20)     2040 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/SOURCES.txt
+-rw-r--r--   0 allen      (501) staff       (20)       20 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/entry_points.txt
+-rw-r--r--   0 allen      (501) staff       (20)       48 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/requires.txt
+-rw-r--r--   0 allen      (501) staff       (20)       19 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/top_level.txt
+-rw-r--r--   0 allen      (501) staff       (20)        1 2020-06-29 21:11:37.000000 btrdb-5.8.1/btrdb.egg-info/dependency_links.txt
+-rw-r--r--   0 allen      (501) staff       (20)     6561 2019-03-06 21:01:18.000000 btrdb-5.8.1/README.md
+-rw-r--r--   0 allen      (501) staff       (20)      472 2019-03-06 21:01:18.000000 btrdb-5.8.1/DESCRIPTION.md
+-rw-r--r--   0 allen      (501) staff       (20)     5168 2019-06-20 20:48:30.000000 btrdb-5.8.1/setup.py
+-rw-r--r--   0 allen      (501) staff       (20)      314 2020-06-29 21:11:37.000000 btrdb-5.8.1/setup.cfg
+-rw-r--r--   0 allen      (501) staff       (20)     1678 2019-03-06 20:58:55.000000 btrdb-5.8.1/LICENSE.txt
+-rw-r--r--   0 allen      (501) staff       (20)     1151 2020-05-13 21:11:01.000000 btrdb-5.8.1/.travis.yml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `btrdb-5.8/.travis.yml` & `btrdb-5.8.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/LICENSE.txt` & `btrdb-5.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/Makefile` & `btrdb-5.8.1/Makefile`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/PKG-INFO` & `btrdb-5.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: btrdb
-Version: 5.8
+Version: 5.8.1
 Summary: Bindings to interact with the Berkeley Tree Database using gRPC.
 Home-page: http://btrdb.io/
 Author: Michael Andersen, Allen Leis
 Author-email: michael@steelcode.com
 Maintainer: Michael Andersen
 Maintainer-email: michael@steelcode.com
 License: BSD-3-Clause
-Download-URL: https://github.com/BTrDB/btrdb-python/tarball/v5.8
+Download-URL: https://github.com/BTrDB/btrdb-python/tarball/v5.8.1
 Project-URL: Documentation, https://btrdb.readthedocs.io/en/latest/
-Project-URL: Download, https://github.com/BTrDB/btrdb-python/tarball/v5.8
+Project-URL: Download, https://github.com/BTrDB/btrdb-python/tarball/v5.8.1
 Project-URL: Source, https://github.com/BTrDB/btrdb-python
 Project-URL: Tracker, https://github.com/BTrDB/btrdb-python/issues
 Description: # btrdb
         
         These are BTrDB Bindings for Python allowing you painless and productive access to the Berkeley Tree Database (BTrDB).  BTrDB is a time series database focusing on blazing speed with respect to univariate time series data at the nanosecond scale.
         
         Please see the full documentation at: [https://btrdb.readthedocs.io/en/latest/](https://btrdb.readthedocs.io/en/latest/) particularly the quick [start guide](https://btrdb.readthedocs.io/en/latest/quick-start.html)
```

### Comparing `btrdb-5.8/README.md` & `btrdb-5.8.1/README.md`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/__init__.py` & `btrdb-5.8.1/btrdb/__init__.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/conn.py` & `btrdb-5.8.1/btrdb/conn.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/endpoint.py` & `btrdb-5.8.1/btrdb/endpoint.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/exceptions.py` & `btrdb-5.8.1/btrdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/grpcinterface/btrdb.proto` & `btrdb-5.8.1/btrdb/grpcinterface/btrdb.proto`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/grpcinterface/btrdb_pb2.py` & `btrdb-5.8.1/btrdb/grpcinterface/btrdb_pb2.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/grpcinterface/btrdb_pb2_grpc.py` & `btrdb-5.8.1/btrdb/grpcinterface/btrdb_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/point.py` & `btrdb-5.8.1/btrdb/point.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/stream.py` & `btrdb-5.8.1/btrdb/stream.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/transformers.py` & `btrdb-5.8.1/btrdb/transformers.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/utils/buffer.py` & `btrdb-5.8.1/btrdb/utils/buffer.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/utils/conversion.py` & `btrdb-5.8.1/btrdb/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/utils/credentials.py` & `btrdb-5.8.1/btrdb/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/utils/general.py` & `btrdb-5.8.1/btrdb/utils/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     @classmethod
     def from_timedelta(cls, delta):
         """
         Returns the closest pointwidth for the given timedelta without going over the
         specified duration. Because pointwidths are in powers of 2, be sure to check
         that the returned real duration is sufficient.
         """
-        return cls.from_nanoseconds(delta.total_seconds()*1e9)
+        return cls.from_nanoseconds(int(delta.total_seconds()*1e9))
 
     @classmethod
     def from_nanoseconds(cls, nsec):
         """
         Returns the closest pointwidth for the given number of nanoseconds without going
         over the specified duration. Because pointwidths are in powers of 2, be sure to
         check that the returned real duration is sufficient.
```

### Comparing `btrdb-5.8/btrdb/utils/timez.py` & `btrdb-5.8.1/btrdb/utils/timez.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb/version.py` & `btrdb-5.8.1/btrdb/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     'major': 5,
     'minor': 8,
-    'micro': 0,
+    'micro': 1,
     'releaselevel': 'final',
-    'serial': 13,
+    'serial': 14,
 }
 
 ##########################################################################
 ## Helper Functions
 ##########################################################################
 
 def get_version(short=False):
```

### Comparing `btrdb-5.8/btrdb.egg-info/PKG-INFO` & `btrdb-5.8.1/btrdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: btrdb
-Version: 5.8
+Version: 5.8.1
 Summary: Bindings to interact with the Berkeley Tree Database using gRPC.
 Home-page: http://btrdb.io/
 Author: Michael Andersen, Allen Leis
 Author-email: michael@steelcode.com
 Maintainer: Michael Andersen
 Maintainer-email: michael@steelcode.com
 License: BSD-3-Clause
-Download-URL: https://github.com/BTrDB/btrdb-python/tarball/v5.8
+Download-URL: https://github.com/BTrDB/btrdb-python/tarball/v5.8.1
 Project-URL: Documentation, https://btrdb.readthedocs.io/en/latest/
-Project-URL: Download, https://github.com/BTrDB/btrdb-python/tarball/v5.8
+Project-URL: Download, https://github.com/BTrDB/btrdb-python/tarball/v5.8.1
 Project-URL: Source, https://github.com/BTrDB/btrdb-python
 Project-URL: Tracker, https://github.com/BTrDB/btrdb-python/issues
 Description: # btrdb
         
         These are BTrDB Bindings for Python allowing you painless and productive access to the Berkeley Tree Database (BTrDB).  BTrDB is a time series database focusing on blazing speed with respect to univariate time series data at the nanosecond scale.
         
         Please see the full documentation at: [https://btrdb.readthedocs.io/en/latest/](https://btrdb.readthedocs.io/en/latest/) particularly the quick [start guide](https://btrdb.readthedocs.io/en/latest/quick-start.html)
```

### Comparing `btrdb-5.8/btrdb.egg-info/SOURCES.txt` & `btrdb-5.8.1/btrdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/btrdb4/__init__.py` & `btrdb-5.8.1/btrdb4/__init__.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/Makefile` & `btrdb-5.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/_static/figures/multiprocessing_architecture.png` & `btrdb-5.8.1/docs/source/_static/figures/multiprocessing_architecture.png`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/_static/figures/ui_zoom.gif` & `btrdb-5.8.1/docs/source/_static/figures/ui_zoom.gif`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/concepts.rst` & `btrdb-5.8.1/docs/source/concepts.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/conf.py` & `btrdb-5.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/explained.rst` & `btrdb-5.8.1/docs/source/explained.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/index.rst` & `btrdb-5.8.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/installing.rst` & `btrdb-5.8.1/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/maintainers/anaconda.rst` & `btrdb-5.8.1/docs/source/maintainers/anaconda.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/quick-start.rst` & `btrdb-5.8.1/docs/source/quick-start.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/multiprocessing.rst` & `btrdb-5.8.1/docs/source/working/multiprocessing.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/server.rst` & `btrdb-5.8.1/docs/source/working/server.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/stream-manage-data.rst` & `btrdb-5.8.1/docs/source/working/stream-manage-data.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/stream-manage-metadata.rst` & `btrdb-5.8.1/docs/source/working/stream-manage-metadata.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/stream-query-manage.rst` & `btrdb-5.8.1/docs/source/working/stream-query-manage.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/stream-view-data.rst` & `btrdb-5.8.1/docs/source/working/stream-view-data.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/docs/source/working/streamsets.rst` & `btrdb-5.8.1/docs/source/working/streamsets.rst`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/setup.py` & `btrdb-5.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/test_base.py` & `btrdb-5.8.1/tests/btrdb/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from btrdb import connect, __version__, BTRDB_ENDPOINTS, BTRDB_API_KEY
 from btrdb.exceptions import ConnectionError
 
 ##########################################################################
 ## Test Constants
 ##########################################################################
 
-EXPECTED_VERSION = "5.8"
+EXPECTED_VERSION = "5.8.1"
 
 
 ##########################################################################
 ## Initialization Tests
 ##########################################################################
 
 class TestPackage(object):
```

### Comparing `btrdb-5.8/tests/btrdb/test_conn.py` & `btrdb-5.8.1/tests/btrdb/test_conn.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/test_point.py` & `btrdb-5.8.1/tests/btrdb/test_point.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/test_stream.py` & `btrdb-5.8.1/tests/btrdb/test_stream.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/test_transformers.py` & `btrdb-5.8.1/tests/btrdb/test_transformers.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/utils/test_buffer.py` & `btrdb-5.8.1/tests/btrdb/utils/test_buffer.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/utils/test_conversions.py` & `btrdb-5.8.1/tests/btrdb/utils/test_conversions.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/utils/test_credentials.py` & `btrdb-5.8.1/tests/btrdb/utils/test_credentials.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb/utils/test_general.py` & `btrdb-5.8.1/tests/btrdb/utils/test_general.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,33 +21,35 @@
 class TestPointwidth(object):
 
     @pytest.mark.parametrize("delta, expected", [
         (timedelta(days=365), 54),
         (timedelta(days=30), 51),
         (timedelta(days=7), 49),
         (timedelta(days=1), 46),
-        (timedelta(hours=4), 45),
-        (timedelta(minutes=15), 40),
-        (timedelta(seconds=30), 29),
+        (timedelta(hours=4), 43),
+        (timedelta(minutes=15), 39),
+        (timedelta(seconds=30), 34),
     ])
-    def test_from_nanoseconds(self, delta, expected):
+
+    def test_from_timedelta(self, delta, expected):
         """
-        Test getting the closest point width from nanoseconds
+        Test getting the closest point width from a timedelta
         """
-        assert pointwidth.from_nanoseconds(nsec) == expected
+        assert pointwidth.from_timedelta(delta) == expected
 
     @pytest.mark.parametrize("nsec, expected", [
         (ns_delta(days=365), 54),
         (ns_delta(days=30), 51),
         (ns_delta(days=7), 49),
         (ns_delta(days=1), 46),
         (ns_delta(hours=12), 45),
         (ns_delta(minutes=30), 40),
         (ns_delta(seconds=1), 29),
     ])
+
     def test_from_nanoseconds(self, nsec, expected):
         """
         Test getting the closest point width from nanoseconds
         """
         assert pointwidth.from_nanoseconds(nsec) == expected
 
     def test_time_conversions(self):
```

### Comparing `btrdb-5.8/tests/btrdb/utils/test_timez.py` & `btrdb-5.8.1/tests/btrdb/utils/test_timez.py`

 * *Files identical despite different names*

### Comparing `btrdb-5.8/tests/btrdb4/test_import.py` & `btrdb-5.8.1/tests/btrdb4/test_import.py`

 * *Files identical despite different names*

