# Comparing `tmp/modelaapi-0.6.230.tar.gz` & `tmp/modelaapi-0.6.231.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelaapi-0.6.230.tar", last modified: Fri Jul 21 17:45:08 2023, max compression
+gzip compressed data, was "modelaapi-0.6.231.tar", last modified: Fri Jul 21 18:09:41 2023, max compression
```

## Comparing `modelaapi-0.6.230.tar` & `modelaapi-0.6.231.tar`

### file list

```diff
@@ -1,481 +1,581 @@
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.487496 modelaapi-0.6.230/
--rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.230/AUTHORS.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.230/CONTRIBUTING.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.230/DESCRIPTION.md
--rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.230/HISTORY.rst
--rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.230/LICENSE.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      437 2023-01-26 17:46:09.000000 modelaapi-0.6.230/MANIFEST.in
--rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.230/Makefile
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-21 17:45:08.487496 modelaapi-0.6.230/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.230/README.md
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/gogo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/gogo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/gogo/protobuf/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/gogo/protobuf/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24619 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    56768 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.459495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.463496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.467496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.471495 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.475496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.479496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-21 17:41:56.000000 modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/google/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/google/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/google/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/google/api/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/annotations_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/annotations_pb2_grpc.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/http_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.230/google/api/http_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/apps/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/apps/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/apps/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/apps/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/api/apps/v1/generated_pb2.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/core/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/core/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/core/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/core/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/api/core/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/core/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/rbac/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/rbac/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/api/rbac/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/rbac/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/api/rbac/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/api/rbac/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/__init__.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.483496 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/
--rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-21 17:41:56.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
--rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.487496 modelaapi-0.6.230/modelaapi/
--rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/__init__.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/consts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/custom_transformers.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/graykite_model.py
--rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.230/modelaapi/ts.py
--rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-21 17:44:56.000000 modelaapi-0.6.230/modelaapi/version.py
-drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 17:45:08.487496 modelaapi-0.6.230/modelaapi.egg-info/
--rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/PKG-INFO
--rw-rw-r--   0 liam      (1000) liam      (1000)    19381 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/SOURCES.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/dependency_links.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/entry_points.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.230/modelaapi.egg-info/not-zip-safe
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/requires.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-21 17:45:08.000000 modelaapi-0.6.230/modelaapi.egg-info/top_level.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.230/requirements.txt
--rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-21 17:45:08.487496 modelaapi-0.6.230/setup.cfg
--rw-rw-r--   0 liam      (1000) liam      (1000)     5349 2023-02-27 17:33:55.000000 modelaapi-0.6.230/setup.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      139 2023-01-26 17:46:09.000000 modelaapi-0.6.231/AUTHORS.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3579 2023-01-26 17:46:09.000000 modelaapi-0.6.231/CONTRIBUTING.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)        0 2023-01-26 17:46:09.000000 modelaapi-0.6.231/DESCRIPTION.md
+-rw-rw-r--   0 liam      (1000) liam      (1000)       89 2023-01-26 17:46:09.000000 modelaapi-0.6.231/HISTORY.rst
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11351 2023-01-26 17:46:09.000000 modelaapi-0.6.231/LICENSE.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1047 2023-01-26 17:46:09.000000 modelaapi-0.6.231/Makefile
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-21 18:09:41.939899 modelaapi-0.6.231/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)      762 2023-01-26 17:46:09.000000 modelaapi-0.6.231/README.md
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/gogo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/gogo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/gogo/protobuf/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/gogo/protobuf/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/gogo/protobuf/gogoproto/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/gogo/protobuf/gogoproto/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14416 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6763 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24619 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    41779 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    50953 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88974 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    22799 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35286 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24864 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    40354 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11918 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18422 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    56768 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    99171 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11310 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8164 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24380 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7196 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4594 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11335 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7919 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4881 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.907900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4798 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3133 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7751 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19189 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12730 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    33508 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6226 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4263 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18211 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14479 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11490 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14189 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23069 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8826 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5445 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14287 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    31897 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    73562 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78486 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   111042 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.911900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9057 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4969 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17941 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8161 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4644 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14642 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10253 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5326 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19897 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8425 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5395 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12265 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8095 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4276 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13350 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19016 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14515 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    35095 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9636 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5885 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16324 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    78210 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    66312 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)   348679 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6605 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3961 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11503 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.915900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10534 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5613 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21293 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7606 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4141 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13040 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3038 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2012 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3345 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.895901 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpc/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.895901 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpc/health/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpc/health/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2035 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1010 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3056 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18392 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    19563 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24869 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20839 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    17943 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    26279 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6886 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4516 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11025 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8088 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4951 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13831 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.919900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    20626 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13520 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    44447 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4690 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2363 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7755 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10011 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    18664 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.895901 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclassrun/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclassrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11990 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6559 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23986 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    51863 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12420 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7054 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4035 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11800 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3626 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1956 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9814 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3276 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1204 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5855 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5036 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4282 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5675 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6924 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3917 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12110 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.923900 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8637 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4820 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16389 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2824 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1294 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3486 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9068 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5788 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    16147 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7197 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6533 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7539 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8686 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5338 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15629 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6809 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3883 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11955 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7381 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4364 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13561 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7474 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4597 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11484 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6596 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3815 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11645 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7910 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4459 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14432 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.927899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13739 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13906 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14535 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14465 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11657 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6909 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23824 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14859 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7442 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     9747 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6597 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    15755 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6407 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3580 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    11180 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12111 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12936 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13516 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     8160 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4784 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12588 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-01-26 17:46:09.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     7168 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     3696 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)    12575 2023-07-21 17:41:56.000000 modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.931899 modelaapi-0.6.231/google/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/google/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/google/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/google/api/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1580 2023-07-21 17:41:56.000000 modelaapi-0.6.231/google/api/annotations_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      310 2023-07-21 17:41:56.000000 modelaapi-0.6.231/google/api/annotations_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/google/api/annotations_pb2_grpc.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2125 2023-07-21 17:41:56.000000 modelaapi-0.6.231/google/api/http_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     2272 2023-07-21 17:41:56.000000 modelaapi-0.6.231/google/api/http_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/google/api/http_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/apps/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/apps/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/apps/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    13162 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/api/apps/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    21422 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/api/apps/v1/generated_pb2.pyi
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/core/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/core/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/core/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    88069 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/api/core/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)   150106 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/api/core/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/rbac/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/rbac/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/api/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/rbac/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     4882 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/api/rbac/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     6650 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/api/rbac/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/api/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/resource/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1329 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      579 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14127 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    23310 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1636 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1267 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/schema/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1085 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      135 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.935899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/__init__.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      170 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/intstr/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1268 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)      577 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-01-26 17:46:09.000000 modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.899901 modelaapi-0.6.231/k8s/io/apps/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/apps/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/apps/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.899901 modelaapi-0.6.231/k8s/io/core/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/core/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/core/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/k8s/io/pkg/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.899901 modelaapi-0.6.231/k8s/io/pkg/api/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/pkg/api/resource/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/pkg/api/resource/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.899901 modelaapi-0.6.231/k8s/io/pkg/apis/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.899901 modelaapi-0.6.231/k8s/io/pkg/apis/meta/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/pkg/apis/meta/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/pkg/runtime/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/pkg/runtime/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/pkg/runtime/schema/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/k8s/io/pkg/util/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/pkg/util/intstr/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/pkg/util/intstr/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.903900 modelaapi-0.6.231/k8s/io/rbac/
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/k8s/io/rbac/v1/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      159 2023-07-21 17:41:56.000000 modelaapi-0.6.231/k8s/io/rbac/v1/generated_pb2_grpc.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/modelaapi/
+-rw-rw-r--   0 liam      (1000) liam      (1000)      257 2023-01-26 17:46:09.000000 modelaapi-0.6.231/modelaapi/__init__.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    62657 2023-01-26 17:46:09.000000 modelaapi-0.6.231/modelaapi/consts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    10291 2023-01-26 17:46:09.000000 modelaapi-0.6.231/modelaapi/custom_transformers.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    14165 2023-01-26 17:46:09.000000 modelaapi-0.6.231/modelaapi/graykite_model.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)    25394 2023-01-26 17:46:09.000000 modelaapi-0.6.231/modelaapi/ts.py
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1129 2023-07-21 17:49:47.000000 modelaapi-0.6.231/modelaapi/version.py
+drwxrwxr-x   0 liam      (1000) liam      (1000)        0 2023-07-21 18:09:41.939899 modelaapi-0.6.231/modelaapi.egg-info/
+-rw-rw-r--   0 liam      (1000) liam      (1000)     1444 2023-07-21 18:09:41.000000 modelaapi-0.6.231/modelaapi.egg-info/PKG-INFO
+-rw-rw-r--   0 liam      (1000) liam      (1000)    24585 2023-07-21 18:09:41.000000 modelaapi-0.6.231/modelaapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-07-21 18:09:41.000000 modelaapi-0.6.231/modelaapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       20 2023-07-21 18:09:41.000000 modelaapi-0.6.231/modelaapi.egg-info/entry_points.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)        1 2023-02-27 17:39:16.000000 modelaapi-0.6.231/modelaapi.egg-info/not-zip-safe
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-07-21 18:09:41.000000 modelaapi-0.6.231/modelaapi.egg-info/requires.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       28 2023-07-21 18:09:41.000000 modelaapi-0.6.231/modelaapi.egg-info/top_level.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)       36 2023-01-26 17:46:09.000000 modelaapi-0.6.231/requirements.txt
+-rw-rw-r--   0 liam      (1000) liam      (1000)      790 2023-07-21 18:09:41.939899 modelaapi-0.6.231/setup.cfg
+-rw-rw-r--   0 liam      (1000) liam      (1000)     5473 2023-07-21 18:09:27.000000 modelaapi-0.6.231/setup.py
```

### Comparing `modelaapi-0.6.230/CONTRIBUTING.rst` & `modelaapi-0.6.231/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/LICENSE.txt` & `modelaapi-0.6.231/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/Makefile` & `modelaapi-0.6.231/Makefile`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/PKG-INFO` & `modelaapi-0.6.231/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.230
+Version: 0.6.231
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.230
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.231
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.230
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.231
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.230/README.md` & `modelaapi-0.6.231/README.md`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/gogo/protobuf/gogoproto/gogo_pb2.py` & `modelaapi-0.6.231/github/com/gogo/protobuf/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/data_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/license_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/report_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/review_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/study_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/v1/system_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py` & `modelaapi-0.6.231/github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/google/api/annotations_pb2.py` & `modelaapi-0.6.231/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/google/api/http_pb2.py` & `modelaapi-0.6.231/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/api/apps/v1/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/api/apps/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/api/core/v1/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/api/core/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/api/rbac/v1/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/api/rbac/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/apimachinery/pkg/api/resource/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py` & `modelaapi-0.6.231/k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/modelaapi/consts.py` & `modelaapi-0.6.231/modelaapi/consts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/modelaapi/custom_transformers.py` & `modelaapi-0.6.231/modelaapi/custom_transformers.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/modelaapi/graykite_model.py` & `modelaapi-0.6.231/modelaapi/graykite_model.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/modelaapi/ts.py` & `modelaapi-0.6.231/modelaapi/ts.py`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/modelaapi/version.py` & `modelaapi-0.6.231/modelaapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
     "minor": 6,
-    "micro": 230,
+    "micro": 231,
     "releaselevel": "alpha",
     "post": 0,
     "serial": 1,
 }
 
 ##########################################################################
 ## Helper Functions
```

### Comparing `modelaapi-0.6.230/modelaapi.egg-info/PKG-INFO` & `modelaapi-0.6.231/modelaapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: modelaapi
-Version: 0.6.230
+Version: 0.6.231
 Summary: A suite of automatic machine learning for kubernetes
 Home-page: http://www.modela.ai
 Author: The modelaapi developers
 Author-email: info@modela.ai
 Maintainer: The modela developers
 Maintainer-email: info@modela.ai
 License: Apache 2
-Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.230
+Download-URL: https://github.com/metaprov/modelaapi/tarball/v0.6.231
 Project-URL: Documentation, http://www.modela.ai
-Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.230
+Project-URL: Download, https://github.com/metaprov/modelaapi/tarball/v0.6.231
 Project-URL: Source, https://github.com/metaprov/modelaapi
 Project-URL: Tracker, https://github.com/metaprov/modelaapi/issues
 Keywords: automl,machine learning,data science
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `modelaapi-0.6.230/modelaapi.egg-info/SOURCES.txt` & `modelaapi-0.6.231/modelaapi.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,317 +1,396 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 DESCRIPTION.md
 HISTORY.rst
 LICENSE.txt
-MANIFEST.in
 Makefile
 README.md
 requirements.txt
 setup.cfg
 setup.py
 github/__init__.py
 github/com/__init__.py
 github/com/gogo/__init__.py
 github/com/gogo/protobuf/__init__.py
 github/com/gogo/protobuf/gogoproto/__init__.py
 github/com/gogo/protobuf/gogoproto/gogo_pb2.py
+github/com/gogo/protobuf/gogoproto/gogo_pb2.pyi
 github/com/gogo/protobuf/gogoproto/gogo_pb2_grpc.py
 github/com/metaprov/__init__.py
 github/com/metaprov/modelaapi/__init__.py
 github/com/metaprov/modelaapi/pkg/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/catalog/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.py
+github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2.pyi
 github/com/metaprov/modelaapi/pkg/apis/catalog/v1alpha1/generated_pb2_grpc.py
 github/com/metaprov/modelaapi/pkg/apis/data/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.py
+github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2.pyi
 github/com/metaprov/modelaapi/pkg/apis/data/v1alpha1/generated_pb2_grpc.py
 github/com/metaprov/modelaapi/pkg/apis/inference/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.py
+github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2.pyi
 github/com/metaprov/modelaapi/pkg/apis/inference/v1alpha1/generated_pb2_grpc.py
 github/com/metaprov/modelaapi/pkg/apis/infra/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.py
+github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2.pyi
 github/com/metaprov/modelaapi/pkg/apis/infra/v1alpha1/generated_pb2_grpc.py
 github/com/metaprov/modelaapi/pkg/apis/team/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.py
+github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2.pyi
 github/com/metaprov/modelaapi/pkg/apis/team/v1alpha1/generated_pb2_grpc.py
 github/com/metaprov/modelaapi/pkg/apis/training/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/__init__.py
 github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.py
+github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2.pyi
 github/com/metaprov/modelaapi/pkg/apis/training/v1alpha1/generated_pb2_grpc.py
 github/com/metaprov/modelaapi/services/__init__.py
 github/com/metaprov/modelaapi/services/account/__init__.py
 github/com/metaprov/modelaapi/services/account/v1/__init__.py
 github/com/metaprov/modelaapi/services/account/v1/account_pb2.py
+github/com/metaprov/modelaapi/services/account/v1/account_pb2.pyi
 github/com/metaprov/modelaapi/services/account/v1/account_pb2_grpc.py
 github/com/metaprov/modelaapi/services/alert/__init__.py
 github/com/metaprov/modelaapi/services/alert/v1/__init__.py
 github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.py
+github/com/metaprov/modelaapi/services/alert/v1/alert_pb2.pyi
 github/com/metaprov/modelaapi/services/alert/v1/alert_pb2_grpc.py
 github/com/metaprov/modelaapi/services/attachment/__init__.py
 github/com/metaprov/modelaapi/services/attachment/v1/__init__.py
 github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.py
+github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2.pyi
 github/com/metaprov/modelaapi/services/attachment/v1/attachment_pb2_grpc.py
 github/com/metaprov/modelaapi/services/batchpredictord/__init__.py
 github/com/metaprov/modelaapi/services/batchpredictord/v1/__init__.py
 github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.py
+github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2.pyi
 github/com/metaprov/modelaapi/services/batchpredictord/v1/batchpredictord_pb2_grpc.py
 github/com/metaprov/modelaapi/services/catalog/__init__.py
 github/com/metaprov/modelaapi/services/catalog/v1/__init__.py
 github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.py
+github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2.pyi
 github/com/metaprov/modelaapi/services/catalog/v1/catalog_pb2_grpc.py
 github/com/metaprov/modelaapi/services/cloudproxyd/__init__.py
 github/com/metaprov/modelaapi/services/cloudproxyd/v1/__init__.py
 github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.py
+github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2.pyi
 github/com/metaprov/modelaapi/services/cloudproxyd/v1/cloudproxyd_pb2_grpc.py
 github/com/metaprov/modelaapi/services/commit/__init__.py
 github/com/metaprov/modelaapi/services/commit/v1/__init__.py
 github/com/metaprov/modelaapi/services/commit/v1/commit_pb2.py
 github/com/metaprov/modelaapi/services/commit/v1/commit_pb2_grpc.py
 github/com/metaprov/modelaapi/services/common/__init__.py
 github/com/metaprov/modelaapi/services/common/v1/__init__.py
 github/com/metaprov/modelaapi/services/common/v1/common_pb2.py
+github/com/metaprov/modelaapi/services/common/v1/common_pb2.pyi
 github/com/metaprov/modelaapi/services/common/v1/common_pb2_grpc.py
 github/com/metaprov/modelaapi/services/connection/__init__.py
 github/com/metaprov/modelaapi/services/connection/v1/__init__.py
 github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.py
+github/com/metaprov/modelaapi/services/connection/v1/connection_pb2.pyi
 github/com/metaprov/modelaapi/services/connection/v1/connection_pb2_grpc.py
 github/com/metaprov/modelaapi/services/conversation/__init__.py
 github/com/metaprov/modelaapi/services/conversation/v1/__init__.py
 github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2.py
 github/com/metaprov/modelaapi/services/conversation/v1/conversation_pb2_grpc.py
 github/com/metaprov/modelaapi/services/data/__init__.py
 github/com/metaprov/modelaapi/services/data/v1/__init__.py
 github/com/metaprov/modelaapi/services/data/v1/data_pb2.py
+github/com/metaprov/modelaapi/services/data/v1/data_pb2.pyi
 github/com/metaprov/modelaapi/services/data/v1/data_pb2_grpc.py
 github/com/metaprov/modelaapi/services/dataapp/__init__.py
 github/com/metaprov/modelaapi/services/dataapp/v1/__init__.py
 github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.py
+github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2.pyi
 github/com/metaprov/modelaapi/services/dataapp/v1/dataapp_pb2_grpc.py
 github/com/metaprov/modelaapi/services/datapipeline/__init__.py
 github/com/metaprov/modelaapi/services/datapipeline/v1/__init__.py
 github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.py
+github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2.pyi
 github/com/metaprov/modelaapi/services/datapipeline/v1/datapipeline_pb2_grpc.py
 github/com/metaprov/modelaapi/services/datapipelinerun/__init__.py
 github/com/metaprov/modelaapi/services/datapipelinerun/v1/__init__.py
 github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.py
+github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2.pyi
 github/com/metaprov/modelaapi/services/datapipelinerun/v1/datapipelinerun_pb2_grpc.py
 github/com/metaprov/modelaapi/services/dataproduct/__init__.py
 github/com/metaprov/modelaapi/services/dataproduct/v1/__init__.py
 github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.py
+github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2.pyi
 github/com/metaprov/modelaapi/services/dataproduct/v1/dataproduct_pb2_grpc.py
 github/com/metaprov/modelaapi/services/dataproductversion/__init__.py
 github/com/metaprov/modelaapi/services/dataproductversion/v1/__init__.py
 github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.py
+github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2.pyi
 github/com/metaprov/modelaapi/services/dataproductversion/v1/dataproductversion_pb2_grpc.py
 github/com/metaprov/modelaapi/services/dataset/__init__.py
 github/com/metaprov/modelaapi/services/dataset/v1/__init__.py
 github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.py
+github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2.pyi
 github/com/metaprov/modelaapi/services/dataset/v1/dataset_pb2_grpc.py
 github/com/metaprov/modelaapi/services/datasource/__init__.py
 github/com/metaprov/modelaapi/services/datasource/v1/__init__.py
 github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.py
+github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2.pyi
 github/com/metaprov/modelaapi/services/datasource/v1/datasource_pb2_grpc.py
 github/com/metaprov/modelaapi/services/dbproxyd/__init__.py
 github/com/metaprov/modelaapi/services/dbproxyd/v1/__init__.py
 github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.py
+github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2.pyi
 github/com/metaprov/modelaapi/services/dbproxyd/v1/dbproxyd_pb2_grpc.py
 github/com/metaprov/modelaapi/services/entity/__init__.py
 github/com/metaprov/modelaapi/services/entity/v1/__init__.py
 github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.py
+github/com/metaprov/modelaapi/services/entity/v1/entity_pb2.pyi
 github/com/metaprov/modelaapi/services/entity/v1/entity_pb2_grpc.py
 github/com/metaprov/modelaapi/services/featuregroup/__init__.py
 github/com/metaprov/modelaapi/services/featuregroup/v1/__init__.py
 github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.py
+github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2.pyi
 github/com/metaprov/modelaapi/services/featuregroup/v1/featuregroup_pb2_grpc.py
 github/com/metaprov/modelaapi/services/featurehistogram/__init__.py
 github/com/metaprov/modelaapi/services/featurehistogram/v1/__init__.py
 github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.py
+github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2.pyi
 github/com/metaprov/modelaapi/services/featurehistogram/v1/featurehistogram_pb2_grpc.py
 github/com/metaprov/modelaapi/services/fileservices/__init__.py
 github/com/metaprov/modelaapi/services/fileservices/v1/__init__.py
 github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.py
+github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2.pyi
 github/com/metaprov/modelaapi/services/fileservices/v1/fileservices_pb2_grpc.py
+github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.py
+github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2.pyi
+github/com/metaprov/modelaapi/services/grpc/health/v1/health_pb2_grpc.py
 github/com/metaprov/modelaapi/services/grpcinferenceservice/__init__.py
 github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/__init__.py
 github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.py
+github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2.pyi
 github/com/metaprov/modelaapi/services/grpcinferenceservice/v1/grpcinferenceservice_pb2_grpc.py
 github/com/metaprov/modelaapi/services/k8score/__init__.py
 github/com/metaprov/modelaapi/services/k8score/v1/__init__.py
 github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.py
+github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2.pyi
 github/com/metaprov/modelaapi/services/k8score/v1/k8score_pb2_grpc.py
 github/com/metaprov/modelaapi/services/lab/__init__.py
 github/com/metaprov/modelaapi/services/lab/v1/__init__.py
 github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.py
+github/com/metaprov/modelaapi/services/lab/v1/lab_pb2.pyi
 github/com/metaprov/modelaapi/services/lab/v1/lab_pb2_grpc.py
 github/com/metaprov/modelaapi/services/license/__init__.py
 github/com/metaprov/modelaapi/services/license/v1/__init__.py
 github/com/metaprov/modelaapi/services/license/v1/license_pb2.py
+github/com/metaprov/modelaapi/services/license/v1/license_pb2.pyi
 github/com/metaprov/modelaapi/services/license/v1/license_pb2_grpc.py
 github/com/metaprov/modelaapi/services/model/__init__.py
 github/com/metaprov/modelaapi/services/model/v1/__init__.py
 github/com/metaprov/modelaapi/services/model/v1/model_pb2.py
+github/com/metaprov/modelaapi/services/model/v1/model_pb2.pyi
 github/com/metaprov/modelaapi/services/model/v1/model_pb2_grpc.py
 github/com/metaprov/modelaapi/services/modelasystem/__init__.py
 github/com/metaprov/modelaapi/services/modelasystem/v1/__init__.py
 github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.py
+github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2.pyi
 github/com/metaprov/modelaapi/services/modelasystem/v1/modelasystem_pb2_grpc.py
 github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2.py
 github/com/metaprov/modelaapi/services/modelasystem/v1/modeldsystem_pb2_grpc.py
 github/com/metaprov/modelaapi/services/modelclass/__init__.py
 github/com/metaprov/modelaapi/services/modelclass/v1/__init__.py
 github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.py
+github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2.pyi
 github/com/metaprov/modelaapi/services/modelclass/v1/modelclass_pb2_grpc.py
+github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.py
+github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2.pyi
+github/com/metaprov/modelaapi/services/modelclassrun/v1/modelclassrun_pb2_grpc.py
 github/com/metaprov/modelaapi/services/modeldsystem/__init__.py
 github/com/metaprov/modelaapi/services/modeldsystem/v1/__init__.py
 github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2.py
 github/com/metaprov/modelaapi/services/modeldsystem/v1/modeldsystem_pb2_grpc.py
 github/com/metaprov/modelaapi/services/notifier/__init__.py
 github/com/metaprov/modelaapi/services/notifier/v1/__init__.py
 github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.py
+github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2.pyi
 github/com/metaprov/modelaapi/services/notifier/v1/notifier_pb2_grpc.py
 github/com/metaprov/modelaapi/services/objectstored/__init__.py
 github/com/metaprov/modelaapi/services/objectstored/v1/__init__.py
 github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.py
+github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2.pyi
 github/com/metaprov/modelaapi/services/objectstored/v1/objectstored_pb2_grpc.py
 github/com/metaprov/modelaapi/services/offlinefeaturestored/__init__.py
 github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/__init__.py
 github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.py
+github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2.pyi
 github/com/metaprov/modelaapi/services/offlinefeaturestored/v1/offlinefeaturestored_pb2_grpc.py
 github/com/metaprov/modelaapi/services/onlinefeaturestored/__init__.py
 github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/__init__.py
 github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.py
+github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2.pyi
 github/com/metaprov/modelaapi/services/onlinefeaturestored/v1/onlinefeaturestored_pb2_grpc.py
 github/com/metaprov/modelaapi/services/postmortem/__init__.py
 github/com/metaprov/modelaapi/services/postmortem/v1/__init__.py
 github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.py
+github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2.pyi
 github/com/metaprov/modelaapi/services/postmortem/v1/postmortem_pb2_grpc.py
 github/com/metaprov/modelaapi/services/prediction/__init__.py
 github/com/metaprov/modelaapi/services/prediction/v1/__init__.py
 github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.py
+github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2.pyi
 github/com/metaprov/modelaapi/services/prediction/v1/prediction_pb2_grpc.py
 github/com/metaprov/modelaapi/services/predictionstore/__init__.py
 github/com/metaprov/modelaapi/services/predictionstore/v1/__init__.py
 github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.py
+github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2.pyi
 github/com/metaprov/modelaapi/services/predictionstore/v1/predictionstore_pb2_grpc.py
 github/com/metaprov/modelaapi/services/predictor/__init__.py
 github/com/metaprov/modelaapi/services/predictor/v1/__init__.py
 github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.py
+github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2.pyi
 github/com/metaprov/modelaapi/services/predictor/v1/predictor_pb2_grpc.py
 github/com/metaprov/modelaapi/services/publisherd/__init__.py
 github/com/metaprov/modelaapi/services/publisherd/v1/__init__.py
 github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.py
+github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2.pyi
 github/com/metaprov/modelaapi/services/publisherd/v1/publisherd_pb2_grpc.py
 github/com/metaprov/modelaapi/services/recipe/__init__.py
 github/com/metaprov/modelaapi/services/recipe/v1/__init__.py
 github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.py
+github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2.pyi
 github/com/metaprov/modelaapi/services/recipe/v1/recipe_pb2_grpc.py
 github/com/metaprov/modelaapi/services/reciperun/__init__.py
 github/com/metaprov/modelaapi/services/reciperun/v1/__init__.py
 github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.py
+github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2.pyi
 github/com/metaprov/modelaapi/services/reciperun/v1/reciperun_pb2_grpc.py
 github/com/metaprov/modelaapi/services/report/__init__.py
 github/com/metaprov/modelaapi/services/report/v1/__init__.py
 github/com/metaprov/modelaapi/services/report/v1/report_pb2.py
+github/com/metaprov/modelaapi/services/report/v1/report_pb2.pyi
 github/com/metaprov/modelaapi/services/report/v1/report_pb2_grpc.py
 github/com/metaprov/modelaapi/services/review/__init__.py
 github/com/metaprov/modelaapi/services/review/v1/__init__.py
 github/com/metaprov/modelaapi/services/review/v1/review_pb2.py
+github/com/metaprov/modelaapi/services/review/v1/review_pb2.pyi
 github/com/metaprov/modelaapi/services/review/v1/review_pb2_grpc.py
 github/com/metaprov/modelaapi/services/runbook/__init__.py
 github/com/metaprov/modelaapi/services/runbook/v1/__init__.py
 github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.py
+github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2.pyi
 github/com/metaprov/modelaapi/services/runbook/v1/runbook_pb2_grpc.py
 github/com/metaprov/modelaapi/services/servingsite/__init__.py
 github/com/metaprov/modelaapi/services/servingsite/v1/__init__.py
 github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.py
+github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2.pyi
 github/com/metaprov/modelaapi/services/servingsite/v1/servingsite_pb2_grpc.py
 github/com/metaprov/modelaapi/services/sqlquery/__init__.py
 github/com/metaprov/modelaapi/services/sqlquery/v1/__init__.py
 github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2.py
 github/com/metaprov/modelaapi/services/sqlquery/v1/sqlquery_pb2_grpc.py
 github/com/metaprov/modelaapi/services/sqlqueryrun/__init__.py
 github/com/metaprov/modelaapi/services/sqlqueryrun/v1/__init__.py
 github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2.py
 github/com/metaprov/modelaapi/services/sqlqueryrun/v1/sqlqueryrun_pb2_grpc.py
 github/com/metaprov/modelaapi/services/study/__init__.py
 github/com/metaprov/modelaapi/services/study/v1/__init__.py
 github/com/metaprov/modelaapi/services/study/v1/study_pb2.py
+github/com/metaprov/modelaapi/services/study/v1/study_pb2.pyi
 github/com/metaprov/modelaapi/services/study/v1/study_pb2_grpc.py
 github/com/metaprov/modelaapi/services/system/__init__.py
 github/com/metaprov/modelaapi/services/system/v1/__init__.py
 github/com/metaprov/modelaapi/services/system/v1/system_pb2.py
 github/com/metaprov/modelaapi/services/system/v1/system_pb2_grpc.py
 github/com/metaprov/modelaapi/services/tenant/__init__.py
 github/com/metaprov/modelaapi/services/tenant/v1/__init__.py
 github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.py
+github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2.pyi
 github/com/metaprov/modelaapi/services/tenant/v1/tenant_pb2_grpc.py
 github/com/metaprov/modelaapi/services/todo/__init__.py
 github/com/metaprov/modelaapi/services/todo/v1/__init__.py
 github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.py
+github/com/metaprov/modelaapi/services/todo/v1/todo_pb2.pyi
 github/com/metaprov/modelaapi/services/todo/v1/todo_pb2_grpc.py
 github/com/metaprov/modelaapi/services/trainerd/__init__.py
 github/com/metaprov/modelaapi/services/trainerd/v1/__init__.py
 github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.py
+github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2.pyi
 github/com/metaprov/modelaapi/services/trainerd/v1/trainerd_pb2_grpc.py
 github/com/metaprov/modelaapi/services/userroleclass/__init__.py
 github/com/metaprov/modelaapi/services/userroleclass/v1/__init__.py
 github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.py
+github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2.pyi
 github/com/metaprov/modelaapi/services/userroleclass/v1/userroleclass_pb2_grpc.py
 github/com/metaprov/modelaapi/services/virtualbucket/__init__.py
 github/com/metaprov/modelaapi/services/virtualbucket/v1/__init__.py
 github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.py
+github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2.pyi
 github/com/metaprov/modelaapi/services/virtualbucket/v1/virtualbucket_pb2_grpc.py
 google/__init__.py
 google/api/__init__.py
 google/api/annotations_pb2.py
+google/api/annotations_pb2.pyi
 google/api/annotations_pb2_grpc.py
 google/api/http_pb2.py
+google/api/http_pb2.pyi
 google/api/http_pb2_grpc.py
 k8s/__init__.py
 k8s/io/__init__.py
 k8s/io/api/__init__.py
 k8s/io/api/apps/__init__.py
 k8s/io/api/apps/v1/__init__.py
 k8s/io/api/apps/v1/generated_pb2.py
+k8s/io/api/apps/v1/generated_pb2.pyi
 k8s/io/api/core/__init__.py
 k8s/io/api/core/v1/__init__.py
 k8s/io/api/core/v1/generated_pb2.py
+k8s/io/api/core/v1/generated_pb2.pyi
 k8s/io/api/core/v1/generated_pb2_grpc.py
 k8s/io/api/rbac/__init__.py
 k8s/io/api/rbac/v1/__init__.py
 k8s/io/api/rbac/v1/generated_pb2.py
+k8s/io/api/rbac/v1/generated_pb2.pyi
 k8s/io/api/rbac/v1/generated_pb2_grpc.py
 k8s/io/apimachinery/__init__.py
 k8s/io/apimachinery/pkg/__init__.py
 k8s/io/apimachinery/pkg/api/__init__.py
 k8s/io/apimachinery/pkg/api/resource/__init__.py
 k8s/io/apimachinery/pkg/api/resource/generated_pb2.py
+k8s/io/apimachinery/pkg/api/resource/generated_pb2.pyi
 k8s/io/apimachinery/pkg/api/resource/generated_pb2_grpc.py
 k8s/io/apimachinery/pkg/apis/__init__.py
 k8s/io/apimachinery/pkg/apis/meta/__init__.py
 k8s/io/apimachinery/pkg/apis/meta/v1/__init__.py
 k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.py
+k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2.pyi
 k8s/io/apimachinery/pkg/apis/meta/v1/generated_pb2_grpc.py
 k8s/io/apimachinery/pkg/runtime/__init__.py
 k8s/io/apimachinery/pkg/runtime/generated_pb2.py
+k8s/io/apimachinery/pkg/runtime/generated_pb2.pyi
 k8s/io/apimachinery/pkg/runtime/generated_pb2_grpc.py
 k8s/io/apimachinery/pkg/runtime/schema/__init__.py
 k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.py
+k8s/io/apimachinery/pkg/runtime/schema/generated_pb2.pyi
 k8s/io/apimachinery/pkg/runtime/schema/generated_pb2_grpc.py
 k8s/io/apimachinery/pkg/util/__init__.py
 k8s/io/apimachinery/pkg/util/intstr/__init__.py
 k8s/io/apimachinery/pkg/util/intstr/generated_pb2.py
+k8s/io/apimachinery/pkg/util/intstr/generated_pb2.pyi
 k8s/io/apimachinery/pkg/util/intstr/generated_pb2_grpc.py
+k8s/io/apps/v1/generated_pb2_grpc.py
+k8s/io/core/v1/generated_pb2_grpc.py
+k8s/io/pkg/api/resource/generated_pb2_grpc.py
+k8s/io/pkg/apis/meta/v1/generated_pb2_grpc.py
+k8s/io/pkg/runtime/generated_pb2_grpc.py
+k8s/io/pkg/runtime/schema/generated_pb2_grpc.py
+k8s/io/pkg/util/intstr/generated_pb2_grpc.py
+k8s/io/rbac/v1/generated_pb2_grpc.py
 modelaapi/__init__.py
 modelaapi/consts.py
 modelaapi/custom_transformers.py
 modelaapi/graykite_model.py
 modelaapi/ts.py
 modelaapi/version.py
 modelaapi.egg-info/PKG-INFO
```

### Comparing `modelaapi-0.6.230/setup.cfg` & `modelaapi-0.6.231/setup.cfg`

 * *Files identical despite different names*

### Comparing `modelaapi-0.6.230/setup.py` & `modelaapi-0.6.231/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,14 +130,16 @@
     return {".rst": "text/x-rst", ".txt": "text/plain", ".md": "text/markdown"}[ext]
 
 
 ##########################################################################
 ## Define the configuration
 ##########################################################################
 
+print(find_packages(where=PROJECT, exclude=EXCLUDES))
+
 config = {
     "name": NAME,
     "version": get_version(),
     "description": DESCRIPTION,
     "long_description": read(PKG_DESCRIBE),
     "long_description_content_type": get_description_type(PKG_DESCRIBE),
     "classifiers": CLASSIFIERS,
@@ -152,15 +154,15 @@
         "Documentation": URL,
         "Download": "{}/tarball/v{}".format(REPOSITORY, get_version()),
         "Source": REPOSITORY,
         "Tracker": "{}/issues".format(REPOSITORY),
     },
     "download_url": "{}/tarball/v{}".format(REPOSITORY, get_version()),
     "packages": find_packages(where=PROJECT, exclude=EXCLUDES),
-    "package_data": {"yellowbrick": ["datasets/manifest.json"]},
+    "package_data": {"yellowbrick": ["datasets/manifest.json"], "github": ["**/*.pyi"], "google": ["**/*.pyi"], "k8s": ["**/*.pyi"]},
     "zip_safe": False,
     "entry_points": {"console_scripts": []},
     "install_requires": list(get_requires()),
     "python_requires": ">=3.4, <4",
     "setup_requires": ["pytest-runner"],
     "tests_require": ["pytest"],
 }
```

