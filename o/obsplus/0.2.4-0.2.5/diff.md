# Comparing `tmp/obsplus-0.2.4.tar.gz` & `tmp/obsplus-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsplus-0.2.4.tar", last modified: Fri Oct 28 03:47:01 2022, max compression
+gzip compressed data, was "obsplus-0.2.5.tar", last modified: Fri Jul 21 19:13:59 2023, max compression
```

## Comparing `obsplus-0.2.4.tar` & `obsplus-0.2.5.tar`

### file list

```diff
@@ -1,86 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.350246 obsplus-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-10-28 03:44:08.000000 obsplus-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-10-28 03:44:08.000000 obsplus-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-10-28 03:47:01.350246 obsplus-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1949 2022-10-28 03:44:08.000000 obsplus-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.350246 obsplus-0.2.4/obsplus/
--rw-r--r--   0 runner    (1001) docker     (121)     1962 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-10-28 03:47:01.350246 obsplus-0.2.4/obsplus/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.342246 obsplus-0.2.4/obsplus/bank/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/bank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11414 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/bank/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    19611 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/bank/eventbank.py
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/bank/stationbank.py
--rw-r--r--   0 runner    (1001) docker     (121)    26971 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/bank/wavebank.py
--rw-r--r--   0 runner    (1001) docker     (121)    20299 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.342246 obsplus-0.2.4/obsplus/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.342246 obsplus-0.2.4/obsplus/datasets/bingham_test/
--rw-r--r--   0 runner    (1001) docker     (121)    67025 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/bingham_test/dataset_hash.json
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/bingham_test/dataset_version.txt
--rw-r--r--   0 runner    (1001) docker     (121)   368051 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/bingham_test/events.xml
--rw-r--r--   0 runner    (1001) docker     (121)   312131 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/bingham_test/inventory.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/bingham_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.342246 obsplus-0.2.4/obsplus/datasets/crandall_test/
--rw-r--r--   0 runner    (1001) docker     (121)    57590 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/crandall_test/dataset_hash.json
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/crandall_test/dataset_version.txt
--rw-r--r--   0 runner    (1001) docker     (121)   644138 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/crandall_test/events.xml
--rw-r--r--   0 runner    (1001) docker     (121)     3065 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/crandall_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    23990 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.346246 obsplus-0.2.4/obsplus/datasets/default_test/
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/default_test/dataset_hash.json
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/default_test/dataset_version.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1122 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/default_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.346246 obsplus-0.2.4/obsplus/datasets/ta_test/
--rw-r--r--   0 runner    (1001) docker     (121)    87305 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/ta_test/dataset_hash.json
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/ta_test/dataset_version.txt
--rw-r--r--   0 runner    (1001) docker     (121)   377749 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/ta_test/inventory.xml
--rw-r--r--   0 runner    (1001) docker     (121)     2196 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/datasets/ta_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.346246 obsplus-0.2.4/obsplus/events/
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8049 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/get_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1527 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/json.py
--rw-r--r--   0 runner    (1001) docker     (121)     9923 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/merge.py
--rw-r--r--   0 runner    (1001) docker     (121)    21787 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/pd.py
--rw-r--r--   0 runner    (1001) docker     (121)    18320 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    10773 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/events/validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4119 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.346246 obsplus-0.2.4/obsplus/stations/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/stations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/stations/get_stations.py
--rw-r--r--   0 runner    (1001) docker     (121)     4353 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/stations/pd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.346246 obsplus-0.2.4/obsplus/structures/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/structures/dfextractor.py
--rw-r--r--   0 runner    (1001) docker     (121)    23301 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/structures/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.346246 obsplus-0.2.4/obsplus/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14821 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/bank.py
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (121)    17667 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     9105 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/geodetics.py
--rw-r--r--   0 runner    (1001) docker     (121)    18175 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3310 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/mseed.py
--rw-r--r--   0 runner    (1001) docker     (121)    17114 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/pd.py
--rw-r--r--   0 runner    (1001) docker     (121)    16196 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/stations.py
--rw-r--r--   0 runner    (1001) docker     (121)    10382 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    12847 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (121)     6859 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/validate.py
--rw-r--r--   0 runner    (1001) docker     (121)    21508 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/utils/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.350246 obsplus-0.2.4/obsplus/waveforms/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/waveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-10-28 03:44:08.000000 obsplus-0.2.4/obsplus/waveforms/get_waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 03:47:01.342246 obsplus-0.2.4/obsplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2675 2022-10-28 03:47:01.000000 obsplus-0.2.4/obsplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2021 2022-10-28 03:47:01.000000 obsplus-0.2.4/obsplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 03:47:01.000000 obsplus-0.2.4/obsplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-28 03:47:01.000000 obsplus-0.2.4/obsplus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 03:46:59.000000 obsplus-0.2.4/obsplus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-28 03:47:01.000000 obsplus-0.2.4/obsplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-28 03:47:01.000000 obsplus-0.2.4/obsplus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-10-28 03:44:08.000000 obsplus-0.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-10-28 03:47:01.350246 obsplus-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-10-28 03:44:08.000000 obsplus-0.2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68751 2022-10-28 03:44:08.000000 obsplus-0.2.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.161007 obsplus-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-21 19:05:28.000000 obsplus-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-21 19:13:59.161007 obsplus-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-07-21 19:05:28.000000 obsplus-0.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-21 19:05:28.000000 obsplus-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 19:13:59.161007 obsplus-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.149007 obsplus-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.149007 obsplus-0.2.5/src/obsplus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.153007 obsplus-0.2.5/src/obsplus/bank/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/bank/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/bank/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/bank/eventbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/bank/stationbank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29462 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/bank/wavebank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20299 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.153007 obsplus-0.2.5/src/obsplus/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.153007 obsplus-0.2.5/src/obsplus/datasets/bingham_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    67025 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/bingham_test/dataset_hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/bingham_test/dataset_version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   368051 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/bingham_test/events.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   312131 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/bingham_test/inventory.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/bingham_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.153007 obsplus-0.2.5/src/obsplus/datasets/crandall_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    57590 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/crandall_test/dataset_hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/crandall_test/dataset_version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   644138 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/crandall_test/events.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/crandall_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23990 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.157007 obsplus-0.2.5/src/obsplus/datasets/default_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/default_test/dataset_hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/default_test/dataset_version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/default_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.157007 obsplus-0.2.5/src/obsplus/datasets/ta_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    87305 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/ta_test/dataset_hash.json
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/ta_test/dataset_version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   377749 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/ta_test/inventory.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/datasets/ta_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.157007 obsplus-0.2.5/src/obsplus/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8049 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21763 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/events/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.157007 obsplus-0.2.5/src/obsplus/stations/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/stations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/stations/get_stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/stations/pd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.157007 obsplus-0.2.5/src/obsplus/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7732 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/structures/dfextractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23301 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/structures/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.161007 obsplus-0.2.5/src/obsplus/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/bank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17667 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/geodetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18330 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/mseed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17114 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/pd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16196 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/utils/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.161007 obsplus-0.2.5/src/obsplus/waveforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/waveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-21 19:05:28.000000 obsplus-0.2.5/src/obsplus/waveforms/get_waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 19:13:59.153007 obsplus-0.2.5/src/obsplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-07-21 19:13:59.000000 obsplus-0.2.5/src/obsplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-21 19:13:59.000000 obsplus-0.2.5/src/obsplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 19:13:59.000000 obsplus-0.2.5/src/obsplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 19:13:59.000000 obsplus-0.2.5/src/obsplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-21 19:13:59.000000 obsplus-0.2.5/src/obsplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-21 19:13:59.000000 obsplus-0.2.5/src/obsplus.egg-info/top_level.txt
```

### Comparing `obsplus-0.2.4/LICENSE` & `obsplus-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/README.rst` & `obsplus-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/__init__.py` & `obsplus-0.2.5/src/obsplus/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -51,17 +51,8 @@
 
 # get the get_client methods into obsplus namespace
 from obsplus.utils.waveforms import get_waveform_client
 from obsplus.utils.events import get_event_client
 from obsplus.utils.stations import get_station_client
 
 # Get version versioneer
-from ._version import get_versions
-
-version_dict = get_versions()
-__version__ = version_dict["version"]
-__last_version__ = __version__.split("+")[0].split("-")[0].replace("v", "")
-
-assert len(__last_version__.split(".")) == 3, "wrong version found!"
-
-
-del get_versions
+from .version import __version__, __last_version__
```

### Comparing `obsplus-0.2.4/obsplus/bank/core.py` & `obsplus-0.2.5/src/obsplus/bank/core.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/bank/eventbank.py` & `obsplus-0.2.5/src/obsplus/bank/eventbank.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/bank/wavebank.py` & `obsplus-0.2.5/src/obsplus/bank/wavebank.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     # index columns and types
     metadata_columns = "last_updated path_structure name_structure".split()
     index_str = tuple(NSLC)
     index_ints = ("starttime", "endtime", "sampling_period")
     index_columns = tuple(list(index_str) + list(index_ints) + ["path"])
     columns_no_path = index_columns[:-1]
     _gap_columns = tuple(list(columns_no_path) + ["gap_duration"])
+    _segment_columns = tuple(list(index_str) + ["starttime", "endtime", "duration"])
     namespace = "/waveforms"
     buffer = np.timedelta64(1_000_000_000, "ns")
     # dict defining lengths of str columns (after seed spec)
     # Note: Empty strings get their dtypes caste as S8, which means 8 is the min
     min_itemsize = {"path": 79, "station": 8, "network": 8, "location": 8, "channel": 8}
     _min_files_for_bar = 5000  # number of files before progress bar kicks in
     _dtypes_input = WAVEFORM_DTYPES_INPUT
@@ -413,16 +414,15 @@
         Return a dataframe containing an entry for every gap in the archive.
 
         Parameters
         ----------
         {get_waveforms_params}
         min_gap
             The minimum gap to report in seconds or as a timedelta64.
-             If None, use 1.5 x sampling rate for
-            each channel.
+             If None, use 1.5 x sampling rate for each channel.
         """
 
         def _get_gap_dfs(df, min_gap):
             """Apply me to each group of seed_id dataframes"""
             if not len(df):
                 return pd.DataFrame(
                     columns=df.columns.union(["starttime", "endtime", "gap_duration"])
@@ -435,15 +435,17 @@
             # get df for determining gaps
             dd = (
                 df.drop_duplicates()
                 .sort_values(["starttime", "endtime"])
                 .reset_index(drop=True)
             )
             shifted_starttimes = dd.starttime.shift(-1)
-            cum_max = np.maximum.accumulate(dd["endtime"] + min_gap)
+            cum_max = np.maximum.accumulate(
+                dd["endtime"] + min_gap
+            )  # Handles data overlaps
             gap_index = cum_max < shifted_starttimes
             # create a dataframe of gaps
             df = dd[gap_index]
             df["starttime"] = dd.endtime[gap_index]
             df["endtime"] = shifted_starttimes[gap_index]
             df["gap_duration"] = df["endtime"] - df["starttime"]
             return df
@@ -454,42 +456,106 @@
         group = index.groupby(group_names, as_index=False, group_keys=False)
         out = group.apply(_get_gap_dfs, min_gap=min_gap)
         if out.empty:  # if not gaps return empty dataframe with needed cols
             return pd.DataFrame(columns=self._gap_columns)
         return out.reset_index(drop=True)
 
     @compose_docstring(get_waveforms_params=get_waveforms_parameters)
-    def get_uptime_df(self, *args, **kwargs) -> pd.DataFrame:
+    def get_uptime_df(
+        self,
+        *args,
+        **kwargs,
+    ) -> pd.DataFrame:
         """
         Return a dataframe with uptime stats for selected channels.
 
         Parameters
         ----------
         {get_waveforms_params}
-
+        min_gap
+            The minimum gap to report in seconds or as a timedelta64.
+            If None, use 1.5 x sampling rate for each channel.
         """
-        # get total number of seconds bank spans for each seed id
+
         avail = self.get_availability_df(*args, **kwargs)
+        gaps_df = self.get_gaps_df(*args, **kwargs)
+
+        # get total number of seconds bank spans for each seed id
         avail["duration"] = avail["endtime"] - avail["starttime"]
         # get total duration of gaps by seed id
-        gaps_df = self.get_gaps_df(*args, **kwargs)
         if gaps_df.empty:
             gap_total_df = pd.DataFrame(avail[list(NSLC)])
             gap_total_df["gap_duration"] = EMPTYTD64
         else:
             gap_totals = gaps_df.groupby(list(NSLC)).gap_duration.sum()
             gap_total_df = pd.DataFrame(gap_totals).reset_index()
         # merge gap dataframe with availability dataframe, add uptime and %
         df = pd.merge(avail, gap_total_df, how="outer")
         # fill any Nan in gap_duration with empty timedelta
         df["gap_duration"] = df["gap_duration"].fillna(EMPTYTD64)
         df["uptime"] = df["duration"] - df["gap_duration"]
         df["availability"] = df["uptime"] / df["duration"]
         return df
 
+    @compose_docstring(get_waveforms_params=get_waveforms_parameters)
+    def get_segments_df(
+        self,
+        *args,
+        **kwargs,
+    ) -> pd.DataFrame:
+        """
+        Return a dataframe of contiguous segments for the selected channels
+
+        Parameters
+        ----------
+        {get_waveforms_params}
+        min_gap
+            The minimum gap to report in seconds or as a timedelta64.
+            If None, use 1.5 x sampling rate for each channel.
+        """
+
+        def _get_details(ser):
+            # Get the gap report for the seed id
+            seed_id = tuple(ser[list(NSLC)].values)
+            if seed_id in gps.groups:
+                df = gps.get_group(seed_id).reset_index(drop=True)
+                df.loc[max(df.index) + 1, :] = None
+                starttime = df["endtime"].shift(
+                    1
+                )  # End of the gap is the start of the next data segment
+                starttime.name = "starttime"
+                endtime = df["starttime"]  # Start of the gap is end of the data segment
+                endtime.name = "endtime"
+                # Fill in the missing values
+                starttime[0] = ser.starttime
+                endtime[max(endtime.index)] = ser.endtime
+                # Build the dataframe
+                uptime = pd.concat([starttime, endtime], axis=1)
+            else:
+                df = pd.DataFrame(columns=gaps_df.columns)
+                uptime = pd.DataFrame(
+                    [[ser["starttime"], ser["endtime"]]],
+                    columns=["starttime", "endtime"],
+                )
+            uptime["duration"] = uptime["endtime"] - uptime["starttime"]
+            for x in NSLC:
+                uptime[x] = ser[x]
+            return uptime
+
+        min_gap = kwargs.pop("min_gap", None)
+
+        avail = self.get_availability_df(*args, **kwargs)
+        gaps_df = self.get_gaps_df(*args, min_gap=min_gap, **kwargs)
+        gps = gaps_df.groupby(list(NSLC))
+        if not len(avail):
+            return pd.DataFrame(columns=self._segment_columns)
+        return pd.concat(
+            [_get_details(row) for _, row in avail.iterrows()]
+        ).reset_index(drop=True)
+
     # ------------------------ get waveform related methods
 
     def get_waveforms_bulk(
         self,
         bulk: bulk_waveform_arg_type,
         index: Optional[pd.DataFrame] = None,
         **kwargs,
```

### Comparing `obsplus-0.2.4/obsplus/constants.py` & `obsplus-0.2.5/src/obsplus/constants.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/bingham_test/dataset_hash.json` & `obsplus-0.2.5/src/obsplus/datasets/bingham_test/dataset_hash.json`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/bingham_test/events.xml` & `obsplus-0.2.5/src/obsplus/datasets/bingham_test/events.xml`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/bingham_test/inventory.xml` & `obsplus-0.2.5/src/obsplus/datasets/bingham_test/inventory.xml`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/bingham_test.py` & `obsplus-0.2.5/src/obsplus/datasets/bingham_test.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/crandall_test/dataset_hash.json` & `obsplus-0.2.5/src/obsplus/datasets/crandall_test/dataset_hash.json`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/crandall_test/events.xml` & `obsplus-0.2.5/src/obsplus/datasets/crandall_test/events.xml`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/crandall_test.py` & `obsplus-0.2.5/src/obsplus/datasets/crandall_test.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/dataset.py` & `obsplus-0.2.5/src/obsplus/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/default_test/dataset_hash.json` & `obsplus-0.2.5/src/obsplus/datasets/default_test/dataset_hash.json`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/default_test.py` & `obsplus-0.2.5/src/obsplus/datasets/default_test.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/ta_test/dataset_hash.json` & `obsplus-0.2.5/src/obsplus/datasets/ta_test/dataset_hash.json`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/ta_test/inventory.xml` & `obsplus-0.2.5/src/obsplus/datasets/ta_test/inventory.xml`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/datasets/ta_test.py` & `obsplus-0.2.5/src/obsplus/datasets/ta_test.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/events/get_events.py` & `obsplus-0.2.5/src/obsplus/events/get_events.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/events/json.py` & `obsplus-0.2.5/src/obsplus/events/json.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/events/merge.py` & `obsplus-0.2.5/src/obsplus/events/merge.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/events/pd.py` & `obsplus-0.2.5/src/obsplus/events/pd.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,22 +111,22 @@
         quality_attrs = (
             ("standard_error", np.NaN),
             ("associated_phase_count", out.get("associated_phase_count", 0)),
             ("azimuthal_gap", np.NaN),
             ("used_phase_count", out.get("used_phase_count", 0)),
         )
         quality = getattr(origin, "quality", ev.OriginQuality())
-        for (attr, default) in quality_attrs:
+        for attr, default in quality_attrs:
             out[attr] = getattr(quality, attr, None) or default
 
     def _get_origin_uncertainty(self, origin, out):
         """Get information from uncertainty."""
         uncert_attrs = (("horizontal_uncertainty", np.NaN),)
         uncert = getattr(origin, "origin_uncertainty", ev.OriginUncertainty())
-        for (attr, default) in uncert_attrs:
+        for attr, default in uncert_attrs:
             out[attr] = getattr(uncert, attr, default) or default
 
     def _get_depth_uncertainty_info(self, origin, out):
         """Get info from depth info."""
         depth_uncert = origin.depth_errors
         out["vertical_uncertainty"] = getattr(depth_uncert, "uncertainty", np.NaN)
 
@@ -565,15 +565,15 @@
         raise ValueError(msg)
     dd = {x: y for x, y in zip(NSLC, seed_id.split("."))}
     return {"seed_id": seed_id, **dd}
 
 
 # --- monkey patch events/event classes to have to_df methods.
 
-# event_to_dataframe
+
 def event_to_dataframe(cat_or_event):
     """
     Given a catalog or event, return a DataFrame summary.
 
     Notes
     -----
     Because of the complexity of obspy catalog and event objects, this extractor
```

### Comparing `obsplus-0.2.4/obsplus/events/schema.py` & `obsplus-0.2.5/src/obsplus/events/schema.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/events/validate.py` & `obsplus-0.2.5/src/obsplus/events/validate.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/exceptions.py` & `obsplus-0.2.5/src/obsplus/exceptions.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/interfaces.py` & `obsplus-0.2.5/src/obsplus/interfaces.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/stations/get_stations.py` & `obsplus-0.2.5/src/obsplus/stations/get_stations.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/stations/pd.py` & `obsplus-0.2.5/src/obsplus/stations/pd.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/structures/dfextractor.py` & `obsplus-0.2.5/src/obsplus/structures/dfextractor.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/structures/fetcher.py` & `obsplus-0.2.5/src/obsplus/structures/fetcher.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/bank.py` & `obsplus-0.2.5/src/obsplus/utils/bank.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/dataset.py` & `obsplus-0.2.5/src/obsplus/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/docs.py` & `obsplus-0.2.5/src/obsplus/utils/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
         The following line will be the string '10':
         {some_value}
         '''
     """
 
     def _wrap(func):
-
         docstring = func.__doc__
         # iterate each provided value and look for it in the docstring
         for key, value in kwargs.items():
             value = value if isinstance(value, str) else "\n".join(value)
             # strip out first line if needed
             value = value.lstrip()
             search_value = "{%s}" % key
```

### Comparing `obsplus-0.2.4/obsplus/utils/events.py` & `obsplus-0.2.5/src/obsplus/utils/events.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/geodetics.py` & `obsplus-0.2.5/src/obsplus/utils/geodetics.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/misc.py` & `obsplus-0.2.5/src/obsplus/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,27 +566,30 @@
     If the version string is not valid raise a ValueError.
     """
     is_str = isinstance(version_str, str)
     # If version_str is not a str or doesnt have a len of 3
     if not (is_str and len(version_str.split(".")) == 3):
         msg = f"version must be a string of the form x.y.z, not {version_str}"
         raise ValueError(msg)
+    # this will split out the dev version tags to just get latest version
+    out = version_str.split("dev")[0].split("+")[0]
+    return out
 
 
 def get_version_tuple(version_str: str) -> Tuple[int, int, int]:
     """
     Convert a semantic version string to a tuple.
 
     Parameters
     ----------
     version_str
         A version of the form "x.y.z". Google semantic versioning for more
         details.
     """
-    validate_version_str(version_str)
+    version_str = validate_version_str(version_str)
     split = version_str.split(".")
     return int(split[0]), int(split[1]), int(split[2])
 
 
 def strip_prefix(some_str: str, prefixes: Union[str, Collection[str]]) -> str:
     """Strip a prefix of a string."""
     out = some_str
```

### Comparing `obsplus-0.2.4/obsplus/utils/mseed.py` & `obsplus-0.2.5/src/obsplus/utils/mseed.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/pd.py` & `obsplus-0.2.5/src/obsplus/utils/pd.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/stations.py` & `obsplus-0.2.5/src/obsplus/utils/stations.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/testing.py` & `obsplus-0.2.5/src/obsplus/utils/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
             st.write(path, "mseed")
 
     def create_directory_from_bulk_args(self, bulk_args):
         """Create a directory from bulk waveform arguments"""
         # ensure directory exists
         path = Path(self.path)
         path.mkdir(exist_ok=True, parents=True)
-        for (net, sta, loc, chan, t1, t2) in bulk_args:
+        for net, sta, loc, chan, t1, t2 in bulk_args:
             nslc = ".".join([net, sta, loc, chan])
             st = self.create_stream(t1, t2, (nslc,))
             time_name = str(t1).split(".")[0].replace(":", "-") + ".mseed"
             save_name = path / f"{net}_{sta}_{time_name}"
             st.write(str(save_name), "mseed")
```

### Comparing `obsplus-0.2.4/obsplus/utils/time.py` & `obsplus-0.2.5/src/obsplus/utils/time.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,23 +310,28 @@
     out = [to_datetime64(x, default=default) for x in value]
     return np.array(out)
 
 
 @to_timedelta64.register(pd.Series)
 def _series_to_timedelta(ser) -> pd.Series:
     """Convert a series to a timedelta."""
+    if np.issubdtype(ser.dtype, np.timedelta64):
+        return ser.astype("timedelta64[ns]")  # convert to ns precision
+    # or iterate all elements of series.
     return ser.apply(to_timedelta64)
 
 
 @to_timedelta64.register(np.ndarray)
 def _array_to_timedelta(obj):
     """Convert a series to a timedelta."""
     if np.issubdtype(obj.dtype, np.timedelta64):
-        return obj
-    return np.array([to_timedelta64(x) for x in obj])
+        array = obj
+    else:
+        array = np.array([to_timedelta64(x) for x in obj])
+    return array.astype("timedelta64[ns]")
 
 
 @compose_docstring(time_keys=str(TIME_COLUMNS))
 def _dict_times_to_npdatetimes(
     input_dict: Dict[str, Any], time_keys: Sequence[str] = TIME_COLUMNS
 ) -> Dict[str, Any]:
     """
```

### Comparing `obsplus-0.2.4/obsplus/utils/validate.py` & `obsplus-0.2.5/src/obsplus/utils/validate.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/utils/waveforms.py` & `obsplus-0.2.5/src/obsplus/utils/waveforms.py`

 * *Files identical despite different names*

### Comparing `obsplus-0.2.4/obsplus/waveforms/get_waveforms.py` & `obsplus-0.2.5/src/obsplus/waveforms/get_waveforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     # get a dataframe of the bulk arguments, convert time to datetime64
     request_df = get_waveform_bulk_df(bulk)
     if not len(request_df):  # return empty string if no bulk reqs provided
         return obspy.Stream()
     # get unique times and check conditions for string columns
     unique_times = np.unique(request_df[["starttime", "endtime"]].values, axis=0)
     traces = []
-    for (t1, t2) in unique_times:
+    for t1, t2 in unique_times:
         sub = _filter_index_to_bulk((t1, t2), index_df=index, bulk_df=request_df)
         new = obspy.Stream(traces=[x.data for x in sub["trace"]]).slice(
             starttime=to_utc(t1), endtime=to_utc(t2)
         )
         traces.extend(new.traces)
     return merge_traces(obspy.Stream(traces=traces))
```

