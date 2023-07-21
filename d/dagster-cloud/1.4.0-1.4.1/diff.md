# Comparing `tmp/dagster_cloud-1.4.0.tar.gz` & `tmp/dagster_cloud-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.4.0.tar", last modified: Thu Jul 20 22:04:26 2023, max compression
+gzip compressed data, was "dagster_cloud-1.4.1.tar", last modified: Fri Jul 21 15:39:21 2023, max compression
```

## Comparing `dagster_cloud-1.4.0.tar` & `dagster_cloud-1.4.1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.508099 dagster_cloud-1.4.0/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-07-20 22:04:26.508099 dagster_cloud-1.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.444098 dagster_cloud-1.4.0/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      223 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.448098 dagster_cloud-1.4.0/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.448098 dagster_cloud-1.4.0/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41815 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.448098 dagster_cloud-1.4.0/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14913 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.456098 dagster_cloud-1.4.0/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.456098 dagster_cloud-1.4.0/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.456098 dagster_cloud-1.4.0/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.460098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.464098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4536 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.468098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.468098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10999 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9826 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    12925 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.472098 dagster_cloud-1.4.0/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.472098 dagster_cloud-1.4.0/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4641 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.476098 dagster_cloud-1.4.0/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.476098 dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.480099 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12868 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    34523 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.480099 dagster_cloud-1.4.0/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19006 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.484099 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7336 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.484099 dagster_cloud-1.4.0/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.484099 dagster_cloud-1.4.0/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.488099 dagster_cloud-1.4.0/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6943 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.492099 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6895 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.492099 dagster_cloud-1.4.0/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12030 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.500099 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26066 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    23557 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4240 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.500099 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17125 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11474 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.504099 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74335 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.444098 dagster_cloud-1.4.0/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4537 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      409 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:04:26.508099 dagster_cloud-1.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.671007 dagster_cloud-1.4.1/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-07-21 15:39:21.671007 dagster_cloud-1.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.587007 dagster_cloud-1.4.1/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.595007 dagster_cloud-1.4.1/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.595007 dagster_cloud-1.4.1/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41815 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.595007 dagster_cloud-1.4.1/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.599007 dagster_cloud-1.4.1/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.599007 dagster_cloud-1.4.1/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.599007 dagster_cloud-1.4.1/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.599007 dagster_cloud-1.4.1/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14913 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.603007 dagster_cloud-1.4.1/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.607007 dagster_cloud-1.4.1/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.607007 dagster_cloud-1.4.1/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.607007 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.611007 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4536 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.619007 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.619007 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    12925 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.627007 dagster_cloud-1.4.1/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.627007 dagster_cloud-1.4.1/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.627007 dagster_cloud-1.4.1/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.631007 dagster_cloud-1.4.1/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.635007 dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12868 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.639007 dagster_cloud-1.4.1/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19006 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.643007 dagster_cloud-1.4.1/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7336 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.643007 dagster_cloud-1.4.1/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.643007 dagster_cloud-1.4.1/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.643007 dagster_cloud-1.4.1/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6943 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.647007 dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.647007 dagster_cloud-1.4.1/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.663007 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26066 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    23557 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.663007 dagster_cloud-1.4.1/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17125 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.671007 dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74335 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 15:39:21.591007 dagster_cloud-1.4.1/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-07-21 15:39:21.000000 dagster_cloud-1.4.1/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-07-21 15:39:21.000000 dagster_cloud-1.4.1/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 15:39:21.000000 dagster_cloud-1.4.1/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-21 15:39:21.000000 dagster_cloud-1.4.1/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-21 15:39:21.000000 dagster_cloud-1.4.1/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 15:39:21.671007 dagster_cloud-1.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-21 15:29:16.000000 dagster_cloud-1.4.1/setup.py
```

### Comparing `dagster_cloud-1.4.0/PKG-INFO` & `dagster_cloud-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.4.0
+Version: 1.4.1
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.4.0/README.md` & `dagster_cloud-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.4.1/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/agent/queries.py` & `dagster_cloud-1.4.1/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.4.1/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/auth/constants.py` & `dagster_cloud-1.4.1/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.4.1/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.4.1/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.4.1/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.4.1/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.4.1/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/client.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/runs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.4.1/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/util/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.4.1/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.4.1/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.4.0
+Version: 1.4.1
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.4.0/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.4.1/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.4.0/setup.py` & `dagster_cloud-1.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.4.0",
-        "dagster-cloud-cli==1.4.0",
+        "dagster==1.4.1",
+        "dagster-cloud-cli==1.4.1",
         "pex",
         "questionary",
         "requests",
         "typer[all]",
     ],
     extras_require={
         "tests": [
@@ -58,19 +58,19 @@
             "mypy",
             "paramiko",
             "pylint",
             "pytest",
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
-            "dagster_k8s==0.20.0",
+            "dagster_k8s==0.20.1",
         ],
-        "docker": ["docker", "dagster_docker==0.20.0"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.20.0"],
-        "ecs": ["dagster_aws==0.20.0", "boto3"],
+        "docker": ["docker", "dagster_docker==0.20.1"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.20.1"],
+        "ecs": ["dagster_aws==0.20.1", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

