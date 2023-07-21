# Comparing `tmp/fabric-orchestrator-client-1.6.0b1.tar.gz` & `tmp/fabric-orchestrator-client-1.6.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabric-orchestrator-client-1.6.0b1.tar", last modified: Thu Jul 20 17:44:15 2023, max compression
+gzip compressed data, was "fabric-orchestrator-client-1.6.0b3.tar", last modified: Fri Jul 21 15:32:48 2023, max compression
```

## Comparing `fabric-orchestrator-client-1.6.0b1.tar` & `fabric-orchestrator-client-1.6.0b3.tar`

### file list

```diff
@@ -1,101 +1,103 @@
--rw-r--r--   0        0        0      793 2023-07-20 16:57:55.683480 fabric-orchestrator-client-1.6.0b1/.gitignore
--rw-r--r--   0        0        0     1030 2023-07-20 16:57:55.683782 fabric-orchestrator-client-1.6.0b1/.swagger-codegen-ignore
--rw-r--r--   0        0        0        7 2023-07-20 17:37:23.319252 fabric-orchestrator-client-1.6.0b1/.swagger-codegen/VERSION
--rw-r--r--   0        0        0      349 2023-07-20 16:57:55.684203 fabric-orchestrator-client-1.6.0b1/.travis.yml
--rw-r--r--   0        0        0      770 2023-07-20 16:57:55.684315 fabric-orchestrator-client-1.6.0b1/CODEGEN.md
--rw-r--r--   0        0        0     1071 2023-07-20 16:57:55.684446 fabric-orchestrator-client-1.6.0b1/LICENSE
--rw-r--r--   0        0        0       59 2023-07-20 16:57:55.684550 fabric-orchestrator-client-1.6.0b1/MANIFEST.in
--rw-r--r--   0        0        0     9867 2023-07-20 16:57:55.684688 fabric-orchestrator-client-1.6.0b1/README.md
--rw-r--r--   0        0        0      340 2023-07-20 16:57:55.684865 fabric-orchestrator-client-1.6.0b1/docs/Poa.md
--rw-r--r--   0        0        0      557 2023-07-20 16:57:55.685023 fabric-orchestrator-client-1.6.0b1/docs/PoaData.md
--rw-r--r--   0        0        0      376 2023-07-20 16:57:55.685156 fabric-orchestrator-client-1.6.0b1/docs/PoaPost.md
--rw-r--r--   0        0        0      472 2023-07-20 17:37:29.102056 fabric-orchestrator-client-1.6.0b1/docs/PoaPostData.md
--rw-r--r--   0        0        0      369 2023-07-20 16:57:55.685376 fabric-orchestrator-client-1.6.0b1/docs/PoaPostDataVcpuCpuMap.md
--rw-r--r--   0        0        0     6404 2023-07-20 16:57:55.685514 fabric-orchestrator-client-1.6.0b1/docs/PoasApi.md
--rw-r--r--   0        0        0     4263 2023-07-20 16:57:55.685654 fabric-orchestrator-client-1.6.0b1/docs/ResourcesApi.md
--rw-r--r--   0        0        0    20667 2023-07-20 16:57:55.685813 fabric-orchestrator-client-1.6.0b1/docs/SlicesApi.md
--rw-r--r--   0        0        0     4102 2023-07-20 16:57:55.685958 fabric-orchestrator-client-1.6.0b1/docs/SliversApi.md
--rw-r--r--   0        0        0      335 2023-07-20 16:57:55.686145 fabric-orchestrator-client-1.6.0b1/docs/Success.md
--rw-r--r--   0        0        0      352 2023-07-20 16:57:55.686293 fabric-orchestrator-client-1.6.0b1/docs/Version.md
--rw-r--r--   0        0        0       24 2023-07-20 16:59:44.471092 fabric-orchestrator-client-1.6.0b1/fabric_cf/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:57:55.686541 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/__init__.py
--rw-r--r--   0        0        0    21942 2023-07-20 17:42:47.201620 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/orchestrator_proxy.py
--rw-r--r--   0        0        0     3557 2023-07-20 16:57:55.686919 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/__init__.py
--rw-r--r--   0        0        0      468 2023-07-20 16:57:55.687067 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/__init__.py
--rw-r--r--   0        0        0    13515 2023-07-20 16:57:55.687291 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py
--rw-r--r--   0        0        0     9597 2023-07-20 16:57:55.687498 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py
--rw-r--r--   0        0        0    43978 2023-07-20 16:57:55.687852 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py
--rw-r--r--   0        0        0     9260 2023-07-20 16:57:55.688058 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
--rw-r--r--   0        0        0     3748 2023-07-20 16:57:55.688305 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py
--rw-r--r--   0        0        0    25272 2023-07-20 16:57:55.688514 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api_client.py
--rw-r--r--   0        0        0     8240 2023-07-20 16:57:55.688681 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/configuration.py
--rw-r--r--   0        0        0     2978 2023-07-20 16:57:55.688830 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py
--rw-r--r--   0        0        0     3427 2023-07-20 16:57:55.689190 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py
--rw-r--r--   0        0        0     6654 2023-07-20 16:57:55.689400 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py
--rw-r--r--   0        0        0     4057 2023-07-20 17:39:40.282831 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py
--rw-r--r--   0        0        0     4469 2023-07-20 17:39:58.609765 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
--rw-r--r--   0        0        0     3648 2023-07-20 16:57:55.690053 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     3055 2023-07-20 16:57:55.690298 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py
--rw-r--r--   0        0        0     3420 2023-07-20 16:57:55.690573 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py
--rw-r--r--   0        0        0     8496 2023-07-20 16:57:55.690977 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py
--rw-r--r--   0        0        0     3444 2023-07-20 16:57:55.691422 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py
--rw-r--r--   0        0        0     3412 2023-07-20 16:57:55.691759 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py
--rw-r--r--   0        0        0     3951 2023-07-20 16:57:55.691993 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py
--rw-r--r--   0        0        0    10905 2023-07-20 16:57:55.692233 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py
--rw-r--r--   0        0        0     3422 2023-07-20 16:57:55.692488 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py
--rw-r--r--   0        0        0     4999 2023-07-20 16:57:55.692698 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
--rw-r--r--   0        0        0     3832 2023-07-20 16:57:55.692922 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
--rw-r--r--   0        0        0     6211 2023-07-20 16:57:55.693156 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
--rw-r--r--   0        0        0     4253 2023-07-20 16:57:55.693385 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
--rw-r--r--   0        0        0     3163 2023-07-20 16:57:55.693582 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
--rw-r--r--   0        0        0     5771 2023-07-20 16:57:55.693786 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
--rw-r--r--   0        0        0     5063 2023-07-20 16:57:55.693960 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
--rw-r--r--   0        0        0     3870 2023-07-20 16:57:55.694158 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
--rw-r--r--   0        0        0     4994 2023-07-20 16:57:55.694424 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
--rw-r--r--   0        0        0     3831 2023-07-20 16:57:55.694605 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
--rw-r--r--   0        0        0     4971 2023-07-20 16:57:55.694784 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
--rw-r--r--   0        0        0     3819 2023-07-20 16:57:55.695203 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
--rw-r--r--   0        0        0     5224 2023-07-20 16:57:55.695486 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
--rw-r--r--   0        0        0     3963 2023-07-20 16:57:55.695726 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
--rw-r--r--   0        0        0     3413 2023-07-20 16:57:55.695941 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version.py
--rw-r--r--   0        0        0     3882 2023-07-20 16:57:55.696224 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py
--rw-r--r--   0        0        0    12988 2023-07-20 16:57:55.696524 fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/rest.py
--rw-r--r--   0        0        0     1663 2023-07-20 16:57:55.696710 fabric-orchestrator-client-1.6.0b1/git_push.sh
--rw-r--r--   0        0        0     1024 2023-07-20 16:57:55.696907 fabric-orchestrator-client-1.6.0b1/pyproject.toml
--rw-r--r--   0        0        0       16 2023-07-20 16:57:55.697079 fabric-orchestrator-client-1.6.0b1/test/__init__.py
--rw-r--r--   0        0        0      809 2023-07-20 16:57:55.697378 fabric-orchestrator-client-1.6.0b1/test/test_poa.py
--rw-r--r--   0        0        0      843 2023-07-20 16:57:55.697602 fabric-orchestrator-client-1.6.0b1/test/test_poa_data.py
--rw-r--r--   0        0        0      843 2023-07-20 16:57:55.697806 fabric-orchestrator-client-1.6.0b1/test/test_poa_post.py
--rw-r--r--   0        0        0      877 2023-07-20 16:57:55.697996 fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data.py
--rw-r--r--   0        0        0      963 2023-07-20 16:57:55.698208 fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data_vcpu_cpu_map.py
--rw-r--r--   0        0        0     1157 2023-07-20 16:57:55.698367 fabric-orchestrator-client-1.6.0b1/test/test_poas_api.py
--rw-r--r--   0        0        0      896 2023-07-20 16:57:55.698574 fabric-orchestrator-client-1.6.0b1/test/test_resource.py
--rw-r--r--   0        0        0      950 2023-07-20 16:57:55.698746 fabric-orchestrator-client-1.6.0b1/test/test_resources.py
--rw-r--r--   0        0        0     1206 2023-07-20 16:57:55.698949 fabric-orchestrator-client-1.6.0b1/test/test_resources_api.py
--rw-r--r--   0        0        0      872 2023-07-20 16:57:55.699318 fabric-orchestrator-client-1.6.0b1/test/test_slice.py
--rw-r--r--   0        0        0      930 2023-07-20 16:57:55.699499 fabric-orchestrator-client-1.6.0b1/test/test_slice_details.py
--rw-r--r--   0        0        0      880 2023-07-20 16:57:55.699671 fabric-orchestrator-client-1.6.0b1/test/test_slices.py
--rw-r--r--   0        0        0     2165 2023-07-20 16:57:55.699921 fabric-orchestrator-client-1.6.0b1/test/test_slices_api.py
--rw-r--r--   0        0        0      867 2023-07-20 16:57:55.700175 fabric-orchestrator-client-1.6.0b1/test/test_slices_post.py
--rw-r--r--   0        0        0      880 2023-07-20 16:57:55.700441 fabric-orchestrator-client-1.6.0b1/test/test_sliver.py
--rw-r--r--   0        0        0      888 2023-07-20 16:57:55.700646 fabric-orchestrator-client-1.6.0b1/test/test_slivers.py
--rw-r--r--   0        0        0      974 2023-07-20 16:57:55.700829 fabric-orchestrator-client-1.6.0b1/test/test_slivers_api.py
--rw-r--r--   0        0        0      998 2023-07-20 16:57:55.701084 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content.py
--rw-r--r--   0        0        0     1032 2023-07-20 16:57:55.701316 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content_data.py
--rw-r--r--   0        0        0      996 2023-07-20 16:57:55.701511 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_paginated.py
--rw-r--r--   0        0        0      972 2023-07-20 16:57:55.701708 fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_single.py
--rw-r--r--   0        0        0      988 2023-07-20 16:57:55.701894 fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request.py
--rw-r--r--   0        0        0     1038 2023-07-20 16:57:55.702089 fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request_errors.py
--rw-r--r--   0        0        0     1002 2023-07-20 16:57:55.702264 fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized.py
--rw-r--r--   0        0        0     1052 2023-07-20 16:57:55.702486 fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized_errors.py
--rw-r--r--   0        0        0      978 2023-07-20 16:57:55.702815 fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden.py
--rw-r--r--   0        0        0     1028 2023-07-20 16:57:55.703064 fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden_errors.py
--rw-r--r--   0        0        0      972 2023-07-20 16:57:55.703225 fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found.py
--rw-r--r--   0        0        0     1022 2023-07-20 16:57:55.703377 fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found_errors.py
--rw-r--r--   0        0        0     1062 2023-07-20 16:57:55.703541 fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error.py
--rw-r--r--   0        0        0     1112 2023-07-20 16:57:55.703700 fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error_errors.py
--rw-r--r--   0        0        0      888 2023-07-20 16:57:55.703904 fabric-orchestrator-client-1.6.0b1/test/test_version.py
--rw-r--r--   0        0        0      814 2023-07-20 16:57:55.704109 fabric-orchestrator-client-1.6.0b1/test/test_version_api.py
--rw-r--r--   0        0        0      922 2023-07-20 16:57:55.704281 fabric-orchestrator-client-1.6.0b1/test/test_version_data.py
--rw-r--r--   0        0        0      143 2023-07-20 16:57:55.704477 fabric-orchestrator-client-1.6.0b1/tox.ini
--rw-r--r--   0        0        0    10818 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.6.0b1/PKG-INFO
+-rw-r--r--   0        0        0      793 2023-07-20 16:57:55.683480 fabric-orchestrator-client-1.6.0b3/.gitignore
+-rw-r--r--   0        0        0     1030 2023-07-20 16:57:55.683782 fabric-orchestrator-client-1.6.0b3/.swagger-codegen-ignore
+-rw-r--r--   0        0        0        7 2023-07-20 17:37:23.319252 fabric-orchestrator-client-1.6.0b3/.swagger-codegen/VERSION
+-rw-r--r--   0        0        0      349 2023-07-20 16:57:55.684203 fabric-orchestrator-client-1.6.0b3/.travis.yml
+-rw-r--r--   0        0        0      770 2023-07-20 16:57:55.684315 fabric-orchestrator-client-1.6.0b3/CODEGEN.md
+-rw-r--r--   0        0        0     1071 2023-07-20 16:57:55.684446 fabric-orchestrator-client-1.6.0b3/LICENSE
+-rw-r--r--   0        0        0       59 2023-07-20 16:57:55.684550 fabric-orchestrator-client-1.6.0b3/MANIFEST.in
+-rw-r--r--   0        0        0     9867 2023-07-20 16:57:55.684688 fabric-orchestrator-client-1.6.0b3/README.md
+-rw-r--r--   0        0        0      340 2023-07-20 16:57:55.684865 fabric-orchestrator-client-1.6.0b3/docs/Poa.md
+-rw-r--r--   0        0        0      557 2023-07-20 16:57:55.685023 fabric-orchestrator-client-1.6.0b3/docs/PoaData.md
+-rw-r--r--   0        0        0      376 2023-07-20 16:57:55.685156 fabric-orchestrator-client-1.6.0b3/docs/PoaPost.md
+-rw-r--r--   0        0        0      506 2023-07-20 21:47:25.455843 fabric-orchestrator-client-1.6.0b3/docs/PoaPostData.md
+-rw-r--r--   0        0        0      344 2023-07-21 13:07:46.502345 fabric-orchestrator-client-1.6.0b3/docs/PoaPostDataKeys.md
+-rw-r--r--   0        0        0      347 2023-07-21 13:07:52.137176 fabric-orchestrator-client-1.6.0b3/docs/PoaPostDataVcpuCpuMap.md
+-rw-r--r--   0        0        0     6404 2023-07-20 16:57:55.685514 fabric-orchestrator-client-1.6.0b3/docs/PoasApi.md
+-rw-r--r--   0        0        0     4263 2023-07-20 16:57:55.685654 fabric-orchestrator-client-1.6.0b3/docs/ResourcesApi.md
+-rw-r--r--   0        0        0    20667 2023-07-20 16:57:55.685813 fabric-orchestrator-client-1.6.0b3/docs/SlicesApi.md
+-rw-r--r--   0        0        0     4102 2023-07-20 16:57:55.685958 fabric-orchestrator-client-1.6.0b3/docs/SliversApi.md
+-rw-r--r--   0        0        0      335 2023-07-20 16:57:55.686145 fabric-orchestrator-client-1.6.0b3/docs/Success.md
+-rw-r--r--   0        0        0      352 2023-07-20 16:57:55.686293 fabric-orchestrator-client-1.6.0b3/docs/Version.md
+-rw-r--r--   0        0        0       24 2023-07-21 15:32:11.829230 fabric-orchestrator-client-1.6.0b3/fabric_cf/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:57:55.686541 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/__init__.py
+-rw-r--r--   0        0        0    21973 2023-07-21 15:24:31.642327 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/orchestrator_proxy.py
+-rw-r--r--   0        0        0     3649 2023-07-20 21:45:34.710418 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/__init__.py
+-rw-r--r--   0        0        0      468 2023-07-20 16:57:55.687067 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/__init__.py
+-rw-r--r--   0        0        0    13557 2023-07-20 21:46:03.451740 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/poas_api.py
+-rw-r--r--   0        0        0     9597 2023-07-20 16:57:55.687498 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/resources_api.py
+-rw-r--r--   0        0        0    43978 2023-07-20 16:57:55.687852 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/slices_api.py
+-rw-r--r--   0        0        0     9260 2023-07-20 16:57:55.688058 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/slivers_api.py
+-rw-r--r--   0        0        0     3748 2023-07-20 16:57:55.688305 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/version_api.py
+-rw-r--r--   0        0        0    25272 2023-07-20 16:57:55.688514 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api_client.py
+-rw-r--r--   0        0        0     8240 2023-07-20 16:57:55.688681 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/configuration.py
+-rw-r--r--   0        0        0     2978 2023-07-20 16:57:55.688830 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/__init__.py
+-rw-r--r--   0        0        0     3427 2023-07-20 16:57:55.689190 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa.py
+-rw-r--r--   0        0        0     6654 2023-07-20 16:57:55.689400 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_data.py
+-rw-r--r--   0        0        0     4057 2023-07-20 17:39:40.282831 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post.py
+-rw-r--r--   0        0        0     4505 2023-07-20 21:44:44.132981 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py
+-rw-r--r--   0        0        0     3804 2023-07-21 13:12:45.305374 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_keys.py
+-rw-r--r--   0        0        0     3813 2023-07-21 13:12:52.745327 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     3055 2023-07-20 16:57:55.690298 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/resource.py
+-rw-r--r--   0        0        0     3420 2023-07-20 16:57:55.690573 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/resources.py
+-rw-r--r--   0        0        0     8496 2023-07-20 16:57:55.690977 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slice.py
+-rw-r--r--   0        0        0     3444 2023-07-20 16:57:55.691422 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slice_details.py
+-rw-r--r--   0        0        0     3412 2023-07-20 16:57:55.691759 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slices.py
+-rw-r--r--   0        0        0     3951 2023-07-20 16:57:55.691993 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slices_post.py
+-rw-r--r--   0        0        0    10905 2023-07-20 16:57:55.692233 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/sliver.py
+-rw-r--r--   0        0        0     3422 2023-07-20 16:57:55.692488 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slivers.py
+-rw-r--r--   0        0        0     4999 2023-07-20 16:57:55.692698 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py
+-rw-r--r--   0        0        0     3832 2023-07-20 16:57:55.692922 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py
+-rw-r--r--   0        0        0     6211 2023-07-20 16:57:55.693156 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py
+-rw-r--r--   0        0        0     4253 2023-07-20 16:57:55.693385 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py
+-rw-r--r--   0        0        0     3163 2023-07-20 16:57:55.693582 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py
+-rw-r--r--   0        0        0     5771 2023-07-20 16:57:55.693786 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py
+-rw-r--r--   0        0        0     5063 2023-07-20 16:57:55.693960 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py
+-rw-r--r--   0        0        0     3870 2023-07-20 16:57:55.694158 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py
+-rw-r--r--   0        0        0     4994 2023-07-20 16:57:55.694424 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py
+-rw-r--r--   0        0        0     3831 2023-07-20 16:57:55.694605 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py
+-rw-r--r--   0        0        0     4971 2023-07-20 16:57:55.694784 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py
+-rw-r--r--   0        0        0     3819 2023-07-20 16:57:55.695203 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py
+-rw-r--r--   0        0        0     5224 2023-07-20 16:57:55.695486 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py
+-rw-r--r--   0        0        0     3963 2023-07-20 16:57:55.695726 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0     3413 2023-07-20 16:57:55.695941 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/version.py
+-rw-r--r--   0        0        0     3882 2023-07-20 16:57:55.696224 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/version_data.py
+-rw-r--r--   0        0        0    12988 2023-07-20 16:57:55.696524 fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/rest.py
+-rw-r--r--   0        0        0     1663 2023-07-20 16:57:55.696710 fabric-orchestrator-client-1.6.0b3/git_push.sh
+-rw-r--r--   0        0        0     1024 2023-07-20 16:57:55.696907 fabric-orchestrator-client-1.6.0b3/pyproject.toml
+-rw-r--r--   0        0        0       16 2023-07-20 16:57:55.697079 fabric-orchestrator-client-1.6.0b3/test/__init__.py
+-rw-r--r--   0        0        0      809 2023-07-20 16:57:55.697378 fabric-orchestrator-client-1.6.0b3/test/test_poa.py
+-rw-r--r--   0        0        0      843 2023-07-20 16:57:55.697602 fabric-orchestrator-client-1.6.0b3/test/test_poa_data.py
+-rw-r--r--   0        0        0      843 2023-07-20 16:57:55.697806 fabric-orchestrator-client-1.6.0b3/test/test_poa_post.py
+-rw-r--r--   0        0        0      877 2023-07-20 16:57:55.697996 fabric-orchestrator-client-1.6.0b3/test/test_poa_post_data.py
+-rw-r--r--   0        0        0      963 2023-07-20 16:57:55.698208 fabric-orchestrator-client-1.6.0b3/test/test_poa_post_data_vcpu_cpu_map.py
+-rw-r--r--   0        0        0     1157 2023-07-20 16:57:55.698367 fabric-orchestrator-client-1.6.0b3/test/test_poas_api.py
+-rw-r--r--   0        0        0      896 2023-07-20 16:57:55.698574 fabric-orchestrator-client-1.6.0b3/test/test_resource.py
+-rw-r--r--   0        0        0      950 2023-07-20 16:57:55.698746 fabric-orchestrator-client-1.6.0b3/test/test_resources.py
+-rw-r--r--   0        0        0     1206 2023-07-20 16:57:55.698949 fabric-orchestrator-client-1.6.0b3/test/test_resources_api.py
+-rw-r--r--   0        0        0      872 2023-07-20 16:57:55.699318 fabric-orchestrator-client-1.6.0b3/test/test_slice.py
+-rw-r--r--   0        0        0      930 2023-07-20 16:57:55.699499 fabric-orchestrator-client-1.6.0b3/test/test_slice_details.py
+-rw-r--r--   0        0        0      880 2023-07-20 16:57:55.699671 fabric-orchestrator-client-1.6.0b3/test/test_slices.py
+-rw-r--r--   0        0        0     2165 2023-07-20 16:57:55.699921 fabric-orchestrator-client-1.6.0b3/test/test_slices_api.py
+-rw-r--r--   0        0        0      867 2023-07-20 16:57:55.700175 fabric-orchestrator-client-1.6.0b3/test/test_slices_post.py
+-rw-r--r--   0        0        0      880 2023-07-20 16:57:55.700441 fabric-orchestrator-client-1.6.0b3/test/test_sliver.py
+-rw-r--r--   0        0        0      888 2023-07-20 16:57:55.700646 fabric-orchestrator-client-1.6.0b3/test/test_slivers.py
+-rw-r--r--   0        0        0      974 2023-07-20 16:57:55.700829 fabric-orchestrator-client-1.6.0b3/test/test_slivers_api.py
+-rw-r--r--   0        0        0      998 2023-07-20 16:57:55.701084 fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_no_content.py
+-rw-r--r--   0        0        0     1032 2023-07-20 16:57:55.701316 fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_no_content_data.py
+-rw-r--r--   0        0        0      996 2023-07-20 16:57:55.701511 fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_paginated.py
+-rw-r--r--   0        0        0      972 2023-07-20 16:57:55.701708 fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_single.py
+-rw-r--r--   0        0        0      988 2023-07-20 16:57:55.701894 fabric-orchestrator-client-1.6.0b3/test/test_status400_bad_request.py
+-rw-r--r--   0        0        0     1038 2023-07-20 16:57:55.702089 fabric-orchestrator-client-1.6.0b3/test/test_status400_bad_request_errors.py
+-rw-r--r--   0        0        0     1002 2023-07-20 16:57:55.702264 fabric-orchestrator-client-1.6.0b3/test/test_status401_unauthorized.py
+-rw-r--r--   0        0        0     1052 2023-07-20 16:57:55.702486 fabric-orchestrator-client-1.6.0b3/test/test_status401_unauthorized_errors.py
+-rw-r--r--   0        0        0      978 2023-07-20 16:57:55.702815 fabric-orchestrator-client-1.6.0b3/test/test_status403_forbidden.py
+-rw-r--r--   0        0        0     1028 2023-07-20 16:57:55.703064 fabric-orchestrator-client-1.6.0b3/test/test_status403_forbidden_errors.py
+-rw-r--r--   0        0        0      972 2023-07-20 16:57:55.703225 fabric-orchestrator-client-1.6.0b3/test/test_status404_not_found.py
+-rw-r--r--   0        0        0     1022 2023-07-20 16:57:55.703377 fabric-orchestrator-client-1.6.0b3/test/test_status404_not_found_errors.py
+-rw-r--r--   0        0        0     1062 2023-07-20 16:57:55.703541 fabric-orchestrator-client-1.6.0b3/test/test_status500_internal_server_error.py
+-rw-r--r--   0        0        0     1112 2023-07-20 16:57:55.703700 fabric-orchestrator-client-1.6.0b3/test/test_status500_internal_server_error_errors.py
+-rw-r--r--   0        0        0      888 2023-07-20 16:57:55.703904 fabric-orchestrator-client-1.6.0b3/test/test_version.py
+-rw-r--r--   0        0        0      814 2023-07-20 16:57:55.704109 fabric-orchestrator-client-1.6.0b3/test/test_version_api.py
+-rw-r--r--   0        0        0      922 2023-07-20 16:57:55.704281 fabric-orchestrator-client-1.6.0b3/test/test_version_data.py
+-rw-r--r--   0        0        0      143 2023-07-20 16:57:55.704477 fabric-orchestrator-client-1.6.0b3/tox.ini
+-rw-r--r--   0        0        0    10818 1970-01-01 00:00:00.000000 fabric-orchestrator-client-1.6.0b3/PKG-INFO
```

### Comparing `fabric-orchestrator-client-1.6.0b1/.gitignore` & `fabric-orchestrator-client-1.6.0b3/.gitignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/.swagger-codegen-ignore` & `fabric-orchestrator-client-1.6.0b3/.swagger-codegen-ignore`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/CODEGEN.md` & `fabric-orchestrator-client-1.6.0b3/CODEGEN.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/LICENSE` & `fabric-orchestrator-client-1.6.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/README.md` & `fabric-orchestrator-client-1.6.0b3/README.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/docs/PoaData.md` & `fabric-orchestrator-client-1.6.0b3/docs/PoaData.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/docs/PoasApi.md` & `fabric-orchestrator-client-1.6.0b3/docs/PoasApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/docs/ResourcesApi.md` & `fabric-orchestrator-client-1.6.0b3/docs/ResourcesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/docs/SlicesApi.md` & `fabric-orchestrator-client-1.6.0b3/docs/SlicesApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/docs/SliversApi.md` & `fabric-orchestrator-client-1.6.0b3/docs/SliversApi.md`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/orchestrator_proxy.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/orchestrator_proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
             self.slices_api.slices_renew_slice_id_post(slice_id=slice_id, lease_end_time=new_lease_end_time)
 
             return Status.OK, None
         except Exception as e:
             return Status.FAILURE, e
 
     def poa(self, *, token: str, sliver_id: str, operation: str, vcpu_cpu_map: List[Dict[str, str]] = None,
-            node_set: List[str] = None, keys: List[str]) -> Tuple[Status, Union[Exception, List[PoaData]]]:
+            node_set: List[str] = None, keys: List[Dict[str, str]]) -> Tuple[Status, Union[Exception, List[PoaData]]]:
         """
         Modify a slice
         @param token fabric token
         @param sliver_id Sliver Id
         @param operation POA operation
         @param vcpu_cpu_map vCPU to physical CPU Map
         @param node_set List of Numa nodes
@@ -486,15 +486,15 @@
                    OrchestratorProxyException(f"Sliver Id {sliver_id} must be specified")
 
         try:
             # Set the tokens
             self.__set_tokens(token=token)
 
             body = PoaPost(operation=operation)
-            if vcpu_cpu_map is not None or node_set is not None:
+            if vcpu_cpu_map is not None or node_set is not None or keys is not None:
                 post_data = PoaPostData()
                 post_data.vcpu_cpu_map = vcpu_cpu_map
                 post_data.node_set = node_set
                 post_data.keys = keys
                 body.data = post_data
 
             poa_data = self.poas_api.poas_create_sliver_id_post(sliver_id=sliver_id, body=body)
```

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/__init__.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from fabric_cf.orchestrator.swagger_client.api_client import ApiClient
 from fabric_cf.orchestrator.swagger_client.configuration import Configuration
 # import models into sdk package
 from fabric_cf.orchestrator.swagger_client.models.poa import Poa
 from fabric_cf.orchestrator.swagger_client.models.poa_data import PoaData
 from fabric_cf.orchestrator.swagger_client.models.poa_post import PoaPost
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data import PoaPostData
+from fabric_cf.orchestrator.swagger_client.models.poa_post_data_keys import PoaPostDataKeys
 from fabric_cf.orchestrator.swagger_client.models.poa_post_data_vcpu_cpu_map import PoaPostDataVcpuCpuMap
 from fabric_cf.orchestrator.swagger_client.models.resource import Resource
 from fabric_cf.orchestrator.swagger_client.models.resources import Resources
 from fabric_cf.orchestrator.swagger_client.models.slice import Slice
 from fabric_cf.orchestrator.swagger_client.models.slice_details import SliceDetails
 from fabric_cf.orchestrator.swagger_client.models.slices import Slices
 from fabric_cf.orchestrator.swagger_client.models.slices_post import SlicesPost
```

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/poas_api.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/poas_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         if api_client is None:
             api_client = ApiClient()
         self.api_client = api_client
 
     def poas_create_sliver_id_post(self, body, sliver_id, **kwargs):  # noqa: E501
         """Perform an operational action on a sliver.  # noqa: E501
 
-        Request to perform an operation action on a sliver. Supported actions include - reboot a VM sliver, get cpu info, get numa info, pin vCPUs, pin memory to a numa node etc.     # noqa: E501
+        Request to perform an operation action on a sliver. Supported actions include - reboot a VM sliver, get cpu info, get numa info, pin vCPUs, pin memory to a numa node etc, add/remove ssh keys.     # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.poas_create_sliver_id_post(body, sliver_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param PoaPost body: Perform Operation Action (required)
@@ -54,15 +54,15 @@
         else:
             (data) = self.poas_create_sliver_id_post_with_http_info(body, sliver_id, **kwargs)  # noqa: E501
             return data
 
     def poas_create_sliver_id_post_with_http_info(self, body, sliver_id, **kwargs):  # noqa: E501
         """Perform an operational action on a sliver.  # noqa: E501
 
-        Request to perform an operation action on a sliver. Supported actions include - reboot a VM sliver, get cpu info, get numa info, pin vCPUs, pin memory to a numa node etc.     # noqa: E501
+        Request to perform an operation action on a sliver. Supported actions include - reboot a VM sliver, get cpu info, get numa info, pin vCPUs, pin memory to a numa node etc, add/remove ssh keys.     # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.poas_create_sliver_id_post_with_http_info(body, sliver_id, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param PoaPost body: Perform Operation Action (required)
```

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/resources_api.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slices_api.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/slivers_api.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api/version_api.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api/version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/api_client.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/configuration.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/__init__.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_data.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'vcpu_cpu_map': 'list[PoaPostDataVcpuCpuMap]',
         'node_set': 'list[str]',
-        'keys': 'list[str]'
+        'keys': 'list[PoaPostDataKeys]'
     }
 
     attribute_map = {
         'vcpu_cpu_map': 'vcpu_cpu_map',
         'node_set': 'node_set',
         'keys': 'keys'
     }
@@ -96,25 +96,25 @@
 
     @property
     def keys(self):
         """Gets the keys of this PoaPostData.  # noqa: E501
 
 
         :return: The keys of this PoaPostData.  # noqa: E501
-        :rtype: list[str]
+        :rtype: list[PoaPostDataKeys]
         """
         return self._keys
 
     @keys.setter
     def keys(self, keys):
         """Sets the keys of this PoaPostData.
 
 
         :param keys: The keys of this PoaPostData.  # noqa: E501
-        :type: list[str]
+        :type: list[PoaPostDataKeys]
         """
 
         self._keys = keys
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/poa_post_data_vcpu_cpu_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,18 +38,16 @@
     }
 
     def __init__(self, vcpu=None, cpu=None):  # noqa: E501
         """PoaPostDataVcpuCpuMap - a model defined in Swagger"""  # noqa: E501
         self._vcpu = None
         self._cpu = None
         self.discriminator = None
-        if vcpu is not None:
-            self.vcpu = vcpu
-        if cpu is not None:
-            self.cpu = cpu
+        self.vcpu = vcpu
+        self.cpu = cpu
 
     @property
     def vcpu(self):
         """Gets the vcpu of this PoaPostDataVcpuCpuMap.  # noqa: E501
 
 
         :return: The vcpu of this PoaPostDataVcpuCpuMap.  # noqa: E501
@@ -61,14 +59,16 @@
     def vcpu(self, vcpu):
         """Sets the vcpu of this PoaPostDataVcpuCpuMap.
 
 
         :param vcpu: The vcpu of this PoaPostDataVcpuCpuMap.  # noqa: E501
         :type: str
         """
+        if vcpu is None:
+            raise ValueError("Invalid value for `vcpu`, must not be `None`")  # noqa: E501
 
         self._vcpu = vcpu
 
     @property
     def cpu(self):
         """Gets the cpu of this PoaPostDataVcpuCpuMap.  # noqa: E501
 
@@ -82,14 +82,16 @@
     def cpu(self, cpu):
         """Sets the cpu of this PoaPostDataVcpuCpuMap.
 
 
         :param cpu: The cpu of this PoaPostDataVcpuCpuMap.  # noqa: E501
         :type: str
         """
+        if cpu is None:
+            raise ValueError("Invalid value for `cpu`, must not be `None`")  # noqa: E501
 
         self._cpu = cpu
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resource.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/resources.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slice_details.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slices_post.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/sliver.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/slivers.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/models/version_data.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/models/version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/fabric_cf/orchestrator/swagger_client/rest.py` & `fabric-orchestrator-client-1.6.0b3/fabric_cf/orchestrator/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/git_push.sh` & `fabric-orchestrator-client-1.6.0b3/git_push.sh`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/pyproject.toml` & `fabric-orchestrator-client-1.6.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_poa.py` & `fabric-orchestrator-client-1.6.0b3/test/test_poa.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_poa_data.py` & `fabric-orchestrator-client-1.6.0b3/test/test_poa_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_poa_post.py` & `fabric-orchestrator-client-1.6.0b3/test/test_poa_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data.py` & `fabric-orchestrator-client-1.6.0b3/test/test_poa_post_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_poa_post_data_vcpu_cpu_map.py` & `fabric-orchestrator-client-1.6.0b3/test/test_poa_post_data_vcpu_cpu_map.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_poas_api.py` & `fabric-orchestrator-client-1.6.0b3/test/test_poas_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_resource.py` & `fabric-orchestrator-client-1.6.0b3/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_resources.py` & `fabric-orchestrator-client-1.6.0b3/test/test_resources.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_resources_api.py` & `fabric-orchestrator-client-1.6.0b3/test/test_resources_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slice.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slice.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slice_details.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slice_details.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slices.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slices.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slices_api.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slices_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slices_post.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slices_post.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_sliver.py` & `fabric-orchestrator-client-1.6.0b3/test/test_sliver.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slivers.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slivers.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_slivers_api.py` & `fabric-orchestrator-client-1.6.0b3/test/test_slivers_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_no_content.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_no_content_data.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_no_content_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_paginated.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_paginated.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status200_ok_single.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status200_ok_single.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status400_bad_request.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status400_bad_request_errors.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status400_bad_request_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status401_unauthorized.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status401_unauthorized_errors.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status401_unauthorized_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status403_forbidden.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status403_forbidden_errors.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status403_forbidden_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status404_not_found.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status404_not_found_errors.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status404_not_found_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status500_internal_server_error.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_status500_internal_server_error_errors.py` & `fabric-orchestrator-client-1.6.0b3/test/test_status500_internal_server_error_errors.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_version.py` & `fabric-orchestrator-client-1.6.0b3/test/test_version.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_version_api.py` & `fabric-orchestrator-client-1.6.0b3/test/test_version_api.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/test/test_version_data.py` & `fabric-orchestrator-client-1.6.0b3/test/test_version_data.py`

 * *Files identical despite different names*

### Comparing `fabric-orchestrator-client-1.6.0b1/PKG-INFO` & `fabric-orchestrator-client-1.6.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabric-orchestrator-client
-Version: 1.6.0b1
+Version: 1.6.0b3
 Summary: Fabric Orchestrator API
 Keywords: Swagger,Fabric Orchestrator API
 Author-email: Komal Thareja <kthare10@renci.org>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

