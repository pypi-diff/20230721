# Comparing `tmp/skypilot-nightly-1.0.0.dev20230719.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230719.tar", last modified: Wed Jul 19 10:41:02 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230720.tar", last modified: Thu Jul 20 10:41:06 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230719.tar` & `skypilot-nightly-1.0.0.dev20230720.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.627978 skypilot-nightly-1.0.0.dev20230719/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-19 10:41:02.627978 skypilot-nightly-1.0.0.dev20230719/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 10:41:02.627978 skypilot-nightly-1.0.0.dev20230719/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-19 10:40:55.000000 skypilot-nightly-1.0.0.dev20230719/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.603978 skypilot-nightly-1.0.0.dev20230719/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-19 10:40:55.000000 skypilot-nightly-1.0.0.dev20230719/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.603978 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.607978 skypilot-nightly-1.0.0.dev20230719/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   200418 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.607978 skypilot-nightly-1.0.0.dev20230719/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.607978 skypilot-nightly-1.0.0.dev20230719/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.607978 skypilot-nightly-1.0.0.dev20230719/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41169 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    45228 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.611979 skypilot-nightly-1.0.0.dev20230719/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-19 10:40:55.000000 skypilot-nightly-1.0.0.dev20230719/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.599979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.615979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.619979 skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.623978 skypilot-nightly-1.0.0.dev20230719/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.623978 skypilot-nightly-1.0.0.dev20230719/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.623978 skypilot-nightly-1.0.0.dev20230719/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.623978 skypilot-nightly-1.0.0.dev20230719/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/env_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.623978 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-19 10:41:02.000000 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-19 10:41:02.000000 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 10:41:02.000000 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-19 10:41:02.000000 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-19 10:41:02.000000 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-19 10:41:02.000000 skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 10:41:02.627978 skypilot-nightly-1.0.0.dev20230719/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   125880 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-19 10:40:51.000000 skypilot-nightly-1.0.0.dev20230719/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.303271 skypilot-nightly-1.0.0.dev20230720/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-20 10:41:06.303271 skypilot-nightly-1.0.0.dev20230720/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:41:06.303271 skypilot-nightly-1.0.0.dev20230720/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-20 10:40:55.000000 skypilot-nightly-1.0.0.dev20230720/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.263271 skypilot-nightly-1.0.0.dev20230720/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-20 10:40:55.000000 skypilot-nightly-1.0.0.dev20230720/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.267271 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15607 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.267271 skypilot-nightly-1.0.0.dev20230720/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112970 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   202208 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.267271 skypilot-nightly-1.0.0.dev20230720/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.271271 skypilot-nightly-1.0.0.dev20230720/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   167453 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.271271 skypilot-nightly-1.0.0.dev20230720/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41169 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25762 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46375 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20117 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24269 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14878 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.275271 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11679 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23188 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.275271 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20590 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.275271 skypilot-nightly-1.0.0.dev20230720/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89247 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.275271 skypilot-nightly-1.0.0.dev20230720/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.275271 skypilot-nightly-1.0.0.dev20230720/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.279271 skypilot-nightly-1.0.0.dev20230720/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42860 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.279271 skypilot-nightly-1.0.0.dev20230720/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-20 10:40:55.000000 skypilot-nightly-1.0.0.dev20230720/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.279271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8899 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.259271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.283271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.283271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52192 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.283271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.283271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34963 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.283271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.287271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8613 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.287271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.287271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.291271 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.291271 skypilot-nightly-1.0.0.dev20230720/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25102 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.291271 skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.291271 skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.291271 skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38424 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.295271 skypilot-nightly-1.0.0.dev20230720/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.295271 skypilot-nightly-1.0.0.dev20230720/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.295271 skypilot-nightly-1.0.0.dev20230720/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.299271 skypilot-nightly-1.0.0.dev20230720/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14891 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14688 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12077 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/env_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.299271 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-20 10:41:06.000000 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-07-20 10:41:06.000000 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:41:06.000000 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 10:41:06.000000 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-20 10:41:06.000000 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 10:41:06.000000 skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:41:06.299271 skypilot-nightly-1.0.0.dev20230720/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125880 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-20 10:40:47.000000 skypilot-nightly-1.0.0.dev20230720/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/LICENSE` & `skypilot-nightly-1.0.0.dev20230720/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230720/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230720/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230719
+Version: 1.0.0.dev20230720
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230719
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230720
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/README.md` & `skypilot-nightly-1.0.0.dev20230720/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230720/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/setup.py` & `skypilot-nightly-1.0.0.dev20230720/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230720/sky/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '9b07ffc27cf8462c26aa359c4bf053e7d25aedcf'
-__version__ = '1.0.0-dev20230719'
+__commit__ = 'c35a1cb901f8099ad1121f520cf74ba90ceae883'
+__version__ = '1.0.0-dev20230720'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230720/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230720/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/cloud_vm_ray_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,18 @@
 _TEARDOWN_PURGE_WARNING = (
     f'{colorama.Fore.YELLOW}'
     'WARNING: Received non-zero exit code from {reason}. '
     'Make sure resources are manually deleted.\n'
     'Details: {details}'
     f'{colorama.Style.RESET_ALL}')
 
+_RSYNC_NOT_FOUND_MESSAGE = (
+    '`rsync` command is not found in the specified image. '
+    'Please use an image with rsync installed.')
+
 _TPU_NOT_FOUND_ERROR = 'ERROR: (gcloud.compute.tpus.delete) NOT_FOUND'
 
 _CTRL_C_TIP_MESSAGE = ('INFO: Tip: use Ctrl-C to exit log streaming '
                        '(task will not be killed).')
 
 _MAX_RAY_UP_RETRY = 5
 
@@ -761,14 +765,17 @@
             if 'was not found' in stderr:
                 # Example: The resource
                 # 'projects/<id>/zones/zone/acceleratorTypes/nvidia-tesla-v100'
                 # was not found.
                 logger.warning(f'Got \'resource not found\' in {zone.name}.')
                 self._blocked_resources.add(
                     launchable_resources.copy(zone=zone.name))
+            elif 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             else:
                 logger.info('====== stdout ======')
                 for s in stdout.split('\n'):
                     print(s)
                 logger.info('====== stderr ======')
                 for s in splits:
                     print(s)
@@ -803,14 +810,17 @@
         #   --> it automatically succeeded in another zone
         #   --> failed in [4/7] Running initialization commands due to user cmd
         # In this case, we should error out.
         head_node_up = any(
             line.startswith('<1/1> Setting up head node')
             for line in stdout_splits + stderr_splits)
         if not errors or head_node_up:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             # TODO: Got transient 'Failed to create security group' that goes
             # away after a few minutes.  Should we auto retry other regions, or
             # let the user retry.
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
@@ -855,14 +865,17 @@
         errors = [
             s.strip()
             for s in stdout_splits + stderr_splits
             if ('Exception Details:' in s.strip() or 'InvalidTemplateDeployment'
                 in s.strip() or '(ReadOnlyDisabledSubscription)' in s.strip())
         ]
         if not errors:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
             for s in stderr_splits:
                 print(s)
             with ux_utils.print_exception_no_traceback():
@@ -888,14 +901,17 @@
         stderr_splits = stderr.split('\n')
         errors = [
             s.strip()
             for s in stdout_splits + stderr_splits
             if 'LambdaCloudError:' in s.strip()
         ]
         if not errors:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
             for s in stderr_splits:
                 print(s)
             with ux_utils.print_exception_no_traceback():
@@ -924,14 +940,17 @@
         stderr_splits = stderr.split('\n')
         errors = [
             s.strip()
             for s in stdout_splits + stderr_splits
             if 'SCPError:' in s.strip()
         ]
         if not errors:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
             for s in stderr_splits:
                 print(s)
             with ux_utils.print_exception_no_traceback():
@@ -961,14 +980,17 @@
         stderr_splits = stderr.split('\n')
         errors = [
             s.strip()
             for s in stdout_splits + stderr_splits
             if 'ERR' in s.strip() or 'PANIC' in s.strip()
         ]
         if not errors:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
             for s in stderr_splits:
                 print(s)
             with ux_utils.print_exception_no_traceback():
@@ -992,14 +1014,17 @@
         stderr_splits = stderr.split('\n')
         errors = [
             s.strip()
             for s in stdout_splits + stderr_splits
             if 'ERR' in s.strip() or 'PANIC' in s.strip()
         ]
         if not errors:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
             for s in stderr_splits:
                 print(s)
             with ux_utils.print_exception_no_traceback():
@@ -1027,14 +1052,17 @@
             if ('VcnSubnetNotFound' in s.strip()) or
             ('oci.exceptions.ServiceError' in s.strip() and
              ('NotAuthorizedOrNotFound' in s.strip() or 'CannotParseRequest' in
               s.strip() or 'InternalError' in s.strip() or
               'LimitExceeded' in s.strip() or 'NotAuthenticated' in s.strip()))
         ]
         if not errors:
+            if 'rsync: command not found' in stderr:
+                with ux_utils.print_exception_no_traceback():
+                    raise RuntimeError(_RSYNC_NOT_FOUND_MESSAGE)
             logger.info('====== stdout ======')
             for s in stdout_splits:
                 print(s)
             logger.info('====== stderr ======')
             for s in stderr_splits:
                 print(s)
             with ux_utils.print_exception_no_traceback():
@@ -1755,14 +1783,19 @@
                 if result is not None:
                     # Retry. Unlikely will succeed if it's due to no capacity.
                     logger.info(
                         'Retrying due to the possibly flaky RESOURCE_NOT_FOUND '
                         'error.')
                     return True
 
+            if 'rsync: command not found' in stderr:
+                logger.info('Skipping retry due to `rsync` not found in '
+                            'the specified image.')
+                return False
+
             if ('Processing file mounts' in stdout and
                     'Running setup commands' not in stdout and
                     'Failed to setup head node.' in stderr):
                 logger.info(
                     'Retrying runtime setup due to ssh connection issue.')
                 return True
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230720/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/check.py` & `skypilot-nightly-1.0.0.dev20230720/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230720/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230720/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/gcp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Google Cloud Platform."""
 import functools
 import json
 import os
+import re
 import subprocess
 import time
 import typing
 from typing import Dict, Iterator, List, Optional, Tuple
 
 from sky import clouds
 from sky import exceptions
@@ -266,16 +267,21 @@
             return 0.11 * num_gigabytes
         else:
             return 0.08 * num_gigabytes
 
     def is_same_cloud(self, other):
         return isinstance(other, GCP)
 
+    @classmethod
+    def _is_machine_image(cls, image_id: str) -> bool:
+        find_machine = re.match(r'projects/.*/.*/machineImages/.*', image_id)
+        return find_machine is not None
+
     def get_image_size(self, image_id: str, region: Optional[str]) -> float:
-        del region  # unused
+        del region  # Unused.
         if image_id.startswith('skypilot:'):
             return DEFAULT_GCP_IMAGE_GB
         try:
             compute = gcp.build('compute',
                                 'v1',
                                 credentials=None,
                                 cache_discovery=False)
@@ -283,17 +289,30 @@
             return DEFAULT_GCP_IMAGE_GB
         try:
             image_attrs = image_id.split('/')
             if len(image_attrs) == 1:
                 raise ValueError(f'Image {image_id!r} not found in GCP.')
             project = image_attrs[1]
             image_name = image_attrs[-1]
-            image_infos = compute.images().get(project=project,
-                                               image=image_name).execute()
-            return float(image_infos['diskSizeGb'])
+            # We support both GCP's Machine Images and Custom Images, both
+            # of which are specified with the image_id field. We will
+            # distinguish them by checking if the image_id contains
+            # 'machineImages'.
+            if self._is_machine_image(image_id):
+                image_infos = compute.machineImages().get(
+                    project=project, machineImage=image_name).execute()
+                # The VM launching in a different region than the machine
+                # image is supported by GCP, so we do not need to check the
+                # storageLocations.
+                return float(
+                    image_infos['instanceProperties']['disks'][0]['diskSizeGb'])
+            else:
+                image_infos = compute.images().get(project=project,
+                                                   image=image_name).execute()
+                return float(image_infos['diskSizeGb'])
         except gcp.http_error_exception() as e:
             if e.resp.status == 403:
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError('Not able to access the image '
                                      f'{image_id!r}') from None
             if e.resp.status == 404:
                 with ux_utils.print_exception_no_traceback():
@@ -388,14 +407,19 @@
                 image_id = resources.image_id[region_name]
         if image_id.startswith('skypilot:'):
             image_id = service_catalog.get_image_id_from_tag(image_id,
                                                              clouds='gcp')
 
         assert image_id is not None, (image_id, r)
         resources_vars['image_id'] = image_id
+        resources_vars['machine_image'] = None
+
+        if self._is_machine_image(image_id):
+            resources_vars['machine_image'] = image_id
+            resources_vars['image_id'] = None
 
         resources_vars['disk_tier'] = GCP._get_disk_type(r.disk_tier)
 
         return resources_vars
 
     def _get_feasible_launchable_resources(self, resources):
         if resources.instance_type is not None:
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230720/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/core.py` & `skypilot-nightly-1.0.0.dev20230720/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230720/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230720/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230720/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230720/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230720/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230720/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230720/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230720/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230720/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230720/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230720/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230720/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230720/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230720/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230720/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230720/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/task.py` & `skypilot-nightly-1.0.0.dev20230720/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/gcp-ray.yml.j2`

 * *Files 8% similar despite different names*

```diff
@@ -42,22 +42,27 @@
       runtimeVersion: {{runtime_version}}
   {%- if use_spot %}
       schedulingConfig:
         preemptible: true
   {%- endif %}
 {%- else %}
       machineType: {{instance_type}}
+    {%- if machine_image is not none %}
+      sourceMachineImage: {{machine_image}}
+    {%- endif %}
       disks:
         - boot: true
           autoDelete: true
           type: PERSISTENT
           initializeParams:
             diskSizeGb: {{disk_size}}
             # See https://cloud.google.com/deep-learning-vm/docs/images
+          {%- if machine_image is none %}
             sourceImage: {{image_id}}
+          {%- endif %}
             diskType: zones/{{zones}}/diskTypes/{{disk_tier}}
   {%- if gpu is not none %}
       guestAccelerators:
         - acceleratorType: projects/{{gcp_project_id}}/zones/{{zones}}/acceleratorTypes/{{gpu}}
           acceleratorCount: {{gpu_count}}
   {%- endif %}
       metadata:
@@ -92,22 +97,27 @@
       runtimeVersion: {{runtime_version}}
     {%- if use_spot %}
       schedulingConfig:
         preemptible: true
     {%- endif %}
   {%- else %}
       machineType: {{instance_type}}
+    {%- if machine_image is not none %}
+      sourceMachineImage: {{machine_image}}
+    {%- endif %}
       disks:
         - boot: true
           autoDelete: true
           type: PERSISTENT
           initializeParams:
             diskSizeGb: {{disk_size}}
             # See https://cloud.google.com/deep-learning-vm/docs/images
+          {%- if machine_image is none %}
             sourceImage: {{image_id}}
+          {%- endif %}
             diskType: zones/{{zones}}/diskTypes/{{disk_tier}}
     {%- if gpu is not none %}
       guestAccelerators:
         - acceleratorType: projects/{{gcp_project_id}}/zones/{{zones}}/acceleratorTypes/{{gpu}}
           acceleratorCount: {{gpu_count}}
     {%- endif %}
       metadata:
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230720/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230720/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230720/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230720/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230719
+Version: 1.0.0.dev20230720
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230719
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230720
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230720/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230719/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230720/tests/test_wheels.py`

 * *Files identical despite different names*

