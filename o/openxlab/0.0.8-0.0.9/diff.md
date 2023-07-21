# Comparing `tmp/openxlab-0.0.8.tar.gz` & `tmp/openxlab-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.8.tar", last modified: Fri Apr 28 10:26:52 2023, max compression
+gzip compressed data, was "openxlab-0.0.9.tar", last modified: Fri May 19 05:40:41 2023, max compression
```

## Comparing `openxlab-0.0.8.tar` & `openxlab-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,80 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.226486 openxlab-0.0.8/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-28 10:26:52.226177 openxlab-0.0.8/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1036 2023-04-10 10:02:47.000000 openxlab-0.0.8/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.200958 openxlab-0.0.8/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.8/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3138 2023-04-14 09:07:13.000000 openxlab-0.0.8/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.204253 openxlab-0.0.8/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.8/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-04-28 10:26:12.000000 openxlab-0.0.8/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.204694 openxlab-0.0.8/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1076 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.205692 openxlab-0.0.8/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      391 2023-04-27 05:13:40.000000 openxlab-0.0.8/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.206914 openxlab-0.0.8/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:36:45.000000 openxlab-0.0.8/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-16 03:45:30.000000 openxlab-0.0.8/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     5272 2023-04-28 09:49:50.000000 openxlab-0.0.8/openxlab/model/clients/openapi_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.213664 openxlab-0.0.8/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      695 2023-04-14 09:21:09.000000 openxlab-0.0.8/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-04-24 10:01:11.000000 openxlab-0.0.8/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      861 2023-04-25 10:15:10.000000 openxlab-0.0.8/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-04-14 09:06:08.000000 openxlab-0.0.8/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-04-24 11:39:15.000000 openxlab-0.0.8/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      702 2023-04-24 11:39:15.000000 openxlab-0.0.8/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1085 2023-04-27 05:56:30.000000 openxlab-0.0.8/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      752 2023-04-24 11:11:49.000000 openxlab-0.0.8/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.215809 openxlab-0.0.8/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 09:38:02.000000 openxlab-0.0.8/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1230 2023-04-28 09:57:07.000000 openxlab-0.0.8/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-04-14 05:07:06.000000 openxlab-0.0.8/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.222566 openxlab-0.0.8/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-13 02:48:29.000000 openxlab-0.0.8/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1285 2023-04-24 09:23:06.000000 openxlab-0.0.8/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2474 2023-04-28 09:56:29.000000 openxlab-0.0.8/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-04-13 03:08:33.000000 openxlab-0.0.8/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-04-24 11:33:14.000000 openxlab-0.0.8/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-04-24 11:39:15.000000 openxlab-0.0.8/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1044 2023-04-24 11:28:18.000000 openxlab-0.0.8/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1131 2023-04-27 06:01:17.000000 openxlab-0.0.8/openxlab/model/handler/update_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1095 2023-04-24 11:05:26.000000 openxlab-0.0.8/openxlab/model/handler/update_repository.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.223702 openxlab-0.0.8/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.8/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.224860 openxlab-0.0.8/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/utils/file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.225379 openxlab-0.0.8/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      418 2023-04-10 10:02:47.000000 openxlab-0.0.8/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-04-28 10:26:52.203624 openxlab-0.0.8/openxlab.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1434 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1487 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       88 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-04-28 10:26:52.000000 openxlab-0.0.8/openxlab.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      283 2023-04-10 10:02:47.000000 openxlab-0.0.8/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-04-28 10:26:52.226591 openxlab-0.0.8/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-04-23 01:59:14.000000 openxlab-0.0.8/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.621049 openxlab-0.0.9/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     4030 2023-05-19 05:40:41.620401 openxlab-0.0.9/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3632 2023-05-19 05:11:41.000000 openxlab-0.0.9/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.581540 openxlab-0.0.9/openxlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.9/openxlab/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/cli.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.586497 openxlab-0.0.9/openxlab/config/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.9/openxlab/config/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/config/const.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/config/version.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.587260 openxlab-0.0.9/openxlab/demo_cmd/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/demo_cmd/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.587856 openxlab-0.0.9/openxlab/model/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.590928 openxlab-0.0.9/openxlab/model/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/model_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     7757 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/openapi_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/oss_client.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/upload_service_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.597310 openxlab-0.0.9/openxlab/model/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/create.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1021 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/download.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/init.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/remove.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/upload.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/visibility.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.599615 openxlab-0.0.9/openxlab/model/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1747 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/constants.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.606814 openxlab-0.0.9/openxlab/model/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/common.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/create_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     4328 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/download_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/model_inference.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/model_list.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/update_repository.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/upload_file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.608183 openxlab-0.0.9/openxlab/types/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.9/openxlab/types/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.9/openxlab/types/command_type.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.612691 openxlab-0.0.9/openxlab/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.9/openxlab/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/utils/auth.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/utils/env_util.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.9/openxlab/utils/file.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/utils/time_util.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.613639 openxlab-0.0.9/openxlab/xlab/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.614826 openxlab-0.0.9/openxlab/xlab/clients/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/clients/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/clients/auth_client.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.615979 openxlab-0.0.9/openxlab/xlab/commands/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/commands/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/commands/config_command.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.617166 openxlab-0.0.9/openxlab/xlab/common/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/common/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/common/response_dto.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.619354 openxlab-0.0.9/openxlab/xlab/handler/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/handler/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/handler/user_config.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3880 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/handler/user_token.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.584961 openxlab-0.0.9/openxlab.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     4030 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1999 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-19 05:11:01.000000 openxlab-0.0.9/pyproject.toml
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-19 05:40:41.621236 openxlab-0.0.9/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-05-19 05:11:41.000000 openxlab-0.0.9/setup.py
```

### Comparing `openxlab-0.0.8/openxlab/cli.py` & `openxlab-0.0.9/openxlab/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from argparse import ArgumentParser, Namespace
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import openxlab
 from openxlab.demo_cmd import Demo
 from openxlab.model.commands import Model
 from openxlab.types.command_type import BaseCommand
+from openxlab.xlab import Config
 from openxlab.xlab import Version
 
 
 # 定义一级子命令
 class AllCommand(BaseCommand):
-    sub_command_list = [Version, Demo, Model]
+    sub_command_list = [Version, Demo, Model, Config]
     def take_action(self, parsed_args: Namespace) -> int:
         return 0
 
+
 # 递归添加子命令
 def _add_sub_commands_recur(
-    main_parser: ArgumentParser, parent_parser: ArgumentParser, command_type: BaseCommand
+        main_parser: ArgumentParser, parent_parser: ArgumentParser, command_type: BaseCommand
 ) -> Dict[str, ArgumentParser]:
     subparsers = main_parser.add_subparsers()
 
     sub_commands = command_type.sub_command_list
     for command_type in sub_commands:
         command = command_type()
         command_name = command.get_name()
@@ -35,52 +37,55 @@
 
         # 通过是否实现 take_action 判定命令的默认行为
         if issubclass(command_type, BaseCommand) and getattr(BaseCommand, "take_action") is not getattr(command_type, "take_action"):
             subparser.set_defaults(handler=command.take_action)
         else:
             def _print_help(args: Namespace) -> None:
                 subparser.print_help()
-            subparser.set_defaults(handler=_print_help)
 
+            subparser.set_defaults(handler=_print_help)
+        
         # 递归添加子命令
         _add_sub_commands_recur(subparser, parent_parser, command_type)
 
     # 添加默认的 help 命令
     def _print_help(args: Namespace) -> None:
         main_parser.print_help()
+
     subparsers.add_parser("help", help="Show help message and exit.").set_defaults(
         handler=_print_help
     )
     return
 
 
 def _get_parser(description: str = "") -> ArgumentParser:
     parent_parser = ArgumentParser(add_help=False)
 
     main_parser = ArgumentParser(description=description, parents=[parent_parser])
 
     _add_sub_commands_recur(main_parser, parent_parser, AllCommand)
-
+        
     return main_parser
 
+
 def _preprocess_argv(argv: List[str]) -> List[str]:
     # Some preprocess is necessary for argv because some subcommand includes space
     # (e.g. optuna study optimize, optuna storage upgrade, ...).
     argv = argv[1:] if len(argv) > 1 else ["help"]
 
     # No subcommand is found.
     return argv
 
 
 def main():
     main_parser = _get_parser()
     argv = sys.argv
     preprocessed_argv = _preprocess_argv(argv)
     args = main_parser.parse_args(preprocessed_argv)
-
+    
     logger = logging.getLogger("openxlab")
     try:
         return args.handler(args)
     except Exception as e:
         logger.exception(e)
         # if args.debug:
         #     logger.exception(e)
```

### Comparing `openxlab-0.0.8/openxlab/demo_cmd/__init__.py` & `openxlab-0.0.9/openxlab/demo_cmd/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from openxlab.config import version as config_version
 from openxlab.types.command_type import *
 
 
 def help():
     print("help")
 
+
 class Upload(BaseCommand):
     """upload"""
-    
+
     def get_name(self) -> str:
         return "upload"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         pass
 
     def take_action(self, parsed_args: Namespace) -> int:
         print("upload something")
         return 0
-    
+
+
 class Demo(BaseCommand):
     """demo"""
-    
+
     sub_command_list = [Upload]
+
     def get_name(self) -> str:
         return "demo"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             "--directions",
             type=str,
@@ -36,9 +39,7 @@
                 " This argument is deprecated. Please create a study in advance."
             ),
         )
 
     # def take_action(self, parsed_args: Namespace) -> int:
     #     help()
     #     return 0
-    
-
```

### Comparing `openxlab-0.0.8/openxlab/model/commands/__init__.py` & `openxlab-0.0.9/openxlab/model/commands/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from openxlab.types.command_type import *
 from openxlab.model.commands.download import Download
 from openxlab.model.commands.upload import Upload
 from openxlab.model.commands.init import Init
 from openxlab.model.commands.create import Create
+from openxlab.model.commands.list import List
+from openxlab.model.commands.visibility import Visibility
+from openxlab.model.commands.remove import Remove
 
 
 class Model(BaseCommand):
     """model"""
 
-    sub_command_list = [Upload, Download, Init, Create]
+    sub_command_list = [Upload, Download, Init, Create, List, Visibility, Remove]
 
     def get_name(self) -> str:
         return "model"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument(
             "--foo",
```

### Comparing `openxlab-0.0.8/openxlab/model/commands/create.py` & `openxlab-0.0.9/openxlab/model/commands/create.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.8/openxlab/model/commands/download.py` & `openxlab-0.0.9/openxlab/model/commands/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,11 +14,13 @@
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('-r', '--model-repo', required=True,
                             help='model repository address. format:username/repository.')
         parser.add_argument('-f', '--file', required=True,
                             help='target file to be download.')
         parser.add_argument('-p', '--path', required=False,
                             help='setting download path.')
+        parser.add_argument('-o', '--overwrite', action='store_true',
+                            help='force overwriting local files.')
 
     def take_action(self, parsed_args: Namespace) -> int:
-        download(parsed_args.model_repo, parsed_args.file, parsed_args.path)
+        download(parsed_args.model_repo, parsed_args.file, parsed_args.path, parsed_args.overwrite)
         return 0
```

### Comparing `openxlab-0.0.8/openxlab/model/commands/init.py` & `openxlab-0.0.9/openxlab/model/commands/init.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.8/openxlab/model/commands/list.py` & `openxlab-0.0.9/openxlab/model/commands/list.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.8/openxlab/model/commands/remove.py` & `openxlab-0.0.9/openxlab/model/commands/remove.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,13 +10,11 @@
 
     def get_name(self) -> str:
         return "remove"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('-r', '--model-repo', required=True,
                             help='model repository address. format:username/repository.')
-        parser.add_argument('-prt', '--private', type=bool, default=False, required=True,
-                            help='remove repository.')
 
     def take_action(self, parsed_args: Namespace) -> int:
-        remove(parsed_args.model_repo, parsed_args.private)
+        remove(parsed_args.model_repo)
         return 0
```

### Comparing `openxlab-0.0.8/openxlab/model/commands/upload.py` & `openxlab-0.0.9/openxlab/model/commands/upload.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     def get_name(self) -> str:
         return "upload"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('-r', '--model-repo', required=True,
                             help='model repository address. format:username/repository.')
-        parser.add_argument('-ft', '--file-type', type=str, required=False,
+        parser.add_argument('-ft', '--file-type', type=str, default='metafile', required=False,
                             help='upload file type, metafile/other.')
         parser.add_argument('-s', '--source', type=str, required=True,
                             help='metafile address or file address.')
         parser.add_argument('-t', '--target', type=str, required=False,
                             help='remote file address, only used when file type is other.')
 
     def take_action(self, parsed_args: Namespace) -> int:
```

### Comparing `openxlab-0.0.8/openxlab/model/commands/visibility.py` & `openxlab-0.0.9/openxlab/model/commands/visibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,13 +10,14 @@
 
     def get_name(self) -> str:
         return "visibility"
 
     def add_arguments(self, parser: ArgumentParser) -> None:
         parser.add_argument('-r', '--model-repo', required=True,
                             help='model repository address. format:username/repository.')
-        parser.add_argument('-prt', '--private', type=bool, default=False, required=True,
+        parser.add_argument('-prt', '--private', type=bool, default=False, required=False,
                             help='set repository visibility.')
 
     def take_action(self, parsed_args: Namespace) -> int:
-        visibility(parsed_args.model_repo, parsed_args.private)
+        private = False
+        visibility(parsed_args.model_repo, private)
         return 0
```

### Comparing `openxlab-0.0.8/openxlab/model/common/constants.py` & `openxlab-0.0.9/openxlab/model/common/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 """
 model module constant define
 """
+import os
 
 model_openapi_url_prefix_dev = "https://dev.openxlab.org.cn/api/v1"
+model_openapi_url_prefix_staging = "https://staging.openxlab.org.cn/api/v1"
 model_openapi_url_prefix_prod = "https://openapi.openxlab.org.cn/api/v1"
 model_url_prefix_dev = "http://localhost:10019"
+model_cache_path = f'{os.path.expanduser("~")}/.cache/model'
 # temp token
 token = "eyJ0eXBlIjoiSldUIiwiYWxnIjoiSFM1MTIifQ.eyJqdGkiOiI1OTcwOTEiLCJyb2wiOiJST0xFX0FETUlOIiwiaXNzIjoiT3BlblhMYWIiLCJpYXQiOjE2ODE5Njg4NzMsInBob25lIjoiIiwiYWsiOiI2cHFnOXprNmRteG9rZ2JnbHZvayIsImVtYWlsIjoiZG9uZ3hpYW96aHVhbmdAcGpsYWIub3JnLmNuIiwiZXhwIjoxNzEzNTA0ODczfQ.eFl8ZH9tDp-pcjY3wz6PeNBarJwhVx90qQ3h82Qvpf0hrcrdrQSBcI8AmEk2TZFpeViC6HBtXRxxGp2YLK1XkA"
 endpoint = model_openapi_url_prefix_prod
 paths = {
     'file_download_path': '/model-center/api/v1/cli/repository/getFileDownloadUrl',
     'meta_file_template_download_path': '/model-center/api/v1/cli/repository/getMetafileTemplateUrl',
     'create_repository_path': '/model-center/api/v1/cli/repository/createModelRepository',
     'update_repository_path': '/model-center/api/v1/cli/repository/updateRepositoryBaseInfo',
     'delete_repository_path': '/model-center/api/v1/cli/repository/deleteRepository',
-    'query_models_path': '/model-center/api/v1/cli/repository/queryModels',
+    'query_models_path': '/model-center/api/v1/cli/repository/getRepositoryModelList',
+    'update_upload_status_path': '/model-center/api/v1/cli/repository/updateFileUploadStatus',
+    'get_upload_signature': "/upload-service/api/v1/getUploadSignature",
 }
+# oss_endpoint = 'https://openmmlab-open.oss-cn-shanghai.aliyuncs.com'
+oss_endpoint = 'https://oss-cn-shanghai.aliyuncs.com'
+oss_bucket_domain = 'openmmlab-open.oss-cn-shanghai.aliyuncs.com'
 default_metafile_template_name = 'metafile.yaml'
```

### Comparing `openxlab-0.0.8/openxlab/model/common/meta_file_util.py` & `openxlab-0.0.9/openxlab/model/common/meta_file_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def get_meta_payload(repository, private, meta_data):
     _name = repository
     _nickname = repository
     _collection = meta_data['Collections'][0]
     _license = _collection['License']
     _github = _collection['Code']['URL']
     _public_status = 0 if private else 1
-    _models = [{"name": m['name'], "weightName": get_filename_from_url(m['Weights']),
+    _models = [{"name": m['Name'], "weightName": get_filename_from_url(m['Weights']),
                 "evaluations": [{"task": e['Task'], "dataset": e['Dataset']} for e in m['Results']]} for m in
                meta_data['Models']]
 
     payload = {"name": _name, "nickname": _nickname, "license": _license,
                "github": _github, "publicStatus": _public_status, "models": _models}
 
     print(f"convert to payload:{payload}")
```

### Comparing `openxlab-0.0.8/openxlab/model/common/response_dto.py` & `openxlab-0.0.9/openxlab/model/common/response_dto.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.8/openxlab/model/handler/query_repo_model.py` & `openxlab-0.0.9/openxlab/model/handler/query_repo_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,17 @@
     """
     list repository models
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
-        client.query_models(repository, metafile)
-        print(f"repository:{repository} visibility update to private successfully.")
+        data = client.query_models(repository, metafile)
+        print(f"repository:{repository} models as list:")
+        print(data)
     except ValueError as e:
         print(f"Error: {e}")
         return
 
 
 def _split_repo(model_repo) -> (str, str):
     """
```

### Comparing `openxlab-0.0.8/openxlab/model/handler/remove_repo_or_file.py` & `openxlab-0.0.9/openxlab/model/handler/update_repository.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-remove repository
+update repository
 """
 import re
 
 from openxlab.model.clients.openapi_client import OpenapiClient
 from openxlab.model.common.constants import endpoint, token
 
 
-def remove(model_repo) -> None:
+def visibility(model_repo, private) -> None:
     """
-    remove repository
+    update repository visibility private -> public
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
-        client.remove_repository(repository)
-        print(f"repository:{repository} visibility update to private successfully.")
+        client.update_repository(repository, private)
+        print(f"repository:{repository} visibility update to public successfully.")
     except ValueError as e:
         print(f"Error: {e}")
         return
 
 
 def _split_repo(model_repo) -> (str, str):
     """
```

### Comparing `openxlab-0.0.8/openxlab/model/handler/update_repository.py` & `openxlab-0.0.9/openxlab/model/handler/remove_repo_or_file.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-update repository
+remove repository
 """
 import re
 
 from openxlab.model.clients.openapi_client import OpenapiClient
 from openxlab.model.common.constants import endpoint, token
 
 
-def visibility(model_repo, private) -> None:
+def remove(model_repo) -> None:
     """
-    update repository visibility private -> public
+    remove repository
     """
     try:
         # split params
         username, repository = _split_repo(model_repo)
         client = OpenapiClient(endpoint, token)
-        client.update_repository(repository, private)
-        print(f"repository:{repository} visibility update to private successfully.")
+        client.remove_repository(repository)
+        print(f"repository:{repository} removed successfully.")
     except ValueError as e:
         print(f"Error: {e}")
         return
 
 
 def _split_repo(model_repo) -> (str, str):
     """
```

### Comparing `openxlab-0.0.8/openxlab/types/command_type.py` & `openxlab-0.0.9/openxlab/types/command_type.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.8/openxlab/utils/file.py` & `openxlab-0.0.9/openxlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `openxlab-0.0.8/openxlab.egg-info/SOURCES.txt` & `openxlab-0.0.9/openxlab.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 openxlab.egg-info/PKG-INFO
 openxlab.egg-info/SOURCES.txt
 openxlab.egg-info/dependency_links.txt
 openxlab.egg-info/entry_points.txt
 openxlab.egg-info/requires.txt
 openxlab.egg-info/top_level.txt
 openxlab/config/__init__.py
+openxlab/config/const.py
 openxlab/config/version.py
 openxlab/demo_cmd/__init__.py
 openxlab/model/__init__.py
 openxlab/model/clients/__init__.py
 openxlab/model/clients/model_client.py
 openxlab/model/clients/openapi_client.py
+openxlab/model/clients/oss_client.py
+openxlab/model/clients/upload_service_client.py
 openxlab/model/commands/__init__.py
 openxlab/model/commands/create.py
 openxlab/model/commands/download.py
 openxlab/model/commands/inference.py
 openxlab/model/commands/init.py
 openxlab/model/commands/list.py
 openxlab/model/commands/remove.py
@@ -33,14 +36,26 @@
 openxlab/model/handler/common.py
 openxlab/model/handler/create_repository.py
 openxlab/model/handler/download_file.py
 openxlab/model/handler/model_inference.py
 openxlab/model/handler/model_list.py
 openxlab/model/handler/query_repo_model.py
 openxlab/model/handler/remove_repo_or_file.py
-openxlab/model/handler/update_file.py
 openxlab/model/handler/update_repository.py
+openxlab/model/handler/upload_file.py
 openxlab/types/__init__.py
 openxlab/types/command_type.py
 openxlab/utils/__init__.py
+openxlab/utils/auth.py
+openxlab/utils/env_util.py
 openxlab/utils/file.py
-openxlab/xlab/__init__.py
+openxlab/utils/time_util.py
+openxlab/xlab/__init__.py
+openxlab/xlab/clients/__init__.py
+openxlab/xlab/clients/auth_client.py
+openxlab/xlab/commands/__init__.py
+openxlab/xlab/commands/config_command.py
+openxlab/xlab/common/__init__.py
+openxlab/xlab/common/response_dto.py
+openxlab/xlab/handler/__init__.py
+openxlab/xlab/handler/user_config.py
+openxlab/xlab/handler/user_token.py
```

### Comparing `openxlab-0.0.8/setup.py` & `openxlab-0.0.9/setup.py`

 * *Files identical despite different names*

