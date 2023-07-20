# Comparing `tmp/dagster_cloud-1.3.9rc0.tar.gz` & `tmp/dagster_cloud-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_cloud-1.3.9rc0.tar", last modified: Thu Jun  8 18:31:19 2023, max compression
+gzip compressed data, was "dagster_cloud-1.4.0.tar", last modified: Thu Jul 20 22:04:26 2023, max compression
```

## Comparing `dagster_cloud-1.3.9rc0.tar` & `dagster_cloud-1.4.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.137182 dagster_cloud-1.3.9rc0/
--rw-r--r--   0 root         (0) root         (0)     4540 2023-06-08 18:31:19.133182 dagster_cloud-1.3.9rc0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.085182 dagster_cloud-1.3.9rc0/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      223 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.085182 dagster_cloud-1.3.9rc0/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.089182 dagster_cloud-1.3.9rc0/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42585 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1578 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.089182 dagster_cloud-1.3.9rc0/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16984 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.093181 dagster_cloud-1.3.9rc0/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/auth/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.093181 dagster_cloud-1.3.9rc0/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.093181 dagster_cloud-1.3.9rc0/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3223 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.093181 dagster_cloud-1.3.9rc0/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    14913 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.097182 dagster_cloud-1.3.9rc0/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.097182 dagster_cloud-1.3.9rc0/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    18147 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.097182 dagster_cloud-1.3.9rc0/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.097182 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.101182 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6822 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7786 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4541 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.105182 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.105182 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     1781 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10999 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)     9826 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    12930 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2889 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.105182 dagster_cloud-1.3.9rc0/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.109182 dagster_cloud-1.3.9rc0/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4641 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.109182 dagster_cloud-1.3.9rc0/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.109182 dagster_cloud-1.3.9rc0/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.113182 dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11717 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    32380 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.117182 dagster_cloud-1.3.9rc0/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6504 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    19041 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.117182 dagster_cloud-1.3.9rc0/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1927 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7209 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.117182 dagster_cloud-1.3.9rc0/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2248 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.121182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.121182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/cli/
--rw-r--r--   0 root         (0) root         (0)     6948 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.121182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)     8613 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6018 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.125182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12030 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.129182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23381 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    23524 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4165 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.133182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17127 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)    11407 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/kubernetes/utils.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.133182 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12807 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    74026 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 18:31:19.085182 dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4540 2023-06-08 18:31:19.000000 dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3216 2023-06-08 18:31:19.000000 dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 18:31:19.000000 dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      427 2023-06-08 18:31:19.000000 dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 18:31:19.000000 dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 18:31:19.137182 dagster_cloud-1.3.9rc0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2908 2023-06-08 18:21:06.000000 dagster_cloud-1.3.9rc0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.508099 dagster_cloud-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-07-20 22:04:26.508099 dagster_cloud-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.444098 dagster_cloud-1.4.0/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      223 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.448098 dagster_cloud-1.4.0/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.448098 dagster_cloud-1.4.0/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41815 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.448098 dagster_cloud-1.4.0/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16984 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/auth/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3223 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.452098 dagster_cloud-1.4.0/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    14913 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.456098 dagster_cloud-1.4.0/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.456098 dagster_cloud-1.4.0/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    18147 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.456098 dagster_cloud-1.4.0/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.460098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.464098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6822 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7786 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4536 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.468098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.468098 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10999 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    12925 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2889 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.472098 dagster_cloud-1.4.0/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.472098 dagster_cloud-1.4.0/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4641 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.476098 dagster_cloud-1.4.0/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.476098 dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.480099 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12868 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    34523 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.480099 dagster_cloud-1.4.0/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6504 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19006 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.484099 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7336 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      280 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.484099 dagster_cloud-1.4.0/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.484099 dagster_cloud-1.4.0/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.488099 dagster_cloud-1.4.0/dagster_cloud/workspace/cli/
+-rw-r--r--   0 root         (0) root         (0)     6943 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.492099 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)     8613 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6895 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.492099 dagster_cloud-1.4.0/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12030 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.500099 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26066 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    23557 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.500099 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17125 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.504099 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    74335 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 22:04:26.444098 dagster_cloud-1.4.0/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3216 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      409 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-20 22:04:26.000000 dagster_cloud-1.4.0/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 22:04:26.508099 dagster_cloud-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-20 21:53:47.000000 dagster_cloud-1.4.0/setup.py
```

### Comparing `dagster_cloud-1.3.9rc0/PKG-INFO` & `dagster_cloud-1.4.0/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster_cloud
-Version: 1.3.9rc0
+Version: 1.4.0
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.9rc0/README.md` & `dagster_cloud-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/agent/cli/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster_cloud-1.4.0/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -865,51 +865,34 @@
     ) -> Iterator[Optional[SerializableErrorInfo]]:
         if not user_code_launcher.ready_to_serve_requests:
             return
 
         num_pending_requests = len(self._pending_requests)
 
         if num_pending_requests < self._pending_requests_limit:
-            if instance.includes_branch_deployments:
-                result = instance.organization_scoped_graphql_client().execute(
-                    GET_USER_CLOUD_REQUESTS_QUERY,
-                    {"forBranchDeployments": True},
-                )
-                json_requests = result["data"]["userCloudAgent"]["popUserCloudAgentRequests"]
-
-                self._logger.debug(
-                    "Iteration #{iteration}: Adding {num_requests} branch deployment requests to be"
-                    " processed. Currently {num_pending_requests} waiting for server to be ready"
-                    .format(
-                        iteration=self._iteration,
-                        num_requests=len(json_requests),
-                        num_pending_requests=num_pending_requests,
-                    )
-                )
-
-                self._pending_requests.extend(json_requests)
-
-            for deployment_name in self._active_deployment_names:
-                result = instance.graphql_client_for_deployment(deployment_name).execute(
-                    GET_USER_CLOUD_REQUESTS_QUERY,
-                    {"forBranchDeployments": False},
-                )
-                json_requests = result["data"]["userCloudAgent"]["popUserCloudAgentRequests"]
-
-                self._logger.debug(
-                    "Iteration #{iteration}: Adding {num_requests} deployment requests to be"
-                    " processed. Currently {num_pending_requests} waiting for server to be ready"
-                    .format(
-                        iteration=self._iteration,
-                        num_requests=len(json_requests),
-                        num_pending_requests=num_pending_requests,
-                    )
+            # limit (implicit default 10) applied separately for requests to branch deployments, and for each full deployment
+            result = instance.organization_scoped_graphql_client().execute(
+                GET_USER_CLOUD_REQUESTS_QUERY,
+                {
+                    "forBranchDeployments": instance.includes_branch_deployments,
+                    "forFullDeployments": self._active_deployment_names,
+                },
+            )
+            json_requests = result["data"]["userCloudAgent"]["popUserCloudAgentRequests"]
+
+            self._logger.debug(
+                "Iteration #{iteration}: Adding {num_requests} requests to be"
+                " processed. Currently {num_pending_requests} waiting for server to be ready"
+                .format(
+                    iteration=self._iteration,
+                    num_requests=len(json_requests),
+                    num_pending_requests=num_pending_requests,
                 )
-
-                self._pending_requests.extend(json_requests)
+            )
+            self._pending_requests.extend(json_requests)
 
         else:
             self._logger.warning(
                 "Iteration #{iteration}: Waiting to pull requests from the queue since there are"
                 " already {num_pending_requests} in the queue".format(
                     iteration=self._iteration,
                     num_pending_requests=len(self._pending_requests),
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/agent/queries.py` & `dagster_cloud-1.4.0/dagster_cloud/agent/queries.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 GET_USER_CLOUD_REQUESTS_QUERY = """
-    mutation GetUserCloudRequests($forBranchDeployments: Boolean) {
+    mutation GetUserCloudRequests($forBranchDeployments: Boolean $forFullDeployments: [String!], $limit: Int) {
         userCloudAgent {
-            popUserCloudAgentRequests(limit:10, forBranchDeployments: $forBranchDeployments) {
+            popUserCloudAgentRequests(limit: $limit, forBranchDeployments: $forBranchDeployments, forFullDeployments: $forFullDeployments) {
                 requestId
                 requestApi
                 requestBody
                 deploymentName
                 isBranchDeployment
             }
         }
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/api/dagster_cloud_api.py` & `dagster_cloud-1.4.0/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/auth/constants.py` & `dagster_cloud-1.4.0/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster_cloud-1.4.0/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/execution/monitoring/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/execution/utils/process.py` & `dagster_cloud-1.4.0/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/instance/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/client.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,11 +106,11 @@
             return
         except Exception:
             last_error = serializable_error_info_from_exc_info(sys.exc_info())
 
         if time.time() - start_time > timeout:
             raise Exception(
                 f"Timed out after waiting {timeout}s for server. "
-                f"Most recent connection error: {str(last_error)}"
+                f"Most recent connection error: {last_error}"
             )
 
         time.sleep(1)
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/compile.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/manager.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/registry.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/server/server.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/server/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 all_run_ids.extend(run_ids)
             except DagsterUserCodeUnreachableError:
                 e = serializable_error_info_from_exc_info(sys.exc_info())
 
                 # If the pex server is unreachable, it may just be in the process of shutting down.
                 check.invariant(
                     not self._pex_manager.is_server_active(handle_id),
-                    f"Active server hit error:\n{str(e)}",
+                    f"Active server hit error:\n{e}",
                 )
 
         return api_pb2.GetCurrentRunsReply(
             serialized_current_runs=serialize_value(
                 GetCurrentRunsResult(current_runs=all_run_ids, serializable_error_info=None)
             )
         )
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/pex/grpc/types.py` & `dagster_cloud-1.4.0/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/secrets/loader.py` & `dagster_cloud-1.4.0/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/serverless/io_manager.py` & `dagster_cloud-1.4.0/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/client.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/queries.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -276,14 +276,55 @@
                     }
                 }
             }
         }
     }
     """
 
+GET_LATEST_STORAGE_ID_BY_PARTITION = """
+    query getLatestStorageIdByPartition($assetKey: String!, $eventType: String!) {
+        eventLogs {
+            getLatestStorageIdByPartition(assetKey: $assetKey, eventType: $eventType) {
+                ... on StorageIdByPartition {
+                    partition
+                    storageId
+                }
+            }
+        }
+    }
+"""
+
+GET_LATEST_TAGS_BY_PARTITION = """
+    query getLatestTagsByPartition(
+        $assetKey: String!,
+        $eventType: String!,
+        $tagKeys: [String!],
+        $assetPartitions: [String!],
+        $beforeCursor: BigInt,
+        $afterCursor: BigInt,
+    ) {
+        eventLogs {
+            getLatestTagsByPartition(
+                assetKey: $assetKey,
+                eventType: $eventType,
+                tagKeys: $tagKeys,
+                assetPartitions: $assetPartitions,
+                beforeCursor: $beforeCursor,
+                afterCursor: $afterCursor,
+            ) {
+                ... on TagByPartition {
+                    partition
+                    key
+                    value
+                }
+            }
+        }
+    }
+"""
+
 GET_LATEST_ASSET_PARTITION_MATERIALIZATION_ATTEMPTS_WITHOUT_MATERIALIZATIONS = """
     query getLatestAssetPartitionMaterializationAttemptsWithoutMaterializations($assetKey: String!) {
         eventLogs {
             getLatestAssetPartitionMaterializationAttemptsWithoutMaterializations(assetKey: $assetKey)
         }
     }
     """
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/storage.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from collections import defaultdict
 from os import getenv
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
@@ -66,14 +67,16 @@
     GET_CONCURRENCY_INFO_QUERY,
     GET_CONCURRENCY_KEYS_QUERY,
     GET_DYNAMIC_PARTITIONS_QUERY,
     GET_EVENT_RECORDS_QUERY,
     GET_EVENT_TAGS_FOR_ASSET,
     GET_LATEST_ASSET_PARTITION_MATERIALIZATION_ATTEMPTS_WITHOUT_MATERIALIZATIONS,
     GET_LATEST_MATERIALIZATION_EVENTS_QUERY,
+    GET_LATEST_STORAGE_ID_BY_PARTITION,
+    GET_LATEST_TAGS_BY_PARTITION,
     GET_MATERIALIZATION_COUNT_BY_PARTITION,
     GET_RECORDS_FOR_RUN_QUERY,
     GET_STATS_FOR_RUN_QUERY,
     GET_STEP_STATS_FOR_RUN_QUERY,
     HAS_ASSET_KEY_QUERY,
     HAS_DYNAMIC_PARTITION_QUERY,
     IS_ASSET_AWARE_QUERY,
@@ -607,14 +610,64 @@
             for graphene_partition_count in asset_count["materializationCountByPartition"]:
                 materialization_count_by_partition[asset_key][
                     graphene_partition_count["partition"]
                 ] = graphene_partition_count["materializationCount"]
 
         return materialization_count_by_partition
 
+    def get_latest_storage_id_by_partition(
+        self, asset_key: AssetKey, event_type: DagsterEventType
+    ) -> Mapping[str, int]:
+        res = self._execute_query(
+            GET_LATEST_STORAGE_ID_BY_PARTITION,
+            variables={
+                "assetKey": asset_key.to_string(),
+                "eventType": event_type.value,
+            },
+        )
+        latest_storage_id_result = res["data"]["eventLogs"]["getLatestStorageIdByPartition"]
+        latest_storage_id_by_partition: Dict[str, int] = {}
+
+        for graphene_latest_storage_id in latest_storage_id_result:
+            latest_storage_id_by_partition[
+                graphene_latest_storage_id["partition"]
+            ] = graphene_latest_storage_id["storageId"]
+
+        return latest_storage_id_by_partition
+
+    def get_latest_tags_by_partition(
+        self,
+        asset_key: AssetKey,
+        event_type: DagsterEventType,
+        tag_keys: Optional[Sequence[str]] = None,
+        asset_partitions: Optional[Sequence[str]] = None,
+        before_cursor: Optional[int] = None,
+        after_cursor: Optional[int] = None,
+    ) -> Mapping[str, Mapping[str, str]]:
+        res = self._execute_query(
+            GET_LATEST_TAGS_BY_PARTITION,
+            variables={
+                "assetKey": asset_key.to_string(),
+                "eventType": event_type.value,
+                "tagKeys": tag_keys,
+                "assetPartitions": asset_partitions,
+                "beforeCursor": before_cursor,
+                "afterCursor": after_cursor,
+            },
+        )
+        latest_tags_by_partition_result = res["data"]["eventLogs"]["getLatestTagsByPartition"]
+        latest_tags_by_partition: Dict[str, Dict[str, str]] = defaultdict(dict)
+        for tag_by_partition in latest_tags_by_partition_result:
+            latest_tags_by_partition[tag_by_partition["partition"]][
+                tag_by_partition["key"]
+            ] = tag_by_partition["value"]
+
+        # convert defaultdict to dict
+        return dict(latest_tags_by_partition)
+
     def get_latest_asset_partition_materialization_attempts_without_materializations(
         self, asset_key: AssetKey
     ) -> Mapping[str, Tuple[str, int]]:
         res = self._execute_query(
             GET_LATEST_ASSET_PARTITION_MATERIALIZATION_ATTEMPTS_WITHOUT_MATERIALIZATIONS,
             variables={
                 "assetKey": asset_key.to_string(),
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/event_logs/utils.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/event_logs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/runs/queries.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/runs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/runs/storage.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/runs/storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,17 +239,15 @@
                     deserialize_value(run, DagsterRun)
                     for run in run_group_or_error["serializedRuns"]
                 ],
             )
         elif run_group_or_error["__typename"] == "RunNotFoundError":
             raise DagsterRunNotFoundError(invalid_run_id=run_group_or_error["runId"])
         else:
-            raise DagsterInvariantViolationError(
-                f"Unexpected getRunGroupOrError response {str(res)}"
-            )
+            raise DagsterInvariantViolationError(f"Unexpected getRunGroupOrError response {res}")
 
     def get_run_groups(
         self,
         filters: Optional[RunsFilter] = None,
         cursor: Optional[str] = None,
         limit: Optional[int] = None,
     ) -> Mapping[str, RunGroupInfo]:
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/schedules/queries.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/schedules/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 tickId
             }
         }
     }
 """
 
 UPDATE_JOB_TICK_MUTATION = """
-    mutation updateJobTickMutation($tickId: Int! $serializedJobTickData: String!) {
+    mutation updateJobTickMutation($tickId: BigInt! $serializedJobTickData: String!) {
         schedules {
             updateJobTick(tickId: $tickId, serializedJobTickData: $serializedJobTickData) {
                 ok
             }
         }
     }
 """
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/storage/schedules/storage.py` & `dagster_cloud-1.4.0/dagster_cloud/storage/schedules/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,24 +140,24 @@
         origin_id: str,
         selector_id: str,
         before: Optional[float] = None,
         after: Optional[float] = None,
         limit: Optional[int] = None,
         statuses: Optional[Sequence[TickStatus]] = None,
     ) -> Iterable[InstigatorTick]:
-        statuses = [status.value for status in statuses] if statuses else None
+        status_strs = [status.value for status in statuses] if statuses else None
         res = self._execute_query(
             GET_JOB_TICKS_QUERY,
             variables={
                 "jobOriginId": origin_id,
                 "selectorId": selector_id,
                 "before": before,
                 "after": after,
                 "limit": limit,
-                "statuses": statuses,
+                "statuses": status_strs,
             },
         )
 
         return [
             deserialize_value(tick, InstigatorTick) for tick in res["data"]["schedules"]["jobTicks"]
         ]
 
@@ -203,12 +203,15 @@
         raise NotImplementedError("Not callable from user cloud")
 
     def get_auto_materialize_asset_evaluations(
         self, asset_key: AssetKey, limit: int, cursor: Optional[int] = None
     ) -> Sequence[AutoMaterializeAssetEvaluationRecord]:
         raise NotImplementedError("Not callable from user cloud")
 
+    def purge_asset_evaluations(self, before: float):
+        raise NotImplementedError("Not callable from user cloud")
+
     def upgrade(self):
         raise NotImplementedError("Not callable from user cloud")
 
     def optimize_for_dagit(self, statement_timeout: int, pool_recycle: int):
         raise NotImplementedError("Not callable from user cloud")
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/util/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/cli/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                 f"Uploaded snapshot of location `{location_data.name}` "
                 f"in image `{location_data.image}` for code preview `{code_preview_uuid}`."
             )
         except Exception as e:
             raise ui.error(
                 f"Failed to upload snapshot of location `{location_data.name}` "
                 f"in image `{location_data.image}` for code preview `{code_preview_uuid}`: "
-                f"{str(e)}"
+                f"{e}"
             )
 
 
 @contextmanager
 def get_location_or_load_error(
     location_data: gql.CliInputCodeLocation,
 ) -> Iterator[Tuple[Optional[InProcessCodeLocation], Optional[SerializableErrorInfo]]]:
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/docker.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/ecs.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,23 @@
                     description="The memory override to use for the launched task.",
                 ),
                 "ephemeral_storage": Field(
                     int,
                     is_required=False,
                     description="The ephemeral storage, in GiB, to use for the launched task.",
                 ),
+                "repository_credentials": Field(
+                    str,
+                    is_required=False,
+                    description=(
+                        "AWS SSM Secret ARN of the credentials used to pull a server's image from a"
+                        " private registry."
+                        " https://docs.aws.amazon.com/AmazonECS/latest/developerguide/private-auth.html"
+                    ),
+                ),
             }
         )
     ),
     "run_resources": Field(
         Permissive(
             {
                 "cpu": Field(
@@ -37,14 +46,23 @@
                     description="The memory override to use for the launched task.",
                 ),
                 "ephemeral_storage": Field(
                     int,
                     is_required=False,
                     description="The ephemeral storage, in GiB, to use for the launched task.",
                 ),
+                "repository_credentials": Field(
+                    str,
+                    is_required=False,
+                    description=(
+                        "AWS SSM Secret ARN of the credentials used to pull a run's image from a"
+                        " private registry."
+                        " https://docs.aws.amazon.com/AmazonECS/latest/developerguide/private-auth.html"
+                    ),
+                ),
             }
         )
     ),
     "runtime_platform": Field(
         Shape(
             {
                 "cpuArchitecture": Field(StringSource, is_required=False),
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/docker/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/client.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import time
 from typing import List, Optional
 
 import boto3
+import botocore
 import dagster._check as check
 from botocore.config import Config
 from botocore.exceptions import ClientError
 from dagster_aws.ecs.tasks import DagsterEcsTaskDefinitionConfig
 from dagster_aws.ecs.utils import task_definitions_match
 
 from dagster_cloud.workspace.ecs.service import Service
@@ -53,15 +54,16 @@
         grace_period: int = DEFAULT_ECS_GRACE_PERIOD,
         launch_type: str = "FARGATE",
         show_debug_cluster_info: bool = True,
     ):
         self.ecs = ecs_client if ecs_client else boto3.client("ecs", config=config)
         self.logs = boto3.client("logs", config=config)
         self.service_discovery = boto3.client("servicediscovery", config=config)
-        self.ec2 = boto3.resource("ec2", config=config)
+        self.tags_client = boto3.client("resourcegroupstaggingapi", config=config)
+        self._use_legacy_tag_filtering = False
 
         self.cluster_name = cluster_name.split("/")[-1]
         self.subnet_ids = check.opt_list_param(subnet_ids, "subnet_ids")
         self.security_group_ids = check.opt_list_param(security_group_ids, "security_group_ids")
         self.service_discovery_namespace_id = check.str_param(
             service_discovery_namespace_id, "service_discovery_namespace_id"
         )
@@ -71,14 +73,20 @@
 
         self.timeout = check.int_param(timeout, "timeout")
         self.grace_period = check.int_param(grace_period, "grace_period")
         self.launch_type = check.str_param(launch_type, "launch_type")
         self._namespace: Optional[str] = None
 
     @property
+    def ec2(self):
+        # Reconstruct the resource on each call because it's not threadsafe
+        # https://boto3.amazonaws.com/v1/documentation/api/latest/guide/resources.html#multithreading-or-multiprocessing-with-resources
+        return boto3.resource("ec2", config=config)
+
+    @property
     def namespace(self):
         if not self._namespace:
             self._namespace = (
                 self.service_discovery.get_namespace(
                     Id=self.service_discovery_namespace_id,
                 )
                 .get("Namespace")
@@ -123,14 +131,15 @@
         env=None,
         secrets=None,
         sidecars=None,
         logger=None,
         cpu=None,
         memory=None,
         ephemeral_storage=None,
+        repository_credentials=None,
         runtime_platform=None,
         mount_points=None,
         volumes=None,
     ):
         container_name = container_name or family
 
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
@@ -160,14 +169,15 @@
             execution_role_arn=execution_role_arn,
             task_role_arn=task_role_arn,
             sidecars=sidecars,
             requires_compatibilities=[self.launch_type],
             cpu=cpu,
             memory=memory,
             ephemeral_storage=ephemeral_storage,
+            repository_credentials=repository_credentials,
             runtime_platform=runtime_platform,
             mount_points=mount_points,
             volumes=volumes,
         )
 
         try:
             existing_task_definition = self.ecs.describe_task_definition(taskDefinition=family)[
@@ -217,14 +227,15 @@
         register_service_discovery=True,
         secrets=None,
         sidecars=None,
         logger=None,
         cpu=None,
         memory=None,
         ephemeral_storage=None,
+        repository_credentials=None,
         allow_ecs_exec=False,
         runtime_platform=None,
         mount_points=None,
         volumes=None,
     ):
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
@@ -243,14 +254,15 @@
             env=env or {},
             secrets=secrets,
             sidecars=sidecars,
             logger=logger,
             cpu=cpu,
             memory=memory,
             ephemeral_storage=ephemeral_storage,
+            repository_credentials=repository_credentials,
             runtime_platform=runtime_platform,
             mount_points=mount_points,
             volumes=volumes,
         )
 
         service_registry_arn = None
         # Configure service discovery
@@ -317,22 +329,66 @@
                     time.sleep(2)
 
             # delete service discovery
             self.service_discovery.delete_service(
                 Id=service_discovery_id,
             )
 
-    def list_services(self):
+    def list_services(self, tags=None, logger=None):
+        logger = logger or logging.getLogger("dagster_cloud.EcsClient")
+
         services = []
 
-        paginator = self.ecs.get_paginator("list_services")
-        for page in paginator.paginate(cluster=self.cluster_name):
-            for arn in page.get("serviceArns"):
-                service = Service(client=self, arn=arn)
-                services.append(service)
+        if tags:
+            if not self._use_legacy_tag_filtering:
+                try:
+                    paginator = self.tags_client.get_paginator("get_resources")
+                    for page in paginator.paginate(
+                        TagFilters=[
+                            {
+                                "Key": key,
+                                "Values": [value],
+                            }
+                            for key, value in tags.items()
+                        ],
+                        ResourceTypeFilters=["ecs:service"],
+                    ):
+                        for resource in page["ResourceTagMappingList"]:
+                            arn = resource["ResourceARN"]
+                            if self.cluster_name in arn:
+                                services.append(Service(client=self, arn=arn))
+                except botocore.exceptions.ClientError as error:
+                    if error.response["Error"]["Code"] == "AccessDeniedException":
+                        self._use_legacy_tag_filtering = True
+                        logger.warning(
+                            "dagster-cloud 1.4.0 includes performance enhancements that rely on the"
+                            " Resource"
+                            " Group Tagging API. To take advantage, add 'tags:GetResources'"
+                            " permissions to"
+                            " your"
+                            " task role."
+                            " https://docs.aws.amazon.com/resourcegroupstagging/latest/APIReference/overview.html"
+                        )
+                        services = self.list_services(tags)
+                    else:
+                        raise
+            else:
+                filtered_services = [
+                    service
+                    for service in self.list_services()
+                    if tags.items() <= service.tags.items()
+                ]
+                return filtered_services
+
+        else:
+            paginator = self.ecs.get_paginator("list_services")
+            for page in paginator.paginate(cluster=self.cluster_name):
+                for arn in page.get("serviceArns"):
+                    service = Service(client=self, arn=arn)
+                    services.append(service)
 
         return services
 
     def _run_task(self, name, image, command, execution_role_arn):
         """This is no longer used except as an integration test util
         for testing various network configurations.
         """
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/launcher.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,14 +268,19 @@
         return container_context.server_resources.get("memory")
 
     def _get_service_ephemeral_storage_override(
         self, container_context: EcsContainerContext
     ) -> Optional[int]:
         return container_context.server_resources.get("ephemeral_storage")
 
+    def _get_service_repository_credentials_override(
+        self, container_context: EcsContainerContext
+    ) -> Optional[str]:
+        return container_context.server_resources.get("repository_credentials")
+
     def _get_enable_ecs_exec(self) -> bool:
         return False
 
     def _get_additional_grpc_server_env(self) -> Dict[str, str]:
         return {}
 
     def _get_dagster_tags(self, deployment_name: str, location_name: str) -> Dict[str, str]:
@@ -361,14 +366,17 @@
             task_role_arn=container_context.task_role_arn,
             secrets=container_context.get_secrets_dict(self.secrets_manager),
             sidecars=self._get_grpc_server_sidecars(container_context),
             logger=self._logger,
             cpu=self._get_service_cpu_override(container_context),
             memory=self._get_service_memory_override(container_context),
             ephemeral_storage=self._get_service_ephemeral_storage_override(container_context),
+            repository_credentials=self._get_service_repository_credentials_override(
+                container_context
+            ),
             allow_ecs_exec=self._get_enable_ecs_exec(),
             runtime_platform=container_context.runtime_platform,
             mount_points=container_context.mount_points,
             volumes=container_context.volumes,
         )
         self._logger.info(
             "Created a new service at hostname {} for {}:{}, waiting for server to be ready..."
@@ -472,35 +480,27 @@
         tags = {
             "dagster/location_hash": deterministic_label_for_location(
                 deployment_name, location_name
             ),
             "dagster/multipex_server": "1",
             "dagster/agent_id": self._instance.instance_uuid,
         }
-        services = self.client.list_services()
-        location_services = [
-            service for service in services if tags.items() <= service.tags.items()
-        ]
-        return location_services
+        return self.client.list_services(tags)
 
     def _get_standalone_dagster_server_handles_for_location(
         self, deployment_name, location_name: str
     ) -> Collection[EcsServerHandleType]:
         tags = {
             "dagster/location_hash": deterministic_label_for_location(
                 deployment_name, location_name
             ),
             "dagster/grpc_server": "1",
             "dagster/agent_id": self._instance.instance_uuid,
         }
-        services = self.client.list_services()
-        location_services = [
-            service for service in services if tags.items() <= service.tags.items()
-        ]
-        return location_services
+        return self.client.list_services(tags)
 
     def _list_server_handles(self) -> List[EcsServerHandleType]:
         return [
             service
             for service in self.client.list_services()
             if "dagster/location_name" in service.tags.keys()
         ]
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/service.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from dagster._utils.cached_method import cached_method
+
 
 class Service:
     def __init__(self, client, arn):
         self.client = client
         self.arn = self._long_arn(arn)
         self.name = arn.split("/")[-1]
 
@@ -37,14 +39,15 @@
                 )
             )
             return {}
 
         return dict([(tag["Key"], tag["Value"]) for tag in tags])
 
     @property
+    @cached_method
     def service_discovery_arn(self):
         service = self.client.ecs.describe_services(
             cluster=self.client.cluster_name,
             services=[self.arn],
         ).get("services", [{}])[0]
 
         registries = service.get("serviceRegistries") or [{}]
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/ecs/utils.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 
         return handles
 
     def _list_server_handles(self) -> List[K8sHandle]:
         namespaces: Set[str] = set()
         if self._namespace:
             namespaces.add(self._namespace)
-        for _, namespace_items in self._used_namespaces.items():
+        for namespace_items in self._used_namespaces.values():
             for namespace in namespace_items:
                 namespaces.add(namespace)
         handles: List[K8sHandle] = []
         with self._get_apps_api_instance() as api_instance:
             for namespace in namespaces:
                 deployments = api_instance.list_namespaced_deployment(
                     namespace,
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/kubernetes/utils.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,17 +117,19 @@
 
     user_defined_env_vars = container_config.pop("env", [])
     user_defined_env_from = container_config.pop("env_from", [])
     user_defined_volume_mounts = container_config.pop("volume_mounts", [])
     user_defined_resources = container_config.pop("resources", {})
     user_defined_security_context = container_config.pop("security_context", None)
 
+    container_name = container_config.get("name", "dagster")
+
     container_config = {
         **container_config,
-        "name": "dagster",
+        "name": container_name,
         "image": metadata.image,
         "env": [{"name": key, "value": value} for key, value in env.items()]
         + user_defined_env_vars,
         "env_from": [{"config_map_ref": {"name": config_map}} for config_map in env_config_maps]
         + [{"secret_ref": {"name": secret_name}} for secret_name in env_secrets]
         + user_defined_env_from,
         "volume_mounts": volume_mounts + user_defined_volume_mounts,
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/origin.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/origin.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 from dagster._grpc.client import DagsterGrpcClient
 from dagster._grpc.types import GetCurrentImageResult
 from dagster._serdes import deserialize_value, serialize_value, whitelist_for_serdes
 from dagster._utils.error import SerializableErrorInfo, serializable_error_info_from_exc_info
 from dagster._utils.merger import merge_dicts
 from dagster_cloud_cli.core.errors import GraphQLStorageError, raise_http_error
 from dagster_cloud_cli.core.workspace import CodeDeploymentMetadata
-from typing_extensions import Self
+from typing_extensions import Self, TypeAlias
 
 from dagster_cloud.agent.queries import GET_AGENTS_QUERY
 from dagster_cloud.api.dagster_cloud_api import (
     DagsterCloudUploadLocationData,
     DagsterCloudUploadRepositoryData,
     DagsterCloudUploadWorkspaceEntry,
     DagsterCloudUploadWorkspaceResponse,
@@ -224,15 +224,16 @@
             "Whether the agent update process expects a liveness sentinel to be written before an"
             " agent is considered healthy. If using zero-downtime agent updates, this should be set"
             " to True."
         ),
     ),
 }
 
-DeploymentAndLocation = Tuple[str, str]
+DeploymentAndLocation: TypeAlias = Tuple[str, str]
+UserCodeLauncherEntryMap: TypeAlias = Dict[DeploymentAndLocation, UserCodeLauncherEntry]
 
 
 class ServerEndpoint(
     NamedTuple(
         "_ServerEndpoint",
         [
             ("host", str),
@@ -549,15 +550,22 @@
                     files={"workspace_entry.tmp": f},
                     timeout=self._instance.dagster_cloud_api_timeout,
                     proxies=self._instance.dagster_cloud_api_proxies,
                 )
                 raise_http_error(resp)
 
             response = deserialize_value(resp.text, DagsterCloudUploadWorkspaceResponse)
-            check.invariant(response.updated, "update failed after job snapshots uploaded")
+
+            if not response.updated:
+                # this condition is expected to be extremely unlikely
+                raise Exception(
+                    "Upload failed, job definitions changed while uploading:"
+                    f" {response.missing_job_snapshots}"
+                )
+
             self._logger.info(
                 "Workspace entry for"
                 f" {deployment_name}:{workspace_entry.location_name} {response.message}"
             )
 
     def _get_upload_location_data(
         self,
@@ -1747,15 +1755,15 @@
                     except Exception:
                         self._logger.exception("Failure fetching debug info after a timeout")
 
                 raise Exception(
                     f"Timed out after waiting {timeout}s for server"
                     f" {client.host}:{client.port or client.socket}."
                     + (f"\n\n{timeout_debug_info}" if timeout_debug_info else "")
-                    + f"\n\nMost recent connection error: {str(last_error)}"
+                    + f"\n\nMost recent connection error: {last_error}"
                 )
 
             time.sleep(1)
 
             if additional_check and (
                 not last_additional_check_time
                 or time.time() - last_additional_check_time > additional_check_interval
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster_cloud-1.4.0/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/PKG-INFO` & `dagster_cloud-1.4.0/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.3.9rc0
+Version: 1.4.0
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster_cloud-1.3.9rc0/dagster_cloud.egg-info/SOURCES.txt` & `dagster_cloud-1.4.0/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster_cloud-1.3.9rc0/setup.py` & `dagster_cloud-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,16 +36,16 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.3.9rc0",
-        "dagster-cloud-cli==1.3.9rc0",
+        "dagster==1.4.0",
+        "dagster-cloud-cli==1.4.0",
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
-            "dagster_k8s==0.19.9rc0",
+            "dagster_k8s==0.20.0",
         ],
-        "docker": ["docker", "dagster_docker==0.19.9rc0"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.19.9rc0"],
-        "ecs": ["dagster_aws==0.19.9rc0", "boto3"],
+        "docker": ["docker", "dagster_docker==0.20.0"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.20.0"],
+        "ecs": ["dagster_aws==0.20.0", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

