# Comparing `tmp/quickmpc-0.5.0.tar.gz` & `tmp/quickmpc-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-o4nte57w/quickmpc-0.5.0.tar", last modified: Thu Jul 13 10:37:40 2023, max compression
+gzip compressed data, was "/home/runner/work/QuickMPC/QuickMPC/packages/client/libclient-py/dist/.tmp-vpxq77ha/quickmpc-1.0.0.tar", last modified: Fri Jul 21 11:55:04 2023, max compression
```

## Comparing `quickmpc-0.5.0.tar` & `quickmpc-1.0.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.isort.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-13 10:37:19.000000 quickmpc-0.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 10:37:19.000000 quickmpc-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-13 10:37:19.000000 quickmpc-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 10:37:40.000000 quickmpc-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-13 10:37:19.000000 quickmpc-0.5.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    38439 2023-07-13 10:37:19.000000 quickmpc-0.5.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-13 10:37:19.000000 quickmpc-0.5.0/README-ja.md
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-13 10:37:19.000000 quickmpc-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-13 10:37:19.000000 quickmpc-0.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-13 10:37:19.000000 quickmpc-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/pandas/share_data_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/proto/common_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/common_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/common_types/common_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/common_types/common_types_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/qmpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/qmpc_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/request/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/qmpc_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/qmpc_request_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/request/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/share/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/share/share.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/if_present.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/utils/overload_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-13 10:37:19.000000 quickmpc-0.5.0/quickmpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-13 10:37:40.000000 quickmpc-0.5.0/quickmpc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-13 10:37:40.000000 quickmpc-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-13 10:37:19.000000 quickmpc-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/local_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/bitvector.csv
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/diff_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/edge_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/empty.csv
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/none.csv
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/not_csv.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/over_number.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_files/string_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/pandas/test_share_data_frame.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/request/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/request/test_qmpc_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/share/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_share_recons.py
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/share/test_share_sharize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/test_qmpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:40.000000 quickmpc-0.5.0/tests/unit_tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/utils/test_make_pieces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tests/unit_tests/utils/test_over_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-13 10:37:19.000000 quickmpc-0.5.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.isort.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-21 11:54:49.000000 quickmpc-1.0.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-21 11:54:49.000000 quickmpc-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-21 11:54:49.000000 quickmpc-1.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-21 11:55:04.000000 quickmpc-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-21 11:54:49.000000 quickmpc-1.0.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    38439 2023-07-21 11:54:49.000000 quickmpc-1.0.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-21 11:54:49.000000 quickmpc-1.0.0/README-ja.md
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-21 11:54:49.000000 quickmpc-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-21 11:54:49.000000 quickmpc-1.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-21 11:54:49.000000 quickmpc-1.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/pandas/share_data_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/proto/common_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/common_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12847 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/qmpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/qmpc_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/request/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19239 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/qmpc_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/qmpc_request_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/request/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/share/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/share/share.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/if_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/utils/overload_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-21 11:54:49.000000 quickmpc-1.0.0/quickmpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-21 11:55:04.000000 quickmpc-1.0.0/quickmpc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-21 11:55:04.000000 quickmpc-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 11:54:49.000000 quickmpc-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/local_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/bitvector.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/diff_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/edge_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/empty.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/none.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/not_csv.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/over_number.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_files/string_data.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/pandas/test_share_data_frame.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/request/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6565 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/request/test_qmpc_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/share/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_share_recons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/share/test_share_sharize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/test_qmpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 11:55:04.000000 quickmpc-1.0.0/tests/unit_tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/utils/test_make_pieces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tests/unit_tests/utils/test_over_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-21 11:54:49.000000 quickmpc-1.0.0/tox.ini
```

### Comparing `quickmpc-0.5.0/.vscode/settings.json` & `quickmpc-1.0.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/LICENSE` & `quickmpc-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/Pipfile.lock` & `quickmpc-1.0.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/README-ja.md` & `quickmpc-1.0.0/README-ja.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/README.md` & `quickmpc-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/mypy.ini` & `quickmpc-1.0.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/README.md` & `quickmpc-1.0.0/quickmpc/README.md`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/pandas/parser.py` & `quickmpc-1.0.0/quickmpc/pandas/parser.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/pandas/progress.py` & `quickmpc-1.0.0/quickmpc/pandas/progress.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/pandas/readers.py` & `quickmpc-1.0.0/quickmpc/pandas/readers.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ----------
     pd.DataFrame
         読み込んだテーブルデータ
     """
     df = pd.read_csv(*args, **kwargs)
     # ID列を数値化
     df[index_col] = df[index_col].map(lambda x: to_float(x))
-    # join時にQMPCのCC側でID列でsortできる様に、座圧を行いindexに設定しておく
+    # send_share時にID列でsortできる様にID列を座標圧縮した列を追加する
     df["__qmpc_sort_index__"] = df.index
     df = df.sort_values(by=index_col)
     df = df.reset_index(drop=True)
     df = df.sort_values(by="__qmpc_sort_index__")
     df["__qmpc_sort_index__"] = df.index
     df = df.reset_index(drop=True)
     return df
```

### Comparing `quickmpc-0.5.0/quickmpc/pandas/share_data_frame.py` & `quickmpc-1.0.0/quickmpc/pandas/share_data_frame.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/proto/common_types/common_types_pb2.pyi` & `quickmpc-1.0.0/quickmpc/proto/common_types/common_types_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _JobStatus:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _JobStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_JobStatus.ValueType], builtins.type):
+class _JobStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_JobStatus.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     UNKNOWN: _JobStatus.ValueType  # 0
     ERROR: _JobStatus.ValueType  # 1
     RECEIVED: _JobStatus.ValueType  # 2
     PRE_JOB: _JobStatus.ValueType  # 3
     READ_DB: _JobStatus.ValueType  # 4
     COMPUTE: _JobStatus.ValueType  # 5
@@ -43,15 +43,15 @@
 COMPLETED: JobStatus.ValueType  # 6
 global___JobStatus = JobStatus
 
 class _ComputationMethod:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ComputationMethodEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ComputationMethod.ValueType], builtins.type):
+class _ComputationMethodEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ComputationMethod.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     COMPUTATION_METHOD_UNSPECIFIED: _ComputationMethod.ValueType  # 0
     COMPUTATION_METHOD_MEAN: _ComputationMethod.ValueType  # 1
     COMPUTATION_METHOD_VARIANCE: _ComputationMethod.ValueType  # 2
     COMPUTATION_METHOD_SUM: _ComputationMethod.ValueType  # 3
     COMPUTATION_METHOD_CORREL: _ComputationMethod.ValueType  # 4
     COMPUTATION_METHOD_MESH_CODE: _ComputationMethod.ValueType  # 5
@@ -68,28 +68,27 @@
 COMPUTATION_METHOD_JOIN_TABLE: ComputationMethod.ValueType  # 6
 global___ComputationMethod = ComputationMethod
 
 class _ShareValueTypeEnum:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
-class _ShareValueTypeEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ShareValueTypeEnum.ValueType], builtins.type):
+class _ShareValueTypeEnumEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_ShareValueTypeEnum.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SHARE_VALUE_TYPE_UNSPECIFIED: _ShareValueTypeEnum.ValueType  # 0
     SHARE_VALUE_TYPE_FIXED_POINT: _ShareValueTypeEnum.ValueType  # 1
     SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION: _ShareValueTypeEnum.ValueType  # 2
 
 class ShareValueTypeEnum(_ShareValueTypeEnum, metaclass=_ShareValueTypeEnumEnumTypeWrapper): ...
 
 SHARE_VALUE_TYPE_UNSPECIFIED: ShareValueTypeEnum.ValueType  # 0
 SHARE_VALUE_TYPE_FIXED_POINT: ShareValueTypeEnum.ValueType  # 1
 SHARE_VALUE_TYPE_UTF_8_INTEGER_REPRESENTATION: ShareValueTypeEnum.ValueType  # 2
 global___ShareValueTypeEnum = ShareValueTypeEnum
 
-@typing_extensions.final
 class ProcedureProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ID_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     COMPLETED_FIELD_NUMBER: builtins.int
@@ -115,15 +114,14 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_details", b"_details", "details", b"details"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_details", b"_details", "completed", b"completed", "description", b"description", "details", b"details", "id", b"id", "progress", b"progress"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_details", b"_details"]) -> typing_extensions.Literal["details"] | None: ...
 
 global___ProcedureProgress = ProcedureProgress
 
-@typing_extensions.final
 class JobProgress(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     PROGRESSES_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
@@ -137,19 +135,17 @@
         status: global___JobStatus.ValueType = ...,
         progresses: collections.abc.Iterable[global___ProcedureProgress] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "progresses", b"progresses", "status", b"status"]) -> None: ...
 
 global___JobProgress = JobProgress
 
-@typing_extensions.final
 class Stacktrace(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
     class Frame(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         SOURCE_LOCATION_FIELD_NUMBER: builtins.int
         SOURCE_LINE_FIELD_NUMBER: builtins.int
         FUNCTION_NAME_FIELD_NUMBER: builtins.int
         source_location: builtins.str
@@ -172,15 +168,14 @@
         *,
         frames: collections.abc.Iterable[global___Stacktrace.Frame] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["frames", b"frames"]) -> None: ...
 
 global___Stacktrace = Stacktrace
 
-@typing_extensions.final
 class JobErrorInfo(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WHAT_FIELD_NUMBER: builtins.int
     ADDITIONAL_INFO_FIELD_NUMBER: builtins.int
     STACKTRACE_FIELD_NUMBER: builtins.int
     what: builtins.str
@@ -199,15 +194,14 @@
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_additional_info", b"_additional_info"]) -> typing_extensions.Literal["additional_info"] | None: ...
     @typing.overload
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_stacktrace", b"_stacktrace"]) -> typing_extensions.Literal["stacktrace"] | None: ...
 
 global___JobErrorInfo = JobErrorInfo
 
-@typing_extensions.final
 class Schema(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     name: builtins.str
     type: global___ShareValueTypeEnum.ValueType
```

### Comparing `quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2.pyi` & `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-@typing_extensions.final
 class SendSharesRequest(google.protobuf.message.Message):
     """*
     the message of SendSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -51,15 +50,14 @@
         matching_column: builtins.int = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "matching_column", b"matching_column", "piece_id", b"piece_id", "schema", b"schema", "sent_at", b"sent_at", "shares", b"shares", "token", b"token"]) -> None: ...
 
 global___SendSharesRequest = SendSharesRequest
 
-@typing_extensions.final
 class DeleteSharesRequest(google.protobuf.message.Message):
     """*
     the message of DeleteSharesRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -74,15 +72,14 @@
         dataIds: collections.abc.Iterable[builtins.str] | None = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["dataIds", b"dataIds", "token", b"token"]) -> None: ...
 
 global___DeleteSharesRequest = DeleteSharesRequest
 
-@typing_extensions.final
 class GetSchemaRequest(google.protobuf.message.Message):
     """*
     the message of GetSchemaRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -96,15 +93,14 @@
         data_id: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_id", b"data_id", "token", b"token"]) -> None: ...
 
 global___GetSchemaRequest = GetSchemaRequest
 
-@typing_extensions.final
 class GetSchemaResponse(google.protobuf.message.Message):
     """*
     the message of GetSchemaResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -116,15 +112,14 @@
         *,
         schema: collections.abc.Iterable[common_types.common_types_pb2.Schema] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["schema", b"schema"]) -> None: ...
 
 global___GetSchemaResponse = GetSchemaResponse
 
-@typing_extensions.final
 class JoinOrder(google.protobuf.message.Message):
     """*
     the message of ExecuteComputationRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -139,15 +134,14 @@
         data_ids: collections.abc.Iterable[builtins.str] | None = ...,
         debug_mode: builtins.bool = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["data_ids", b"data_ids", "debug_mode", b"debug_mode"]) -> None: ...
 
 global___JoinOrder = JoinOrder
 
-@typing_extensions.final
 class Input(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SRC_FIELD_NUMBER: builtins.int
     TARGET_FIELD_NUMBER: builtins.int
     @property
     def src(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
@@ -159,15 +153,14 @@
         src: collections.abc.Iterable[builtins.int] | None = ...,
         target: collections.abc.Iterable[builtins.int] | None = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["src", b"src", "target", b"target"]) -> None: ...
 
 global___Input = Input
 
-@typing_extensions.final
 class ExecuteComputationRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     METHOD_ID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     TABLE_FIELD_NUMBER: builtins.int
     ARG_FIELD_NUMBER: builtins.int
@@ -186,15 +179,14 @@
         arg: global___Input | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["arg", b"arg", "table", b"table"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["arg", b"arg", "method_id", b"method_id", "table", b"table", "token", b"token"]) -> None: ...
 
 global___ExecuteComputationRequest = ExecuteComputationRequest
 
-@typing_extensions.final
 class ExecuteComputationResponse(google.protobuf.message.Message):
     """
     the message of ExecuteComputationResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -205,15 +197,14 @@
         *,
         job_uuid: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid"]) -> None: ...
 
 global___ExecuteComputationResponse = ExecuteComputationResponse
 
-@typing_extensions.final
 class GetComputationRequest(google.protobuf.message.Message):
     """*
     the message of GetComputationResultRequest
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -227,15 +218,14 @@
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetComputationRequest = GetComputationRequest
 
-@typing_extensions.final
 class GetComputationResultResponse(google.protobuf.message.Message):
     """*
     the message of GetComputationResultResponse
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -264,15 +254,14 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "result_type", b"result_type"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["column_number", b"column_number", "is_dim1", b"is_dim1", "is_dim2", b"is_dim2", "is_schema", b"is_schema", "piece_id", b"piece_id", "result", b"result", "result_type", b"result_type"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["result_type", b"result_type"]) -> typing_extensions.Literal["is_dim1", "is_dim2", "is_schema"] | None: ...
 
 global___GetComputationResultResponse = GetComputationResultResponse
 
-@typing_extensions.final
 class GetComputationStatusResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     STATUS_FIELD_NUMBER: builtins.int
     PROGRESS_FIELD_NUMBER: builtins.int
     status: common_types.common_types_pb2.JobStatus.ValueType
     @property
@@ -285,15 +274,14 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "progress", b"progress"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_progress", b"_progress", "progress", b"progress", "status", b"status"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_progress", b"_progress"]) -> typing_extensions.Literal["progress"] | None: ...
 
 global___GetComputationStatusResponse = GetComputationStatusResponse
 
-@typing_extensions.final
 class GetElapsedTimeRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_UUID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     job_uuid: builtins.str
     token: builtins.str
@@ -303,30 +291,28 @@
         job_uuid: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["job_uuid", b"job_uuid", "token", b"token"]) -> None: ...
 
 global___GetElapsedTimeRequest = GetElapsedTimeRequest
 
-@typing_extensions.final
 class GetElapsedTimeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     ELAPSED_TIME_FIELD_NUMBER: builtins.int
     elapsed_time: builtins.float
     def __init__(
         self,
         *,
         elapsed_time: builtins.float = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["elapsed_time", b"elapsed_time"]) -> None: ...
 
 global___GetElapsedTimeResponse = GetElapsedTimeResponse
 
-@typing_extensions.final
 class GetJobErrorInfoResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     JOB_ERROR_INFO_FIELD_NUMBER: builtins.int
     @property
     def job_error_info(self) -> common_types.common_types_pb2.JobErrorInfo: ...
     def __init__(
@@ -336,15 +322,14 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["_job_error_info", b"_job_error_info", "job_error_info", b"job_error_info"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["_job_error_info", b"_job_error_info"]) -> typing_extensions.Literal["job_error_info"] | None: ...
 
 global___GetJobErrorInfoResponse = GetJobErrorInfoResponse
 
-@typing_extensions.final
 class AddShareDataFrameRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     BASE_DATA_ID_FIELD_NUMBER: builtins.int
     ADD_DATA_ID_FIELD_NUMBER: builtins.int
     TOKEN_FIELD_NUMBER: builtins.int
     base_data_id: builtins.str
@@ -357,15 +342,14 @@
         add_data_id: builtins.str = ...,
         token: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["add_data_id", b"add_data_id", "base_data_id", b"base_data_id", "token", b"token"]) -> None: ...
 
 global___AddShareDataFrameRequest = AddShareDataFrameRequest
 
-@typing_extensions.final
 class AddShareDataFrameResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DATA_ID_FIELD_NUMBER: builtins.int
     data_id: builtins.str
     def __init__(
         self,
```

### Comparing `quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.py` & `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi` & `quickmpc-1.0.0/quickmpc/proto/libc_to_manage_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/qmpc.py` & `quickmpc-1.0.0/quickmpc/qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/request/qmpc_request.py` & `quickmpc-1.0.0/quickmpc/request/qmpc_request.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/request/qmpc_request_interface.py` & `quickmpc-1.0.0/quickmpc/request/qmpc_request_interface.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/request/response.py` & `quickmpc-1.0.0/quickmpc/request/response.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/share/random.py` & `quickmpc-1.0.0/quickmpc/share/random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/share/restore.py` & `quickmpc-1.0.0/quickmpc/share/restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/share/share.py` & `quickmpc-1.0.0/quickmpc/share/share.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc/utils/make_pieces.py` & `quickmpc-1.0.0/quickmpc/utils/make_pieces.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     @methoddispatch(is_static_method=True)
     @staticmethod
     def make_pieces(_, __):
         raise ArgumentError("不正な引数が与えられています．")
 
     @staticmethod
     def check_max_size(max_size: int):
-        # NOTE: Couchbaseのアイテムサイズ上限:1MB
         # NOTE: grpcの送受信データサイズ上限:4MB
         lower_limit_size: int = 1
         upper_limit_size: int = 1_000_000
         if max_size > upper_limit_size:
             raise RuntimeError(
                 f"max size of piece ({max_size}) is over "
                 f"specified limit size ({upper_limit_size})"
```

### Comparing `quickmpc-0.5.0/quickmpc/utils/overload_tools.py` & `quickmpc-1.0.0/quickmpc/utils/overload_tools.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/quickmpc.egg-info/SOURCES.txt` & `quickmpc-1.0.0/quickmpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/conftest.py` & `quickmpc-1.0.0/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/local_server.py` & `quickmpc-1.0.0/tests/unit_tests/local_server.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/pandas/test_files/edge_data.csv` & `quickmpc-1.0.0/tests/unit_tests/pandas/test_files/edge_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/pandas/test_files/string_data.csv` & `quickmpc-1.0.0/tests/unit_tests/pandas/test_files/string_data.csv`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/pandas/test_parser.py` & `quickmpc-1.0.0/tests/unit_tests/pandas/test_parser.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/pandas/test_reader.py` & `quickmpc-1.0.0/tests/unit_tests/pandas/test_reader.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/pandas/test_share_data_frame.py` & `quickmpc-1.0.0/tests/unit_tests/pandas/test_share_data_frame.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/request/test_qmpc_request.py` & `quickmpc-1.0.0/tests/unit_tests/request/test_qmpc_request.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/share/test_random.py` & `quickmpc-1.0.0/tests/unit_tests/share/test_random.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/share/test_restore.py` & `quickmpc-1.0.0/tests/unit_tests/share/test_restore.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/share/test_share_recons.py` & `quickmpc-1.0.0/tests/unit_tests/share/test_share_recons.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/share/test_share_sharize.py` & `quickmpc-1.0.0/tests/unit_tests/share/test_share_sharize.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/test_qmpc.py` & `quickmpc-1.0.0/tests/unit_tests/test_qmpc.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/utils/test_make_pieces.py` & `quickmpc-1.0.0/tests/unit_tests/utils/test_make_pieces.py`

 * *Files identical despite different names*

### Comparing `quickmpc-0.5.0/tests/unit_tests/utils/test_over_load.py` & `quickmpc-1.0.0/tests/unit_tests/utils/test_over_load.py`

 * *Files identical despite different names*

