# Comparing `tmp/modelaapi-0.6.225.tar.gz` & `tmp/modelaapi-0.6.230.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.225.tar", last modified: Tue Jul 11 21:59:27 2023, max compression
+gzip compressed data, was "modelaapi-0.6.230.tar", last modified: Fri Jul 21 17:45:08 2023, max compression
```

## Comparing `modelaapi-0.6.225.tar` & `modelaapi-0.6.230.tar`

### file list

```diff
@@ -1,481 +1,481 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.869420 modelaapi-0.6.225/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.225/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.225/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.225/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.225/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.225/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.225/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.225/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-11 21:59:27.869420 modelaapi-0.6.225/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.225/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23368 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22698 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.841406 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    56885 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.845408 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.849410 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18564 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.853412 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.857414 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.861416 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-11 21:58:24.000000 modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-11 21:58:24.000000 modelaapi-0.6.225/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-11 21:58:24.000000 modelaapi-0.6.225/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-11 21:58:24.000000 modelaapi-0.6.225/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.865418 modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-11 21:58:24.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.869420 modelaapi-0.6.225/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.225/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.225/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.225/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.225/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.225/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-11 21:59:25.000000 modelaapi-0.6.225/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-11 21:59:27.869420 modelaapi-0.6.225/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-11 21:59:27.000000 modelaapi-0.6.225/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-11 21:59:27.000000 modelaapi-0.6.225/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-11 21:59:27.000000 modelaapi-0.6.225/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-11 21:59:27.000000 modelaapi-0.6.225/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.225/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-11 21:59:27.000000 modelaapi-0.6.225/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-11 21:59:27.000000 modelaapi-0.6.225/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.225/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-11 21:59:27.869420 modelaapi-0.6.225/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.225/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.487496 modelaapi-0.6.230/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.230/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.230/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.230/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.230/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.230/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.230/MANIFEST.in
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.230/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-21 17:45:08.487496 modelaapi-0.6.230/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.230/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24619 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    56768 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/api/apps/v1/generated_pb2.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.487496 modelaapi-0.6.230/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-21 17:44:56.000000 modelaapi-0.6.230/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.487496 modelaapi-0.6.230/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.230/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.230/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-21 17:45:08.487496 modelaapi-0.6.230/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.230/setup.py
```

### Comparing `modelaapi-0.6.225/CONTRIBUTING.rst` & `modelaapi-0.6.230/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/LICENSE.txt` & `modelaapi-0.6.230/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/Makefile` & `modelaapi-0.6.230/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/PKG-INFO` & `modelaapi-0.6.230/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.225
+Version: 0.6.230
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.225
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.230
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.225
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.230
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.225/README.md` & `modelaapi-0.6.230/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.api.resource import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_api_dot_resource_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xae\x01\n\nAccessSpec\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08nodePort\x18\x02 \x01(\x05\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x12\n\naccessType\x18\x04 \x01(\t\x12\x0c\n\x04http\x18\x05 \x01(\x08\x12\x12\n\nauthMethod\x18\x06 \x01(\t\x12<\n\x0f\x61pikeySecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\"b\n\x12\x41\x63\x63ountPermissions\x12\x13\n\x0b\x61\x63\x63ountName\x18\x01 \x01(\t\x12\x37\n\x05roles\x18\x02 \x03(\x0b\x32(.k8s.io.api.core.v1.LocalObjectReference\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc0\x01\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05tasks\x18\x04 \x03(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12W\n\x06ranges\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\"K\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xc5\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x12\n\ndataFilter\x18\x16 \x01(\t\x12\x15\n\rreferenceType\x18\x17 \x01(\t\x12\x0f\n\x07periods\x18\x18 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"0\n\x0c\x46ileLocation\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"\xaf\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"q\n\x04Logs\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\x9a\x02\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08taskType\x18\n \x01(\t\x12\x11\n\talgorithm\x18\x0b \x01(\t\"\xc5\x01\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0f\n\x07traffic\x18\x03 \x01(\x05\x12\x0c\n\x04role\x18\x04 \x01(\t\x12\x11\n\timageName\x18\x05 \x01(\t\x12\x37\n\napprovedBy\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xd1\x01\n\x10NotificationSpec\x12\x0b\n\x03ttl\x18\x01 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x02 \x01(\t\x12i\n\x08selector\x18\x03 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\rObjectiveSpec\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0c\n\x04goal\x18\x02 \x01(\t\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x93\x02\n\x0eParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0c\n\x04step\x18\x05 \x01(\x05\x12\x0b\n\x03log\x18\x06 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x07 \x03(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\x01\x12\x15\n\rdefaultChoice\x18\t \x01(\t\x12\x13\n\x0b\x63onditional\x18\n \x01(\x08\x12\x0e\n\x06parent\x18\x0b \x01(\t\x12\x16\n\x0eparentValueCat\x18\x0c \x01(\t\x12\x1a\n\x12parentValueInteger\x18\r \x01(\x05\x12\x18\n\x10parentValueFloat\x18\x0e \x01(\x01\"p\n\x0fPermissionsSpec\x12]\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccountPermissions\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"?\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x04\x12\x0e\n\x06memory\x18\x02 \x01(\x04\x12\x0b\n\x03gpu\x18\x03 \x01(\x04\"t\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12>\n\x0crequirements\x18\x03 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\xcd\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rmaxRetryCount\x18\x04 \x01(\x05\x12\x15\n\rretryDelaySec\x18\x05 \x01(\x05\x12\x12\n\ntimeoutSec\x18\x06 \x01(\x05\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12=\n\tnextRunAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xfe\x01\n\x11RunScheduleStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12R\n\x0blastRunLogs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x12\n\nretryCount\x18\x06 \x01(\x05\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc7\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"G\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x12\x37github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/api/resource/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\xae\x01\n\nAccessSpec\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08nodePort\x18\x02 \x01(\x05\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x12\n\naccessType\x18\x04 \x01(\t\x12\x0c\n\x04http\x18\x05 \x01(\x08\x12\x12\n\nauthMethod\x18\x06 \x01(\t\x12<\n\x0f\x61pikeySecretRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.SecretReference\"b\n\x12\x41\x63\x63ountPermissions\x12\x13\n\x0b\x61\x63\x63ountName\x18\x01 \x01(\t\x12\x37\n\x05roles\x18\x02 \x03(\x0b\x32(.k8s.io.api.core.v1.LocalObjectReference\"\xa5\x01\n\tAlgorithm\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AlgorithmSpec\"\xa4\x01\n\rAlgorithmList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Algorithm\"\xc0\x01\n\rAlgorithmSpec\x12\x15\n\rframeworkName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\r\n\x05tasks\x18\x04 \x03(\t\x12\x0e\n\x06sparse\x18\x05 \x01(\x08\x12W\n\x06ranges\x18\x06 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\xf3\x01\n\x05\x43loud\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12P\n\x04spec\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudSpec\x12T\n\x06status\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CloudStatus\"\x9c\x01\n\tCloudList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12M\n\x05items\x18\x02 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Cloud\"\xec\x02\n\tCloudSpec\x12\x19\n\x11\x64\x65\x66\x61ultRegionName\x18\x01 \x01(\t\x12\x1f\n\x17\x64\x65\x66\x61ultMachineClassName\x18\x02 \x01(\t\x12\x1b\n\x13\x64\x65\x66\x61ultGpuClassName\x18\x03 \x01(\t\x12]\n\x0emachineClasses\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClass\x12U\n\ngpuClasses\x18\x05 \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClass\x12P\n\x07regions\x18\x06 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Region\"\xc7\x01\n\x0b\x43loudStatus\x12_\n\x0cmachineCosts\x18\x01 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MachineClassCost\x12W\n\x08gpuCosts\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.GpuClassCost\"A\n\x0c\x43ompilerSpec\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12\x10\n\x08\x63ompiler\x18\x02 \x01(\t\x12\x0f\n\x07targets\x18\x03 \x03(\t\"l\n\x0f\x43onfusionMatrix\x12Y\n\x04rows\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrixRow\"F\n\x12\x43onfusionMatrixRow\x12\t\n\x01t\x18\x01 \x01(\t\x12\t\n\x01p\x18\x02 \x01(\t\x12\r\n\x05\x63ount\x18\x03 \x01(\x05\x12\x0b\n\x03pct\x18\x04 \x01(\x01\"K\n\x0c\x43ontainerLog\x12\x0b\n\x03job\x18\x01 \x01(\t\x12\x11\n\tcontainer\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x0e\n\x06\x62ucket\x18\x04 \x01(\t\"O\n\x0c\x43ronSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x12\n\nmaxRecords\x18\x04 \x01(\x05\"\"\n\nCurvePoint\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"(\n\nDataCenter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\"\xda\x01\n\x0c\x44\x61taLocation\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x16\n\x0e\x63onnectionName\x18\x02 \x01(\t\x12\x12\n\nbucketName\x18\x03 \x01(\t\x12\x0c\n\x04path\x18\x04 \x01(\t\x12\r\n\x05table\x18\x05 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x06 \x01(\t\x12\x0b\n\x03sql\x18\x07 \x01(\t\x12\r\n\x05topic\x18\x08 \x01(\t\x12\x0b\n\x03url\x18\t \x01(\t\x12\x38\n\x0bresourceRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xc5\x04\n\x0c\x44\x61taTestCase\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x12\n\nassertThat\x18\x03 \x01(\t\x12\x36\n\tentityRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0c\x63ompareToRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x06 \x01(\t\x12\x0c\n\x04type\x18\x07 \x01(\t\x12\x0e\n\x06metric\x18\x08 \x01(\t\x12\x15\n\rexpectedValue\x18\t \x01(\x01\x12\x18\n\x10\x65xpectedCategory\x18\n \x01(\t\x12\r\n\x05lower\x18\x0b \x01(\x01\x12\r\n\x05upper\x18\x0c \x01(\x01\x12\x13\n\x0b\x65xpectedSet\x18\r \x03(\t\x12\x16\n\x0elowerInclusive\x18\x0e \x01(\x08\x12\x16\n\x0eupperInclusive\x18\x0f \x01(\x08\x12\x11\n\tgenerated\x18\x10 \x01(\x08\x12\x0c\n\x04tags\x18\x11 \x03(\t\x12\x0f\n\x07\x63olumn2\x18\x12 \x01(\t\x12\x37\n\nentityRef2\x18\x13 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07\x63olumns\x18\x14 \x03(\t\x12\x15\n\rfeatureFilter\x18\x15 \x01(\t\x12\x12\n\ndataFilter\x18\x16 \x01(\t\x12\x15\n\rreferenceType\x18\x17 \x01(\t\x12\x0f\n\x07periods\x18\x18 \x01(\x05\"\xac\x01\n\x12\x44\x61taTestCaseResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12T\n\x06\x61\x63tual\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\x0f\n\x07\x66\x61ilure\x18\x03 \x01(\x08\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\"0\n\x0c\x46ileLocation\x12\x12\n\nbucketName\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"t\n\x0cGithubEvents\x12\x19\n\x11gitConnectionName\x18\x01 \x01(\t\x12\x12\n\nrepository\x18\x02 \x01(\t\x12\x0e\n\x06\x62ranch\x18\x03 \x01(\t\x12\x15\n\rblobNameRegex\x18\x04 \x01(\t\x12\x0e\n\x06\x65vents\x18\x05 \x03(\t\"z\n\x08GpuClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12\x0c\n\x04vcpu\x18\x03 \x01(\x05\x12>\n\x06gpumem\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xb5\x01\n\x0cGpuClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"c\n\rHistogramData\x12\x0c\n\x04\x62ins\x18\x01 \x03(\x01\x12\x12\n\ncategories\x18\x02 \x03(\t\x12\x0e\n\x06\x63ounts\x18\x03 \x03(\x01\x12\x0f\n\x07missing\x18\x04 \x01(\x05\x12\x0f\n\x07invalid\x18\x05 \x01(\x05\"I\n\x06Images\x12\x14\n\x0ctrainerImage\x18\x01 \x01(\t\x12\x11\n\tdataImage\x18\x02 \x01(\t\x12\x16\n\x0epublisherImage\x18\x03 \x01(\t\"\xaf\x01\n\rLastRunStatus\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08\x64uration\x18\x04 \x01(\x05\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\"*\n\x03Lib\x12\x12\n\nframeworks\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"q\n\x04Logs\x12\x0e\n\x06\x62ucket\x18\x01 \x01(\t\x12Y\n\ncontainers\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xa9\x01\n\x0bMLFramework\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFrameworkSpec\"\xa8\x01\n\x0fMLFrameworkList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.MLFramework\"R\n\x0fMLFrameworkSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0c\n\x04lang\x18\x04 \x01(\t\"\x8c\x01\n\x0cMachineClass\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x12\n\nregionName\x18\x02 \x01(\t\x12;\n\x03mem\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12\x0c\n\x04vcpu\x18\x04 \x01(\x05\x12\x0f\n\x07storage\x18\x05 \x01(\t\"\xb9\x01\n\x10MachineClassCost\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0e\n\x06region\x18\x02 \x01(\t\x12\x45\n\rcostPerMinute\x18\x03 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\x12@\n\x08\x63ostSpot\x18\x04 \x01(\x0b\x32..k8s.io.apimachinery.pkg.api.resource.Quantity\"\xab\x01\n\x0cManagedImage\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImageSpec\"\xaa\x01\n\x10ManagedImageList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ManagedImage\"\xbb\x03\n\x10ManagedImageSpec\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x10\n\x08registry\x18\x02 \x01(\t\x12\x12\n\nrepository\x18\x03 \x01(\t\x12\x0b\n\x03tag\x18\x04 \x01(\t\x12\'\n\x03\x65nv\x18\x05 \x03(\x0b\x32\x1a.k8s.io.api.core.v1.EnvVar\x12\x0b\n\x03gpu\x18\x06 \x01(\x08\x12\x0e\n\x06\x61\x63tive\x18\x07 \x01(\x08\x12\x0f\n\x07preload\x18\x08 \x01(\x08\x12:\n\rconnectionRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04\x62\x61se\x18\n \x01(\t\x12\x0c\n\x04role\x18\x0b \x01(\t\x12\x13\n\x0bmantainedBy\x18\x0c \x01(\t\x12\x0b\n\x03uri\x18\r \x01(\t\x12\x12\n\nframeworks\x18\x0e \x03(\t\x12J\n\x04libs\x18\x0f \x03(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Lib\x12\n\n\x02os\x18\x10 \x01(\t\x12\x11\n\tosVersion\x18\x11 \x01(\t\x12\x0f\n\x07private\x18\x12 \x01(\x08\"\x9a\x02\n\x0bMeasurement\x12\x33\n\x06\x65ntity\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0e\n\x06metric\x18\x03 \x01(\t\x12\r\n\x05value\x18\x04 \x01(\x01\x12\x0e\n\x06stddev\x18\x05 \x01(\x01\x12\x0f\n\x07\x62oolQty\x18\x06 \x01(\x08\x12\x10\n\x08\x63\x61tegory\x18\x07 \x01(\t\x12\x10\n\x08valueSet\x18\x08 \x03(\t\x12=\n\ttimePoint\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x10\n\x08taskType\x18\n \x01(\t\x12\x11\n\talgorithm\x18\x0b \x01(\t\"\xc5\x01\n\x13ModelDeploymentSpec\x12\x35\n\x08modelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0f\n\x07traffic\x18\x03 \x01(\x05\x12\x0c\n\x04role\x18\x04 \x01(\t\x12\x11\n\timageName\x18\x05 \x01(\t\x12\x37\n\napprovedBy\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xd1\x01\n\x10NotificationSpec\x12\x0b\n\x03ttl\x18\x01 \x01(\x05\x12\x14\n\x0cnotifierName\x18\x02 \x01(\t\x12i\n\x08selector\x18\x03 \x03(\x0b\x32W.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec.SelectorEntry\x1a/\n\rSelectorEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"-\n\rObjectiveSpec\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0c\n\x04goal\x18\x02 \x01(\t\"^\n\x07PRCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x93\x02\n\x0eParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0b\n\x03low\x18\x03 \x01(\x01\x12\x0c\n\x04high\x18\x04 \x01(\x01\x12\x0c\n\x04step\x18\x05 \x01(\x05\x12\x0b\n\x03log\x18\x06 \x01(\x08\x12\x0f\n\x07\x63hoices\x18\x07 \x03(\t\x12\x14\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\x01\x12\x15\n\rdefaultChoice\x18\t \x01(\t\x12\x13\n\x0b\x63onditional\x18\n \x01(\x08\x12\x0e\n\x06parent\x18\x0b \x01(\t\x12\x16\n\x0eparentValueCat\x18\x0c \x01(\t\x12\x1a\n\x12parentValueInteger\x18\r \x01(\x05\x12\x18\n\x10parentValueFloat\x18\x0e \x01(\x01\"p\n\x0fPermissionsSpec\x12]\n\x08\x61\x63\x63ounts\x18\x01 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccountPermissions\"\xb1\x01\n\x0fPretrainedModel\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Z\n\x04spec\x18\x02 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModelSpec\"\xb0\x01\n\x13PretrainedModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12W\n\x05items\x18\x02 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PretrainedModel\"$\n\x13PretrainedModelSpec\x12\r\n\x05image\x18\x01 \x01(\t\"\xad\x01\n\rPublicDataset\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDatasetSpec\"\xac\x01\n\x11PublicDatasetList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PublicDataset\"\xb6\x02\n\x11PublicDatasetSpec\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\x10\n\x08openMLID\x18\x04 \x01(\t\x12\x0f\n\x07\x64\x61taUrl\x18\x05 \x01(\t\x12\x10\n\x08\x63itation\x18\x06 \x01(\t\x12\x0c\n\x04rows\x18\x07 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x08 \x01(\x05\x12\x10\n\x08\x66ileSize\x18\t \x01(\x05\x12\x14\n\x0ctargetColumn\x18\n \x01(\t\x12\x10\n\x08industry\x18\x0b \x01(\t\x12\x12\n\nimbalanced\x18\x0c \x01(\x08\x12\x14\n\x0c\x64\x61tasourceCR\x18\r \x01(\t\x12\x11\n\tdatasetCR\x18\x0e \x01(\t\x12\x0f\n\x07studyCR\x18\x0f \x01(\t\x12\x15\n\rdataProductCR\x18\x10 \x01(\t\"\xb6\x01\n\x06Region\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x1d\n\x15\x64\x65\x66\x61ultDatacenterName\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x13\n\x0b\x62illingCode\x18\x04 \x01(\t\x12X\n\x0b\x64\x61tacenters\x18\x05 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataCenter\"?\n\x13ResourceConsumption\x12\x0b\n\x03\x63pu\x18\x01 \x01(\x04\x12\x0e\n\x06memory\x18\x02 \x01(\x04\x12\x0b\n\x03gpu\x18\x03 \x01(\x04\"t\n\x0cResourceSpec\x12\x14\n\x0cworkloadName\x18\x01 \x01(\t\x12\x0e\n\x06\x63ustom\x18\x02 \x01(\x08\x12>\n\x0crequirements\x18\x03 \x01(\x0b\x32(.k8s.io.api.core.v1.ResourceRequirements\"b\n\x0bRocAucCurve\x12S\n\x06values\x18\x01 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CurvePoint\"\x9d\x02\n\tRunRecord\x12\n\n\x02id\x18\x01 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x02 \x01(\t\x12\x17\n\x0fresourceVersion\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12S\n\x04logs\x18\x06 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\"\xcd\x01\n\x0bRunSchedule\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\x12\x0c\n\x04type\x18\x03 \x01(\t\x12\x15\n\rmaxRetryCount\x18\x04 \x01(\x05\x12\x15\n\rretryDelaySec\x18\x05 \x01(\x05\x12\x12\n\ntimeoutSec\x18\x06 \x01(\x05\x12\x10\n\x08timezone\x18\x07 \x01(\t\x12=\n\tnextRunAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xfe\x01\n\x11RunScheduleStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x15\n\rfailureReason\x18\x02 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x03 \x01(\t\x12\x13\n\x0blastRunName\x18\x04 \x01(\t\x12R\n\x0blastRunLogs\x18\x05 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x12\n\nretryCount\x18\x06 \x01(\x05\"\xa8\x02\n\tRunStatus\x12=\n\tlastRunAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tlastRunId\x18\x02 \x01(\t\x12\x13\n\x0b\x61\x63tiveRunId\x18\x03 \x01(\t\x12\\\n\ractiveRunLogs\x18\x04 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ContainerLog\x12V\n\nrunRecords\x18\x05 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunRecord\"r\n\tTestSuite\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12T\n\x05tests\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCase\"\xc7\x02\n\x0fTestSuiteResult\x12\x36\n\tentityRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08\x66\x61ilures\x18\x02 \x01(\x05\x12\x0e\n\x06\x65rrors\x18\x03 \x01(\x05\x12=\n\tstartedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12Z\n\x05tests\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataTestCaseResult\"G\n\x0fWorkerRunResult\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0b\n\x03uri\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12\r\n\x05\x65rror\x18\x04 \x01(\t\"\xad\x01\n\rWorkloadClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12X\n\x04spec\x18\x02 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClassSpec\"\xac\x01\n\x11WorkloadClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12U\n\x05items\x18\x02 \x03(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkloadClass\"u\n\x11WorkloadClassSpec\x12`\n\x11resourcesTemplate\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpecB9Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z7github.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1'
@@ -50,104 +50,110 @@
   _COMPILERSPEC._serialized_end=2227
   _CONFUSIONMATRIX._serialized_start=2229
   _CONFUSIONMATRIX._serialized_end=2337
   _CONFUSIONMATRIXROW._serialized_start=2339
   _CONFUSIONMATRIXROW._serialized_end=2409
   _CONTAINERLOG._serialized_start=2411
   _CONTAINERLOG._serialized_end=2486
-  _CURVEPOINT._serialized_start=2488
-  _CURVEPOINT._serialized_end=2522
-  _DATACENTER._serialized_start=2524
-  _DATACENTER._serialized_end=2564
-  _DATALOCATION._serialized_start=2567
-  _DATALOCATION._serialized_end=2785
-  _DATATESTCASE._serialized_start=2788
-  _DATATESTCASE._serialized_end=3369
-  _DATATESTCASERESULT._serialized_start=3372
-  _DATATESTCASERESULT._serialized_end=3544
-  _FILELOCATION._serialized_start=3546
-  _FILELOCATION._serialized_end=3594
-  _GITHUBEVENTS._serialized_start=3596
-  _GITHUBEVENTS._serialized_end=3712
-  _GPUCLASS._serialized_start=3714
-  _GPUCLASS._serialized_end=3836
-  _GPUCLASSCOST._serialized_start=3839
-  _GPUCLASSCOST._serialized_end=4020
-  _HISTOGRAMDATA._serialized_start=4022
-  _HISTOGRAMDATA._serialized_end=4121
-  _IMAGES._serialized_start=4123
-  _IMAGES._serialized_end=4196
-  _LASTRUNSTATUS._serialized_start=4199
-  _LASTRUNSTATUS._serialized_end=4374
-  _LIB._serialized_start=4376
-  _LIB._serialized_end=4418
-  _LOGS._serialized_start=4420
-  _LOGS._serialized_end=4533
-  _MLFRAMEWORK._serialized_start=4536
-  _MLFRAMEWORK._serialized_end=4705
-  _MLFRAMEWORKLIST._serialized_start=4708
-  _MLFRAMEWORKLIST._serialized_end=4876
-  _MLFRAMEWORKSPEC._serialized_start=4878
-  _MLFRAMEWORKSPEC._serialized_end=4960
-  _MACHINECLASS._serialized_start=4963
-  _MACHINECLASS._serialized_end=5103
-  _MACHINECLASSCOST._serialized_start=5106
-  _MACHINECLASSCOST._serialized_end=5291
-  _MANAGEDIMAGE._serialized_start=5294
-  _MANAGEDIMAGE._serialized_end=5465
-  _MANAGEDIMAGELIST._serialized_start=5468
-  _MANAGEDIMAGELIST._serialized_end=5638
-  _MANAGEDIMAGESPEC._serialized_start=5641
-  _MANAGEDIMAGESPEC._serialized_end=6084
-  _MEASUREMENT._serialized_start=6087
-  _MEASUREMENT._serialized_end=6369
-  _MODELDEPLOYMENTSPEC._serialized_start=6372
-  _MODELDEPLOYMENTSPEC._serialized_end=6569
-  _NOTIFICATIONSPEC._serialized_start=6572
-  _NOTIFICATIONSPEC._serialized_end=6781
-  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_start=6734
-  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_end=6781
-  _OBJECTIVESPEC._serialized_start=6783
-  _OBJECTIVESPEC._serialized_end=6828
-  _PRCURVE._serialized_start=6830
-  _PRCURVE._serialized_end=6924
-  _PARAMETERRANGE._serialized_start=6927
-  _PARAMETERRANGE._serialized_end=7202
-  _PERMISSIONSSPEC._serialized_start=7204
-  _PERMISSIONSSPEC._serialized_end=7316
-  _PRETRAINEDMODEL._serialized_start=7319
-  _PRETRAINEDMODEL._serialized_end=7496
-  _PRETRAINEDMODELLIST._serialized_start=7499
-  _PRETRAINEDMODELLIST._serialized_end=7675
-  _PRETRAINEDMODELSPEC._serialized_start=7677
-  _PRETRAINEDMODELSPEC._serialized_end=7713
-  _PUBLICDATASET._serialized_start=7716
-  _PUBLICDATASET._serialized_end=7889
-  _PUBLICDATASETLIST._serialized_start=7892
-  _PUBLICDATASETLIST._serialized_end=8064
-  _PUBLICDATASETSPEC._serialized_start=8067
-  _PUBLICDATASETSPEC._serialized_end=8377
-  _REGION._serialized_start=8380
-  _REGION._serialized_end=8562
-  _RESOURCECONSUMPTION._serialized_start=8564
-  _RESOURCECONSUMPTION._serialized_end=8627
-  _RESOURCESPEC._serialized_start=8629
-  _RESOURCESPEC._serialized_end=8745
-  _ROCAUCCURVE._serialized_start=8747
-  _ROCAUCCURVE._serialized_end=8845
-  _RUNSCHEDULE._serialized_start=8848
-  _RUNSCHEDULE._serialized_end=9053
-  _RUNSCHEDULESTATUS._serialized_start=9056
-  _RUNSCHEDULESTATUS._serialized_end=9310
-  _TESTSUITE._serialized_start=9312
-  _TESTSUITE._serialized_end=9426
-  _TESTSUITERESULT._serialized_start=9429
-  _TESTSUITERESULT._serialized_end=9756
-  _WORKERRUNRESULT._serialized_start=9758
-  _WORKERRUNRESULT._serialized_end=9829
-  _WORKLOADCLASS._serialized_start=9832
-  _WORKLOADCLASS._serialized_end=10005
-  _WORKLOADCLASSLIST._serialized_start=10008
-  _WORKLOADCLASSLIST._serialized_end=10180
-  _WORKLOADCLASSSPEC._serialized_start=10182
-  _WORKLOADCLASSSPEC._serialized_end=10299
+  _CRONSCHEDULE._serialized_start=2488
+  _CRONSCHEDULE._serialized_end=2567
+  _CURVEPOINT._serialized_start=2569
+  _CURVEPOINT._serialized_end=2603
+  _DATACENTER._serialized_start=2605
+  _DATACENTER._serialized_end=2645
+  _DATALOCATION._serialized_start=2648
+  _DATALOCATION._serialized_end=2866
+  _DATATESTCASE._serialized_start=2869
+  _DATATESTCASE._serialized_end=3450
+  _DATATESTCASERESULT._serialized_start=3453
+  _DATATESTCASERESULT._serialized_end=3625
+  _FILELOCATION._serialized_start=3627
+  _FILELOCATION._serialized_end=3675
+  _GITHUBEVENTS._serialized_start=3677
+  _GITHUBEVENTS._serialized_end=3793
+  _GPUCLASS._serialized_start=3795
+  _GPUCLASS._serialized_end=3917
+  _GPUCLASSCOST._serialized_start=3920
+  _GPUCLASSCOST._serialized_end=4101
+  _HISTOGRAMDATA._serialized_start=4103
+  _HISTOGRAMDATA._serialized_end=4202
+  _IMAGES._serialized_start=4204
+  _IMAGES._serialized_end=4277
+  _LASTRUNSTATUS._serialized_start=4280
+  _LASTRUNSTATUS._serialized_end=4455
+  _LIB._serialized_start=4457
+  _LIB._serialized_end=4499
+  _LOGS._serialized_start=4501
+  _LOGS._serialized_end=4614
+  _MLFRAMEWORK._serialized_start=4617
+  _MLFRAMEWORK._serialized_end=4786
+  _MLFRAMEWORKLIST._serialized_start=4789
+  _MLFRAMEWORKLIST._serialized_end=4957
+  _MLFRAMEWORKSPEC._serialized_start=4959
+  _MLFRAMEWORKSPEC._serialized_end=5041
+  _MACHINECLASS._serialized_start=5044
+  _MACHINECLASS._serialized_end=5184
+  _MACHINECLASSCOST._serialized_start=5187
+  _MACHINECLASSCOST._serialized_end=5372
+  _MANAGEDIMAGE._serialized_start=5375
+  _MANAGEDIMAGE._serialized_end=5546
+  _MANAGEDIMAGELIST._serialized_start=5549
+  _MANAGEDIMAGELIST._serialized_end=5719
+  _MANAGEDIMAGESPEC._serialized_start=5722
+  _MANAGEDIMAGESPEC._serialized_end=6165
+  _MEASUREMENT._serialized_start=6168
+  _MEASUREMENT._serialized_end=6450
+  _MODELDEPLOYMENTSPEC._serialized_start=6453
+  _MODELDEPLOYMENTSPEC._serialized_end=6650
+  _NOTIFICATIONSPEC._serialized_start=6653
+  _NOTIFICATIONSPEC._serialized_end=6862
+  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_start=6815
+  _NOTIFICATIONSPEC_SELECTORENTRY._serialized_end=6862
+  _OBJECTIVESPEC._serialized_start=6864
+  _OBJECTIVESPEC._serialized_end=6909
+  _PRCURVE._serialized_start=6911
+  _PRCURVE._serialized_end=7005
+  _PARAMETERRANGE._serialized_start=7008
+  _PARAMETERRANGE._serialized_end=7283
+  _PERMISSIONSSPEC._serialized_start=7285
+  _PERMISSIONSSPEC._serialized_end=7397
+  _PRETRAINEDMODEL._serialized_start=7400
+  _PRETRAINEDMODEL._serialized_end=7577
+  _PRETRAINEDMODELLIST._serialized_start=7580
+  _PRETRAINEDMODELLIST._serialized_end=7756
+  _PRETRAINEDMODELSPEC._serialized_start=7758
+  _PRETRAINEDMODELSPEC._serialized_end=7794
+  _PUBLICDATASET._serialized_start=7797
+  _PUBLICDATASET._serialized_end=7970
+  _PUBLICDATASETLIST._serialized_start=7973
+  _PUBLICDATASETLIST._serialized_end=8145
+  _PUBLICDATASETSPEC._serialized_start=8148
+  _PUBLICDATASETSPEC._serialized_end=8458
+  _REGION._serialized_start=8461
+  _REGION._serialized_end=8643
+  _RESOURCECONSUMPTION._serialized_start=8645
+  _RESOURCECONSUMPTION._serialized_end=8708
+  _RESOURCESPEC._serialized_start=8710
+  _RESOURCESPEC._serialized_end=8826
+  _ROCAUCCURVE._serialized_start=8828
+  _ROCAUCCURVE._serialized_end=8926
+  _RUNRECORD._serialized_start=8929
+  _RUNRECORD._serialized_end=9214
+  _RUNSCHEDULE._serialized_start=9217
+  _RUNSCHEDULE._serialized_end=9422
+  _RUNSCHEDULESTATUS._serialized_start=9425
+  _RUNSCHEDULESTATUS._serialized_end=9679
+  _RUNSTATUS._serialized_start=9682
+  _RUNSTATUS._serialized_end=9978
+  _TESTSUITE._serialized_start=9980
+  _TESTSUITE._serialized_end=10094
+  _TESTSUITERESULT._serialized_start=10097
+  _TESTSUITERESULT._serialized_end=10424
+  _WORKERRUNRESULT._serialized_start=10426
+  _WORKERRUNRESULT._serialized_end=10497
+  _WORKLOADCLASS._serialized_start=10500
+  _WORKLOADCLASS._serialized_end=10673
+  _WORKLOADCLASSLIST._serialized_start=10676
+  _WORKLOADCLASSLIST._serialized_end=10848
+  _WORKLOADCLASSSPEC._serialized_start=10850
+  _WORKLOADCLASSSPEC._serialized_end=10967
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_training_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xf0\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12]\n\x11unitTestsTemplate\x18\x06 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xd8\x06\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12R\n\x05input\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12;\n\x0eservingSiteRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08modelRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rcreateDataset\x18\x07 \x01(\x08\x12\x0f\n\x07labeled\x18\x08 \x01(\x08\x12[\n\tunitTests\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12\r\n\x05\x61\x62ort\x18\x0c \x01(\x08\x12g\n\x0c\x66orecastSpec\x18\r \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12v\n\x11partitionLocation\x18\x0e \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x16\n\x0emodelClassName\x18\x0f \x01(\t\"\xcb\x05\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x10 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nIgithub.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated.proto\x12\x39github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1aHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x82\x01\n\x0f\x41utoScalingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x13\n\x0bminReplicas\x18\x02 \x01(\x05\x12\x13\n\x0bmaxReplicas\x18\x03 \x01(\x05\x12\x19\n\x11\x63puAvgUtilization\x18\x04 \x01(\x05\x12\x19\n\x11memAvgUtilization\x18\x05 \x01(\x05\"\x8e\x01\n\x13\x42\x61\x63kwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rconfidenceLow\x18\x04 \x01(\x01\x12\x16\n\x0e\x63onfidenceHigh\x18\x05 \x01(\x01\"|\n\rCustomAppSpec\x12\r\n\x05owner\x18\x01 \x01(\x08\x12\r\n\x05title\x18\x02 \x01(\t\x12M\n\x05pages\x18\x03 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"\xfd\x01\n\x07\x44\x61taApp\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12T\n\x04spec\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppSpec\x12X\n\x06status\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataAppStatus\"\xa2\x01\n\x0b\x44\x61taAppList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12Q\n\x05items\x18\x02 \x03(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DataApp\"\xc9\x03\n\x0b\x44\x61taAppSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x16\n\x0emodelClassName\x18\x03 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x04 \x01(\t\x12\x11\n\tmodelName\x18\x05 \x01(\t\x12S\n\x06\x61\x63\x63\x65ss\x18\x06 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x07 \x01(\x05\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingsiteRef\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12X\n\x06\x63ustom\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.CustomAppSpec\"\xd8\x02\n\rDataAppStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\x10\x64\x65ploymentStatus\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0eservicetStatus\x18\x04 \x01(\x0b\x32!.k8s.io.api.core.v1.ServiceStatus\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12\x43\n\nconditions\x18\x07 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x91\x03\n\x12\x44riftDetectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rgenDriftTests\x18\x02 \x01(\x08\x12\x16\n\x0eminPredictions\x18\x03 \x01(\x05\x12\x0f\n\x07\x63olumns\x18\x04 \x03(\t\x12]\n\x0f\x64riftThresholds\x18\x05 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DriftThreshold\x12V\n\x08schedule\x18\x07 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x45\n\x18outlierDetectionModelRef\x18\x08 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rmaxHistograms\x18\t \x01(\x05\x12\x15\n\rperiodSeconds\x18\n \x01(\x05\"\xc5\x01\n\x11\x46\x61stSlowModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x39\n\x0c\x66\x61stModelRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x39\n\x0cslowModelRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bprobaLowPct\x18\x04 \x01(\x05\x12\x14\n\x0cprobaHighPct\x18\x05 \x01(\x05\"\xce\x01\n\x10\x46\x65\x65\x64\x62\x61\x63kTestSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12V\n\x08schedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\"\xa8\x02\n\x16\x46orecastPredictionSpec\x12\x7f\n\x0fhierarchyValues\x18\x01 \x03(\x0b\x32\x66.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec.HierarchyValuesEntry\x12U\n\x07horizon\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x1a\x36\n\x14HierarchyValuesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x88\x01\n\x0b\x46orecastRun\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x15\n\rmodelLocation\x18\x02 \x01(\t\x12U\n\x07horizon\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\"\xe4\x01\n\x0c\x46orecastSpec\x12_\n\x04runs\x18\t \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastSpec.RunsEntry\x1as\n\tRunsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12U\n\x05value\x18\x02 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastRun:\x02\x38\x01\"\xd1\x01\n\x0e\x46orecastStatus\x12\x12\n\nprofileURI\x18\x01 \x01(\t\x12\x11\n\treportURI\x18\x02 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x03 \x01(\t\x12\x0e\n\x06\x66\x61iled\x18\x04 \x01(\x08\x12\x12\n\nfailureMsg\x18\x05 \x01(\t\x12_\n\rworkerResults\x18\x06 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"o\n\x12\x46orwardCurtainSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x37\n\naccountRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0f\n\x07percent\x18\x03 \x01(\x05\"0\n\rMetricHistory\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x0f\n\x07history\x18\x02 \x03(\x01\"\xad\x02\n\x15ModelDeploymentRecord\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12>\n\ndeployedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12=\n\tretiredAt\x18\x06 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x07 \x01(\t\x12\x1a\n\x12\x61vgDailyPrediction\x18\x08 \x01(\x05\x12\x12\n\navgLatency\x18\t \x01(\x01\"\x9d\x07\n\x15ModelDeploymentStatus\x12\x11\n\tmodelName\x18\x01 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x02 \x01(\t\x12\x11\n\tmodelRole\x18\x03 \x01(\t\x12\x11\n\timageName\x18\x04 \x01(\t\x12:\n\rdeploymentRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x33\n\x06hpaRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x16\n\x0e\x66\x61ilureMessage\x18\x08 \x01(\t\x12>\n\ndeployedAt\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x43\n\x16lastFeedbackDatasetRef\x18\n \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x46\n\x12lastFeedbackTestAt\x18\x0b \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x65\n\x17lastFeedbackTestResults\x18\x0c \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12|\n\x0emetricsHistory\x18\r \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus.MetricsHistoryEntry\x12\x1a\n\x12\x61vgDailyPrediction\x18\x0e \x01(\x05\x12\x12\n\navgLatency\x18\x0f \x01(\x01\x12\x10\n\x08\x65ndpoint\x18\x10 \x01(\t\x1a\x7f\n\x13MetricsHistoryEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.MetricHistory:\x02\x38\x01\"\x80\x01\n\x10ModelServingSpec\x12\x12\n\nserverless\x18\x02 \x01(\x08\x12X\n\x0cservingTests\x18\x04 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\";\n\x16OnlineFeatureStoreSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08hostname\x18\x02 \x01(\t\"U\n\x11OnlineStoreStatus\x12@\n\x0clastAccessed\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"=\n PartitionPredictionLocationsSpec\x12\x19\n\x11groupForecastFile\x18\x02 \x01(\t\"\x86\x02\n\nPrediction\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12W\n\x04spec\x18\x02 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionSpec\x12[\n\x06status\x18\x03 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionStatus\"\x83\x01\n\x13PredictionCacheSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x10\n\x08inMemory\x18\x02 \x01(\x08\x12\r\n\x05redis\x18\x03 \x01(\x08\x12:\n\rconnectionRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\"\xa8\x01\n\x0ePredictionList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12T\n\x05items\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Prediction\"\x83\x02\n\x15PredictionLoggingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rsamplePercent\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x19\n\x11\x62\x61\x63kupFreqSeconds\x18\x04 \x01(\x05\x12@\n\x13\x62\x61\x63kupConnectionRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12W\n\x08location\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\xb1\x07\n\x0ePredictionSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\r\n\x05owner\x18\x02 \x01(\t\x12R\n\x05input\x18\x03 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataInputSpec\x12T\n\x06output\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.DataOutputSpec\x12;\n\x0eservingSiteRef\x18\x05 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x35\n\x08modelRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x15\n\rcreateDataset\x18\x07 \x01(\x08\x12\x0f\n\x07labeled\x18\x08 \x01(\x08\x12[\n\tunitTests\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelTestSuite\x12X\n\tresources\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x0b \x01(\x03\x12W\n\x08schedule\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.CronSchedule\x12\r\n\x05\x61\x62ort\x18\r \x01(\x08\x12g\n\x0c\x66orecastSpec\x18\x0e \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastPredictionSpec\x12v\n\x11partitionLocation\x18\x0f \x01(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PartitionPredictionLocationsSpec\x12\x16\n\x0emodelClassName\x18\x10 \x01(\t\"\x9d\x06\n\x10PredictionStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12\x61\n\x0funitTestsResult\x18\x03 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12\x37\n\ndatasetRef\x18\x0b \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12[\n\x08\x66orecast\x18\x0e \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForecastStatus\x12[\n\x05usage\x18\x0f \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12P\n\x04runs\x18\x10 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunStatus\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x83\x02\n\tPredictor\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorStatus\"\xa6\x01\n\rPredictorList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.Predictor\"\xb1\r\n\rPredictorSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x16\n\x0emodelClassName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x37\n\nproductRef\x18\x04 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08template\x18\x05 \x01(\x08\x12;\n\x0eservingSiteRef\x18\x07 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\\\n\x06models\x18\x08 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ModelDeploymentSpec\x12_\n\x0bprogressive\x18\t \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ProgressiveSpec\x12S\n\x06\x61\x63\x63\x65ss\x18\x0b \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x0c \x01(\x05\x12_\n\x0b\x61utoScaling\x18\r \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.AutoScalingSpec\x12\r\n\x05owner\x18\x0e \x01(\t\x12X\n\tresources\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12]\n\x05\x63\x61\x63he\x18\x10 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionCacheSpec\x12`\n\x05store\x18\x11 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineFeatureStoreSpec\x12\\\n\x07serving\x18\x12 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelServingSpec\x12\x0c\n\x04task\x18\x13 \x01(\t\x12\\\n\x05\x64rift\x18\x15 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.DriftDetectionSpec\x12]\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x16 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FeedbackTestSpec\x12_\n\x0cnotification\x18\x17 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12k\n\x11predictionLogging\x18\x18 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictionLoggingSpec\x12\x65\n\x0e\x66orwardCurtain\x18\x19 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ForwardCurtainSpec\x12g\n\x0f\x62\x61\x63kwardCurtain\x18\x1a \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.BackwardCurtainSpec\x12^\n\x08\x66\x61stSlow\x18\x1b \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.FastSlowModelSpec\"\xd6\x06\n\x0fPredictorStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12\x61\n\x07history\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentRecord\x12\x65\n\x0bmodelStatus\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.ModelDeploymentStatus\x12i\n\x12predictorletStatus\x18\x05 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.PredictorletStatus\x12g\n\x11onlineStoreStatus\x18\x07 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.OnlineStoreStatus\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0b \x01(\t\x12\x42\n\x12loadBalancerStatus\x18\x0c \x01(\x0b\x32&.k8s.io.api.core.v1.LoadBalancerStatus\x12\x42\n\x15lastPredictionDataset\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x65\n\x13servingTestsResults\x18\x0e \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x43\n\nconditions\x18\x11 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x86\x03\n\x12PredictorletStatus\x12:\n\rdeploymentRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\nserviceRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\ndeployedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0b\n\x03p50\x18\x04 \x01(\x01\x12\x0b\n\x03p95\x18\x05 \x01(\x01\x12\x0b\n\x03p99\x18\x06 \x01(\x01\x12\x1a\n\x12\x61vgDailyPrediction\x18\x07 \x01(\x05\x12\x18\n\x10totalPredictions\x18\x08 \x01(\x05\x12\x46\n\x12lastPredictionTime\x18\t \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\"R\n\x0fProgressiveSpec\x12\x0e\n\x06warmup\x18\x01 \x01(\x05\x12\x18\n\x10trafficIncrement\x18\x02 \x01(\x05\x12\x15\n\rcanaryMetrics\x18\x03 \x03(\t\"[\n\x0fValidationError\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\x0e\n\x06metric\x18\x02 \x01(\t\x12\x0b\n\x03min\x18\x03 \x01(\x01\x12\x0b\n\x03max\x18\x04 \x01(\x01\x12\x0e\n\x06\x61\x63tual\x18\x05 \x01(\x01\x42;Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.inference.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z9github.com/metaprov/modelaapi/pkg/apis/inference/v1alpha1'
@@ -45,69 +45,69 @@
   _DATAAPPLIST._serialized_start=1209
   _DATAAPPLIST._serialized_end=1371
   _DATAAPPSPEC._serialized_start=1374
   _DATAAPPSPEC._serialized_end=1831
   _DATAAPPSTATUS._serialized_start=1834
   _DATAAPPSTATUS._serialized_end=2178
   _DRIFTDETECTIONSPEC._serialized_start=2181
-  _DRIFTDETECTIONSPEC._serialized_end=2677
-  _FASTSLOWMODELSPEC._serialized_start=2680
-  _FASTSLOWMODELSPEC._serialized_end=2877
-  _FEEDBACKTESTSPEC._serialized_start=2880
-  _FEEDBACKTESTSPEC._serialized_end=3086
-  _FORECASTPREDICTIONSPEC._serialized_start=3089
-  _FORECASTPREDICTIONSPEC._serialized_end=3385
-  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_start=3331
-  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_end=3385
-  _FORECASTRUN._serialized_start=3388
-  _FORECASTRUN._serialized_end=3524
-  _FORECASTSPEC._serialized_start=3527
-  _FORECASTSPEC._serialized_end=3755
-  _FORECASTSPEC_RUNSENTRY._serialized_start=3640
-  _FORECASTSPEC_RUNSENTRY._serialized_end=3755
-  _FORECASTSTATUS._serialized_start=3758
-  _FORECASTSTATUS._serialized_end=3967
-  _FORWARDCURTAINSPEC._serialized_start=3969
-  _FORWARDCURTAINSPEC._serialized_end=4080
-  _METRICHISTORY._serialized_start=4082
-  _METRICHISTORY._serialized_end=4130
-  _MODELDEPLOYMENTRECORD._serialized_start=4133
-  _MODELDEPLOYMENTRECORD._serialized_end=4434
-  _MODELDEPLOYMENTSTATUS._serialized_start=4437
-  _MODELDEPLOYMENTSTATUS._serialized_end=5362
-  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_start=5235
-  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_end=5362
-  _MODELSERVINGSPEC._serialized_start=5365
-  _MODELSERVINGSPEC._serialized_end=5493
-  _ONLINEFEATURESTORESPEC._serialized_start=5495
-  _ONLINEFEATURESTORESPEC._serialized_end=5554
-  _ONLINESTORESTATUS._serialized_start=5556
-  _ONLINESTORESTATUS._serialized_end=5641
-  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_start=5643
-  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_end=5704
-  _PREDICTION._serialized_start=5707
-  _PREDICTION._serialized_end=5969
-  _PREDICTIONCACHESPEC._serialized_start=5972
-  _PREDICTIONCACHESPEC._serialized_end=6103
-  _PREDICTIONLIST._serialized_start=6106
-  _PREDICTIONLIST._serialized_end=6274
-  _PREDICTIONLOGGINGSPEC._serialized_start=6277
-  _PREDICTIONLOGGINGSPEC._serialized_end=6536
-  _PREDICTIONSPEC._serialized_start=6539
-  _PREDICTIONSPEC._serialized_end=7395
-  _PREDICTIONSTATUS._serialized_start=7398
-  _PREDICTIONSTATUS._serialized_end=8113
-  _PREDICTOR._serialized_start=8116
-  _PREDICTOR._serialized_end=8375
-  _PREDICTORLIST._serialized_start=8378
-  _PREDICTORLIST._serialized_end=8544
-  _PREDICTORSPEC._serialized_start=8547
-  _PREDICTORSPEC._serialized_end=10260
-  _PREDICTORSTATUS._serialized_start=10263
-  _PREDICTORSTATUS._serialized_end=11117
-  _PREDICTORLETSTATUS._serialized_start=11120
-  _PREDICTORLETSTATUS._serialized_end=11510
-  _PROGRESSIVESPEC._serialized_start=11512
-  _PROGRESSIVESPEC._serialized_end=11594
-  _VALIDATIONERROR._serialized_start=11596
-  _VALIDATIONERROR._serialized_end=11687
+  _DRIFTDETECTIONSPEC._serialized_end=2582
+  _FASTSLOWMODELSPEC._serialized_start=2585
+  _FASTSLOWMODELSPEC._serialized_end=2782
+  _FEEDBACKTESTSPEC._serialized_start=2785
+  _FEEDBACKTESTSPEC._serialized_end=2991
+  _FORECASTPREDICTIONSPEC._serialized_start=2994
+  _FORECASTPREDICTIONSPEC._serialized_end=3290
+  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_start=3236
+  _FORECASTPREDICTIONSPEC_HIERARCHYVALUESENTRY._serialized_end=3290
+  _FORECASTRUN._serialized_start=3293
+  _FORECASTRUN._serialized_end=3429
+  _FORECASTSPEC._serialized_start=3432
+  _FORECASTSPEC._serialized_end=3660
+  _FORECASTSPEC_RUNSENTRY._serialized_start=3545
+  _FORECASTSPEC_RUNSENTRY._serialized_end=3660
+  _FORECASTSTATUS._serialized_start=3663
+  _FORECASTSTATUS._serialized_end=3872
+  _FORWARDCURTAINSPEC._serialized_start=3874
+  _FORWARDCURTAINSPEC._serialized_end=3985
+  _METRICHISTORY._serialized_start=3987
+  _METRICHISTORY._serialized_end=4035
+  _MODELDEPLOYMENTRECORD._serialized_start=4038
+  _MODELDEPLOYMENTRECORD._serialized_end=4339
+  _MODELDEPLOYMENTSTATUS._serialized_start=4342
+  _MODELDEPLOYMENTSTATUS._serialized_end=5267
+  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_start=5140
+  _MODELDEPLOYMENTSTATUS_METRICSHISTORYENTRY._serialized_end=5267
+  _MODELSERVINGSPEC._serialized_start=5270
+  _MODELSERVINGSPEC._serialized_end=5398
+  _ONLINEFEATURESTORESPEC._serialized_start=5400
+  _ONLINEFEATURESTORESPEC._serialized_end=5459
+  _ONLINESTORESTATUS._serialized_start=5461
+  _ONLINESTORESTATUS._serialized_end=5546
+  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_start=5548
+  _PARTITIONPREDICTIONLOCATIONSSPEC._serialized_end=5609
+  _PREDICTION._serialized_start=5612
+  _PREDICTION._serialized_end=5874
+  _PREDICTIONCACHESPEC._serialized_start=5877
+  _PREDICTIONCACHESPEC._serialized_end=6008
+  _PREDICTIONLIST._serialized_start=6011
+  _PREDICTIONLIST._serialized_end=6179
+  _PREDICTIONLOGGINGSPEC._serialized_start=6182
+  _PREDICTIONLOGGINGSPEC._serialized_end=6441
+  _PREDICTIONSPEC._serialized_start=6444
+  _PREDICTIONSPEC._serialized_end=7389
+  _PREDICTIONSTATUS._serialized_start=7392
+  _PREDICTIONSTATUS._serialized_end=8189
+  _PREDICTOR._serialized_start=8192
+  _PREDICTOR._serialized_end=8451
+  _PREDICTORLIST._serialized_start=8454
+  _PREDICTORLIST._serialized_end=8620
+  _PREDICTORSPEC._serialized_start=8623
+  _PREDICTORSPEC._serialized_end=10336
+  _PREDICTORSTATUS._serialized_start=10339
+  _PREDICTORSTATUS._serialized_end=11193
+  _PREDICTORLETSTATUS._serialized_start=11196
+  _PREDICTORLETSTATUS._serialized_end=11586
+  _PROGRESSIVESPEC._serialized_start=11588
+  _PROGRESSIVESPEC._serialized_end=11670
+  _VALIDATIONERROR._serialized_start=11672
+  _VALIDATIONERROR._serialized_end=11763
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1 import generated_pb2 as github_dot_com_dot_metaprov_dot_modelaapi_dot_pkg_dot_apis_dot_data_dot_v1alpha1_dot_generated__pb2
 from k8s.io.api.core.v1 import generated_pb2 as k8s_dot_io_dot_api_dot_core_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.apis.meta.v1 import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_apis_dot_meta_dot_v1_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_generated__pb2
 from k8s.io.apimachinery.pkg.runtime.schema import generated_pb2 as k8s_dot_io_dot_apimachinery_dot_pkg_dot_runtime_dot_schema_dot_generated__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xf2\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0c \x01(\x08\x12\x13\n\x0bpassthrough\x18\r \x01(\x08\"\xcd\x02\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x10\n\x08trainers\x18\x06 \x01(\x05\x12\r\n\x05reuse\x18\t \x01(\x08\x12h\n\x10\x66\x65\x61tureSelection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xed\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x15\n\rfailureReason\x18\t \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\x95\x0c\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x14\n\x0cmodelVersion\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x05 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xeb\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0bsizeInBytes\x18, \x01(\x05\x12\x0f\n\x07latency\x18- \x01(\x01\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xd2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc5\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xfe\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1e \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12p\n\x16\x62\x65stFeatureEngineering\x18  \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18! \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nHgithub.com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated.proto\x12\x38github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1\x1aGgithub.com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated.proto\x1a\x44github.com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated.proto\x1a\"k8s.io/api/core/v1/generated.proto\x1a\x34k8s.io/apimachinery/pkg/apis/meta/v1/generated.proto\x1a/k8s.io/apimachinery/pkg/runtime/generated.proto\x1a\x36k8s.io/apimachinery/pkg/runtime/schema/generated.proto\"\x80\x01\n\x17\x41lgorithmParameterRange\x12\x0c\n\x04name\x18\x01 \x01(\t\x12W\n\x06ranges\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ParameterRange\"\x9f\x01\n\x18\x41lgorithmSearchSpaceSpec\x12\x0f\n\x07include\x18\x01 \x03(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\x12\x61\n\x06\x63ustom\x18\x03 \x03(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmParameterRange\"`\n\x07\x41nomaly\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bvalueColumn\x18\x02 \x01(\t\x12\x16\n\x0e\x61\x64jDeltaColumn\x18\x03 \x01(\t\x12\r\n\x05start\x18\x04 \x01(\t\x12\x0b\n\x03\x65nd\x18\x05 \x01(\t\"\'\n\x11\x41udioPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"M\n\x0c\x42\x61\x63ktestSpec\x12\x0f\n\x07sliding\x18\x01 \x01(\x08\x12\x0e\n\x06splits\x18\x02 \x01(\x05\x12\x0f\n\x07Initial\x18\x03 \x01(\x05\x12\x0b\n\x03gap\x18\x05 \x01(\x05\"?\n\x0c\x42\x61selineSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tbaselines\x18\x02 \x03(\t\x12\x0b\n\x03\x61ll\x18\x03 \x01(\x08\"\r\n\x0b\x43hangePoint\"\x96\x01\n\x0e\x43heckpointSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1a\n\x12\x63heckpointInterval\x18\x02 \x01(\x05\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\"\x92\x01\n\x16\x43lassicalEstimatorSpec\x12\x15\n\ralgorithmName\x18\x01 \x01(\t\x12\x61\n\nparameters\x18\x02 \x03(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperParameterValue\"a\n\x10\x43ustomReportSpec\x12M\n\x05pages\x18\x08 \x03(\x0b\x32>.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.PageSpec\"L\n\nDataHashes\x12\x11\n\ttrainHash\x18\x01 \x01(\t\x12\x13\n\x0btestingHash\x18\x02 \x01(\t\x12\x16\n\x0evalidationHash\x18\x03 \x01(\t\"\xab\x01\n\rDataSplitSpec\x12\x0e\n\x06method\x18\x01 \x01(\t\x12\r\n\x05train\x18\x02 \x01(\x05\x12\x12\n\nvalidation\x18\x03 \x01(\x05\x12\x0c\n\x04test\x18\x04 \x01(\x05\x12\x13\n\x0bsplitColumn\x18\x05 \x01(\t\x12\x14\n\x0ctrainDataset\x18\x07 \x01(\t\x12\x13\n\x0btestDataset\x18\x08 \x01(\t\x12\x19\n\x11validationDataset\x18\t \x01(\t\"\xa5\x01\n\x12\x44\x65\x65pEstimatorLayer\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12^\n\nparameters\x18\x03 \x03(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.NNLayerParameter\x12\x13\n\x0binputLayers\x18\x04 \x03(\t\"\xe6\x01\n\x11\x44\x65\x65pEstimatorSpec\x12\\\n\x06layers\x18\x01 \x03(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DeepEstimatorLayer\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x11\n\tbatchSize\x18\x03 \x01(\x05\x12\x0e\n\x06\x65pochs\x18\x04 \x01(\x05\x12\x17\n\x0fvalidationSplit\x18\x05 \x01(\x05\x12\r\n\x05isSeq\x18\x06 \x01(\x08\x12\x0c\n\x04gpus\x18\x07 \x01(\x05\x12\x0c\n\x04loss\x18\x08 \x01(\t\".\n\x13\x44riftDetectorStatus\x12\x17\n\x0foutlierModelURI\x18\x01 \x01(\t\"O\n\rEarlyStopSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07initial\x18\x02 \x01(\x05\x12\x1c\n\x14modelsWithNoProgress\x18\x03 \x01(\x05\"\xfb\x01\n\x0c\x45nsembleSpec\x12\x0e\n\x06models\x18\x01 \x03(\t\x12\x64\n\nestimators\x18\x02 \x03(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12g\n\rbaseEstimator\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x0c\n\x04type\x18\x04 \x01(\t\"_\n\rEnsemblesSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x16\n\x0evotingEnsemble\x18\x02 \x01(\x08\x12\x18\n\x10stackingEnsemble\x18\x03 \x01(\x08\x12\x0b\n\x03top\x18\x04 \x01(\x05\"*\n\tEntityRef\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07\x65xclude\x18\x02 \x03(\t\"\x89\x01\n\x0b\x45valMetrics\x12\x11\n\tselection\x18\x01 \x01(\t\x12\x11\n\treporting\x18\x02 \x03(\t\x12\x0f\n\x07\x61ggFunc\x18\x03 \x01(\t\x12\x11\n\taggPeriod\x18\x04 \x01(\x05\x12\x17\n\x0fnullModelParams\x18\x05 \x01(\t\x12\x17\n\x0frelErrTolerance\x18\x06 \x01(\x01\"\xe0\x01\n\nEvalPeriod\x12\x13\n\x0btestHorizon\x18\x01 \x01(\x05\x12\x1f\n\x17periodsBetweenTrainTest\x18\x02 \x01(\x05\x12\x1e\n\x16\x63vPeriodsBetweenSplits\x18\x03 \x01(\x05\x12\x1a\n\x12\x63vExpandingWindows\x18\x04 \x01(\x08\x12\x11\n\tcvHorizon\x18\x05 \x01(\x05\x12\x19\n\x11\x63vMinTrainPeriods\x18\x06 \x01(\x05\x12\x13\n\x0b\x63vMaxSplits\x18\x07 \x01(\x05\x12\x1d\n\x15\x63vUseMostRecentSplits\x18\x08 \x01(\x08\"\xf2\x02\n\x1a\x46\x65\x61tureEngineeringPipeline\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\x12\x12\n\nimputation\x18\x04 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x05 \x01(\t\x12\x0f\n\x07scaling\x18\x06 \x01(\t\x12\x16\n\x0e\x64iscretisation\x18\x07 \x01(\t\x12\x1e\n\x16variableTransformation\x18\x08 \x01(\t\x12\x17\n\x0foutlierHandling\x18\t \x01(\t\x12\x1e\n\x16\x64\x61tetimeTransformation\x18\n \x01(\t\x12X\n\x04text\x18\x0b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TextPipelineSpec\x12\x0c\n\x04\x64rop\x18\x0c \x01(\x08\x12\x13\n\x0bpassthrough\x18\r \x01(\x08\"\xcd\x02\n\x1c\x46\x65\x61tureEngineeringSearchSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\testimator\x18\x03 \x01(\t\x12\x11\n\tmaxModels\x18\x04 \x01(\x05\x12\x0f\n\x07maxTime\x18\x05 \x01(\x05\x12\x10\n\x08trainers\x18\x06 \x01(\x05\x12\r\n\x05reuse\x18\t \x01(\x08\x12h\n\x10\x66\x65\x61tureSelection\x18\n \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\"\x80\x01\n\x1e\x46\x65\x61tureEngineeringSearchStatus\x12^\n\x04\x62\x65st\x18\x01 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\"\xf7\x01\n\x16\x46\x65\x61tureEngineeringSpec\x12g\n\tpipelines\x18\x01 \x03(\x0b\x32T.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringPipeline\x12\x11\n\timbalance\x18\x02 \x01(\t\x12\x61\n\tselection\x18\x03 \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureSelectionSpec\"8\n\x11\x46\x65\x61tureImportance\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\x12\n\nimportance\x18\x02 \x01(\x01\":\n\x0b\x46\x65\x61tureInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x01\"#\n\x0b\x46\x65\x61turePair\x12\t\n\x01x\x18\x01 \x01(\t\x12\t\n\x01y\x18\x02 \x01(\t\"\xd5\x01\n\x14\x46\x65\x61tureSelectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\tembedding\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ilter\x18\x04 \x01(\x08\x12\x0f\n\x07wrapper\x18\x05 \x01(\x08\x12\x10\n\x08pipeline\x18\x06 \x03(\t\x12\x14\n\x0cvarThreshold\x18\x07 \x01(\x05\x12\x15\n\rcorrThreshold\x18\x08 \x01(\x05\x12\x13\n\x0bmaxFeatures\x18\t \x01(\x05\x12\x12\n\npercentile\x18\n \x01(\x05\x12\x10\n\x08reserved\x18\x0c \x03(\t\"\xf8\x07\n\x0e\x46orecasterSpec\x12Y\n\x06\x65vents\x18\x02 \x03(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TimeSeriesEvent\x12R\n\x04past\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12T\n\x06\x66uture\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.WindowSpec\x12\x10\n\x08\x66orecast\x18\x05 \x01(\x08\x12\x10\n\x08\x63overage\x18\x06 \x01(\x01\x12]\n\x0eoutputLocation\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12\x10\n\x08\x66\x65\x61tures\x18\x08 \x03(\t\x12\x0e\n\x06groups\x18\t \x03(\t\x12\x1a\n\x12predefinedTemplate\x18\n \x01(\t\x12T\n\tanomalies\x18\x0b \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Anomaly\x12\x14\n\x0ctrainEndData\x18\x0c \x01(\t\x12\x13\n\x0bvalueColumn\x18\r \x01(\t\x12\x11\n\thpoBudget\x18\x0e \x01(\x05\x12`\n\x11\x65valuationMetrics\x18\x0f \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalMetrics\x12^\n\x10\x65valuationPeriod\x18\x10 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EvalPeriod\x12^\n\x0bseasonality\x18\x11 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalitySpec\x12\x12\n\nregressors\x18\x12 \x03(\t\x12\x18\n\x10laggedRegressors\x18\x13 \x03(\t\x12\x0e\n\x06growth\x18\x14 \x01(\t\x12\x0b\n\x03key\x18\x15 \x03(\t\x12\x12\n\nestimators\x18\x16 \x03(\t\x12\x0b\n\x03hts\x18\x17 \x01(\t\"e\n\x15GarbageCollectionSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12!\n\x19keepBestModelPerAlgorithm\x18\x02 \x01(\x08\x12\x18\n\x10keepPrunedModels\x18\x03 \x01(\x08\"\x8e\x01\n\x17GarbageCollectionStatus\x12\x1c\n\x14\x63ollectedModelsCount\x18\x01 \x01(\x05\x12U\n\x06models\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelResult\"f\n\x13GeneratedColumnSpec\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05\x66irst\x18\x03 \x01(\t\x12\x0e\n\x06second\x18\x04 \x01(\t\x12\x10\n\x08original\x18\x05 \x01(\t\"V\n\x17GroupSplitLocationsSpec\x12\x1d\n\x15groupTrainingDataFile\x18\x01 \x01(\t\x12\x1c\n\x14groupTestingDataFile\x18\x02 \x01(\t\"2\n\x13HyperParameterValue\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"o\n\x10HyperbandOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x14\n\x0cmaxResources\x18\x02 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"\'\n\x11ImagePipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\";\n\x15ImbalanceHandlingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\timbalance\x18\x02 \x01(\t\"\x9a\x02\n\x14InterpretabilitySpec\x12\x0b\n\x03ice\x18\x01 \x01(\x08\x12W\n\x08icepairs\x18\x02 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x0c\n\x04lime\x18\x03 \x01(\x08\x12\x0c\n\x04shap\x18\x04 \x01(\t\x12X\n\tshappairs\x18\x05 \x03(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeaturePair\x12\x16\n\x0e\x63ounterfactual\x18\x06 \x01(\x08\x12\x0e\n\x06\x61nchor\x18\x07 \x01(\x08\"\xaa\x04\n\x16InterpretabilityStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x11\x65xplainerLocation\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x66\n\x17trainShapValuesLocation\x18\x04 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x65\n\x16testShapValuesLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\nimportance\x18\x06 \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\"k\n\x13MedianPrunerOptions\x12\x15\n\rstartupTrials\x18\x01 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x02 \x01(\x05\x12\x15\n\rintervalSteps\x18\x03 \x01(\x05\x12\x11\n\tminTrials\x18\x04 \x01(\x05\"\xf5\x01\n\x05Model\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelSpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelStatus\"\x84\x02\n\nModelClass\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12V\n\x04spec\x18\x02 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassSpec\x12Z\n\x06status\x18\x03 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassStatus\"\xcd\x04\n\x12ModelClassDataSpec\x12[\n\x0cobservations\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12Z\n\x0bpredictions\x18\x02 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.DataLocation\x12L\n\x06schema\x18\x03 \x01(\x0b\x32<.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Schema\x12Z\n\x08\x66latFile\x18\x04 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.FlatFileFormatSpec\x12\x12\n\nprimaryKey\x18\x05 \x03(\t\x12\x1c\n\x14predictionTimeColumn\x18\x06 \x01(\t\x12\x0e\n\x06target\x18\x07 \x01(\t\x12Q\n\x05tests\x18\x08 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12\x1e\n\x16onlineFeatureStoreName\x18\t \x01(\t\x12\x1f\n\x17offlineFeatureStoreName\x18\n \x01(\t\"\xa7\x01\n\x0eModelClassList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12S\n\x05items\x18\x02 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClass\"\x8d\x02\n\rModelClassRun\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Y\n\x04spec\x18\x02 \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunSpec\x12]\n\x06status\x18\x03 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRunStatus\"\xad\x01\n\x11ModelClassRunList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12V\n\x05items\x18\x02 \x03(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassRun\"\xce\x01\n\x11ModelClassRunSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61tasetName\x18\x03 \x01(\t\x12\x16\n\x0emodelClassName\x18\x04 \x01(\t\x12\r\n\x05owner\x18\x05 \x01(\t\x12\x10\n\x08priority\x18\x06 \x01(\t\x12\x0e\n\x06paused\x18\x07 \x01(\x08\x12\x0f\n\x07\x61\x62orted\x18\x08 \x01(\x08\x12\x0b\n\x03ttl\x18\t \x01(\x05\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\"\xd6\x04\n\x13ModelClassRunStatus\x12\x13\n\x0b\x64\x61tasetName\x18\x01 \x01(\t\x12\x11\n\tstudyName\x18\x02 \x01(\t\x12\x11\n\tmodelName\x18\x03 \x01(\t\x12?\n\x0b\x63ompletedAt\x18\x05 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x06 \x01(\t\x12\x1a\n\x12observedGeneration\x18\x07 \x01(\x03\x12\x13\n\x0b\x65valMetrics\x18\x08 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\n \x01(\t\x12=\n\tupdatedAt\x18\x0c \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12K\n\x04logs\x18\r \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12>\n\npromotedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x0c\n\x04\x61uto\x18\x0f \x01(\x08\x12\x37\n\napprovedBy\x18\x10 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0bmodelsCount\x18\x11 \x01(\x05\x12\x43\n\nconditions\x18\x12 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xd5\x02\n\x15ModelClassServingSpec\x12W\n\x08template\x18\x01 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\x12`\n\x12monitoringSchedule\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12`\n\x12predictionSchedule\x18\x03 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0e\n\x06preSQL\x18\x04 \x03(\t\x12\x0f\n\x07postSQL\x18\x05 \x03(\t\"\xc9\x06\n\x0eModelClassSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x13\n\x0bversionName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x0c\n\x04task\x18\x04 \x01(\t\x12\x0f\n\x07subtask\x18\x05 \x01(\t\x12Y\n\tobjective\x18\x06 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12U\n\x08\x65ntities\x18\x07 \x03(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EntityRef\x12Z\n\x04\x64\x61ta\x18\x08 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassDataSpec\x12\x62\n\x08training\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassTrainingSpec\x12`\n\x07serving\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelClassServingSpec\x12_\n\x0cnotification\x18\x0b \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\\\n\x0ereportSchedule\x18\x0c \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12\x0c\n\x04\x66\x61st\x18\r \x01(\x08\x12\x0e\n\x06paused\x18\x0e \x01(\x08\x12\x12\n\nregistered\x18\x0f \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x10 \x01(\t\"\xe7\x08\n\x10ModelClassStatus\x12\x1a\n\x12observedGeneration\x18\x01 \x01(\x03\x12=\n\tupdatedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12`\n\x06\x62\x65stFE\x18\x03 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12j\n\x16trainingScheduleStatus\x18\x04 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18predictionScheduleStatus\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12l\n\x18monitoringScheduleStatus\x18\x06 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12h\n\x14reportScheduleStatus\x18\x07 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunScheduleStatus\x12\x16\n\x0e\x62\x65stModelScore\x18\x08 \x01(\x01\x12\x0f\n\x07retired\x18\t \x03(\t\x12\x15\n\rpredictorName\x18\n \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x0b \x01(\t\x12\x13\n\x0btriggeredBy\x18\x0c \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x0e \x01(\t\x12=\n\tlastRunAt\x18\x0f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x13\n\x0blastRunName\x18\x10 \x01(\t\x12\x44\n\x10lastPredictionAt\x18\x11 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12lastPredictionName\x18\x12 \x01(\t\x12\x18\n\x10predictionsCount\x18\x13 \x01(\x05\x12\x11\n\trunsCount\x18\x14 \x01(\x05\x12\x13\n\x0bmodelsCount\x18\x15 \x01(\x05\x12\x0c\n\x04live\x18\x16 \x01(\x08\x12\x17\n\x0fpredictorsCount\x18\x17 \x01(\x05\x12\x43\n\nconditions\x18\x18 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x87\x05\n\x16ModelClassTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x19\n\x11studyTemplateName\x18\x02 \x01(\t\x12Z\n\x0emodelUnitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12^\n\x10trainingSchedule\x18\x04 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RunSchedule\x12g\n\x0bsearchSpace\x18\x08 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12X\n\tresources\x18\t \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x13\n\x0btriggeredBy\x18\n \x01(\t\x12\x0e\n\x06paused\x18\x0b \x01(\x08\x12\x0f\n\x07maxTime\x18\x0c \x01(\x05\x12\x11\n\tmaxModels\x18\r \x01(\x05\x12\x10\n\x08trainers\x18\x0e \x01(\x05\x12\x0f\n\x07\x61\x62orted\x18\x0f \x01(\x08\x12\x11\n\texplained\x18\x10 \x01(\x08\x12\x0e\n\x06preSQL\x18\x11 \x03(\t\x12\x0f\n\x07postSQL\x18\x12 \x03(\t\"\xb3\x01\n\x12ModelGroupByStatus\x12\x11\n\tmodelsURI\x18\x01 \x01(\t\x12\x13\n\x0bprofilesURI\x18\x02 \x01(\t\x12\x14\n\x0c\x66orecastsURI\x18\x03 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9d\x01\n\tModelList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Model\"]\n\x0bModelResult\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\talgorithm\x18\x02 \x01(\t\x12\r\n\x05score\x18\x03 \x01(\x01\x12\r\n\x05\x65rror\x18\x04 \x01(\x08\x12\x0f\n\x07trialID\x18\x05 \x01(\x05\"\xe6\x0b\n\tModelSpec\x12\r\n\x05owner\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x11\n\tstudyName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x06 \x01(\t\x12\x0f\n\x07subtask\x18\x07 \x01(\t\x12Y\n\tobjective\x18\x08 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12l\n\x12\x66\x65\x61tureEngineering\x18\t \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12\x63\n\testimator\x18\n \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12X\n\x08\x65nsemble\x18\x0b \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsembleSpec\x12X\n\x08training\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x0c\n\x04test\x18\r \x01(\x08\x12\r\n\x05\x61\x62ort\x18\x0e \x01(\x08\x12\x0f\n\x07package\x18\x0f \x01(\x08\x12\x0e\n\x06report\x18\x10 \x01(\x08\x12\r\n\x05pause\x18\x11 \x01(\x08\x12\x0f\n\x07profile\x18\x12 \x01(\x08\x12\x10\n\x08\x66orecast\x18\x13 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x14 \x01(\x08\x12\x10\n\x08unitTest\x18\x15 \x01(\x08\x12\x10\n\x08\x62\x61seline\x18\x16 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x17 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x18 \x01(\t\x12]\n\x0b\x66orecasting\x18\x19 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12\x1d\n\x15\x61\x63tiveDeadlineSeconds\x18\x1a \x01(\x03\x12\x15\n\restimatorType\x18\x1b \x01(\t\x12\x12\n\nmodelClass\x18\x1c \x01(\t\x12\x0f\n\x07trialID\x18\x1d \x01(\x05\x12T\n\x08\x61pproval\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalSpec\x12h\n\x10interpretability\x18\x1f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12U\n\tunitTests\x18  \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12q\n\x12partitionLocations\x18! \x01(\x0b\x32U.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PartitionModelLocationsSpec\x12\x16\n\x0emodelClassName\x18\" \x01(\t\x12\x19\n\x11modelClassRunName\x18# \x01(\t\x12_\n\x0cnotification\x18$ \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\"\x93\x02\n\x10ModelStageStatus\x12\r\n\x05phase\x18\x01 \x01(\t\x12=\n\tstartedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x61\n\x0funitTestsResult\x18\t \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\r\n\x05\x65rror\x18\n \x01(\t\"\xf2\"\n\x0bModelStatus\x12\x45\n\x11trainingStartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12G\n\x13trainingCompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x44\n\x10testingStartedAt\x18\x03 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x46\n\x12testingCompletedAt\x18\x04 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x07 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x17\n\x0fvalidationScore\x18\x08 \x01(\x01\x12\x15\n\rtrainingScore\x18\t \x01(\x01\x12\x11\n\ttestScore\x18\n \x01(\x01\x12X\n\nvalidation\x18\r \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12S\n\x05train\x18\x0e \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04test\x18\x0f \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12R\n\x04tune\x18\x10 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12V\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x11 \x03(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Measurement\x12\r\n\x05phase\x18\x12 \x01(\t\x12\x12\n\nreportName\x18\x13 \x01(\t\x12]\n\x0ereportLocation\x18\x14 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x63\n\x14trainWeightsLocation\x18\x15 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testWeightsLocation\x18\x16 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13\x66ullWeightsLocation\x18\x17 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19trainLabelEncoderLocation\x18\x18 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fprofileLocation\x18\x1b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19misclassificationLocation\x18\x1c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12_\n\x10\x66orecastLocation\x18\x1d \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12^\n\x0fpackageLocation\x18\x1e \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12g\n\x12impurityImportance\x18\x1f \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12j\n\x15permutationImportance\x18  \x03(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureImportance\x12X\n\x07runtime\x18! \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus\x12\x63\n\x14trainDatasetLocation\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18# \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18$ \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18% \x01(\x03\x12\x14\n\x0ctrainingRows\x18& \x01(\x05\x12\x13\n\x0btestingRows\x18\' \x01(\x05\x12\x16\n\x0evalidationRows\x18( \x01(\x05\x12\x16\n\x0e\x66\x61ilureMessage\x18* \x01(\t\x12\x10\n\x08progress\x18+ \x01(\x05\x12\x13\n\x0b\x64\x61tasetName\x18, \x01(\t\x12\x16\n\x0e\x64\x61taSourceName\x18- \x01(\t\x12X\n\x07serving\x18/ \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingStatus\x12\x13\n\x0btarFileHash\x18\x30 \x01(\t\x12^\n\x10trainingDataHash\x18\x31 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12g\n\x11trainingResources\x18\x32 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x66\n\x10testingResources\x18\x33 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x11\n\ttrainedBy\x18\x34 \x01(\t\x12K\n\x04logs\x18\x35 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12V\n\x08rocCurve\x18\x36 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.RocAucCurve\x12Q\n\x07prCurve\x18\x37 \x01(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.PRCurve\x12\x66\n\x14trainConfusionMatrix\x18\x38 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x65\n\x13testConfusionMatrix\x18\x39 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ConfusionMatrix\x12\x61\n\x16\x63orrelationsWithTarget\x18: \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12Z\n\x0ftopCorrelations\x18; \x03(\x0b\x32\x41.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.Correlation\x12=\n\tupdatedAt\x18< \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12V\n\x08\x61pproval\x18= \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.data.v1alpha1.ApprovalStatus\x12j\n\x10interpretability\x18> \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilityStatus\x12O\n\x06images\x18? \x01(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Images\x12\x61\n\x0funitTestResults\x18@ \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12\x65\n\x13\x66\x65\x65\x64\x62\x61\x63kTestResults\x18\x41 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuiteResult\x12]\n\x07groupby\x18\x42 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ModelGroupByStatus\x12[\n\x05usage\x18\x44 \x01(\x0b\x32L.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceConsumption\x12\x43\n\nconditions\x18\x45 \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xdf\x01\n\x0eModelTestSuite\x12=\n\x10\x62\x61selineModelRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x37\n\ndatasetRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12U\n\tunitTests\x18\x03 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\"/\n\x10NNLayerParameter\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"=\n\x10OutlierModelSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x18\n\x10outlierAlgorithm\x18\x02 \x01(\t\"\xcc\x01\n\x1bPartitionModelLocationsSpec\x12\x17\n\x0fpartitionFolder\x18\x01 \x01(\t\x12\x1e\n\x16partitionProfileFolder\x18\x02 \x01(\t\x12\x1b\n\x13partitionReportFile\x18\x03 \x01(\t\x12\x1c\n\x14partitionModelFolder\x18\x04 \x01(\t\x12\x1a\n\x12partitionModelFile\x18\x05 \x01(\t\x12\x1d\n\x15partitionForecastFile\x18\x06 \x01(\t\"\x84\x01\n\x17PercentilePrunerOptions\x12\x12\n\npercentile\x18\x01 \x01(\x05\x12\x15\n\rstartupTrials\x18\x02 \x01(\x05\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x16\n\x0eintervalTrials\x18\x04 \x01(\x05\x12\x11\n\tminTrials\x18\x05 \x01(\x05\"\x93\x04\n\nPrunerSpec\x12\x0c\n\x04type\x18\x01 \x01(\t\x12]\n\x06median\x18\x02 \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.MedianPrunerOptions\x12\x65\n\npercentile\x18\x03 \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PercentilePrunerOptions\x12m\n\x11successiveHalving\x18\x04 \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingOptions\x12]\n\thyperband\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.HyperbandOptions\x12\x63\n\tthreshold\x18\x06 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ThresholdPrunerOptions\"\xd0\x01\n\x18RegressionForecasterSpec\x12\x10\n\x08\x65nsemble\x18\x01 \x01(\x08\x12\x12\n\nimputation\x18\x02 \x01(\t\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x0f\n\x07scaling\x18\x04 \x01(\t\x12\x0c\n\x04\x64\x61te\x18\x05 \x01(\x08\x12\x0f\n\x07windows\x18\x06 \x03(\x05\x12\x0c\n\x04lags\x18\x07 \x03(\x05\x12\x11\n\tfunctions\x18\x08 \x03(\t\x12\x0b\n\x03\x65ma\x18\t \x01(\x08\x12\x0b\n\x03log\x18\n \x01(\x08\x12\x11\n\treduction\x18\x0b \x01(\t\"\xf8\x01\n\x06Report\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12R\n\x04spec\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportSpec\x12V\n\x06status\x18\x03 \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportStatus\"\x8a\x01\n\x13ReportGroupByStatus\x12\x12\n\nreportsURI\x18\x01 \x01(\t\x12_\n\rworkerResults\x18\x04 \x03(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.WorkerRunResult\"\x9f\x01\n\nReportList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12O\n\x05items\x18\x02 \x03(\x0b\x32@.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Report\"\xe9\x03\n\nReportSpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x36\n\tentityRef\x18\x02 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x12\n\nreportType\x18\x03 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12_\n\x0cnotification\x18\x05 \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12\r\n\x05owner\x18\x06 \x01(\t\x12X\n\tresources\x18\x07 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0f\n\x07timeout\x18\x08 \x01(\x03\x12\x33\n\x06labRef\x18\t \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x0b\n\x03key\x18\n \x03(\t\x12\x1a\n\x12\x61rtifactBucketName\x18\x0b \x01(\t\x12\x16\n\x0emodelClassName\x18\x0c \x01(\t\x12\x19\n\x11modelClassRunName\x18\r \x01(\t\"\xb3\x04\n\x0cReportStatus\x12?\n\x0b\x63ompletedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\r\n\x05phase\x18\x02 \x01(\t\x12W\n\x08location\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x1a\n\x12observedGeneration\x18\x04 \x01(\x03\x12\x15\n\rfailureReason\x18\x05 \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x06 \x01(\t\x12K\n\x04logs\x18\x07 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12=\n\tupdatedAt\x18\x08 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12^\n\x07groupby\x18\t \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ReportGroupByStatus\x12\x43\n\nconditions\x18\n \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\xde\x01\n\rRuntimeStatus\x12\x15\n\rpythonVersion\x18\x01 \x01(\t\x12\n\n\x02os\x18\x03 \x01(\t\x12s\n\x0epythonPackages\x18\x04 \x03(\x0b\x32[.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.RuntimeStatus.PythonPackagesEntry\x1a\x35\n\x13PythonPackagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x83\x05\n\nSearchSpec\x12\x0f\n\x07sampler\x18\x01 \x01(\t\x12T\n\x06pruner\x18\x02 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.PrunerSpec\x12\x0f\n\x07maxTime\x18\x04 \x01(\x05\x12\x11\n\tmaxModels\x18\x05 \x01(\x05\x12\x10\n\x08maxScore\x18\x06 \x01(\x01\x12\x10\n\x08trainers\x18\x07 \x01(\x05\x12\x0c\n\x04test\x18\x08 \x01(\x05\x12\x11\n\tretainTop\x18\t \x01(\x05\x12\x13\n\x0bretainedFor\x18\n \x01(\x05\x12g\n\x0bsearchSpace\x18\x0b \x01(\x0b\x32R.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.AlgorithmSearchSpaceSpec\x12Z\n\tearlyStop\x18\x0c \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EarlyStopSpec\x12Y\n\tobjective\x18\r \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x62\n\x12secondaryObjective\x18\x0e \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ObjectiveSpec\x12\x0c\n\x04goal\x18\x0f \x01(\t\"L\n\x15SeasonalityPeriodSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x61uto\x18\x02 \x01(\x08\x12\x14\n\x0c\x66ourierOrder\x18\x03 \x01(\x05\"\x87\x04\n\x0fSeasonalitySpec\x12\x0c\n\x04\x61uto\x18\x01 \x01(\x08\x12_\n\x06yearly\x18\x02 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12\x62\n\tquarterly\x18\x03 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12`\n\x07monthly\x18\x04 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12_\n\x06weekly\x18\x05 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\x12^\n\x05\x64\x61ily\x18\x06 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SeasonalityPeriodSpec\"\xb7\x03\n\x12ServingEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12Q\n\x05tests\x18\x02 \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12;\n\x0eservingSiteRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12S\n\x06\x61\x63\x63\x65ss\x18\x04 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\x05 \x01(\x05\x12\x0e\n\x06online\x18\x06 \x01(\x08\x12\x11\n\tdashboard\x18\x07 \x01(\x08\x12X\n\tresources\x18\x08 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0e\n\x06preSQL\x18\t \x03(\t\x12\x0f\n\x07postSQL\x18\n \x03(\t\"\xd2\x03\n\x0bServingSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12X\n\tresources\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12;\n\x0eservingSiteRef\x18\x06 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x11\n\tdashboard\x18\x08 \x01(\x08\x12S\n\x06\x61\x63\x63\x65ss\x18\t \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.AccessSpec\x12\x10\n\x08replicas\x18\n \x01(\x05\x12\x11\n\tpromotion\x18\x0c \x01(\t\x12\x37\n\napprovedBy\x18\r \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12>\n\napprovedAt\x18\x0e \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\x7f\n\rServingStatus\x12\x15\n\rpredictorName\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x61taAppName\x18\x03 \x01(\t\x12\x19\n\x11predictorEndpoint\x18\x04 \x01(\t\x12\x19\n\x11\x64\x61shboardEndpoint\x18\x05 \x01(\t\x12\x0c\n\x04role\x18\x06 \x01(\t\"\xf5\x01\n\x05Study\x12\x42\n\x08metadata\x18\x01 \x01(\x0b\x32\x30.k8s.io.apimachinery.pkg.apis.meta.v1.ObjectMeta\x12Q\n\x04spec\x18\x02 \x01(\x0b\x32\x43.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudySpec\x12U\n\x06status\x18\x03 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyStatus\"\x9d\x01\n\tStudyList\x12@\n\x08metadata\x18\x01 \x01(\x0b\x32..k8s.io.apimachinery.pkg.apis.meta.v1.ListMeta\x12N\n\x05items\x18\x02 \x03(\x0b\x32?.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.Study\"\xb4\x02\n\x10StudyPhaseStatus\x12=\n\tstartedAt\x18\x01 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x1a\n\x12waitingModelsCount\x18\x03 \x01(\x05\x12\x1a\n\x12runningModelsCount\x18\x04 \x01(\x05\x12\x19\n\x11\x66\x61iledModelsCount\x18\x05 \x01(\x05\x12\x1c\n\x14\x63ompletedModelsCount\x18\x06 \x01(\x05\x12\x11\n\tbestScore\x18\x07 \x01(\x01\x12\x1c\n\x14modelsWithNoProgress\x18\x08 \x01(\x05\"a\n\x11StudyScheduleSpec\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12;\n\x07startAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\"\xc5\x0e\n\tStudySpec\x12\x13\n\x0bversionName\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x33\n\x06labRef\x18\x03 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x13\n\x0b\x64\x61tasetName\x18\x04 \x01(\t\x12\x0c\n\x04task\x18\x05 \x01(\t\x12\x0f\n\x07subtask\x18\x06 \x01(\t\x12h\n\x08\x66\x65Search\x18\x07 \x01(\x0b\x32V.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSearchSpec\x12i\n\x10imbalanceHandler\x18\x08 \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ImbalanceHandlingSpec\x12X\n\x08\x62\x61seline\x18\t \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.BaselineSpec\x12T\n\x06search\x18\n \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SearchSpec\x12Z\n\tensembles\x18\x0b \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.EnsemblesSpec\x12`\n\x10trainingTemplate\x18\x0c \x01(\x0b\x32\x46.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.TrainingSpec\x12\x62\n\x10\x66orecastTemplate\x18\r \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ForecasterSpec\x12]\n\x08schedule\x18\x0e \x01(\x0b\x32K.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyScheduleSpec\x12h\n\x10interpretability\x18\x0f \x01(\x0b\x32N.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.InterpretabilitySpec\x12`\n\x0coutlierModel\x18\x10 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.OutlierModelSpec\x12\r\n\x05\x61\x62ort\x18\x11 \x01(\x08\x12\x0e\n\x06report\x18\x12 \x01(\x08\x12\r\n\x05pause\x18\x13 \x01(\x08\x12\x0f\n\x07profile\x18\x14 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x15 \x01(\x08\x12\x0c\n\x04\x66\x61st\x18\x16 \x01(\x08\x12\x1a\n\x12\x61rtifactBucketName\x18\x17 \x01(\t\x12\r\n\x05owner\x18\x18 \x01(\t\x12\x10\n\x08template\x18\x19 \x01(\x08\x12_\n\x0cnotification\x18\x1a \x01(\x0b\x32I.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.NotificationSpec\x12[\n\x02gc\x18\x1b \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionSpec\x12\x14\n\x0cmodelVersion\x18\x1c \x01(\t\x12\x0f\n\x07timeout\x18\x1d \x01(\x05\x12]\n\x11unitTestsTemplate\x18\x1e \x01(\x0b\x32\x42.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.TestSuite\x12i\n\x0egroupLocations\x18\x1f \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GroupSplitLocationsSpec\x12\x16\n\x0emodelClassName\x18  \x01(\t\x12\x19\n\x11modelClassRunName\x18! \x01(\t\x12V\n\x07serving\x18\" \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ServingSpec\"\xfe\x10\n\x0bStudyStatus\x12\x13\n\x0bmodelsCount\x18\x01 \x01(\x05\x12?\n\x0b\x63ompletedAt\x18\x02 \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12\x11\n\tbestModel\x18\x03 \x01(\t\x12\x16\n\x0e\x62\x65stModelScore\x18\x04 \x01(\x01\x12^\n\x0fprofileLocation\x18\x05 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12]\n\x0ereportLocation\x18\x06 \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x12\n\nreportName\x18\x07 \x01(\t\x12\r\n\x05phase\x18\x08 \x01(\t\x12\x1a\n\x12observedGeneration\x18\t \x01(\x03\x12\x63\n\x14trainDatasetLocation\x18\n \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x62\n\x13testDatasetLocation\x18\x0b \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12h\n\x19validationDatasetLocation\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12`\n\x11optimizerLocation\x18\r \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.FileLocation\x12\x13\n\x0blastModelID\x18\x0e \x01(\x03\x12\x15\n\rfailureReason\x18\x0f \x01(\t\x12\x16\n\x0e\x66\x61ilureMessage\x18\x10 \x01(\t\x12\x19\n\x11trainingRowsCount\x18\x11 \x01(\x05\x12\x18\n\x10testingRowsCount\x18\x12 \x01(\x05\x12\x1b\n\x13validationRowsCount\x18\x13 \x01(\x05\x12\x10\n\x08progress\x18\x14 \x01(\x05\x12^\n\x10trainingDataHash\x18\x15 \x01(\x0b\x32\x44.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataHashes\x12\x13\n\x0btriggeredBy\x18\x16 \x01(\t\x12K\n\x04logs\x18\x17 \x01(\x0b\x32=.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.Logs\x12\x66\n\x12\x66\x65\x61tureEngineering\x18\x18 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x62\x61seline\x18\x19 \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12Z\n\x06search\x18\x1a \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\\\n\x08\x65nsemble\x18\x1b \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12X\n\x04test\x18\x1c \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12[\n\x07\x65xplain\x18\x1d \x01(\x0b\x32J.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.StudyPhaseStatus\x12\x65\n\x0e\x64riftDetection\x18\x1e \x01(\x0b\x32M.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DriftDetectorStatus\x12=\n\tupdatedAt\x18\x1f \x01(\x0b\x32*.k8s.io.apimachinery.pkg.apis.meta.v1.Time\x12p\n\x16\x62\x65stFeatureEngineering\x18  \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.FeatureEngineeringSpec\x12]\n\x02gc\x18! \x01(\x0b\x32Q.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.GarbageCollectionStatus\x12\x43\n\nconditions\x18% \x03(\x0b\x32/.k8s.io.apimachinery.pkg.apis.meta.v1.Condition\"\x7f\n\x18SuccessiveHalvingOptions\x12\x14\n\x0cminResources\x18\x01 \x01(\x05\x12\x17\n\x0freductionFactor\x18\x02 \x01(\x05\x12\x1c\n\x14minEarlyStoppingRate\x18\x03 \x01(\x05\x12\x16\n\x0e\x62ootstrapCount\x18\x04 \x01(\x05\"h\n\x15SuccessiveHalvingSpec\x12\x0e\n\x06\x62udget\x18\x01 \x01(\x05\x12\x0f\n\x07\x62racket\x18\x02 \x01(\x05\x12\x0c\n\x04rung\x18\x03 \x01(\x05\x12\x0e\n\x06\x63onfID\x18\x04 \x01(\x05\x12\x10\n\x08modality\x18\x1a \x01(\t\"\xad\x01\n\x10TextPipelineSpec\x12\x0f\n\x07\x65ncoder\x18\x01 \x01(\t\x12\x11\n\ttokenizer\x18\x02 \x01(\t\x12\x11\n\tstopwords\x18\x03 \x01(\x08\x12\x0b\n\x03pos\x18\x04 \x01(\x08\x12\r\n\x05lemma\x18\x05 \x01(\x08\x12\x0c\n\x04stem\x18\x06 \x01(\x08\x12\x11\n\tembedding\x18\x07 \x01(\t\x12\x0b\n\x03svd\x18\x08 \x01(\x08\x12\x18\n\x10maxSvdComponents\x18\t \x01(\x05\"b\n\x16ThresholdPrunerOptions\x12\r\n\x05lower\x18\x01 \x01(\x01\x12\r\n\x05upper\x18\x02 \x01(\x01\x12\x13\n\x0bwarmupSteps\x18\x03 \x01(\x05\x12\x15\n\rintervalSteps\x18\x04 \x01(\x05\"\x8a\x01\n\x0fTimeSeriesEvent\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0f\n\x07holiday\x18\x03 \x01(\x08\x12\x0f\n\x07\x63ountry\x18\x04 \x01(\t\x12\x10\n\x08preEvent\x18\x05 \x01(\x05\x12\x11\n\tpostEvent\x18\x06 \x01(\x05\x12\x12\n\ntimePoints\x18\x07 \x03(\t\"\xe2\x04\n\x0cTrainingSpec\x12\x33\n\x06labRef\x18\x01 \x01(\x0b\x32#.k8s.io.api.core.v1.ObjectReference\x12\x10\n\x08priority\x18\x02 \x01(\t\x12\x0e\n\x06\x63vtype\x18\x03 \x01(\t\x12\r\n\x05\x66olds\x18\x05 \x01(\x05\x12V\n\x05split\x18\x06 \x01(\x0b\x32G.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.DataSplitSpec\x12\x13\n\x0b\x65valMetrics\x18\x07 \x03(\t\x12[\n\x02sh\x18\n \x01(\x0b\x32O.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.SuccessiveHalvingSpec\x12\x0c\n\x04seed\x18\x0b \x01(\x01\x12X\n\tresources\x18\x0c \x01(\x0b\x32\x45.github.com.metaprov.modelaapi.pkg.apis.catalog.v1alpha1.ResourceSpec\x12\x0b\n\x03gpu\x18\r \x01(\x08\x12\x19\n\x11\x66\x65\x61tureImportance\x18\x0f \x01(\x08\x12\x11\n\tsamplePct\x18\x11 \x01(\x05\x12\\\n\ncheckpoint\x18\x12 \x01(\x0b\x32H.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.CheckpointSpec\x12\x10\n\x08logLevel\x18\x13 \x01(\t\x12\x0f\n\x07timeout\x18\x14 \x01(\x05\"\xdc\x01\n\x18UnivariateForecastStatus\x12\x1b\n\x13gridSearchResultURI\x18\x01 \x01(\t\x12g\n\rbaseEstimator\x18\x02 \x01(\x0b\x32P.github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.ClassicalEstimatorSpec\x12\x10\n\x08modelURI\x18\x03 \x01(\t\x12\x13\n\x0b\x63vResultURI\x18\x04 \x01(\t\x12\x13\n\x0b\x66orecastURI\x18\x05 \x01(\t\"\'\n\x11VideoPipelineSpec\x12\x12\n\nfeaturizer\x18\x01 \x01(\t\"=\n\nWindowSpec\x12\x10\n\x08interval\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x05\x12\x0e\n\x06length\x18\x03 \x01(\x05\x42:Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.pkg.apis.training.v1alpha1.generated_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z8github.com/metaprov/modelaapi/pkg/apis/training/v1alpha1'
@@ -122,99 +122,99 @@
   _MODELCLASSRUN._serialized_start=8420
   _MODELCLASSRUN._serialized_end=8689
   _MODELCLASSRUNLIST._serialized_start=8692
   _MODELCLASSRUNLIST._serialized_end=8865
   _MODELCLASSRUNSPEC._serialized_start=8868
   _MODELCLASSRUNSPEC._serialized_end=9074
   _MODELCLASSRUNSTATUS._serialized_start=9077
-  _MODELCLASSRUNSTATUS._serialized_end=9698
-  _MODELCLASSSERVINGSPEC._serialized_start=9701
-  _MODELCLASSSERVINGSPEC._serialized_end=10042
-  _MODELCLASSSPEC._serialized_start=10045
-  _MODELCLASSSPEC._serialized_end=10886
-  _MODELCLASSSTATUS._serialized_start=10889
-  _MODELCLASSSTATUS._serialized_end=12016
-  _MODELCLASSTRAININGSPEC._serialized_start=12019
-  _MODELCLASSTRAININGSPEC._serialized_end=12666
-  _MODELGROUPBYSTATUS._serialized_start=12669
-  _MODELGROUPBYSTATUS._serialized_end=12848
-  _MODELLIST._serialized_start=12851
-  _MODELLIST._serialized_end=13008
-  _MODELRESULT._serialized_start=13010
-  _MODELRESULT._serialized_end=13103
-  _MODELSPEC._serialized_start=13106
-  _MODELSPEC._serialized_end=14663
-  _MODELSTAGESTATUS._serialized_start=14666
-  _MODELSTAGESTATUS._serialized_end=14941
-  _MODELSTATUS._serialized_start=14944
-  _MODELSTATUS._serialized_end=19403
-  _MODELTESTSUITE._serialized_start=19406
-  _MODELTESTSUITE._serialized_end=19629
-  _NNLAYERPARAMETER._serialized_start=19631
-  _NNLAYERPARAMETER._serialized_end=19678
-  _OUTLIERMODELSPEC._serialized_start=19680
-  _OUTLIERMODELSPEC._serialized_end=19741
-  _PARTITIONMODELLOCATIONSSPEC._serialized_start=19744
-  _PARTITIONMODELLOCATIONSSPEC._serialized_end=19948
-  _PERCENTILEPRUNEROPTIONS._serialized_start=19951
-  _PERCENTILEPRUNEROPTIONS._serialized_end=20083
-  _PRUNERSPEC._serialized_start=20086
-  _PRUNERSPEC._serialized_end=20617
-  _REGRESSIONFORECASTERSPEC._serialized_start=20620
-  _REGRESSIONFORECASTERSPEC._serialized_end=20828
-  _REPORT._serialized_start=20831
-  _REPORT._serialized_end=21079
-  _REPORTGROUPBYSTATUS._serialized_start=21082
-  _REPORTGROUPBYSTATUS._serialized_end=21220
-  _REPORTLIST._serialized_start=21223
-  _REPORTLIST._serialized_end=21382
-  _REPORTSPEC._serialized_start=21385
-  _REPORTSPEC._serialized_end=21874
-  _REPORTSTATUS._serialized_start=21877
-  _REPORTSTATUS._serialized_end=22440
-  _RUNTIMESTATUS._serialized_start=22443
-  _RUNTIMESTATUS._serialized_end=22665
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=22612
-  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=22665
-  _SEARCHSPEC._serialized_start=22668
-  _SEARCHSPEC._serialized_end=23311
-  _SEASONALITYPERIODSPEC._serialized_start=23313
-  _SEASONALITYPERIODSPEC._serialized_end=23389
-  _SEASONALITYSPEC._serialized_start=23392
-  _SEASONALITYSPEC._serialized_end=23911
-  _SERVINGENVIRONMENT._serialized_start=23914
-  _SERVINGENVIRONMENT._serialized_end=24353
-  _SERVINGSPEC._serialized_start=24356
-  _SERVINGSPEC._serialized_end=24822
-  _SERVINGSTATUS._serialized_start=24824
-  _SERVINGSTATUS._serialized_end=24951
-  _STUDY._serialized_start=24954
-  _STUDY._serialized_end=25199
-  _STUDYLIST._serialized_start=25202
-  _STUDYLIST._serialized_end=25359
-  _STUDYPHASESTATUS._serialized_start=25362
-  _STUDYPHASESTATUS._serialized_end=25670
-  _STUDYSCHEDULESPEC._serialized_start=25672
-  _STUDYSCHEDULESPEC._serialized_end=25769
-  _STUDYSPEC._serialized_start=25772
-  _STUDYSPEC._serialized_end=27633
-  _STUDYSTATUS._serialized_start=27636
-  _STUDYSTATUS._serialized_end=29810
-  _SUCCESSIVEHALVINGOPTIONS._serialized_start=29812
-  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29939
-  _SUCCESSIVEHALVINGSPEC._serialized_start=29941
-  _SUCCESSIVEHALVINGSPEC._serialized_end=30045
-  _TEXTPIPELINESPEC._serialized_start=30048
-  _TEXTPIPELINESPEC._serialized_end=30221
-  _THRESHOLDPRUNEROPTIONS._serialized_start=30223
-  _THRESHOLDPRUNEROPTIONS._serialized_end=30321
-  _TIMESERIESEVENT._serialized_start=30324
-  _TIMESERIESEVENT._serialized_end=30462
-  _TRAININGSPEC._serialized_start=30465
-  _TRAININGSPEC._serialized_end=31075
-  _UNIVARIATEFORECASTSTATUS._serialized_start=31078
-  _UNIVARIATEFORECASTSTATUS._serialized_end=31298
-  _VIDEOPIPELINESPEC._serialized_start=31300
-  _VIDEOPIPELINESPEC._serialized_end=31339
-  _WINDOWSPEC._serialized_start=31341
-  _WINDOWSPEC._serialized_end=31402
+  _MODELCLASSRUNSTATUS._serialized_end=9675
+  _MODELCLASSSERVINGSPEC._serialized_start=9678
+  _MODELCLASSSERVINGSPEC._serialized_end=10019
+  _MODELCLASSSPEC._serialized_start=10022
+  _MODELCLASSSPEC._serialized_end=10863
+  _MODELCLASSSTATUS._serialized_start=10866
+  _MODELCLASSSTATUS._serialized_end=11993
+  _MODELCLASSTRAININGSPEC._serialized_start=11996
+  _MODELCLASSTRAININGSPEC._serialized_end=12643
+  _MODELGROUPBYSTATUS._serialized_start=12646
+  _MODELGROUPBYSTATUS._serialized_end=12825
+  _MODELLIST._serialized_start=12828
+  _MODELLIST._serialized_end=12985
+  _MODELRESULT._serialized_start=12987
+  _MODELRESULT._serialized_end=13080
+  _MODELSPEC._serialized_start=13083
+  _MODELSPEC._serialized_end=14593
+  _MODELSTAGESTATUS._serialized_start=14596
+  _MODELSTAGESTATUS._serialized_end=14871
+  _MODELSTATUS._serialized_start=14874
+  _MODELSTATUS._serialized_end=19340
+  _MODELTESTSUITE._serialized_start=19343
+  _MODELTESTSUITE._serialized_end=19566
+  _NNLAYERPARAMETER._serialized_start=19568
+  _NNLAYERPARAMETER._serialized_end=19615
+  _OUTLIERMODELSPEC._serialized_start=19617
+  _OUTLIERMODELSPEC._serialized_end=19678
+  _PARTITIONMODELLOCATIONSSPEC._serialized_start=19681
+  _PARTITIONMODELLOCATIONSSPEC._serialized_end=19885
+  _PERCENTILEPRUNEROPTIONS._serialized_start=19888
+  _PERCENTILEPRUNEROPTIONS._serialized_end=20020
+  _PRUNERSPEC._serialized_start=20023
+  _PRUNERSPEC._serialized_end=20554
+  _REGRESSIONFORECASTERSPEC._serialized_start=20557
+  _REGRESSIONFORECASTERSPEC._serialized_end=20765
+  _REPORT._serialized_start=20768
+  _REPORT._serialized_end=21016
+  _REPORTGROUPBYSTATUS._serialized_start=21019
+  _REPORTGROUPBYSTATUS._serialized_end=21157
+  _REPORTLIST._serialized_start=21160
+  _REPORTLIST._serialized_end=21319
+  _REPORTSPEC._serialized_start=21322
+  _REPORTSPEC._serialized_end=21811
+  _REPORTSTATUS._serialized_start=21814
+  _REPORTSTATUS._serialized_end=22377
+  _RUNTIMESTATUS._serialized_start=22380
+  _RUNTIMESTATUS._serialized_end=22602
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_start=22549
+  _RUNTIMESTATUS_PYTHONPACKAGESENTRY._serialized_end=22602
+  _SEARCHSPEC._serialized_start=22605
+  _SEARCHSPEC._serialized_end=23248
+  _SEASONALITYPERIODSPEC._serialized_start=23250
+  _SEASONALITYPERIODSPEC._serialized_end=23326
+  _SEASONALITYSPEC._serialized_start=23329
+  _SEASONALITYSPEC._serialized_end=23848
+  _SERVINGENVIRONMENT._serialized_start=23851
+  _SERVINGENVIRONMENT._serialized_end=24290
+  _SERVINGSPEC._serialized_start=24293
+  _SERVINGSPEC._serialized_end=24759
+  _SERVINGSTATUS._serialized_start=24761
+  _SERVINGSTATUS._serialized_end=24888
+  _STUDY._serialized_start=24891
+  _STUDY._serialized_end=25136
+  _STUDYLIST._serialized_start=25139
+  _STUDYLIST._serialized_end=25296
+  _STUDYPHASESTATUS._serialized_start=25299
+  _STUDYPHASESTATUS._serialized_end=25607
+  _STUDYSCHEDULESPEC._serialized_start=25609
+  _STUDYSCHEDULESPEC._serialized_end=25706
+  _STUDYSPEC._serialized_start=25709
+  _STUDYSPEC._serialized_end=27570
+  _STUDYSTATUS._serialized_start=27573
+  _STUDYSTATUS._serialized_end=29747
+  _SUCCESSIVEHALVINGOPTIONS._serialized_start=29749
+  _SUCCESSIVEHALVINGOPTIONS._serialized_end=29876
+  _SUCCESSIVEHALVINGSPEC._serialized_start=29878
+  _SUCCESSIVEHALVINGSPEC._serialized_end=29982
+  _TEXTPIPELINESPEC._serialized_start=29985
+  _TEXTPIPELINESPEC._serialized_end=30158
+  _THRESHOLDPRUNEROPTIONS._serialized_start=30160
+  _THRESHOLDPRUNEROPTIONS._serialized_end=30258
+  _TIMESERIESEVENT._serialized_start=30261
+  _TIMESERIESEVENT._serialized_end=30399
+  _TRAININGSPEC._serialized_start=30402
+  _TRAININGSPEC._serialized_end=31012
+  _UNIVARIATEFORECASTSTATUS._serialized_start=31015
+  _UNIVARIATEFORECASTSTATUS._serialized_end=31235
+  _VIDEOPIPELINESPEC._serialized_start=31237
+  _VIDEOPIPELINESPEC._serialized_end=31276
+  _WINDOWSPEC._serialized_start=31278
+  _WINDOWSPEC._serialized_end=31339
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from protoc_gen_swagger.options import annotations_pb2 as protoc__gen__swagger_dot_options_dot_annotations__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nYgithub.com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice.proto\x12>github.com.metaprov.modelaapi.services.grpcinferenceservice.v1\x1a,protoc-gen-swagger/options/annotations.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x17\n\x15ServerShutdownRequest\"\x18\n\x16ServerShutdownResponse\"\x13\n\x11ServerLiveRequest\"\"\n\x12ServerLiveResponse\x12\x0c\n\x04live\x18\x01 \x01(\x08\"\x14\n\x12ServerReadyRequest\"$\n\x13ServerReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"2\n\x11ModelReadyRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"#\n\x12ModelReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"\x17\n\x15ServerMetadataRequest\"K\n\x16ServerMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\nextensions\x18\x03 \x03(\t\"5\n\x14ModelMetadataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\xf7\x02\n\x15ModelMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08versions\x18\x02 \x03(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\x12t\n\x06inputs\x18\x04 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataResponse.TensorMetadata\x12u\n\x07outputs\x18\x05 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataResponse.TensorMetadata\x1a?\n\x0eTensorMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\"\xd0\n\n\x11ModelInferRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12u\n\nparameters\x18\x04 \x03(\x0b\x32\x61.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.ParametersEntry\x12r\n\x06inputs\x18\x05 \x03(\x0b\x32\x62.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferInputTensor\x12}\n\x07outputs\x18\x06 \x03(\x0b\x32l.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferRequestedOutputTensor\x12\x1a\n\x12raw_input_contents\x18\x07 \x03(\x0c\x1a\xb5\x03\n\x10InferInputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\x12\x86\x01\n\nparameters\x18\x04 \x03(\x0b\x32r.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferInputTensor.ParametersEntry\x12\x65\n\x08\x63ontents\x18\x05 \x01(\x0b\x32S.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferTensorContents\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\x1a\xc1\x02\n\x1aInferRequestedOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x90\x01\n\nparameters\x18\x02 \x03(\x0b\x32|.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferRequestedOutputTensor.ParametersEntry\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\"\x96\x07\n\x12ModelInferResponse\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12v\n\nparameters\x18\x04 \x03(\x0b\x32\x62.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse.ParametersEntry\x12u\n\x07outputs\x18\x05 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse.InferOutputTensor\x12\x1b\n\x13raw_output_contents\x18\x06 \x03(\x0c\x1a\xb8\x03\n\x11InferOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\x12\x88\x01\n\nparameters\x18\x04 \x03(\x0b\x32t.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse.InferOutputTensor.ParametersEntry\x12\x65\n\x08\x63ontents\x18\x05 \x01(\x0b\x32S.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferTensorContents\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\"i\n\x0eInferParameter\x12\x14\n\nbool_param\x18\x01 \x01(\x08H\x00\x12\x15\n\x0bint64_param\x18\x02 \x01(\x03H\x00\x12\x16\n\x0cstring_param\x18\x03 \x01(\tH\x00\x42\x12\n\x10parameter_choice\"\xd0\x01\n\x13InferTensorContents\x12\x15\n\rbool_contents\x18\x01 \x03(\x08\x12\x14\n\x0cint_contents\x18\x02 \x03(\x05\x12\x16\n\x0eint64_contents\x18\x03 \x03(\x03\x12\x15\n\ruint_contents\x18\x04 \x03(\r\x12\x17\n\x0fuint64_contents\x18\x05 \x03(\x04\x12\x15\n\rfp32_contents\x18\x06 \x03(\x02\x12\x15\n\rfp64_contents\x18\x07 \x03(\x01\x12\x16\n\x0e\x62ytes_contents\x18\x08 \x03(\x0c\"\xf5\x01\n\rPredictorInfo\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12Y\n\x06models\x18\x04 \x03(\x0b\x32I.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInfo\x12Z\n\x06schema\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.SchemaInfo\"\xbb\x02\n\tModelInfo\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0f\n\x07product\x18\x04 \x01(\t\x12\x16\n\x0etrainingMetric\x18\x05 \x01(\t\x12\x15\n\rtrainingScore\x18\x06 \x01(\x02\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x0e\n\x06\x63\x61nary\x18\x08 \x01(\x08\x12\x0e\n\x06shadow\x18\t \x01(\x08\x12\x0f\n\x07traffic\x18\n \x01(\x02\x12\x0e\n\x06\x66ilter\x18\x0b \x01(\t\x12\x0c\n\x04rank\x18\x0c \x01(\x03\x12\x0f\n\x07logPath\x18\r \x01(\t\x12\x0b\n\x03p95\x18\x0e \x01(\x02\x12\x0b\n\x03p99\x18\x0f \x01(\x02\x12\x16\n\x0elastPrediction\x18\x10 \x01(\x03\x12\x1a\n\x12\x64\x61ilyPredictionAvg\x18\x11 \x01(\x05\"i\n\nSchemaInfo\x12[\n\x07\x63olumns\x18\x01 \x03(\x0b\x32J.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ColumnInfo\"|\n\nColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x12\n\ndatasetMin\x18\x03 \x01(\x02\x12\x13\n\x0b\x64\x61tasetMean\x18\x04 \x01(\x02\x12\x15\n\rdatasetStdDev\x18\x05 \x01(\x02\x12\x12\n\ndatasetMax\x18\x06 \x01(\x02\"\x15\n\x13GetPredictorRequest\"s\n\x14GetPredictorResponse\x12[\n\x04item\x18\x01 \x01(\x0b\x32M.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictorInfo\"\x1f\n\x0fGetModelRequest\x12\x0c\n\x04name\x18\x03 \x01(\t\"k\n\x10GetModelResponse\x12W\n\x04item\x18\x01 \x01(\x0b\x32I.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInfo\"\x9f\x01\n\x0ePredictRequest\x12\x11\n\tpredictor\x18\x01 \x01(\t\x12\x10\n\x08validate\x18\x02 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x0f\n\x07payload\x18\x05 \x01(\t\x12\x0f\n\x07labeled\x18\x06 \x01(\x08\x12\x0f\n\x07metrics\x18\x07 \x03(\t\x12\x14\n\x0cmodelversion\x18\x08 \x01(\t\"\x93\x02\n\x0fPredictResponse\x12\x64\n\x05items\x18\x01 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictResultLineItem\x12k\n\x06scores\x18\x02 \x03(\x0b\x32[.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictResponse.ScoresEntry\x1a-\n\x0bScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xe6\x02\n\x15PredictResultLineItem\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05score\x18\x02 \x01(\x02\x12\r\n\x05label\x18\x03 \x01(\t\x12g\n\rprobabilities\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ProbabilityValue\x12\x16\n\x0emissingColumns\x18\x05 \x03(\t\x12\x12\n\noutOfBound\x18\x06 \x03(\t\x12\x15\n\rbaseShapValue\x18\x07 \x01(\x02\x12]\n\nshapValues\x18\x08 \x03(\x0b\x32I.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ShapValue\x12\x13\n\x0bprobability\x18\t \x01(\x02\"6\n\x10ProbabilityValue\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0bprobability\x18\x02 \x01(\x02\"+\n\tShapValue\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\x32\xae\x0f\n\x14GRPCInferenceService\x12\xb5\x01\n\nServerLive\x12Q.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerLiveRequest\x1aR.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerLiveResponse\"\x00\x12\xb8\x01\n\x0bServerReady\x12R.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerReadyRequest\x1aS.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerReadyResponse\"\x00\x12\xb5\x01\n\nModelReady\x12Q.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelReadyRequest\x1aR.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelReadyResponse\"\x00\x12\xc1\x01\n\x0eServerMetadata\x12U.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerMetadataRequest\x1aV.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerMetadataResponse\"\x00\x12\xbe\x01\n\rModelMetadata\x12T.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataRequest\x1aU.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataResponse\"\x00\x12\xb5\x01\n\nModelInfer\x12Q.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest\x1aR.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse\"\x00\x12\xd0\x01\n\x0cGetPredictor\x12S.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetPredictorRequest\x1aT.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetPredictorResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v1/predictor\x12\xc8\x01\n\x08GetModel\x12O.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetModelRequest\x1aP.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetModelResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/models/{name}\x12\xd1\x01\n\x07Predict\x12N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictRequest\x1aO.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictResponse\"%\x82\xd3\xe4\x93\x02\x1f\"\x1a/v1/predictors/{predictor}:\x01*\x12\xbb\x01\n\x08Shutdown\x12U.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerShutdownRequest\x1aV.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerShutdownResponse\"\x00\x42\x9e\x03\n!io.modela.grpcinferenceservice.v1B\x14GrpcInferenceServiceZ>github.com/metaprov/modelaapi/services/grpcinferenceservice/v1\xaa\x02\x1dModela.Client.Autogen.Grpc.v1\x92\x41\x81\x02\x12\x61\n\x14GrpcInferenceService\"D\n\x0emodela authors\x12\x11https://modela.ai\x1a\x1fmodela-discuss@googlegroups.com2\x03\x31.0*\x02\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonR;\n\x03\x34\x30\x34\x12\x34\n*Returned when the resource does not exist.\x12\x06\n\x04\x9a\x02\x01\x07r7\n\x17modela.ai documentation\x12\x1chttps://modela.ai/site/docs/b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\nYgithub.com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice.proto\x12>github.com.metaprov.modelaapi.services.grpcinferenceservice.v1\x1a,protoc-gen-swagger/options/annotations.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x17\n\x15ServerShutdownRequest\"\x18\n\x16ServerShutdownResponse\"\x13\n\x11ServerLiveRequest\"\"\n\x12ServerLiveResponse\x12\x0c\n\x04live\x18\x01 \x01(\x08\"\x14\n\x12ServerReadyRequest\"$\n\x13ServerReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"2\n\x11ModelReadyRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"#\n\x12ModelReadyResponse\x12\r\n\x05ready\x18\x01 \x01(\x08\"\x17\n\x15ServerMetadataRequest\"K\n\x16ServerMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x12\n\nextensions\x18\x03 \x03(\t\"5\n\x14ModelMetadataRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\"\xf7\x02\n\x15ModelMetadataResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08versions\x18\x02 \x03(\t\x12\x10\n\x08platform\x18\x03 \x01(\t\x12t\n\x06inputs\x18\x04 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataResponse.TensorMetadata\x12u\n\x07outputs\x18\x05 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataResponse.TensorMetadata\x1a?\n\x0eTensorMetadata\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\"\xd0\n\n\x11ModelInferRequest\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12u\n\nparameters\x18\x04 \x03(\x0b\x32\x61.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.ParametersEntry\x12r\n\x06inputs\x18\x05 \x03(\x0b\x32\x62.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferInputTensor\x12}\n\x07outputs\x18\x06 \x03(\x0b\x32l.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferRequestedOutputTensor\x12\x1a\n\x12raw_input_contents\x18\x07 \x03(\x0c\x1a\xb5\x03\n\x10InferInputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\x12\x86\x01\n\nparameters\x18\x04 \x03(\x0b\x32r.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferInputTensor.ParametersEntry\x12\x65\n\x08\x63ontents\x18\x05 \x01(\x0b\x32S.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferTensorContents\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\x1a\xc1\x02\n\x1aInferRequestedOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x90\x01\n\nparameters\x18\x02 \x03(\x0b\x32|.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest.InferRequestedOutputTensor.ParametersEntry\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\"\x96\x07\n\x12ModelInferResponse\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\t\x12v\n\nparameters\x18\x04 \x03(\x0b\x32\x62.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse.ParametersEntry\x12u\n\x07outputs\x18\x05 \x03(\x0b\x32\x64.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse.InferOutputTensor\x12\x1b\n\x13raw_output_contents\x18\x06 \x03(\x0c\x1a\xb8\x03\n\x11InferOutputTensor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tatype\x18\x02 \x01(\t\x12\r\n\x05shape\x18\x03 \x03(\x03\x12\x88\x01\n\nparameters\x18\x04 \x03(\x0b\x32t.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse.InferOutputTensor.ParametersEntry\x12\x65\n\x08\x63ontents\x18\x05 \x01(\x0b\x32S.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferTensorContents\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\x1a\x81\x01\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12]\n\x05value\x18\x02 \x01(\x0b\x32N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.InferParameter:\x02\x38\x01\"i\n\x0eInferParameter\x12\x14\n\nbool_param\x18\x01 \x01(\x08H\x00\x12\x15\n\x0bint64_param\x18\x02 \x01(\x03H\x00\x12\x16\n\x0cstring_param\x18\x03 \x01(\tH\x00\x42\x12\n\x10parameter_choice\"\xd0\x01\n\x13InferTensorContents\x12\x15\n\rbool_contents\x18\x01 \x03(\x08\x12\x14\n\x0cint_contents\x18\x02 \x03(\x05\x12\x16\n\x0eint64_contents\x18\x03 \x03(\x03\x12\x15\n\ruint_contents\x18\x04 \x03(\r\x12\x17\n\x0fuint64_contents\x18\x05 \x03(\x04\x12\x15\n\rfp32_contents\x18\x06 \x03(\x02\x12\x15\n\rfp64_contents\x18\x07 \x03(\x01\x12\x16\n\x0e\x62ytes_contents\x18\x08 \x03(\x0c\"\xf5\x01\n\rPredictorInfo\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04task\x18\x03 \x01(\t\x12Y\n\x06models\x18\x04 \x03(\x0b\x32I.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInfo\x12Z\n\x06schema\x18\x05 \x01(\x0b\x32J.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.SchemaInfo\"\xbb\x02\n\tModelInfo\x12\x11\n\tnamespace\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x0f\n\x07product\x18\x04 \x01(\t\x12\x16\n\x0etrainingMetric\x18\x05 \x01(\t\x12\x15\n\rtrainingScore\x18\x06 \x01(\x02\x12\x0e\n\x06status\x18\x07 \x01(\t\x12\x0e\n\x06\x63\x61nary\x18\x08 \x01(\x08\x12\x0e\n\x06shadow\x18\t \x01(\x08\x12\x0f\n\x07traffic\x18\n \x01(\x02\x12\x0e\n\x06\x66ilter\x18\x0b \x01(\t\x12\x0c\n\x04rank\x18\x0c \x01(\x03\x12\x0f\n\x07logPath\x18\r \x01(\t\x12\x0b\n\x03p95\x18\x0e \x01(\x02\x12\x0b\n\x03p99\x18\x0f \x01(\x02\x12\x16\n\x0elastPrediction\x18\x10 \x01(\x03\x12\x1a\n\x12\x64\x61ilyPredictionAvg\x18\x11 \x01(\x05\"i\n\nSchemaInfo\x12[\n\x07\x63olumns\x18\x01 \x03(\x0b\x32J.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ColumnInfo\"(\n\nColumnInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x15\n\x13GetPredictorRequest\"s\n\x14GetPredictorResponse\x12[\n\x04item\x18\x01 \x01(\x0b\x32M.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictorInfo\"\x1f\n\x0fGetModelRequest\x12\x0c\n\x04name\x18\x03 \x01(\t\"k\n\x10GetModelResponse\x12W\n\x04item\x18\x01 \x01(\x0b\x32I.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInfo\"\x9f\x01\n\x0ePredictRequest\x12\x11\n\tpredictor\x18\x01 \x01(\t\x12\x10\n\x08validate\x18\x02 \x01(\x08\x12\x0f\n\x07\x65xplain\x18\x03 \x01(\x08\x12\x0e\n\x06\x66ormat\x18\x04 \x01(\t\x12\x0f\n\x07payload\x18\x05 \x01(\t\x12\x0f\n\x07labeled\x18\x06 \x01(\x08\x12\x0f\n\x07metrics\x18\x07 \x03(\t\x12\x14\n\x0cmodelversion\x18\x08 \x01(\t\"\x93\x02\n\x0fPredictResponse\x12\x64\n\x05items\x18\x01 \x03(\x0b\x32U.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictResultLineItem\x12k\n\x06scores\x18\x02 \x03(\x0b\x32[.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictResponse.ScoresEntry\x1a-\n\x0bScoresEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\"\xe6\x02\n\x15PredictResultLineItem\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05score\x18\x02 \x01(\x02\x12\r\n\x05label\x18\x03 \x01(\t\x12g\n\rprobabilities\x18\x04 \x03(\x0b\x32P.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ProbabilityValue\x12\x16\n\x0emissingColumns\x18\x05 \x03(\t\x12\x12\n\noutOfBound\x18\x06 \x03(\t\x12\x15\n\rbaseShapValue\x18\x07 \x01(\x02\x12]\n\nshapValues\x18\x08 \x03(\x0b\x32I.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ShapValue\x12\x13\n\x0bprobability\x18\t \x01(\x02\"6\n\x10ProbabilityValue\x12\r\n\x05label\x18\x01 \x01(\t\x12\x13\n\x0bprobability\x18\x02 \x01(\x02\"+\n\tShapValue\x12\x0f\n\x07\x66\x65\x61ture\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x02\x32\xae\x0f\n\x14GRPCInferenceService\x12\xb5\x01\n\nServerLive\x12Q.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerLiveRequest\x1aR.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerLiveResponse\"\x00\x12\xb8\x01\n\x0bServerReady\x12R.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerReadyRequest\x1aS.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerReadyResponse\"\x00\x12\xb5\x01\n\nModelReady\x12Q.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelReadyRequest\x1aR.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelReadyResponse\"\x00\x12\xc1\x01\n\x0eServerMetadata\x12U.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerMetadataRequest\x1aV.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerMetadataResponse\"\x00\x12\xbe\x01\n\rModelMetadata\x12T.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataRequest\x1aU.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelMetadataResponse\"\x00\x12\xb5\x01\n\nModelInfer\x12Q.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferRequest\x1aR.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ModelInferResponse\"\x00\x12\xd0\x01\n\x0cGetPredictor\x12S.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetPredictorRequest\x1aT.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetPredictorResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v1/predictor\x12\xc8\x01\n\x08GetModel\x12O.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetModelRequest\x1aP.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.GetModelResponse\"\x19\x82\xd3\xe4\x93\x02\x13\x12\x11/v1/models/{name}\x12\xd1\x01\n\x07Predict\x12N.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictRequest\x1aO.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.PredictResponse\"%\x82\xd3\xe4\x93\x02\x1f\"\x1a/v1/predictors/{predictor}:\x01*\x12\xbb\x01\n\x08Shutdown\x12U.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerShutdownRequest\x1aV.github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.ServerShutdownResponse\"\x00\x42\x9e\x03\n!io.modela.grpcinferenceservice.v1B\x14GrpcInferenceServiceZ>github.com/metaprov/modelaapi/services/grpcinferenceservice/v1\xaa\x02\x1dModela.Client.Autogen.Grpc.v1\x92\x41\x81\x02\x12\x61\n\x14GrpcInferenceService\"D\n\x0emodela authors\x12\x11https://modela.ai\x1a\x1fmodela-discuss@googlegroups.com2\x03\x31.0*\x02\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonR;\n\x03\x34\x30\x34\x12\x34\n*Returned when the resource does not exist.\x12\x06\n\x04\x9a\x02\x01\x07r7\n\x17modela.ai documentation\x12\x1chttps://modela.ai/site/docs/b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'github.com.metaprov.modelaapi.services.grpcinferenceservice.v1.grpcinferenceservice_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n!io.modela.grpcinferenceservice.v1B\024GrpcInferenceServiceZ>github.com/metaprov/modelaapi/services/grpcinferenceservice/v1\252\002\035Modela.Client.Autogen.Grpc.v1\222A\201\002\022a\n\024GrpcInferenceService\"D\n\016modela authors\022\021https://modela.ai\032\037modela-discuss@googlegroups.com2\0031.0*\002\001\0022\020application/json:\020application/jsonR;\n\003404\0224\n*Returned when the resource does not exist.\022\006\n\004\232\002\001\007r7\n\027modela.ai documentation\022\034https://modela.ai/site/docs/'
@@ -95,31 +95,31 @@
   _PREDICTORINFO._serialized_start=3658
   _PREDICTORINFO._serialized_end=3903
   _MODELINFO._serialized_start=3906
   _MODELINFO._serialized_end=4221
   _SCHEMAINFO._serialized_start=4223
   _SCHEMAINFO._serialized_end=4328
   _COLUMNINFO._serialized_start=4330
-  _COLUMNINFO._serialized_end=4454
-  _GETPREDICTORREQUEST._serialized_start=4456
-  _GETPREDICTORREQUEST._serialized_end=4477
-  _GETPREDICTORRESPONSE._serialized_start=4479
-  _GETPREDICTORRESPONSE._serialized_end=4594
-  _GETMODELREQUEST._serialized_start=4596
-  _GETMODELREQUEST._serialized_end=4627
-  _GETMODELRESPONSE._serialized_start=4629
-  _GETMODELRESPONSE._serialized_end=4736
-  _PREDICTREQUEST._serialized_start=4739
-  _PREDICTREQUEST._serialized_end=4898
-  _PREDICTRESPONSE._serialized_start=4901
-  _PREDICTRESPONSE._serialized_end=5176
-  _PREDICTRESPONSE_SCORESENTRY._serialized_start=5131
-  _PREDICTRESPONSE_SCORESENTRY._serialized_end=5176
-  _PREDICTRESULTLINEITEM._serialized_start=5179
-  _PREDICTRESULTLINEITEM._serialized_end=5537
-  _PROBABILITYVALUE._serialized_start=5539
-  _PROBABILITYVALUE._serialized_end=5593
-  _SHAPVALUE._serialized_start=5595
-  _SHAPVALUE._serialized_end=5638
-  _GRPCINFERENCESERVICE._serialized_start=5641
-  _GRPCINFERENCESERVICE._serialized_end=7607
+  _COLUMNINFO._serialized_end=4370
+  _GETPREDICTORREQUEST._serialized_start=4372
+  _GETPREDICTORREQUEST._serialized_end=4393
+  _GETPREDICTORRESPONSE._serialized_start=4395
+  _GETPREDICTORRESPONSE._serialized_end=4510
+  _GETMODELREQUEST._serialized_start=4512
+  _GETMODELREQUEST._serialized_end=4543
+  _GETMODELRESPONSE._serialized_start=4545
+  _GETMODELRESPONSE._serialized_end=4652
+  _PREDICTREQUEST._serialized_start=4655
+  _PREDICTREQUEST._serialized_end=4814
+  _PREDICTRESPONSE._serialized_start=4817
+  _PREDICTRESPONSE._serialized_end=5092
+  _PREDICTRESPONSE_SCORESENTRY._serialized_start=5047
+  _PREDICTRESPONSE_SCORESENTRY._serialized_end=5092
+  _PREDICTRESULTLINEITEM._serialized_start=5095
+  _PREDICTRESULTLINEITEM._serialized_end=5453
+  _PROBABILITYVALUE._serialized_start=5455
+  _PROBABILITYVALUE._serialized_end=5509
+  _SHAPVALUE._serialized_start=5511
+  _SHAPVALUE._serialized_end=5554
+  _GRPCINFERENCESERVICE._serialized_start=5557
+  _GRPCINFERENCESERVICE._serialized_end=7523
 # @@protoc_insertion_point(module_scope)
```

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/google/api/annotations_pb2.py` & `modelaapi-0.6.230/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/google/api/http_pb2.py` & `modelaapi-0.6.230/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/modelaapi/consts.py` & `modelaapi-0.6.230/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/modelaapi/custom_transformers.py` & `modelaapi-0.6.230/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/modelaapi/graykite_model.py` & `modelaapi-0.6.230/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/modelaapi/ts.py` & `modelaapi-0.6.230/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/modelaapi/version.py` & `modelaapi-0.6.230/modelaapi/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 225,
+    "micro": 230,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.225/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.230/modelaapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.225
+Version: 0.6.230
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.225
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.230
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.225
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.230
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.225/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.230/modelaapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/setup.cfg` & `modelaapi-0.6.230/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.225/setup.py` & `modelaapi-0.6.230/setup.py`

 * *Files identical despite different names*

